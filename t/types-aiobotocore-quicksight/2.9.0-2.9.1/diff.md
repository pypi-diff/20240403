# Comparing `tmp/types-aiobotocore-quicksight-2.9.0.tar.gz` & `tmp/types-aiobotocore-quicksight-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-quicksight-2.9.0.tar", last modified: Wed Dec 13 20:00:13 2023, max compression
+gzip compressed data, was "types-aiobotocore-quicksight-2.9.1.tar", last modified: Thu Jan 18 01:21:33 2024, max compression
```

## Comparing `types-aiobotocore-quicksight-2.9.0.tar` & `types-aiobotocore-quicksight-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:13.861282 types-aiobotocore-quicksight-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:53:50.000000 types-aiobotocore-quicksight-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    17596 2023-12-13 20:00:13.861282 types-aiobotocore-quicksight-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16021 2023-12-13 19:53:50.000000 types-aiobotocore-quicksight-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:13.861282 types-aiobotocore-quicksight-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2023-12-13 19:53:50.000000 types-aiobotocore-quicksight-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:13.861282 types-aiobotocore-quicksight-2.9.0/types_aiobotocore_quicksight/
--rw-r--r--   0 runner    (1001) docker     (127)     7026 2023-12-13 19:53:51.000000 types-aiobotocore-quicksight-2.9.0/types_aiobotocore_quicksight/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7025 2023-12-13 19:53:51.000000 types-aiobotocore-quicksight-2.9.0/types_aiobotocore_quicksight/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      944 2023-12-13 19:53:51.000000 types-aiobotocore-quicksight-2.9.0/types_aiobotocore_quicksight/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)   140107 2023-12-13 19:53:51.000000 types-aiobotocore-quicksight-2.9.0/types_aiobotocore_quicksight/client.py
--rw-r--r--   0 runner    (1001) docker     (127)   140103 2023-12-13 19:53:51.000000 types-aiobotocore-quicksight-2.9.0/types_aiobotocore_quicksight/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    39289 2023-12-13 19:53:52.000000 types-aiobotocore-quicksight-2.9.0/types_aiobotocore_quicksight/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    39287 2023-12-13 19:53:52.000000 types-aiobotocore-quicksight-2.9.0/types_aiobotocore_quicksight/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    37671 2023-12-13 19:53:51.000000 types-aiobotocore-quicksight-2.9.0/types_aiobotocore_quicksight/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    37638 2023-12-13 19:53:51.000000 types-aiobotocore-quicksight-2.9.0/types_aiobotocore_quicksight/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:53:51.000000 types-aiobotocore-quicksight-2.9.0/types_aiobotocore_quicksight/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   377052 2023-12-13 19:54:01.000000 types-aiobotocore-quicksight-2.9.0/types_aiobotocore_quicksight/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   377051 2023-12-13 19:53:58.000000 types-aiobotocore-quicksight-2.9.0/types_aiobotocore_quicksight/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:53:50.000000 types-aiobotocore-quicksight-2.9.0/types_aiobotocore_quicksight/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:13.861282 types-aiobotocore-quicksight-2.9.0/types_aiobotocore_quicksight.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17596 2023-12-13 20:00:13.000000 types-aiobotocore-quicksight-2.9.0/types_aiobotocore_quicksight.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      870 2023-12-13 20:00:13.000000 types-aiobotocore-quicksight-2.9.0/types_aiobotocore_quicksight.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:13.000000 types-aiobotocore-quicksight-2.9.0/types_aiobotocore_quicksight.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:13.000000 types-aiobotocore-quicksight-2.9.0/types_aiobotocore_quicksight.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:13.000000 types-aiobotocore-quicksight-2.9.0/types_aiobotocore_quicksight.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-13 20:00:13.000000 types-aiobotocore-quicksight-2.9.0/types_aiobotocore_quicksight.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:33.777101 types-aiobotocore-quicksight-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:15:23.000000 types-aiobotocore-quicksight-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17616 2024-01-18 01:21:33.777101 types-aiobotocore-quicksight-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16021 2024-01-18 01:15:23.000000 types-aiobotocore-quicksight-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:33.777101 types-aiobotocore-quicksight-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-01-18 01:15:23.000000 types-aiobotocore-quicksight-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:33.777101 types-aiobotocore-quicksight-2.9.1/types_aiobotocore_quicksight/
+-rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-01-18 01:15:23.000000 types-aiobotocore-quicksight-2.9.1/types_aiobotocore_quicksight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-01-18 01:15:23.000000 types-aiobotocore-quicksight-2.9.1/types_aiobotocore_quicksight/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-01-18 01:15:23.000000 types-aiobotocore-quicksight-2.9.1/types_aiobotocore_quicksight/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   140167 2024-01-18 01:15:24.000000 types-aiobotocore-quicksight-2.9.1/types_aiobotocore_quicksight/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   140164 2024-01-18 01:15:24.000000 types-aiobotocore-quicksight-2.9.1/types_aiobotocore_quicksight/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    39287 2024-01-18 01:15:25.000000 types-aiobotocore-quicksight-2.9.1/types_aiobotocore_quicksight/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39287 2024-01-18 01:15:25.000000 types-aiobotocore-quicksight-2.9.1/types_aiobotocore_quicksight/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    37684 2024-01-18 01:15:25.000000 types-aiobotocore-quicksight-2.9.1/types_aiobotocore_quicksight/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37652 2024-01-18 01:15:24.000000 types-aiobotocore-quicksight-2.9.1/types_aiobotocore_quicksight/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:15:23.000000 types-aiobotocore-quicksight-2.9.1/types_aiobotocore_quicksight/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   377051 2024-01-18 01:15:37.000000 types-aiobotocore-quicksight-2.9.1/types_aiobotocore_quicksight/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   377051 2024-01-18 01:15:34.000000 types-aiobotocore-quicksight-2.9.1/types_aiobotocore_quicksight/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:15:23.000000 types-aiobotocore-quicksight-2.9.1/types_aiobotocore_quicksight/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:33.777101 types-aiobotocore-quicksight-2.9.1/types_aiobotocore_quicksight.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17616 2024-01-18 01:21:33.000000 types-aiobotocore-quicksight-2.9.1/types_aiobotocore_quicksight.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-01-18 01:21:33.000000 types-aiobotocore-quicksight-2.9.1/types_aiobotocore_quicksight.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:33.000000 types-aiobotocore-quicksight-2.9.1/types_aiobotocore_quicksight.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:33.000000 types-aiobotocore-quicksight-2.9.1/types_aiobotocore_quicksight.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:33.000000 types-aiobotocore-quicksight-2.9.1/types_aiobotocore_quicksight.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-01-18 01:21:33.000000 types-aiobotocore-quicksight-2.9.1/types_aiobotocore_quicksight.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-quicksight-2.9.0/LICENSE` & `types-aiobotocore-quicksight-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-quicksight-2.9.0/PKG-INFO` & `types-aiobotocore-quicksight-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-quicksight
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.QuickSight 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.QuickSight 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/
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
 
 <a id="types-aiobotocore-quicksight"></a>
 
 # types-aiobotocore-quicksight
 
 [![PyPI - types-aiobotocore-quicksight](https://img.shields.io/pypi/v/types-aiobotocore-quicksight.svg?color=blue)](https://pypi.org/project/types-aiobotocore-quicksight)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-quicksight.svg?color=blue)](https://pypi.org/project/types-aiobotocore-quicksight)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-quicksight)](https://pepy.tech/project/types-aiobotocore-quicksight)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.QuickSight 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight)
+[aiobotocore.QuickSight 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight)
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
 [types-aiobotocore-quicksight docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-quicksight-2.9.0/README.md` & `types-aiobotocore-quicksight-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-quicksight.svg?color=blue)](https://pypi.org/project/types-aiobotocore-quicksight)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-quicksight)](https://pepy.tech/project/types-aiobotocore-quicksight)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.QuickSight 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight)
+[aiobotocore.QuickSight 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight)
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
 [types-aiobotocore-quicksight docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-quicksight-2.9.0/setup.py` & `types-aiobotocore-quicksight-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-quicksight",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_quicksight"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.QuickSight 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.QuickSight 2.9.1 service generated with"
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
     keywords="aiobotocore quicksight type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_quicksight": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-quicksight-2.9.0/types_aiobotocore_quicksight/__init__.py` & `types-aiobotocore-quicksight-2.9.1/types_aiobotocore_quicksight/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,14 @@
     SearchDataSourcesPaginator,
     SearchFoldersPaginator,
     SearchGroupsPaginator,
 )
 
 Client = QuickSightClient
 
-
 __all__ = (
     "Client",
     "DescribeFolderPermissionsPaginator",
     "DescribeFolderResolvedPermissionsPaginator",
     "ListAnalysesPaginator",
     "ListAssetBundleExportJobsPaginator",
     "ListAssetBundleImportJobsPaginator",
```

### Comparing `types-aiobotocore-quicksight-2.9.0/types_aiobotocore_quicksight/__init__.pyi` & `types-aiobotocore-quicksight-2.9.1/types_aiobotocore_quicksight/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-quicksight-2.9.0/types_aiobotocore_quicksight/__main__.py` & `types-aiobotocore-quicksight-2.9.1/types_aiobotocore_quicksight/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.QuickSight 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.QuickSight 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight\nOther"
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

### Comparing `types-aiobotocore-quicksight-2.9.0/types_aiobotocore_quicksight/client.py` & `types-aiobotocore-quicksight-2.9.1/types_aiobotocore_quicksight/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -295,15 +295,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("QuickSightClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -379,15 +378,15 @@
 
     async def create_account_customization(
         self,
         *,
         AwsAccountId: str,
         AccountCustomization: AccountCustomizationTypeDef,
         Namespace: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateAccountCustomizationResponseTypeDef:
         """
         Creates Amazon QuickSight customizations for the current Amazon Web Services
         Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_account_customization)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#create_account_customization)
@@ -406,15 +405,15 @@
         DirectoryId: str = ...,
         AdminGroup: Sequence[str] = ...,
         AuthorGroup: Sequence[str] = ...,
         ReaderGroup: Sequence[str] = ...,
         FirstName: str = ...,
         LastName: str = ...,
         EmailAddress: str = ...,
-        ContactNumber: str = ...
+        ContactNumber: str = ...,
     ) -> CreateAccountSubscriptionResponseTypeDef:
         """
         Creates an Amazon QuickSight account, or subscribes to Amazon QuickSight Q.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_account_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#create_account_subscription)
         """
@@ -428,15 +427,15 @@
         Parameters: ParametersTypeDef = ...,
         Permissions: Sequence[ResourcePermissionTypeDef] = ...,
         SourceEntity: AnalysisSourceEntityTypeDef = ...,
         ThemeArn: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         Definition: AnalysisDefinitionTypeDef = ...,
         ValidationStrategy: ValidationStrategyTypeDef = ...,
-        FolderArns: Sequence[str] = ...
+        FolderArns: Sequence[str] = ...,
     ) -> CreateAnalysisResponseTypeDef:
         """
         Creates an analysis in Amazon QuickSight.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_analysis)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#create_analysis)
         """
@@ -453,15 +452,15 @@
         Tags: Sequence[TagTypeDef] = ...,
         VersionDescription: str = ...,
         DashboardPublishOptions: DashboardPublishOptionsTypeDef = ...,
         ThemeArn: str = ...,
         Definition: DashboardVersionDefinitionTypeDef = ...,
         ValidationStrategy: ValidationStrategyTypeDef = ...,
         FolderArns: Sequence[str] = ...,
-        LinkSharingConfiguration: LinkSharingConfigurationTypeDef = ...
+        LinkSharingConfiguration: LinkSharingConfigurationTypeDef = ...,
     ) -> CreateDashboardResponseTypeDef:
         """
         Creates a dashboard from either a template or directly with a
         `DashboardDefinition`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_dashboard)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#create_dashboard)
@@ -481,15 +480,15 @@
         Permissions: Sequence[ResourcePermissionTypeDef] = ...,
         RowLevelPermissionDataSet: RowLevelPermissionDataSetTypeDef = ...,
         RowLevelPermissionTagConfiguration: RowLevelPermissionTagConfigurationTypeDef = ...,
         ColumnLevelPermissionRules: Sequence[ColumnLevelPermissionRuleTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DataSetUsageConfiguration: DataSetUsageConfigurationTypeDef = ...,
         DatasetParameters: Sequence[DatasetParameterTypeDef] = ...,
-        FolderArns: Sequence[str] = ...
+        FolderArns: Sequence[str] = ...,
     ) -> CreateDataSetResponseTypeDef:
         """
         Creates a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_data_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#create_data_set)
         """
@@ -503,15 +502,15 @@
         Type: DataSourceTypeType,
         DataSourceParameters: DataSourceParametersTypeDef = ...,
         Credentials: DataSourceCredentialsTypeDef = ...,
         Permissions: Sequence[ResourcePermissionTypeDef] = ...,
         VpcConnectionProperties: VpcConnectionPropertiesTypeDef = ...,
         SslProperties: SslPropertiesTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        FolderArns: Sequence[str] = ...
+        FolderArns: Sequence[str] = ...,
     ) -> CreateDataSourceResponseTypeDef:
         """
         Creates a data source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_data_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#create_data_source)
         """
@@ -522,15 +521,15 @@
         AwsAccountId: str,
         FolderId: str,
         Name: str = ...,
         FolderType: FolderTypeType = ...,
         ParentFolderArn: str = ...,
         Permissions: Sequence[ResourcePermissionTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        SharingModel: SharingModelType = ...
+        SharingModel: SharingModelType = ...,
     ) -> CreateFolderResponseTypeDef:
         """
         Creates an empty shared folder.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_folder)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#create_folder)
         """
@@ -569,15 +568,15 @@
         self,
         *,
         AwsAccountId: str,
         AssignmentName: str,
         AssignmentStatus: AssignmentStatusType,
         Namespace: str,
         PolicyArn: str = ...,
-        Identities: Mapping[str, Sequence[str]] = ...
+        Identities: Mapping[str, Sequence[str]] = ...,
     ) -> CreateIAMPolicyAssignmentResponseTypeDef:
         """
         Creates an assignment with one specified IAM policy, identified by its Amazon
         Resource Name
         (ARN).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_iam_policy_assignment)
@@ -586,30 +585,30 @@
 
     async def create_ingestion(
         self,
         *,
         DataSetId: str,
         IngestionId: str,
         AwsAccountId: str,
-        IngestionType: IngestionTypeType = ...
+        IngestionType: IngestionTypeType = ...,
     ) -> CreateIngestionResponseTypeDef:
         """
         Creates and starts a new SPICE ingestion for a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_ingestion)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#create_ingestion)
         """
 
     async def create_namespace(
         self,
         *,
         AwsAccountId: str,
         Namespace: str,
         IdentityStore: Literal["QUICKSIGHT"],
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateNamespaceResponseTypeDef:
         """
         (Enterprise edition only) Creates a new namespace for you to use with Amazon
         QuickSight.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_namespace)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#create_namespace)
