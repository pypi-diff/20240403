# Comparing `tmp/types-aiobotocore-importexport-2.9.0.tar.gz` & `tmp/types-aiobotocore-importexport-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-importexport-2.9.0.tar", last modified: Wed Dec 13 19:59:28 2023, max compression
+gzip compressed data, was "types-aiobotocore-importexport-2.9.1.tar", last modified: Thu Jan 18 01:20:51 2024, max compression
```

## Comparing `types-aiobotocore-importexport-2.9.0.tar` & `types-aiobotocore-importexport-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:28.077689 types-aiobotocore-importexport-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:47:27.000000 types-aiobotocore-importexport-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13185 2023-12-13 19:59:28.077689 types-aiobotocore-importexport-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11602 2023-12-13 19:47:27.000000 types-aiobotocore-importexport-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:28.077689 types-aiobotocore-importexport-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2023-12-13 19:47:26.000000 types-aiobotocore-importexport-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:28.077689 types-aiobotocore-importexport-2.9.0/types_aiobotocore_importexport/
--rw-r--r--   0 runner    (1001) docker     (127)      652 2023-12-13 19:47:27.000000 types-aiobotocore-importexport-2.9.0/types_aiobotocore_importexport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2023-12-13 19:47:27.000000 types-aiobotocore-importexport-2.9.0/types_aiobotocore_importexport/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      952 2023-12-13 19:47:27.000000 types-aiobotocore-importexport-2.9.0/types_aiobotocore_importexport/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9856 2023-12-13 19:47:27.000000 types-aiobotocore-importexport-2.9.0/types_aiobotocore_importexport/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     9852 2023-12-13 19:47:27.000000 types-aiobotocore-importexport-2.9.0/types_aiobotocore_importexport/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8296 2023-12-13 19:47:27.000000 types-aiobotocore-importexport-2.9.0/types_aiobotocore_importexport/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8294 2023-12-13 19:47:27.000000 types-aiobotocore-importexport-2.9.0/types_aiobotocore_importexport/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2023-12-13 19:47:27.000000 types-aiobotocore-importexport-2.9.0/types_aiobotocore_importexport/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2023-12-13 19:47:27.000000 types-aiobotocore-importexport-2.9.0/types_aiobotocore_importexport/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:47:27.000000 types-aiobotocore-importexport-2.9.0/types_aiobotocore_importexport/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5580 2023-12-13 19:47:27.000000 types-aiobotocore-importexport-2.9.0/types_aiobotocore_importexport/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5579 2023-12-13 19:47:27.000000 types-aiobotocore-importexport-2.9.0/types_aiobotocore_importexport/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:47:27.000000 types-aiobotocore-importexport-2.9.0/types_aiobotocore_importexport/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:28.077689 types-aiobotocore-importexport-2.9.0/types_aiobotocore_importexport.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13185 2023-12-13 19:59:28.000000 types-aiobotocore-importexport-2.9.0/types_aiobotocore_importexport.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      908 2023-12-13 19:59:28.000000 types-aiobotocore-importexport-2.9.0/types_aiobotocore_importexport.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:28.000000 types-aiobotocore-importexport-2.9.0/types_aiobotocore_importexport.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:28.000000 types-aiobotocore-importexport-2.9.0/types_aiobotocore_importexport.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:28.000000 types-aiobotocore-importexport-2.9.0/types_aiobotocore_importexport.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-13 19:59:28.000000 types-aiobotocore-importexport-2.9.0/types_aiobotocore_importexport.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:51.901291 types-aiobotocore-importexport-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:09:19.000000 types-aiobotocore-importexport-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13205 2024-01-18 01:20:51.901291 types-aiobotocore-importexport-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11602 2024-01-18 01:09:19.000000 types-aiobotocore-importexport-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:51.901291 types-aiobotocore-importexport-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-01-18 01:09:19.000000 types-aiobotocore-importexport-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:51.901291 types-aiobotocore-importexport-2.9.1/types_aiobotocore_importexport/
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-01-18 01:09:19.000000 types-aiobotocore-importexport-2.9.1/types_aiobotocore_importexport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-01-18 01:09:19.000000 types-aiobotocore-importexport-2.9.1/types_aiobotocore_importexport/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-01-18 01:09:19.000000 types-aiobotocore-importexport-2.9.1/types_aiobotocore_importexport/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9858 2024-01-18 01:09:19.000000 types-aiobotocore-importexport-2.9.1/types_aiobotocore_importexport/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9855 2024-01-18 01:09:19.000000 types-aiobotocore-importexport-2.9.1/types_aiobotocore_importexport/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8294 2024-01-18 01:09:19.000000 types-aiobotocore-importexport-2.9.1/types_aiobotocore_importexport/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8294 2024-01-18 01:09:19.000000 types-aiobotocore-importexport-2.9.1/types_aiobotocore_importexport/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-01-18 01:09:19.000000 types-aiobotocore-importexport-2.9.1/types_aiobotocore_importexport/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-01-18 01:09:19.000000 types-aiobotocore-importexport-2.9.1/types_aiobotocore_importexport/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:09:19.000000 types-aiobotocore-importexport-2.9.1/types_aiobotocore_importexport/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-01-18 01:09:19.000000 types-aiobotocore-importexport-2.9.1/types_aiobotocore_importexport/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-01-18 01:09:19.000000 types-aiobotocore-importexport-2.9.1/types_aiobotocore_importexport/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:09:19.000000 types-aiobotocore-importexport-2.9.1/types_aiobotocore_importexport/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:51.901291 types-aiobotocore-importexport-2.9.1/types_aiobotocore_importexport.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13205 2024-01-18 01:20:51.000000 types-aiobotocore-importexport-2.9.1/types_aiobotocore_importexport.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-01-18 01:20:51.000000 types-aiobotocore-importexport-2.9.1/types_aiobotocore_importexport.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:51.000000 types-aiobotocore-importexport-2.9.1/types_aiobotocore_importexport.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:51.000000 types-aiobotocore-importexport-2.9.1/types_aiobotocore_importexport.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:51.000000 types-aiobotocore-importexport-2.9.1/types_aiobotocore_importexport.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-01-18 01:20:51.000000 types-aiobotocore-importexport-2.9.1/types_aiobotocore_importexport.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-importexport-2.9.0/LICENSE` & `types-aiobotocore-importexport-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-importexport-2.9.0/PKG-INFO` & `types-aiobotocore-importexport-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-importexport
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ImportExport 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ImportExport 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_importexport/
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
 
 <a id="types-aiobotocore-importexport"></a>
 
 # types-aiobotocore-importexport
 
 [![PyPI - types-aiobotocore-importexport](https://img.shields.io/pypi/v/types-aiobotocore-importexport.svg?color=blue)](https://pypi.org/project/types-aiobotocore-importexport)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-importexport.svg?color=blue)](https://pypi.org/project/types-aiobotocore-importexport)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_importexport/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-importexport)](https://pepy.tech/project/types-aiobotocore-importexport)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ImportExport 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport)
+[aiobotocore.ImportExport 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport)
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
 [types-aiobotocore-importexport docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_importexport/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-importexport-2.9.0/README.md` & `types-aiobotocore-importexport-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-importexport.svg?color=blue)](https://pypi.org/project/types-aiobotocore-importexport)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_importexport/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-importexport)](https://pepy.tech/project/types-aiobotocore-importexport)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ImportExport 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport)
+[aiobotocore.ImportExport 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport)
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
 [types-aiobotocore-importexport docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_importexport/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-importexport-2.9.0/setup.py` & `types-aiobotocore-importexport-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-importexport",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_importexport"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ImportExport 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.ImportExport 2.9.1 service generated with"
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
     keywords="aiobotocore importexport type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_importexport": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_importexport/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-importexport-2.9.0/types_aiobotocore_importexport/__init__.py` & `types-aiobotocore-importexport-2.9.1/types_aiobotocore_importexport/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,9 +22,8 @@
 """
 
 from .client import ImportExportClient
 from .paginator import ListJobsPaginator
 
 Client = ImportExportClient
 
-
 __all__ = ("Client", "ImportExportClient", "ListJobsPaginator")
```

### Comparing `types-aiobotocore-importexport-2.9.0/types_aiobotocore_importexport/__init__.pyi` & `types-aiobotocore-importexport-2.9.1/types_aiobotocore_importexport/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-importexport-2.9.0/types_aiobotocore_importexport/__main__.py` & `types-aiobotocore-importexport-2.9.1/types_aiobotocore_importexport/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ImportExport 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.ImportExport 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_importexport//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport\nOther"
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

### Comparing `types-aiobotocore-importexport-2.9.0/types_aiobotocore_importexport/client.py` & `types-aiobotocore-importexport-2.9.1/types_aiobotocore_importexport/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ImportExportClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -117,15 +116,15 @@
     async def create_job(
         self,
         *,
         JobType: JobTypeType,
         Manifest: str,
         ValidateOnly: bool,
         ManifestAddendum: str = ...,
-        APIVersion: str = ...
+        APIVersion: str = ...,
     ) -> CreateJobOutputTypeDef:
         """
         This operation initiates the process of scheduling an upload or download of
         your
         data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Client.create_job)
@@ -156,15 +155,15 @@
         country: str = ...,
         stateOrProvince: str = ...,
         city: str = ...,
         postalCode: str = ...,
         street1: str = ...,
         street2: str = ...,
         street3: str = ...,
-        APIVersion: str = ...
+        APIVersion: str = ...,
     ) -> GetShippingLabelOutputTypeDef:
         """
         This operation generates a pre-paid UPS shipping label that you will use to
         ship your device to AWS for
         processing.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Client.get_shipping_label)
@@ -195,15 +194,15 @@
     async def update_job(
         self,
         *,
         JobId: str,
         Manifest: str,
         JobType: JobTypeType,
         ValidateOnly: bool,
-        APIVersion: str = ...
+        APIVersion: str = ...,
     ) -> UpdateJobOutputTypeDef:
         """
         You use this operation to change the parameters specified in the original
         manifest file by supplying a new manifest
         file.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Client.update_job)