@@ -644,15 +643,15 @@
         TemplateId: str,
         Name: str = ...,
         Permissions: Sequence[ResourcePermissionTypeDef] = ...,
         SourceEntity: TemplateSourceEntityTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         VersionDescription: str = ...,
         Definition: TemplateVersionDefinitionTypeDef = ...,
-        ValidationStrategy: ValidationStrategyTypeDef = ...
+        ValidationStrategy: ValidationStrategyTypeDef = ...,
     ) -> CreateTemplateResponseTypeDef:
         """
         Creates a template either from a `TemplateDefinition` or from an existing
         Amazon QuickSight analysis or
         template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_template)
@@ -675,15 +674,15 @@
         AwsAccountId: str,
         ThemeId: str,
         Name: str,
         BaseThemeId: str,
         Configuration: ThemeConfigurationTypeDef,
         VersionDescription: str = ...,
         Permissions: Sequence[ResourcePermissionTypeDef] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateThemeResponseTypeDef:
         """
         Creates a theme.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_theme)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#create_theme)
         """
@@ -700,15 +699,15 @@
 
     async def create_topic(
         self,
         *,
         AwsAccountId: str,
         TopicId: str,
         Topic: TopicDetailsTypeDef,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateTopicResponseTypeDef:
         """
         Creates a new Q topic.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_topic)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#create_topic)
         """
@@ -716,15 +715,15 @@
     async def create_topic_refresh_schedule(
         self,
         *,
         AwsAccountId: str,
         TopicId: str,
         DatasetArn: str,
         RefreshSchedule: TopicRefreshScheduleTypeDef,
-        DatasetName: str = ...
+        DatasetName: str = ...,
     ) -> CreateTopicRefreshScheduleResponseTypeDef:
         """
         Creates a topic refresh schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_topic_refresh_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#create_topic_refresh_schedule)
         """
@@ -735,15 +734,15 @@
         AwsAccountId: str,
         VPCConnectionId: str,
         Name: str,
         SubnetIds: Sequence[str],
         SecurityGroupIds: Sequence[str],
         RoleArn: str,
         DnsResolvers: Sequence[str] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateVPCConnectionResponseTypeDef:
         """
         Creates a new VPC connection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_vpc_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#create_vpc_connection)
         """
@@ -773,15 +772,15 @@
 
     async def delete_analysis(
         self,
         *,
         AwsAccountId: str,
         AnalysisId: str,
         RecoveryWindowInDays: int = ...,
-        ForceDeleteWithoutRecovery: bool = ...
+        ForceDeleteWithoutRecovery: bool = ...,
     ) -> DeleteAnalysisResponseTypeDef:
         """
         Deletes an analysis from Amazon QuickSight.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.delete_analysis)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#delete_analysis)
         """
@@ -1218,15 +1217,15 @@
     async def describe_folder_permissions(
         self,
         *,
         AwsAccountId: str,
         FolderId: str,
         Namespace: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeFolderPermissionsResponseTypeDef:
         """
         Describes permissions for a folder.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.describe_folder_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#describe_folder_permissions)
         """
@@ -1234,15 +1233,15 @@
     async def describe_folder_resolved_permissions(
         self,
         *,
         AwsAccountId: str,
         FolderId: str,
         Namespace: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeFolderResolvedPermissionsResponseTypeDef:
         """
         Describes the folder resolved permissions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.describe_folder_resolved_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#describe_folder_resolved_permissions)
         """
@@ -1465,15 +1464,15 @@
         *,
         AwsAccountId: str,
         Namespace: str,
         AuthorizedResourceArns: Sequence[str],
         ExperienceConfiguration: AnonymousUserEmbeddingExperienceConfigurationTypeDef,
         SessionLifetimeInMinutes: int = ...,
         SessionTags: Sequence[SessionTagTypeDef] = ...,
-        AllowedDomains: Sequence[str] = ...
+        AllowedDomains: Sequence[str] = ...,
     ) -> GenerateEmbedUrlForAnonymousUserResponseTypeDef:
         """
         Generates an embed URL that you can use to embed an Amazon QuickSight dashboard
         or visual in your website, without having to register any reader
         users.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.generate_embed_url_for_anonymous_user)
@@ -1483,15 +1482,15 @@
     async def generate_embed_url_for_registered_user(
         self,
         *,
         AwsAccountId: str,
         UserArn: str,
         ExperienceConfiguration: RegisteredUserEmbeddingExperienceConfigurationTypeDef,
         SessionLifetimeInMinutes: int = ...,
-        AllowedDomains: Sequence[str] = ...
+        AllowedDomains: Sequence[str] = ...,
     ) -> GenerateEmbedUrlForRegisteredUserResponseTypeDef:
         """
         Generates an embed URL that you can use to embed an Amazon QuickSight
         experience in your
         website.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.generate_embed_url_for_registered_user)
@@ -1520,15 +1519,15 @@
         IdentityType: EmbeddingIdentityTypeType,
         SessionLifetimeInMinutes: int = ...,
         UndoRedoDisabled: bool = ...,
         ResetDisabled: bool = ...,
         StatePersistenceEnabled: bool = ...,
         UserArn: str = ...,
         Namespace: str = ...,
-        AdditionalDashboardIds: Sequence[str] = ...
+        AdditionalDashboardIds: Sequence[str] = ...,
     ) -> GetDashboardEmbedUrlResponseTypeDef:
         """
         Generates a temporary session URL and authorization code(bearer token) that you
         can use to embed an Amazon QuickSight read-only dashboard in your website or
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.get_dashboard_embed_url)
@@ -1537,15 +1536,15 @@
 
     async def get_session_embed_url(
         self,
         *,
         AwsAccountId: str,
         EntryPoint: str = ...,
         SessionLifetimeInMinutes: int = ...,
-        UserArn: str = ...
+        UserArn: str = ...,
     ) -> GetSessionEmbedUrlResponseTypeDef:
         """
         Generates a session URL and authorization code that you can use to embed the
         Amazon Amazon QuickSight console in your web server
         code.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.get_session_embed_url)
@@ -1652,15 +1651,15 @@
     async def list_group_memberships(
         self,
         *,
         GroupName: str,
         AwsAccountId: str,
         Namespace: str,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListGroupMembershipsResponseTypeDef:
         """
         Lists member users in a group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.list_group_memberships)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#list_group_memberships)
         """
@@ -1678,15 +1677,15 @@
     async def list_iam_policy_assignments(
         self,
         *,
         AwsAccountId: str,
         Namespace: str,
         AssignmentStatus: AssignmentStatusType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListIAMPolicyAssignmentsResponseTypeDef:
         """
         Lists the IAM policy assignments in the current Amazon QuickSight account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.list_iam_policy_assignments)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#list_iam_policy_assignments)
         """
@@ -1694,15 +1693,15 @@
     async def list_iam_policy_assignments_for_user(
         self,
         *,
         AwsAccountId: str,
         UserName: str,
         Namespace: str,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListIAMPolicyAssignmentsForUserResponseTypeDef:
         """
         Lists all of the IAM policy assignments, including the Amazon Resource Names
         (ARNs), for the IAM policies assigned to the specified user and group, or
         groups that the user belongs
         to.
 
@@ -1755,15 +1754,15 @@
     async def list_role_memberships(
         self,
         *,
         Role: RoleType,
         AwsAccountId: str,
         Namespace: str,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListRoleMembershipsResponseTypeDef:
         """
         Lists all groups that are associated with a role.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.list_role_memberships)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#list_role_memberships)
         """
@@ -1831,15 +1830,15 @@
 
     async def list_themes(
         self,
         *,
         AwsAccountId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
-        Type: ThemeTypeType = ...
+        Type: ThemeTypeType = ...,
     ) -> ListThemesResponseTypeDef:
         """
         Lists all the themes in the current Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.list_themes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#list_themes)
         """
@@ -1867,15 +1866,15 @@
     async def list_user_groups(
         self,
         *,
         UserName: str,
         AwsAccountId: str,
         Namespace: str,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListUserGroupsResponseTypeDef:
         """
         Lists the Amazon QuickSight groups that an Amazon QuickSight user is a member
         of.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.list_user_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#list_user_groups)
@@ -1904,15 +1903,15 @@
         """
 
     async def put_data_set_refresh_properties(
         self,
         *,
         AwsAccountId: str,
         DataSetId: str,
-        DataSetRefreshProperties: DataSetRefreshPropertiesTypeDef
+        DataSetRefreshProperties: DataSetRefreshPropertiesTypeDef,
     ) -> PutDataSetRefreshPropertiesResponseTypeDef:
         """
         Creates or updates the dataset refresh properties for the dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.put_data_set_refresh_properties)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#put_data_set_refresh_properties)
         """
@@ -1928,15 +1927,15 @@
         IamArn: str = ...,
         SessionName: str = ...,
         UserName: str = ...,
         CustomPermissionsName: str = ...,
         ExternalLoginFederationProviderType: str = ...,
         CustomFederationProviderUrl: str = ...,
         ExternalLoginId: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> RegisterUserResponseTypeDef:
         """
         Creates an Amazon QuickSight user whose identity is associated with the
         Identity and Access Management (IAM) identity or role specified in the
         request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.register_user)
@@ -1955,45 +1954,45 @@
 
     async def search_analyses(
         self,
         *,
         AwsAccountId: str,
         Filters: Sequence[AnalysisSearchFilterTypeDef],
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> SearchAnalysesResponseTypeDef:
         """
         Searches for analyses that belong to the user specified in the filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.search_analyses)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#search_analyses)
         """
 
     async def search_dashboards(
         self,
         *,
         AwsAccountId: str,
         Filters: Sequence[DashboardSearchFilterTypeDef],
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> SearchDashboardsResponseTypeDef:
         """
         Searches for dashboards that belong to a user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.search_dashboards)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#search_dashboards)
         """
 
     async def search_data_sets(
         self,
         *,
         AwsAccountId: str,
         Filters: Sequence[DataSetSearchFilterTypeDef],
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> SearchDataSetsResponseTypeDef:
         """
         Use the `SearchDataSets` operation to search for datasets that belong to an
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.search_data_sets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#search_data_sets)
@@ -2001,15 +2000,15 @@
 
     async def search_data_sources(
         self,
         *,
         AwsAccountId: str,
         Filters: Sequence[DataSourceSearchFilterTypeDef],
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> SearchDataSourcesResponseTypeDef:
         """
         Use the `SearchDataSources` operation to search for data sources that belong to
         an
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.search_data_sources)
@@ -2018,15 +2017,15 @@
 
     async def search_folders(
         self,
         *,
         AwsAccountId: str,
         Filters: Sequence[FolderSearchFilterTypeDef],
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> SearchFoldersResponseTypeDef:
         """
         Searches the subfolders in a folder.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.search_folders)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#search_folders)
         """
@@ -2034,15 +2033,15 @@
     async def search_groups(
         self,
         *,
         AwsAccountId: str,
         Namespace: str,
         Filters: Sequence[GroupSearchFilterTypeDef],
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> SearchGroupsResponseTypeDef:
         """
         Use the `SearchGroups` operation to search groups in a specified Amazon
         QuickSight namespace using the supplied
         filters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.search_groups)
@@ -2056,15 +2055,15 @@
         AssetBundleExportJobId: str,
         ResourceArns: Sequence[str],
         ExportFormat: AssetBundleExportFormatType,
         IncludeAllDependencies: bool = ...,
         CloudFormationOverridePropertyConfiguration: AssetBundleCloudFormationOverridePropertyConfigurationTypeDef = ...,
         IncludePermissions: bool = ...,
         IncludeTags: bool = ...,
-        ValidationStrategy: AssetBundleExportJobValidationStrategyTypeDef = ...
+        ValidationStrategy: AssetBundleExportJobValidationStrategyTypeDef = ...,
     ) -> StartAssetBundleExportJobResponseTypeDef:
         """
         Starts an Asset Bundle export job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.start_asset_bundle_export_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#start_asset_bundle_export_job)
         """
@@ -2075,15 +2074,15 @@
         AwsAccountId: str,
         AssetBundleImportJobId: str,
         AssetBundleImportSource: AssetBundleImportSourceTypeDef,
         OverrideParameters: AssetBundleImportJobOverrideParametersTypeDef = ...,
         FailureAction: AssetBundleImportFailureActionType = ...,
         OverridePermissions: AssetBundleImportJobOverridePermissionsTypeDef = ...,
         OverrideTags: AssetBundleImportJobOverrideTagsTypeDef = ...,
-        OverrideValidationStrategy: AssetBundleImportJobOverrideValidationStrategyTypeDef = ...
+        OverrideValidationStrategy: AssetBundleImportJobOverrideValidationStrategyTypeDef = ...,
     ) -> StartAssetBundleImportJobResponseTypeDef:
         """
         Starts an Asset Bundle import job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.start_asset_bundle_import_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#start_asset_bundle_import_job)
         """
@@ -2091,15 +2090,15 @@
     async def start_dashboard_snapshot_job(
         self,
         *,
         AwsAccountId: str,
         DashboardId: str,
         SnapshotJobId: str,
         UserConfiguration: SnapshotUserConfigurationTypeDef,
-        SnapshotConfiguration: SnapshotConfigurationTypeDef
+        SnapshotConfiguration: SnapshotConfigurationTypeDef,
     ) -> StartDashboardSnapshotJobResponseTypeDef:
         """
         Starts an asynchronous job that generates a dashboard snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.start_dashboard_snapshot_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#start_dashboard_snapshot_job)
         """
@@ -2126,15 +2125,15 @@
         """
 
     async def update_account_customization(
         self,
         *,
         AwsAccountId: str,
         AccountCustomization: AccountCustomizationTypeDef,
-        Namespace: str = ...
+        Namespace: str = ...,
     ) -> UpdateAccountCustomizationResponseTypeDef:
         """
         Updates Amazon QuickSight customizations for the current Amazon Web Services
         Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_account_customization)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#update_account_customization)
@@ -2142,15 +2141,15 @@
 
     async def update_account_settings(
         self,
         *,
         AwsAccountId: str,
         DefaultNamespace: str,
         NotificationEmail: str = ...,
-        TerminationProtectionEnabled: bool = ...
+        TerminationProtectionEnabled: bool = ...,
     ) -> UpdateAccountSettingsResponseTypeDef:
         """
         Updates the Amazon QuickSight settings in your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_account_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#update_account_settings)
         """
@@ -2161,15 +2160,15 @@
         AwsAccountId: str,
         AnalysisId: str,
         Name: str,
         Parameters: ParametersTypeDef = ...,
         SourceEntity: AnalysisSourceEntityTypeDef = ...,
         ThemeArn: str = ...,
         Definition: AnalysisDefinitionTypeDef = ...,