```

### Comparing `types-aiobotocore-importexport-2.9.0/types_aiobotocore_importexport/client.pyi` & `types-aiobotocore-importexport-2.9.1/types_aiobotocore_importexport/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
     async def create_job(
         self,
         *,
         JobType: JobTypeType,
         Manifest: str,
         ValidateOnly: bool,
         ManifestAddendum: str = ...,
-        APIVersion: str = ...
+        APIVersion: str = ...,
     ) -> CreateJobOutputTypeDef:
         """
         This operation initiates the process of scheduling an upload or download of
         your
         data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Client.create_job)
@@ -152,15 +152,15 @@
         country: str = ...,
         stateOrProvince: str = ...,
         city: str = ...,
         postalCode: str = ...,
         street1: str = ...,
         street2: str = ...,
         street3: str = ...,
-        APIVersion: str = ...
+        APIVersion: str = ...,
     ) -> GetShippingLabelOutputTypeDef:
         """
         This operation generates a pre-paid UPS shipping label that you will use to
         ship your device to AWS for
         processing.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Client.get_shipping_label)
@@ -191,15 +191,15 @@
     async def update_job(
         self,
         *,
         JobId: str,
         Manifest: str,
         JobType: JobTypeType,
         ValidateOnly: bool,
-        APIVersion: str = ...
+        APIVersion: str = ...,
     ) -> UpdateJobOutputTypeDef:
         """
         You use this operation to change the parameters specified in the original
         manifest file by supplying a new manifest
         file.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Client.update_job)
```

### Comparing `types-aiobotocore-importexport-2.9.0/types_aiobotocore_importexport/literals.py` & `types-aiobotocore-importexport-2.9.1/types_aiobotocore_importexport/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,25 +15,23 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "JobTypeType",
     "ListJobsPaginatorName",
     "ImportExportServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 JobTypeType = Literal["Export", "Import"]
 ListJobsPaginatorName = Literal["list_jobs"]
 ImportExportServiceName = Literal["importexport"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
```

### Comparing `types-aiobotocore-importexport-2.9.0/types_aiobotocore_importexport/literals.pyi` & `types-aiobotocore-importexport-2.9.1/types_aiobotocore_importexport/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-importexport-2.9.0/types_aiobotocore_importexport/paginator.py` & `types-aiobotocore-importexport-2.9.1/types_aiobotocore_importexport/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .type_defs import ListJobsOutputTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListJobsPaginator",)
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
```

### Comparing `types-aiobotocore-importexport-2.9.0/types_aiobotocore_importexport/paginator.pyi` & `types-aiobotocore-importexport-2.9.1/types_aiobotocore_importexport/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-importexport-2.9.0/types_aiobotocore_importexport/type_defs.py` & `types-aiobotocore-importexport-2.9.1/types_aiobotocore_importexport/type_defs.py`

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
     "ArtifactTypeDef",
     "CancelJobInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CreateJobInputRequestTypeDef",
     "GetShippingLabelInputRequestTypeDef",
     "GetStatusInputRequestTypeDef",
```

### Comparing `types-aiobotocore-importexport-2.9.0/types_aiobotocore_importexport/type_defs.pyi` & `types-aiobotocore-importexport-2.9.1/types_aiobotocore_importexport/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-importexport-2.9.0/types_aiobotocore_importexport.egg-info/PKG-INFO` & `types-aiobotocore-importexport-2.9.1/types_aiobotocore_importexport.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-importexport
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ImportExport 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ImportExport 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_importexport/
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
 
 <a id="types-aiobotocore-importexport"></a>
 
 # types-aiobotocore-importexport
 
 [![PyPI - types-aiobotocore-importexport](https://img.shields.io/pypi/v/types-aiobotocore-importexport.svg?color=blue)](https://pypi.org/project/types-aiobotocore-importexport)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-importexport.svg?color=blue)](https://pypi.org/project/types-aiobotocore-importexport)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_importexport/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-importexport)](https://pepy.tech/project/types-aiobotocore-importexport)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ImportExport 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport)
+[aiobotocore.ImportExport 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport)
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
 [types-aiobotocore-importexport docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_importexport/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-importexport-2.9.0/types_aiobotocore_importexport.egg-info/SOURCES.txt` & `types-aiobotocore-importexport-2.9.1/types_aiobotocore_importexport.egg-info/SOURCES.txt`

 * *Files identical despite different names*