-        ValidationStrategy: ValidationStrategyTypeDef = ...
+        ValidationStrategy: ValidationStrategyTypeDef = ...,
     ) -> UpdateAnalysisResponseTypeDef:
         """
         Updates an analysis in Amazon QuickSight See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/quicksight-2018-04-01/UpdateAnalysis).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_analysis)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#update_analysis)
@@ -2177,15 +2176,15 @@
 
     async def update_analysis_permissions(
         self,
         *,
         AwsAccountId: str,
         AnalysisId: str,
         GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...
+        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...,
     ) -> UpdateAnalysisPermissionsResponseTypeDef:
         """
         Updates the read and write permissions for an analysis.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_analysis_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#update_analysis_permissions)
         """
@@ -2198,15 +2197,15 @@
         Name: str,
         SourceEntity: DashboardSourceEntityTypeDef = ...,
         Parameters: ParametersTypeDef = ...,
         VersionDescription: str = ...,
         DashboardPublishOptions: DashboardPublishOptionsTypeDef = ...,
         ThemeArn: str = ...,
         Definition: DashboardVersionDefinitionTypeDef = ...,
-        ValidationStrategy: ValidationStrategyTypeDef = ...
+        ValidationStrategy: ValidationStrategyTypeDef = ...,
     ) -> UpdateDashboardResponseTypeDef:
         """
         Updates a dashboard in an Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_dashboard)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#update_dashboard)
         """
@@ -2215,15 +2214,15 @@
         self,
         *,
         AwsAccountId: str,
         DashboardId: str,
         GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,
         RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...,
         GrantLinkPermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        RevokeLinkPermissions: Sequence[ResourcePermissionTypeDef] = ...
+        RevokeLinkPermissions: Sequence[ResourcePermissionTypeDef] = ...,
     ) -> UpdateDashboardPermissionsResponseTypeDef:
         """
         Updates read and write permissions on a dashboard.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_dashboard_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#update_dashboard_permissions)
         """
@@ -2249,30 +2248,30 @@
         LogicalTableMap: Mapping[str, LogicalTableTypeDef] = ...,
         ColumnGroups: Sequence[ColumnGroupTypeDef] = ...,
         FieldFolders: Mapping[str, FieldFolderTypeDef] = ...,
         RowLevelPermissionDataSet: RowLevelPermissionDataSetTypeDef = ...,
         RowLevelPermissionTagConfiguration: RowLevelPermissionTagConfigurationTypeDef = ...,
         ColumnLevelPermissionRules: Sequence[ColumnLevelPermissionRuleTypeDef] = ...,
         DataSetUsageConfiguration: DataSetUsageConfigurationTypeDef = ...,
-        DatasetParameters: Sequence[DatasetParameterTypeDef] = ...
+        DatasetParameters: Sequence[DatasetParameterTypeDef] = ...,
     ) -> UpdateDataSetResponseTypeDef:
         """
         Updates a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_data_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#update_data_set)
         """
 
     async def update_data_set_permissions(
         self,
         *,
         AwsAccountId: str,
         DataSetId: str,
         GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...
+        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...,
     ) -> UpdateDataSetPermissionsResponseTypeDef:
         """
         Updates the permissions on a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_data_set_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#update_data_set_permissions)
         """
@@ -2282,30 +2281,30 @@
         *,
         AwsAccountId: str,
         DataSourceId: str,
         Name: str,
         DataSourceParameters: DataSourceParametersTypeDef = ...,
         Credentials: DataSourceCredentialsTypeDef = ...,
         VpcConnectionProperties: VpcConnectionPropertiesTypeDef = ...,
-        SslProperties: SslPropertiesTypeDef = ...
+        SslProperties: SslPropertiesTypeDef = ...,
     ) -> UpdateDataSourceResponseTypeDef:
         """
         Updates a data source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_data_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#update_data_source)
         """
 
     async def update_data_source_permissions(
         self,
         *,
         AwsAccountId: str,
         DataSourceId: str,
         GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...
+        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...,
     ) -> UpdateDataSourcePermissionsResponseTypeDef:
         """
         Updates the permissions to a data source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_data_source_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#update_data_source_permissions)
         """
@@ -2322,15 +2321,15 @@
 
     async def update_folder_permissions(
         self,
         *,
         AwsAccountId: str,
         FolderId: str,
         GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...
+        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...,
     ) -> UpdateFolderPermissionsResponseTypeDef:
         """
         Updates permissions of a folder.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_folder_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#update_folder_permissions)
         """
@@ -2349,29 +2348,29 @@
         self,
         *,
         AwsAccountId: str,
         AssignmentName: str,
         Namespace: str,
         AssignmentStatus: AssignmentStatusType = ...,
         PolicyArn: str = ...,
-        Identities: Mapping[str, Sequence[str]] = ...
+        Identities: Mapping[str, Sequence[str]] = ...,
     ) -> UpdateIAMPolicyAssignmentResponseTypeDef:
         """
         Updates an existing IAM policy assignment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_iam_policy_assignment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#update_iam_policy_assignment)
         """
 
     async def update_identity_propagation_config(
         self,
         *,
         AwsAccountId: str,
         Service: Literal["REDSHIFT"],
-        AuthorizedTargets: Sequence[str] = ...
+        AuthorizedTargets: Sequence[str] = ...,
     ) -> UpdateIdentityPropagationConfigResponseTypeDef:
         """
         Adds or updates services and authorized targets to configure what the Amazon
         QuickSight IAM Identity Center application can
         access.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_identity_propagation_config)
@@ -2379,15 +2378,15 @@
         """
 
     async def update_ip_restriction(
         self,
         *,
         AwsAccountId: str,
         IpRestrictionRuleMap: Mapping[str, str] = ...,
-        Enabled: bool = ...
+        Enabled: bool = ...,
     ) -> UpdateIpRestrictionResponseTypeDef:
         """
         Updates the content and status of IP rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_ip_restriction)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#update_ip_restriction)
         """
@@ -2429,15 +2428,15 @@
         *,
         AwsAccountId: str,
         TemplateId: str,
         SourceEntity: TemplateSourceEntityTypeDef = ...,
         VersionDescription: str = ...,
         Name: str = ...,
         Definition: TemplateVersionDefinitionTypeDef = ...,
-        ValidationStrategy: ValidationStrategyTypeDef = ...
+        ValidationStrategy: ValidationStrategyTypeDef = ...,
     ) -> UpdateTemplateResponseTypeDef:
         """
         Updates a template from an existing Amazon QuickSight analysis or another
         template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#update_template)
@@ -2455,15 +2454,15 @@
 
     async def update_template_permissions(
         self,
         *,
         AwsAccountId: str,
         TemplateId: str,
         GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...
+        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...,
     ) -> UpdateTemplatePermissionsResponseTypeDef:
         """
         Updates the resource permissions for a template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_template_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#update_template_permissions)
         """
@@ -2472,15 +2471,15 @@
         self,
         *,
         AwsAccountId: str,
         ThemeId: str,
         BaseThemeId: str,
         Name: str = ...,
         VersionDescription: str = ...,
-        Configuration: ThemeConfigurationTypeDef = ...
+        Configuration: ThemeConfigurationTypeDef = ...,
     ) -> UpdateThemeResponseTypeDef:
         """
         Updates a theme.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_theme)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#update_theme)
         """
@@ -2497,15 +2496,15 @@
 
     async def update_theme_permissions(
         self,
         *,
         AwsAccountId: str,
         ThemeId: str,
         GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...
+        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...,
     ) -> UpdateThemePermissionsResponseTypeDef:
         """
         Updates the resource permissions for a theme.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_theme_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#update_theme_permissions)
         """
@@ -2522,30 +2521,30 @@
 
     async def update_topic_permissions(
         self,
         *,
         AwsAccountId: str,
         TopicId: str,
         GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...
+        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...,
     ) -> UpdateTopicPermissionsResponseTypeDef:
         """
         Updates the permissions of a topic.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_topic_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#update_topic_permissions)
         """
 
     async def update_topic_refresh_schedule(
         self,
         *,
         AwsAccountId: str,
         TopicId: str,
         DatasetId: str,
-        RefreshSchedule: TopicRefreshScheduleTypeDef
+        RefreshSchedule: TopicRefreshScheduleTypeDef,
     ) -> UpdateTopicRefreshScheduleResponseTypeDef:
         """
         Updates a topic refresh schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_topic_refresh_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#update_topic_refresh_schedule)
         """
@@ -2558,15 +2557,15 @@
         Namespace: str,
         Email: str,
         Role: UserRoleType,
         CustomPermissionsName: str = ...,
         UnapplyCustomPermissions: bool = ...,
         ExternalLoginFederationProviderType: str = ...,
         CustomFederationProviderUrl: str = ...,
-        ExternalLoginId: str = ...
+        ExternalLoginId: str = ...,
     ) -> UpdateUserResponseTypeDef:
         """
         Updates an Amazon QuickSight user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#update_user)
         """
@@ -2576,15 +2575,15 @@
         *,
         AwsAccountId: str,
         VPCConnectionId: str,
         Name: str,
         SubnetIds: Sequence[str],
         SecurityGroupIds: Sequence[str],
         RoleArn: str,
-        DnsResolvers: Sequence[str] = ...
+        DnsResolvers: Sequence[str] = ...,
     ) -> UpdateVPCConnectionResponseTypeDef:
         """
         Updates a VPC connection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_vpc_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#update_vpc_connection)
         """
```

### Comparing `types-aiobotocore-quicksight-2.9.0/types_aiobotocore_quicksight/client.pyi` & `types-aiobotocore-quicksight-2.9.1/types_aiobotocore_quicksight/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -375,15 +375,15 @@
 
     async def create_account_customization(
         self,
         *,
         AwsAccountId: str,
         AccountCustomization: AccountCustomizationTypeDef,
         Namespace: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateAccountCustomizationResponseTypeDef:
         """
         Creates Amazon QuickSight customizations for the current Amazon Web Services
         Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_account_customization)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#create_account_customization)
@@ -402,15 +402,15 @@
         DirectoryId: str = ...,
         AdminGroup: Sequence[str] = ...,
         AuthorGroup: Sequence[str] = ...,
         ReaderGroup: Sequence[str] = ...,
         FirstName: str = ...,
         LastName: str = ...,
         EmailAddress: str = ...,
-        ContactNumber: str = ...
+        ContactNumber: str = ...,
     ) -> CreateAccountSubscriptionResponseTypeDef:
         """
         Creates an Amazon QuickSight account, or subscribes to Amazon QuickSight Q.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_account_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#create_account_subscription)
         """
@@ -424,15 +424,15 @@
         Parameters: ParametersTypeDef = ...,
         Permissions: Sequence[ResourcePermissionTypeDef] = ...,
         SourceEntity: AnalysisSourceEntityTypeDef = ...,
         ThemeArn: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         Definition: AnalysisDefinitionTypeDef = ...,
         ValidationStrategy: ValidationStrategyTypeDef = ...,
-        FolderArns: Sequence[str] = ...
+        FolderArns: Sequence[str] = ...,
     ) -> CreateAnalysisResponseTypeDef:
         """
         Creates an analysis in Amazon QuickSight.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_analysis)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#create_analysis)
         """
@@ -449,15 +449,15 @@
         Tags: Sequence[TagTypeDef] = ...,
         VersionDescription: str = ...,
         DashboardPublishOptions: DashboardPublishOptionsTypeDef = ...,
         ThemeArn: str = ...,
         Definition: DashboardVersionDefinitionTypeDef = ...,
         ValidationStrategy: ValidationStrategyTypeDef = ...,
         FolderArns: Sequence[str] = ...,
-        LinkSharingConfiguration: LinkSharingConfigurationTypeDef = ...
+        LinkSharingConfiguration: LinkSharingConfigurationTypeDef = ...,
     ) -> CreateDashboardResponseTypeDef:
         """
         Creates a dashboard from either a template or directly with a
         `DashboardDefinition`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_dashboard)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#create_dashboard)
@@ -477,15 +477,15 @@
         Permissions: Sequence[ResourcePermissionTypeDef] = ...,
         RowLevelPermissionDataSet: RowLevelPermissionDataSetTypeDef = ...,
         RowLevelPermissionTagConfiguration: RowLevelPermissionTagConfigurationTypeDef = ...,
         ColumnLevelPermissionRules: Sequence[ColumnLevelPermissionRuleTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DataSetUsageConfiguration: DataSetUsageConfigurationTypeDef = ...,
         DatasetParameters: Sequence[DatasetParameterTypeDef] = ...,
-        FolderArns: Sequence[str] = ...
+        FolderArns: Sequence[str] = ...,
     ) -> CreateDataSetResponseTypeDef:
         """
         Creates a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_data_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#create_data_set)
         """
@@ -499,15 +499,15 @@
         Type: DataSourceTypeType,
         DataSourceParameters: DataSourceParametersTypeDef = ...,
         Credentials: DataSourceCredentialsTypeDef = ...,
         Permissions: Sequence[ResourcePermissionTypeDef] = ...,
         VpcConnectionProperties: VpcConnectionPropertiesTypeDef = ...,
         SslProperties: SslPropertiesTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        FolderArns: Sequence[str] = ...
+        FolderArns: Sequence[str] = ...,
     ) -> CreateDataSourceResponseTypeDef:
         """
         Creates a data source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_data_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#create_data_source)
         """
@@ -518,15 +518,15 @@
         AwsAccountId: str,
         FolderId: str,
         Name: str = ...,
         FolderType: FolderTypeType = ...,
         ParentFolderArn: str = ...,
         Permissions: Sequence[ResourcePermissionTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        SharingModel: SharingModelType = ...
+        SharingModel: SharingModelType = ...,
     ) -> CreateFolderResponseTypeDef:
         """
         Creates an empty shared folder.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_folder)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#create_folder)
         """
@@ -565,15 +565,15 @@
         self,
         *,
         AwsAccountId: str,
         AssignmentName: str,
         AssignmentStatus: AssignmentStatusType,
         Namespace: str,
         PolicyArn: str = ...,
-        Identities: Mapping[str, Sequence[str]] = ...
+        Identities: Mapping[str, Sequence[str]] = ...,
     ) -> CreateIAMPolicyAssignmentResponseTypeDef:
         """
         Creates an assignment with one specified IAM policy, identified by its Amazon
         Resource Name
         (ARN).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_iam_policy_assignment)
@@ -582,30 +582,30 @@
 
     async def create_ingestion(
         self,
         *,
         DataSetId: str,
         IngestionId: str,
         AwsAccountId: str,
-        IngestionType: IngestionTypeType = ...
+        IngestionType: IngestionTypeType = ...,
     ) -> CreateIngestionResponseTypeDef:
         """
         Creates and starts a new SPICE ingestion for a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_ingestion)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#create_ingestion)
         """
 
     async def create_namespace(
         self,
         *,
         AwsAccountId: str,
         Namespace: str,
         IdentityStore: Literal["QUICKSIGHT"],
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateNamespaceResponseTypeDef:
         """
         (Enterprise edition only) Creates a new namespace for you to use with Amazon
         QuickSight.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_namespace)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#create_namespace)
@@ -640,15 +640,15 @@
         TemplateId: str,
         Name: str = ...,
         Permissions: Sequence[ResourcePermissionTypeDef] = ...,
         SourceEntity: TemplateSourceEntityTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         VersionDescription: str = ...,
         Definition: TemplateVersionDefinitionTypeDef = ...,
-        ValidationStrategy: ValidationStrategyTypeDef = ...
+        ValidationStrategy: ValidationStrategyTypeDef = ...,
     ) -> CreateTemplateResponseTypeDef:
         """
         Creates a template either from a `TemplateDefinition` or from an existing
         Amazon QuickSight analysis or
         template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_template)
@@ -671,15 +671,15 @@
         AwsAccountId: str,
         ThemeId: str,
         Name: str,
         BaseThemeId: str,
         Configuration: ThemeConfigurationTypeDef,
         VersionDescription: str = ...,
         Permissions: Sequence[ResourcePermissionTypeDef] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateThemeResponseTypeDef:
         """
         Creates a theme.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_theme)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#create_theme)
         """
@@ -696,15 +696,15 @@
 
     async def create_topic(
         self,
         *,
         AwsAccountId: str,
         TopicId: str,
         Topic: TopicDetailsTypeDef,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateTopicResponseTypeDef:
         """
         Creates a new Q topic.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_topic)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#create_topic)
         """
@@ -712,15 +712,15 @@
     async def create_topic_refresh_schedule(
         self,
         *,
         AwsAccountId: str,
         TopicId: str,
         DatasetArn: str,
         RefreshSchedule: TopicRefreshScheduleTypeDef,
-        DatasetName: str = ...
+        DatasetName: str = ...,
     ) -> CreateTopicRefreshScheduleResponseTypeDef:
         """
         Creates a topic refresh schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_topic_refresh_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#create_topic_refresh_schedule)
         """
@@ -731,15 +731,15 @@
         AwsAccountId: str,
         VPCConnectionId: str,
         Name: str,
         SubnetIds: Sequence[str],
         SecurityGroupIds: Sequence[str],
         RoleArn: str,
         DnsResolvers: Sequence[str] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateVPCConnectionResponseTypeDef:
         """
         Creates a new VPC connection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_vpc_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#create_vpc_connection)
         """
@@ -769,15 +769,15 @@
 
     async def delete_analysis(
         self,
         *,
         AwsAccountId: str,
         AnalysisId: str,
         RecoveryWindowInDays: int = ...,
-        ForceDeleteWithoutRecovery: bool = ...
+        ForceDeleteWithoutRecovery: bool = ...,
     ) -> DeleteAnalysisResponseTypeDef:
         """
         Deletes an analysis from Amazon QuickSight.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.delete_analysis)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#delete_analysis)
         """
@@ -1214,15 +1214,15 @@
     async def describe_folder_permissions(
         self,
         *,
         AwsAccountId: str,
         FolderId: str,
         Namespace: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeFolderPermissionsResponseTypeDef:
         """
         Describes permissions for a folder.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.describe_folder_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#describe_folder_permissions)
         """
@@ -1230,15 +1230,15 @@
     async def describe_folder_resolved_permissions(
         self,
         *,
         AwsAccountId: str,
         FolderId: str,
         Namespace: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeFolderResolvedPermissionsResponseTypeDef:
         """
         Describes the folder resolved permissions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.describe_folder_resolved_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#describe_folder_resolved_permissions)
         """
@@ -1461,15 +1461,15 @@
         *,
         AwsAccountId: str,
         Namespace: str,
         AuthorizedResourceArns: Sequence[str],
         ExperienceConfiguration: AnonymousUserEmbeddingExperienceConfigurationTypeDef,
         SessionLifetimeInMinutes: int = ...,
         SessionTags: Sequence[SessionTagTypeDef] = ...,
-        AllowedDomains: Sequence[str] = ...
+        AllowedDomains: Sequence[str] = ...,
     ) -> GenerateEmbedUrlForAnonymousUserResponseTypeDef:
         """
         Generates an embed URL that you can use to embed an Amazon QuickSight dashboard
         or visual in your website, without having to register any reader
         users.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.generate_embed_url_for_anonymous_user)
@@ -1479,15 +1479,15 @@
     async def generate_embed_url_for_registered_user(
         self,
         *,
         AwsAccountId: str,
         UserArn: str,
         ExperienceConfiguration: RegisteredUserEmbeddingExperienceConfigurationTypeDef,
         SessionLifetimeInMinutes: int = ...,
-        AllowedDomains: Sequence[str] = ...
+        AllowedDomains: Sequence[str] = ...,
     ) -> GenerateEmbedUrlForRegisteredUserResponseTypeDef:
         """
         Generates an embed URL that you can use to embed an Amazon QuickSight
         experience in your
         website.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.generate_embed_url_for_registered_user)
@@ -1516,15 +1516,15 @@
         IdentityType: EmbeddingIdentityTypeType,
         SessionLifetimeInMinutes: int = ...,
         UndoRedoDisabled: bool = ...,
         ResetDisabled: bool = ...,
         StatePersistenceEnabled: bool = ...,
         UserArn: str = ...,
         Namespace: str = ...,
-        AdditionalDashboardIds: Sequence[str] = ...
+        AdditionalDashboardIds: Sequence[str] = ...,
     ) -> GetDashboardEmbedUrlResponseTypeDef:
         """
         Generates a temporary session URL and authorization code(bearer token) that you
         can use to embed an Amazon QuickSight read-only dashboard in your website or
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.get_dashboard_embed_url)
@@ -1533,15 +1533,15 @@
 
     async def get_session_embed_url(
         self,
         *,
         AwsAccountId: str,
         EntryPoint: str = ...,
         SessionLifetimeInMinutes: int = ...,
-        UserArn: str = ...
+        UserArn: str = ...,
     ) -> GetSessionEmbedUrlResponseTypeDef:
         """
         Generates a session URL and authorization code that you can use to embed the
         Amazon Amazon QuickSight console in your web server
         code.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.get_session_embed_url)
@@ -1648,15 +1648,15 @@
     async def list_group_memberships(
         self,
         *,
         GroupName: str,
         AwsAccountId: str,
         Namespace: str,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListGroupMembershipsResponseTypeDef:
         """
         Lists member users in a group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.list_group_memberships)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#list_group_memberships)
         """
@@ -1674,15 +1674,15 @@
     async def list_iam_policy_assignments(
         self,
         *,
         AwsAccountId: str,
         Namespace: str,
         AssignmentStatus: AssignmentStatusType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListIAMPolicyAssignmentsResponseTypeDef:
         """
         Lists the IAM policy assignments in the current Amazon QuickSight account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.list_iam_policy_assignments)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#list_iam_policy_assignments)
         """
@@ -1690,15 +1690,15 @@
     async def list_iam_policy_assignments_for_user(
         self,
         *,
         AwsAccountId: str,
         UserName: str,
         Namespace: str,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListIAMPolicyAssignmentsForUserResponseTypeDef:
         """
         Lists all of the IAM policy assignments, including the Amazon Resource Names
         (ARNs), for the IAM policies assigned to the specified user and group, or
         groups that the user belongs
         to.
 
@@ -1751,15 +1751,15 @@
     async def list_role_memberships(
         self,
         *,
         Role: RoleType,
         AwsAccountId: str,
         Namespace: str,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListRoleMembershipsResponseTypeDef:
         """
         Lists all groups that are associated with a role.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.list_role_memberships)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#list_role_memberships)
         """
@@ -1827,15 +1827,15 @@
 
     async def list_themes(
         self,
         *,
         AwsAccountId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
-        Type: ThemeTypeType = ...
+        Type: ThemeTypeType = ...,
     ) -> ListThemesResponseTypeDef:
         """
         Lists all the themes in the current Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.list_themes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#list_themes)
         """
@@ -1863,15 +1863,15 @@
     async def list_user_groups(
         self,
         *,
         UserName: str,
         AwsAccountId: str,
         Namespace: str,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListUserGroupsResponseTypeDef:
         """
         Lists the Amazon QuickSight groups that an Amazon QuickSight user is a member
         of.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.list_user_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#list_user_groups)
@@ -1900,15 +1900,15 @@
         """
 
     async def put_data_set_refresh_properties(
         self,
         *,
         AwsAccountId: str,
         DataSetId: str,
-        DataSetRefreshProperties: DataSetRefreshPropertiesTypeDef
+        DataSetRefreshProperties: DataSetRefreshPropertiesTypeDef,
     ) -> PutDataSetRefreshPropertiesResponseTypeDef:
         """
         Creates or updates the dataset refresh properties for the dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.put_data_set_refresh_properties)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#put_data_set_refresh_properties)
         """
@@ -1924,15 +1924,15 @@
         IamArn: str = ...,
         SessionName: str = ...,
         UserName: str = ...,
         CustomPermissionsName: str = ...,
         ExternalLoginFederationProviderType: str = ...,
         CustomFederationProviderUrl: str = ...,
         ExternalLoginId: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> RegisterUserResponseTypeDef:
         """
         Creates an Amazon QuickSight user whose identity is associated with the
         Identity and Access Management (IAM) identity or role specified in the
         request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.register_user)
@@ -1951,45 +1951,45 @@
 
     async def search_analyses(
         self,
         *,
         AwsAccountId: str,
         Filters: Sequence[AnalysisSearchFilterTypeDef],
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> SearchAnalysesResponseTypeDef:
         """
         Searches for analyses that belong to the user specified in the filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.search_analyses)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#search_analyses)
         """
 
     async def search_dashboards(
         self,
         *,
         AwsAccountId: str,
         Filters: Sequence[DashboardSearchFilterTypeDef],
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> SearchDashboardsResponseTypeDef:
         """
         Searches for dashboards that belong to a user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.search_dashboards)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#search_dashboards)
         """
 
     async def search_data_sets(
         self,
         *,
         AwsAccountId: str,
         Filters: Sequence[DataSetSearchFilterTypeDef],
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> SearchDataSetsResponseTypeDef:
         """
         Use the `SearchDataSets` operation to search for datasets that belong to an
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.search_data_sets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#search_data_sets)
@@ -1997,15 +1997,15 @@
 
     async def search_data_sources(
         self,
         *,
         AwsAccountId: str,
         Filters: Sequence[DataSourceSearchFilterTypeDef],
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> SearchDataSourcesResponseTypeDef:
         """
         Use the `SearchDataSources` operation to search for data sources that belong to
         an
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.search_data_sources)
@@ -2014,15 +2014,15 @@
 
     async def search_folders(
         self,
         *,
         AwsAccountId: str,
         Filters: Sequence[FolderSearchFilterTypeDef],
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> SearchFoldersResponseTypeDef:
         """
         Searches the subfolders in a folder.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.search_folders)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#search_folders)
         """
@@ -2030,15 +2030,15 @@
     async def search_groups(
         self,
         *,
         AwsAccountId: str,
         Namespace: str,
         Filters: Sequence[GroupSearchFilterTypeDef],
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> SearchGroupsResponseTypeDef:
         """
         Use the `SearchGroups` operation to search groups in a specified Amazon
         QuickSight namespace using the supplied
         filters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.search_groups)
@@ -2052,15 +2052,15 @@
         AssetBundleExportJobId: str,
         ResourceArns: Sequence[str],
         ExportFormat: AssetBundleExportFormatType,
         IncludeAllDependencies: bool = ...,
         CloudFormationOverridePropertyConfiguration: AssetBundleCloudFormationOverridePropertyConfigurationTypeDef = ...,
         IncludePermissions: bool = ...,
         IncludeTags: bool = ...,
-        ValidationStrategy: AssetBundleExportJobValidationStrategyTypeDef = ...
+        ValidationStrategy: AssetBundleExportJobValidationStrategyTypeDef = ...,
     ) -> StartAssetBundleExportJobResponseTypeDef:
         """
         Starts an Asset Bundle export job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.start_asset_bundle_export_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#start_asset_bundle_export_job)
         """
@@ -2071,15 +2071,15 @@
         AwsAccountId: str,
         AssetBundleImportJobId: str,
         AssetBundleImportSource: AssetBundleImportSourceTypeDef,
         OverrideParameters: AssetBundleImportJobOverrideParametersTypeDef = ...,
         FailureAction: AssetBundleImportFailureActionType = ...,
         OverridePermissions: AssetBundleImportJobOverridePermissionsTypeDef = ...,
         OverrideTags: AssetBundleImportJobOverrideTagsTypeDef = ...,
-        OverrideValidationStrategy: AssetBundleImportJobOverrideValidationStrategyTypeDef = ...
+        OverrideValidationStrategy: AssetBundleImportJobOverrideValidationStrategyTypeDef = ...,
     ) -> StartAssetBundleImportJobResponseTypeDef:
         """
         Starts an Asset Bundle import job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.start_asset_bundle_import_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#start_asset_bundle_import_job)
         """
@@ -2087,15 +2087,15 @@
     async def start_dashboard_snapshot_job(
         self,
         *,
         AwsAccountId: str,
         DashboardId: str,
         SnapshotJobId: str,
         UserConfiguration: SnapshotUserConfigurationTypeDef,
-        SnapshotConfiguration: SnapshotConfigurationTypeDef
+        SnapshotConfiguration: SnapshotConfigurationTypeDef,
     ) -> StartDashboardSnapshotJobResponseTypeDef:
         """
         Starts an asynchronous job that generates a dashboard snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.start_dashboard_snapshot_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#start_dashboard_snapshot_job)
         """
@@ -2122,15 +2122,15 @@
         """
 
     async def update_account_customization(
         self,
         *,
         AwsAccountId: str,
         AccountCustomization: AccountCustomizationTypeDef,
-        Namespace: str = ...
+        Namespace: str = ...,
     ) -> UpdateAccountCustomizationResponseTypeDef:
         """
         Updates Amazon QuickSight customizations for the current Amazon Web Services
         Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_account_customization)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#update_account_customization)
@@ -2138,15 +2138,15 @@
 
     async def update_account_settings(
         self,
         *,
         AwsAccountId: str,
         DefaultNamespace: str,
         NotificationEmail: str = ...,
-        TerminationProtectionEnabled: bool = ...
+        TerminationProtectionEnabled: bool = ...,
     ) -> UpdateAccountSettingsResponseTypeDef:
         """
         Updates the Amazon QuickSight settings in your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_account_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#update_account_settings)
         """
@@ -2157,15 +2157,15 @@
         AwsAccountId: str,
         AnalysisId: str,
         Name: str,
         Parameters: ParametersTypeDef = ...,
         SourceEntity: AnalysisSourceEntityTypeDef = ...,
         ThemeArn: str = ...,
         Definition: AnalysisDefinitionTypeDef = ...,
-        ValidationStrategy: ValidationStrategyTypeDef = ...
+        ValidationStrategy: ValidationStrategyTypeDef = ...,
     ) -> UpdateAnalysisResponseTypeDef:
         """
         Updates an analysis in Amazon QuickSight See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/quicksight-2018-04-01/UpdateAnalysis).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_analysis)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#update_analysis)
@@ -2173,15 +2173,15 @@
 
     async def update_analysis_permissions(
         self,
         *,
         AwsAccountId: str,
         AnalysisId: str,
         GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...
+        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...,
     ) -> UpdateAnalysisPermissionsResponseTypeDef:
         """
         Updates the read and write permissions for an analysis.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_analysis_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#update_analysis_permissions)
         """
@@ -2194,15 +2194,15 @@
         Name: str,
         SourceEntity: DashboardSourceEntityTypeDef = ...,
         Parameters: ParametersTypeDef = ...,
         VersionDescription: str = ...,
         DashboardPublishOptions: DashboardPublishOptionsTypeDef = ...,
         ThemeArn: str = ...,
         Definition: DashboardVersionDefinitionTypeDef = ...,
-        ValidationStrategy: ValidationStrategyTypeDef = ...
+        ValidationStrategy: ValidationStrategyTypeDef = ...,
     ) -> UpdateDashboardResponseTypeDef:
         """
         Updates a dashboard in an Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_dashboard)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#update_dashboard)
         """
@@ -2211,15 +2211,15 @@
         self,
         *,
         AwsAccountId: str,
         DashboardId: str,
         GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,
         RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...,
         GrantLinkPermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        RevokeLinkPermissions: Sequence[ResourcePermissionTypeDef] = ...
+        RevokeLinkPermissions: Sequence[ResourcePermissionTypeDef] = ...,
     ) -> UpdateDashboardPermissionsResponseTypeDef:
         """
         Updates read and write permissions on a dashboard.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_dashboard_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#update_dashboard_permissions)
         """
@@ -2245,30 +2245,30 @@
         LogicalTableMap: Mapping[str, LogicalTableTypeDef] = ...,
         ColumnGroups: Sequence[ColumnGroupTypeDef] = ...,
         FieldFolders: Mapping[str, FieldFolderTypeDef] = ...,
         RowLevelPermissionDataSet: RowLevelPermissionDataSetTypeDef = ...,
         RowLevelPermissionTagConfiguration: RowLevelPermissionTagConfigurationTypeDef = ...,
         ColumnLevelPermissionRules: Sequence[ColumnLevelPermissionRuleTypeDef] = ...,
         DataSetUsageConfiguration: DataSetUsageConfigurationTypeDef = ...,
-        DatasetParameters: Sequence[DatasetParameterTypeDef] = ...
+        DatasetParameters: Sequence[DatasetParameterTypeDef] = ...,
     ) -> UpdateDataSetResponseTypeDef:
         """
         Updates a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_data_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#update_data_set)
         """
 
     async def update_data_set_permissions(
         self,
         *,
         AwsAccountId: str,
         DataSetId: str,
         GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...
+        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...,
     ) -> UpdateDataSetPermissionsResponseTypeDef:
         """
         Updates the permissions on a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_data_set_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#update_data_set_permissions)
         """
@@ -2278,30 +2278,30 @@
         *,
         AwsAccountId: str,
         DataSourceId: str,
         Name: str,
         DataSourceParameters: DataSourceParametersTypeDef = ...,
         Credentials: DataSourceCredentialsTypeDef = ...,
         VpcConnectionProperties: VpcConnectionPropertiesTypeDef = ...,
-        SslProperties: SslPropertiesTypeDef = ...
+        SslProperties: SslPropertiesTypeDef = ...,
     ) -> UpdateDataSourceResponseTypeDef:
         """
         Updates a data source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_data_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#update_data_source)
         """
 
     async def update_data_source_permissions(
         self,
         *,
         AwsAccountId: str,
         DataSourceId: str,
         GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...
+        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...,
     ) -> UpdateDataSourcePermissionsResponseTypeDef:
         """
         Updates the permissions to a data source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_data_source_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#update_data_source_permissions)
         """
@@ -2318,15 +2318,15 @@
 
     async def update_folder_permissions(
         self,
         *,
         AwsAccountId: str,
         FolderId: str,
         GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...
+        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...,
     ) -> UpdateFolderPermissionsResponseTypeDef:
         """
         Updates permissions of a folder.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_folder_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#update_folder_permissions)
         """
@@ -2345,29 +2345,29 @@
         self,
         *,
         AwsAccountId: str,
         AssignmentName: str,
         Namespace: str,
         AssignmentStatus: AssignmentStatusType = ...,
         PolicyArn: str = ...,
-        Identities: Mapping[str, Sequence[str]] = ...
+        Identities: Mapping[str, Sequence[str]] = ...,
     ) -> UpdateIAMPolicyAssignmentResponseTypeDef:
         """
         Updates an existing IAM policy assignment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_iam_policy_assignment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#update_iam_policy_assignment)
         """
 
     async def update_identity_propagation_config(
         self,
         *,
         AwsAccountId: str,
         Service: Literal["REDSHIFT"],
-        AuthorizedTargets: Sequence[str] = ...
+        AuthorizedTargets: Sequence[str] = ...,
     ) -> UpdateIdentityPropagationConfigResponseTypeDef:
         """
         Adds or updates services and authorized targets to configure what the Amazon
         QuickSight IAM Identity Center application can
         access.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_identity_propagation_config)
@@ -2375,15 +2375,15 @@
         """
 
     async def update_ip_restriction(
         self,
         *,
         AwsAccountId: str,
         IpRestrictionRuleMap: Mapping[str, str] = ...,
-        Enabled: bool = ...
+        Enabled: bool = ...,
     ) -> UpdateIpRestrictionResponseTypeDef:
         """
         Updates the content and status of IP rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_ip_restriction)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#update_ip_restriction)
         """
@@ -2425,15 +2425,15 @@
         *,
         AwsAccountId: str,
         TemplateId: str,
         SourceEntity: TemplateSourceEntityTypeDef = ...,
         VersionDescription: str = ...,
         Name: str = ...,
         Definition: TemplateVersionDefinitionTypeDef = ...,
-        ValidationStrategy: ValidationStrategyTypeDef = ...
+        ValidationStrategy: ValidationStrategyTypeDef = ...,
     ) -> UpdateTemplateResponseTypeDef:
         """
         Updates a template from an existing Amazon QuickSight analysis or another
         template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#update_template)
@@ -2451,15 +2451,15 @@
 
     async def update_template_permissions(
         self,
         *,
         AwsAccountId: str,
         TemplateId: str,
         GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...
+        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...,
     ) -> UpdateTemplatePermissionsResponseTypeDef:
         """
         Updates the resource permissions for a template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_template_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#update_template_permissions)
         """
@@ -2468,15 +2468,15 @@
         self,
         *,
         AwsAccountId: str,
         ThemeId: str,
         BaseThemeId: str,
         Name: str = ...,
         VersionDescription: str = ...,
-        Configuration: ThemeConfigurationTypeDef = ...
+        Configuration: ThemeConfigurationTypeDef = ...,
     ) -> UpdateThemeResponseTypeDef:
         """
         Updates a theme.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_theme)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#update_theme)
         """
@@ -2493,15 +2493,15 @@
 
     async def update_theme_permissions(
         self,
         *,
         AwsAccountId: str,
         ThemeId: str,
         GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...
+        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...,
     ) -> UpdateThemePermissionsResponseTypeDef:
         """
         Updates the resource permissions for a theme.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_theme_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#update_theme_permissions)
         """
@@ -2518,30 +2518,30 @@
 
     async def update_topic_permissions(
         self,
         *,
         AwsAccountId: str,
         TopicId: str,
         GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...
+        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...,
     ) -> UpdateTopicPermissionsResponseTypeDef:
         """
         Updates the permissions of a topic.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_topic_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#update_topic_permissions)
         """
 
     async def update_topic_refresh_schedule(
         self,
         *,
         AwsAccountId: str,
         TopicId: str,
         DatasetId: str,
-        RefreshSchedule: TopicRefreshScheduleTypeDef
+        RefreshSchedule: TopicRefreshScheduleTypeDef,
     ) -> UpdateTopicRefreshScheduleResponseTypeDef:
         """
         Updates a topic refresh schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_topic_refresh_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#update_topic_refresh_schedule)
         """
@@ -2554,15 +2554,15 @@
         Namespace: str,
         Email: str,
         Role: UserRoleType,
         CustomPermissionsName: str = ...,
         UnapplyCustomPermissions: bool = ...,
         ExternalLoginFederationProviderType: str = ...,
         CustomFederationProviderUrl: str = ...,
-        ExternalLoginId: str = ...
+        ExternalLoginId: str = ...,
     ) -> UpdateUserResponseTypeDef:
         """
         Updates an Amazon QuickSight user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#update_user)
         """
@@ -2572,15 +2572,15 @@
         *,
         AwsAccountId: str,
         VPCConnectionId: str,
         Name: str,
         SubnetIds: Sequence[str],
         SecurityGroupIds: Sequence[str],
         RoleArn: str,
-        DnsResolvers: Sequence[str] = ...
+        DnsResolvers: Sequence[str] = ...,
     ) -> UpdateVPCConnectionResponseTypeDef:
         """
         Updates a VPC connection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_vpc_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/client/#update_vpc_connection)
         """
```

### Comparing `types-aiobotocore-quicksight-2.9.0/types_aiobotocore_quicksight/literals.py` & `types-aiobotocore-quicksight-2.9.1/types_aiobotocore_quicksight/literals.py`

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
     "AnalysisErrorTypeType",
     "AnalysisFilterAttributeType",
     "AnchorOptionType",
     "ArcThicknessOptionsType",
     "ArcThicknessType",
     "AssetBundleExportFormatType",
@@ -260,15 +259,14 @@
     "QuickSightServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AnalysisErrorTypeType = Literal[
     "ACCESS_DENIED",
     "COLUMN_GEOGRAPHIC_ROLE_MISMATCH",
     "COLUMN_REPLACEMENT_MISSING",
     "COLUMN_TYPE_MISMATCH",
     "DATA_SET_NOT_FOUND",
     "INTERNAL_FAILURE",
```

### Comparing `types-aiobotocore-quicksight-2.9.0/types_aiobotocore_quicksight/literals.pyi` & `types-aiobotocore-quicksight-2.9.1/types_aiobotocore_quicksight/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-quicksight-2.9.0/types_aiobotocore_quicksight/paginator.py` & `types-aiobotocore-quicksight-2.9.1/types_aiobotocore_quicksight/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -158,15 +158,14 @@
     "SearchDashboardsPaginator",
     "SearchDataSetsPaginator",
     "SearchDataSourcesPaginator",
     "SearchFoldersPaginator",
     "SearchGroupsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -181,15 +180,15 @@
 
     def paginate(
         self,
         *,
         AwsAccountId: str,
         FolderId: str,
         Namespace: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeFolderPermissionsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Paginator.DescribeFolderPermissions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/paginators/#describefolderpermissionspaginator)
         """
 
 
@@ -201,15 +200,15 @@
 
     def paginate(
         self,
         *,
         AwsAccountId: str,
         FolderId: str,
         Namespace: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeFolderResolvedPermissionsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Paginator.DescribeFolderResolvedPermissions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/paginators/#describefolderresolvedpermissionspaginator)
         """
 
 
@@ -356,15 +355,15 @@
 
     def paginate(
         self,
         *,
         GroupName: str,
         AwsAccountId: str,
         Namespace: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListGroupMembershipsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Paginator.ListGroupMemberships.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/paginators/#listgroupmembershipspaginator)
         """
 
 
@@ -391,15 +390,15 @@
 
     def paginate(
         self,
         *,
         AwsAccountId: str,
         Namespace: str,
         AssignmentStatus: AssignmentStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListIAMPolicyAssignmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Paginator.ListIAMPolicyAssignments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/paginators/#listiampolicyassignmentspaginator)
         """
 
 
@@ -411,15 +410,15 @@
 
     def paginate(
         self,
         *,
         AwsAccountId: str,
         UserName: str,
         Namespace: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListIAMPolicyAssignmentsForUserResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Paginator.ListIAMPolicyAssignmentsForUser.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/paginators/#listiampolicyassignmentsforuserpaginator)
         """
 
 
@@ -461,15 +460,15 @@
 
     def paginate(
         self,
         *,
         Role: RoleType,
         AwsAccountId: str,
         Namespace: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRoleMembershipsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Paginator.ListRoleMemberships.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/paginators/#listrolemembershipspaginator)
         """
 
 
@@ -540,15 +539,15 @@
     """
 
     def paginate(
         self,
         *,
         AwsAccountId: str,
         Type: ThemeTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListThemesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Paginator.ListThemes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/paginators/#listthemespaginator)
         """
 
 
@@ -560,15 +559,15 @@
 
     def paginate(
         self,
         *,
         UserName: str,
         AwsAccountId: str,
         Namespace: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListUserGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Paginator.ListUserGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/paginators/#listusergroupspaginator)
         """
 
 
@@ -594,15 +593,15 @@
     """
 
     def paginate(
         self,
         *,
         AwsAccountId: str,
         Filters: Sequence[AnalysisSearchFilterTypeDef],
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchAnalysesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Paginator.SearchAnalyses.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/paginators/#searchanalysespaginator)
         """
 
 
@@ -613,15 +612,15 @@
     """
 
     def paginate(
         self,
         *,
         AwsAccountId: str,
         Filters: Sequence[DashboardSearchFilterTypeDef],
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchDashboardsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Paginator.SearchDashboards.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/paginators/#searchdashboardspaginator)
         """
 
 
@@ -632,15 +631,15 @@
     """
 
     def paginate(
         self,
         *,
         AwsAccountId: str,
         Filters: Sequence[DataSetSearchFilterTypeDef],
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchDataSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Paginator.SearchDataSets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/paginators/#searchdatasetspaginator)
         """
 
 
@@ -651,15 +650,15 @@
     """
 
     def paginate(
         self,
         *,
         AwsAccountId: str,
         Filters: Sequence[DataSourceSearchFilterTypeDef],
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchDataSourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Paginator.SearchDataSources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/paginators/#searchdatasourcespaginator)
         """
 
 
@@ -670,15 +669,15 @@
     """
 
     def paginate(
         self,
         *,
         AwsAccountId: str,
         Filters: Sequence[FolderSearchFilterTypeDef],
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchFoldersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Paginator.SearchFolders.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/paginators/#searchfolderspaginator)
         """
 
 
@@ -690,13 +689,13 @@
 
     def paginate(
         self,
         *,
         AwsAccountId: str,
         Namespace: str,
         Filters: Sequence[GroupSearchFilterTypeDef],
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Paginator.SearchGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/paginators/#searchgroupspaginator)
         """
```

### Comparing `types-aiobotocore-quicksight-2.9.0/types_aiobotocore_quicksight/paginator.pyi` & `types-aiobotocore-quicksight-2.9.1/types_aiobotocore_quicksight/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -178,15 +178,15 @@
 
     def paginate(
         self,
         *,
         AwsAccountId: str,
         FolderId: str,
         Namespace: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeFolderPermissionsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Paginator.DescribeFolderPermissions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/paginators/#describefolderpermissionspaginator)
         """
 
 class DescribeFolderResolvedPermissionsPaginator(AioPaginator):
@@ -197,15 +197,15 @@
 
     def paginate(
         self,
         *,
         AwsAccountId: str,
         FolderId: str,
         Namespace: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeFolderResolvedPermissionsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Paginator.DescribeFolderResolvedPermissions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/paginators/#describefolderresolvedpermissionspaginator)
         """
 
 class ListAnalysesPaginator(AioPaginator):
@@ -342,15 +342,15 @@
 
     def paginate(
         self,
         *,
         GroupName: str,
         AwsAccountId: str,
         Namespace: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListGroupMembershipsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Paginator.ListGroupMemberships.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/paginators/#listgroupmembershipspaginator)
         """
 
 class ListGroupsPaginator(AioPaginator):
@@ -375,15 +375,15 @@
 
     def paginate(
         self,
         *,
         AwsAccountId: str,
         Namespace: str,
         AssignmentStatus: AssignmentStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListIAMPolicyAssignmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Paginator.ListIAMPolicyAssignments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/paginators/#listiampolicyassignmentspaginator)
         """
 
 class ListIAMPolicyAssignmentsForUserPaginator(AioPaginator):
@@ -394,15 +394,15 @@
 
     def paginate(
         self,
         *,
         AwsAccountId: str,
         UserName: str,
         Namespace: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListIAMPolicyAssignmentsForUserResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Paginator.ListIAMPolicyAssignmentsForUser.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/paginators/#listiampolicyassignmentsforuserpaginator)
         """
 
 class ListIngestionsPaginator(AioPaginator):
@@ -441,15 +441,15 @@
 
     def paginate(
         self,
         *,
         Role: RoleType,
         AwsAccountId: str,
         Namespace: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRoleMembershipsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Paginator.ListRoleMemberships.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/paginators/#listrolemembershipspaginator)
         """
 
 class ListTemplateAliasesPaginator(AioPaginator):
@@ -515,15 +515,15 @@
     """
 
     def paginate(
         self,
         *,
         AwsAccountId: str,
         Type: ThemeTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListThemesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Paginator.ListThemes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/paginators/#listthemespaginator)
         """
 
 class ListUserGroupsPaginator(AioPaginator):
@@ -534,15 +534,15 @@
 
     def paginate(
         self,
         *,
         UserName: str,
         AwsAccountId: str,
         Namespace: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListUserGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Paginator.ListUserGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/paginators/#listusergroupspaginator)
         """
 
 class ListUsersPaginator(AioPaginator):
@@ -566,15 +566,15 @@
     """
 
     def paginate(
         self,
         *,
         AwsAccountId: str,
         Filters: Sequence[AnalysisSearchFilterTypeDef],
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchAnalysesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Paginator.SearchAnalyses.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/paginators/#searchanalysespaginator)
         """
 
 class SearchDashboardsPaginator(AioPaginator):
@@ -584,15 +584,15 @@
     """
 
     def paginate(
         self,
         *,
         AwsAccountId: str,
         Filters: Sequence[DashboardSearchFilterTypeDef],
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchDashboardsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Paginator.SearchDashboards.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/paginators/#searchdashboardspaginator)
         """
 
 class SearchDataSetsPaginator(AioPaginator):
@@ -602,15 +602,15 @@
     """
 
     def paginate(
         self,
         *,
         AwsAccountId: str,
         Filters: Sequence[DataSetSearchFilterTypeDef],
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchDataSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Paginator.SearchDataSets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/paginators/#searchdatasetspaginator)
         """
 
 class SearchDataSourcesPaginator(AioPaginator):
@@ -620,15 +620,15 @@
     """
 
     def paginate(
         self,
         *,
         AwsAccountId: str,
         Filters: Sequence[DataSourceSearchFilterTypeDef],
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchDataSourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Paginator.SearchDataSources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/paginators/#searchdatasourcespaginator)
         """
 
 class SearchFoldersPaginator(AioPaginator):
@@ -638,15 +638,15 @@
     """
 
     def paginate(
         self,
         *,
         AwsAccountId: str,
         Filters: Sequence[FolderSearchFilterTypeDef],
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchFoldersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Paginator.SearchFolders.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/paginators/#searchfolderspaginator)
         """
 
 class SearchGroupsPaginator(AioPaginator):
@@ -657,13 +657,13 @@
 
     def paginate(
         self,
         *,
         AwsAccountId: str,
         Namespace: str,
         Filters: Sequence[GroupSearchFilterTypeDef],
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Paginator.SearchGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/paginators/#searchgroupspaginator)
         """
```

### Comparing `types-aiobotocore-quicksight-2.9.0/types_aiobotocore_quicksight/type_defs.py` & `types-aiobotocore-quicksight-2.9.1/types_aiobotocore_quicksight/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,15 +215,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccountCustomizationTypeDef",
     "AccountInfoTypeDef",
     "AccountSettingsTypeDef",
     "ActiveIAMPolicyAssignmentTypeDef",
     "AdHocFilteringOptionTypeDef",
     "AttributeAggregationFunctionTypeDef",
```

### Comparing `types-aiobotocore-quicksight-2.9.0/types_aiobotocore_quicksight/type_defs.pyi` & `types-aiobotocore-quicksight-2.9.1/types_aiobotocore_quicksight/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-quicksight-2.9.0/types_aiobotocore_quicksight.egg-info/PKG-INFO` & `types-aiobotocore-quicksight-2.9.1/types_aiobotocore_quicksight.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-quicksight
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.QuickSight 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.QuickSight 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/
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
 
 <a id="types-aiobotocore-quicksight"></a>
 
 # types-aiobotocore-quicksight
 
 [![PyPI - types-aiobotocore-quicksight](https://img.shields.io/pypi/v/types-aiobotocore-quicksight.svg?color=blue)](https://pypi.org/project/types-aiobotocore-quicksight)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-quicksight.svg?color=blue)](https://pypi.org/project/types-aiobotocore-quicksight)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-quicksight)](https://pepy.tech/project/types-aiobotocore-quicksight)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.QuickSight 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight)
+[aiobotocore.QuickSight 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight)
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
 [types-aiobotocore-quicksight docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-quicksight-2.9.0/types_aiobotocore_quicksight.egg-info/SOURCES.txt` & `types-aiobotocore-quicksight-2.9.1/types_aiobotocore_quicksight.egg-info/SOURCES.txt`

 * *Files identical despite different names*

