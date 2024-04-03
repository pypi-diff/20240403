# Comparing `tmp/types-aiobotocore-workdocs-2.9.0.tar.gz` & `tmp/types-aiobotocore-workdocs-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-workdocs-2.9.0.tar", last modified: Wed Dec 13 20:00:46 2023, max compression
+gzip compressed data, was "types-aiobotocore-workdocs-2.9.1.tar", last modified: Thu Jan 18 01:22:03 2024, max compression
```

## Comparing `types-aiobotocore-workdocs-2.9.0.tar` & `types-aiobotocore-workdocs-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:46.381002 types-aiobotocore-workdocs-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:57:58.000000 types-aiobotocore-workdocs-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14546 2023-12-13 20:00:46.381002 types-aiobotocore-workdocs-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12979 2023-12-13 19:57:58.000000 types-aiobotocore-workdocs-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:46.381002 types-aiobotocore-workdocs-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2023-12-13 19:57:58.000000 types-aiobotocore-workdocs-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:46.381002 types-aiobotocore-workdocs-2.9.0/types_aiobotocore_workdocs/
--rw-r--r--   0 runner    (1001) docker     (127)     2766 2023-12-13 19:57:58.000000 types-aiobotocore-workdocs-2.9.0/types_aiobotocore_workdocs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2023-12-13 19:57:58.000000 types-aiobotocore-workdocs-2.9.0/types_aiobotocore_workdocs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      936 2023-12-13 19:57:58.000000 types-aiobotocore-workdocs-2.9.0/types_aiobotocore_workdocs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40888 2023-12-13 19:57:58.000000 types-aiobotocore-workdocs-2.9.0/types_aiobotocore_workdocs/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    40884 2023-12-13 19:57:58.000000 types-aiobotocore-workdocs-2.9.0/types_aiobotocore_workdocs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14373 2023-12-13 19:57:58.000000 types-aiobotocore-workdocs-2.9.0/types_aiobotocore_workdocs/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    14371 2023-12-13 19:57:58.000000 types-aiobotocore-workdocs-2.9.0/types_aiobotocore_workdocs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14408 2023-12-13 19:57:58.000000 types-aiobotocore-workdocs-2.9.0/types_aiobotocore_workdocs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    14395 2023-12-13 19:57:58.000000 types-aiobotocore-workdocs-2.9.0/types_aiobotocore_workdocs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:57:58.000000 types-aiobotocore-workdocs-2.9.0/types_aiobotocore_workdocs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    38544 2023-12-13 19:57:59.000000 types-aiobotocore-workdocs-2.9.0/types_aiobotocore_workdocs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    38543 2023-12-13 19:57:59.000000 types-aiobotocore-workdocs-2.9.0/types_aiobotocore_workdocs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:57:58.000000 types-aiobotocore-workdocs-2.9.0/types_aiobotocore_workdocs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:46.381002 types-aiobotocore-workdocs-2.9.0/types_aiobotocore_workdocs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14546 2023-12-13 20:00:46.000000 types-aiobotocore-workdocs-2.9.0/types_aiobotocore_workdocs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      832 2023-12-13 20:00:46.000000 types-aiobotocore-workdocs-2.9.0/types_aiobotocore_workdocs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:46.000000 types-aiobotocore-workdocs-2.9.0/types_aiobotocore_workdocs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:46.000000 types-aiobotocore-workdocs-2.9.0/types_aiobotocore_workdocs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:46.000000 types-aiobotocore-workdocs-2.9.0/types_aiobotocore_workdocs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-13 20:00:46.000000 types-aiobotocore-workdocs-2.9.0/types_aiobotocore_workdocs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:22:03.304968 types-aiobotocore-workdocs-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:19:22.000000 types-aiobotocore-workdocs-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14566 2024-01-18 01:22:03.304968 types-aiobotocore-workdocs-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12979 2024-01-18 01:19:22.000000 types-aiobotocore-workdocs-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:22:03.304968 types-aiobotocore-workdocs-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-01-18 01:19:22.000000 types-aiobotocore-workdocs-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:22:03.300969 types-aiobotocore-workdocs-2.9.1/types_aiobotocore_workdocs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-01-18 01:19:22.000000 types-aiobotocore-workdocs-2.9.1/types_aiobotocore_workdocs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-01-18 01:19:22.000000 types-aiobotocore-workdocs-2.9.1/types_aiobotocore_workdocs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-01-18 01:19:22.000000 types-aiobotocore-workdocs-2.9.1/types_aiobotocore_workdocs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40913 2024-01-18 01:19:22.000000 types-aiobotocore-workdocs-2.9.1/types_aiobotocore_workdocs/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40910 2024-01-18 01:19:22.000000 types-aiobotocore-workdocs-2.9.1/types_aiobotocore_workdocs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14371 2024-01-18 01:19:23.000000 types-aiobotocore-workdocs-2.9.1/types_aiobotocore_workdocs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14371 2024-01-18 01:19:23.000000 types-aiobotocore-workdocs-2.9.1/types_aiobotocore_workdocs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14414 2024-01-18 01:19:22.000000 types-aiobotocore-workdocs-2.9.1/types_aiobotocore_workdocs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14403 2024-01-18 01:19:22.000000 types-aiobotocore-workdocs-2.9.1/types_aiobotocore_workdocs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:19:22.000000 types-aiobotocore-workdocs-2.9.1/types_aiobotocore_workdocs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    38543 2024-01-18 01:19:28.000000 types-aiobotocore-workdocs-2.9.1/types_aiobotocore_workdocs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38543 2024-01-18 01:19:27.000000 types-aiobotocore-workdocs-2.9.1/types_aiobotocore_workdocs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:19:22.000000 types-aiobotocore-workdocs-2.9.1/types_aiobotocore_workdocs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:22:03.304968 types-aiobotocore-workdocs-2.9.1/types_aiobotocore_workdocs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14566 2024-01-18 01:22:03.000000 types-aiobotocore-workdocs-2.9.1/types_aiobotocore_workdocs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-01-18 01:22:03.000000 types-aiobotocore-workdocs-2.9.1/types_aiobotocore_workdocs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:22:03.000000 types-aiobotocore-workdocs-2.9.1/types_aiobotocore_workdocs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:22:03.000000 types-aiobotocore-workdocs-2.9.1/types_aiobotocore_workdocs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:22:03.000000 types-aiobotocore-workdocs-2.9.1/types_aiobotocore_workdocs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-18 01:22:03.000000 types-aiobotocore-workdocs-2.9.1/types_aiobotocore_workdocs.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-workdocs-2.9.0/LICENSE` & `types-aiobotocore-workdocs-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-workdocs-2.9.0/PKG-INFO` & `types-aiobotocore-workdocs-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-workdocs
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.WorkDocs 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.WorkDocs 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/
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
 
 <a id="types-aiobotocore-workdocs"></a>
 
 # types-aiobotocore-workdocs
 
 [![PyPI - types-aiobotocore-workdocs](https://img.shields.io/pypi/v/types-aiobotocore-workdocs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-workdocs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-workdocs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-workdocs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-workdocs)](https://pepy.tech/project/types-aiobotocore-workdocs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.WorkDocs 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs)
+[aiobotocore.WorkDocs 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs)
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
 [types-aiobotocore-workdocs docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-workdocs-2.9.0/README.md` & `types-aiobotocore-workdocs-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-workdocs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-workdocs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-workdocs)](https://pepy.tech/project/types-aiobotocore-workdocs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.WorkDocs 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs)
+[aiobotocore.WorkDocs 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs)
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
 [types-aiobotocore-workdocs docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-workdocs-2.9.0/setup.py` & `types-aiobotocore-workdocs-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-workdocs",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_workdocs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.WorkDocs 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.WorkDocs 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore workdocs type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_workdocs": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-workdocs-2.9.0/types_aiobotocore_workdocs/__init__.py` & `types-aiobotocore-workdocs-2.9.1/types_aiobotocore_workdocs/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,14 @@
     DescribeRootFoldersPaginator,
     DescribeUsersPaginator,
     SearchResourcesPaginator,
 )
 
 Client = WorkDocsClient
 
-
 __all__ = (
     "Client",
     "DescribeActivitiesPaginator",
     "DescribeCommentsPaginator",
     "DescribeDocumentVersionsPaginator",
     "DescribeFolderContentsPaginator",
     "DescribeGroupsPaginator",
```

### Comparing `types-aiobotocore-workdocs-2.9.0/types_aiobotocore_workdocs/__init__.pyi` & `types-aiobotocore-workdocs-2.9.1/types_aiobotocore_workdocs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workdocs-2.9.0/types_aiobotocore_workdocs/__main__.py` & `types-aiobotocore-workdocs-2.9.1/types_aiobotocore_workdocs/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.WorkDocs 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.WorkDocs 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs\nOther"
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

### Comparing `types-aiobotocore-workdocs-2.9.0/types_aiobotocore_workdocs/client.py` & `types-aiobotocore-workdocs-2.9.1/types_aiobotocore_workdocs/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("WorkDocsClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -170,15 +169,15 @@
 
     async def add_resource_permissions(
         self,
         *,
         ResourceId: str,
         Principals: Sequence[SharePrincipalTypeDef],
         AuthenticationToken: str = ...,
-        NotificationOptions: NotificationOptionsTypeDef = ...
+        NotificationOptions: NotificationOptionsTypeDef = ...,
     ) -> AddResourcePermissionsResponseTypeDef:
         """
         Creates a set of permissions for the specified folder or document.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.add_resource_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/client/#add_resource_permissions)
         """
@@ -205,30 +204,30 @@
         DocumentId: str,
         VersionId: str,
         Text: str,
         AuthenticationToken: str = ...,
         ParentId: str = ...,
         ThreadId: str = ...,
         Visibility: CommentVisibilityTypeType = ...,
-        NotifyCollaborators: bool = ...
+        NotifyCollaborators: bool = ...,
     ) -> CreateCommentResponseTypeDef:
         """
         Adds a new comment to the specified document version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.create_comment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/client/#create_comment)
         """
 
     async def create_custom_metadata(
         self,
         *,
         ResourceId: str,
         CustomMetadata: Mapping[str, str],
         AuthenticationToken: str = ...,
-        VersionId: str = ...
+        VersionId: str = ...,
     ) -> Dict[str, Any]:
         """
         Adds one or more custom properties to the specified resource (a folder,
         document, or
         version).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.create_custom_metadata)
@@ -259,15 +258,15 @@
 
     async def create_notification_subscription(
         self,
         *,
         OrganizationId: str,
         Endpoint: str,
         Protocol: SubscriptionProtocolTypeType,
-        SubscriptionType: Literal["ALL"]
+        SubscriptionType: Literal["ALL"],
     ) -> CreateNotificationSubscriptionResponseTypeDef:
         """
         Configure Amazon WorkDocs to use Amazon SNS notifications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.create_notification_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/client/#create_notification_subscription)
         """
@@ -279,15 +278,15 @@
         GivenName: str,
         Surname: str,
         Password: str,
         OrganizationId: str = ...,
         EmailAddress: str = ...,
         TimeZoneId: str = ...,
         StorageRule: StorageRuleTypeTypeDef = ...,
-        AuthenticationToken: str = ...
+        AuthenticationToken: str = ...,
     ) -> CreateUserResponseTypeDef:
         """
         Creates a user in a Simple AD or Microsoft AD directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.create_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/client/#create_user)
         """
@@ -316,15 +315,15 @@
     async def delete_custom_metadata(
         self,
         *,
         ResourceId: str,
         AuthenticationToken: str = ...,
         VersionId: str = ...,
         Keys: Sequence[str] = ...,
-        DeleteAll: bool = ...
+        DeleteAll: bool = ...,
     ) -> Dict[str, Any]:
         """
         Deletes custom metadata from the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.delete_custom_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/client/#delete_custom_metadata)
         """
@@ -341,15 +340,15 @@
 
     async def delete_document_version(
         self,
         *,
         DocumentId: str,
         VersionId: str,
         DeletePriorVersions: bool,
-        AuthenticationToken: str = ...
+        AuthenticationToken: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a specific version of a document.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.delete_document_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/client/#delete_document_version)
         """
@@ -376,15 +375,15 @@
 
     async def delete_labels(
         self,
         *,
         ResourceId: str,
         AuthenticationToken: str = ...,
         Labels: Sequence[str] = ...,
-        DeleteAll: bool = ...
+        DeleteAll: bool = ...,
     ) -> Dict[str, Any]:
         """
         Deletes the specified list of labels from a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.delete_labels)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/client/#delete_labels)
         """
@@ -417,15 +416,15 @@
         EndTime: TimestampTypeDef = ...,
         OrganizationId: str = ...,
         ActivityTypes: str = ...,
         ResourceId: str = ...,
         UserId: str = ...,
         IncludeIndirectActivities: bool = ...,
         Limit: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DescribeActivitiesResponseTypeDef:
         """
         Describes the user activities in a specified time period.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.describe_activities)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/client/#describe_activities)
         """
@@ -433,15 +432,15 @@
     async def describe_comments(
         self,
         *,
         DocumentId: str,
         VersionId: str,
         AuthenticationToken: str = ...,
         Limit: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DescribeCommentsResponseTypeDef:
         """
         List all the comments for the specified document version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.describe_comments)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/client/#describe_comments)
         """
@@ -450,15 +449,15 @@
         self,
         *,
         DocumentId: str,
         AuthenticationToken: str = ...,
         Marker: str = ...,
         Limit: int = ...,
         Include: str = ...,
-        Fields: str = ...
+        Fields: str = ...,
     ) -> DescribeDocumentVersionsResponseTypeDef:
         """
         Retrieves the document versions for the specified document.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.describe_document_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/client/#describe_document_versions)
         """
@@ -469,15 +468,15 @@
         FolderId: str,
         AuthenticationToken: str = ...,
         Sort: ResourceSortTypeType = ...,
         Order: OrderTypeType = ...,
         Limit: int = ...,
         Marker: str = ...,
         Type: FolderContentTypeType = ...,
-        Include: str = ...
+        Include: str = ...,
     ) -> DescribeFolderContentsResponseTypeDef:
         """
         Describes the contents of the specified folder, including its documents and
         subfolders.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.describe_folder_contents)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/client/#describe_folder_contents)
@@ -486,15 +485,15 @@
     async def describe_groups(
         self,
         *,
         SearchQuery: str,
         AuthenticationToken: str = ...,
         OrganizationId: str = ...,
         Marker: str = ...,
-        Limit: int = ...
+        Limit: int = ...,
     ) -> DescribeGroupsResponseTypeDef:
         """
         Describes the groups specified by the query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.describe_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/client/#describe_groups)
         """
@@ -512,15 +511,15 @@
     async def describe_resource_permissions(
         self,
         *,
         ResourceId: str,
         AuthenticationToken: str = ...,
         PrincipalId: str = ...,
         Limit: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DescribeResourcePermissionsResponseTypeDef:
         """
         Describes the permissions of a specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.describe_resource_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/client/#describe_resource_permissions)
         """
@@ -544,15 +543,15 @@
         UserIds: str = ...,
         Query: str = ...,
         Include: UserFilterTypeType = ...,
         Order: OrderTypeType = ...,
         Sort: UserSortTypeType = ...,
         Marker: str = ...,
         Limit: int = ...,
-        Fields: str = ...
+        Fields: str = ...,
     ) -> DescribeUsersResponseTypeDef:
         """
         Describes the specified users.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.describe_users)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/client/#describe_users)
         """
@@ -593,15 +592,15 @@
     async def get_document_path(
         self,
         *,
         DocumentId: str,
         AuthenticationToken: str = ...,
         Limit: int = ...,
         Fields: str = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> GetDocumentPathResponseTypeDef:
         """
         Retrieves the path information (the hierarchy from the root folder) for the
         requested
         document.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.get_document_path)
@@ -611,15 +610,15 @@
     async def get_document_version(
         self,
         *,
         DocumentId: str,
         VersionId: str,
         AuthenticationToken: str = ...,
         Fields: str = ...,
-        IncludeCustomMetadata: bool = ...
+        IncludeCustomMetadata: bool = ...,
     ) -> GetDocumentVersionResponseTypeDef:
         """
         Retrieves version metadata for the specified document.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.get_document_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/client/#get_document_version)
         """
@@ -637,15 +636,15 @@
     async def get_folder_path(
         self,
         *,
         FolderId: str,
         AuthenticationToken: str = ...,
         Limit: int = ...,
         Fields: str = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> GetFolderPathResponseTypeDef:
         """
         Retrieves the path information (the hierarchy from the root folder) for the
         specified
         folder.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.get_folder_path)
@@ -655,15 +654,15 @@
     async def get_resources(
         self,
         *,
         AuthenticationToken: str = ...,
         UserId: str = ...,
         CollectionType: Literal["SHARED_WITH_ME"] = ...,
         Limit: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> GetResourcesResponseTypeDef:
         """
         Retrieves a collection of resources, including folders and documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.get_resources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/client/#get_resources)
         """
@@ -674,15 +673,15 @@
         AuthenticationToken: str = ...,
         Id: str = ...,
         Name: str = ...,
         ContentCreatedTimestamp: TimestampTypeDef = ...,
         ContentModifiedTimestamp: TimestampTypeDef = ...,
         ContentType: str = ...,
         DocumentSizeInBytes: int = ...,
-        ParentFolderId: str = ...
+        ParentFolderId: str = ...,
     ) -> InitiateDocumentVersionUploadResponseTypeDef:
         """
         Creates a new document object and version object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.initiate_document_version_upload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/client/#initiate_document_version_upload)
         """
@@ -699,15 +698,15 @@
 
     async def remove_resource_permission(
         self,
         *,
         ResourceId: str,
         PrincipalId: str,
         AuthenticationToken: str = ...,
-        PrincipalType: PrincipalTypeType = ...
+        PrincipalType: PrincipalTypeType = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Removes the permission for the specified principal from the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.remove_resource_permission)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/client/#remove_resource_permission)
         """
@@ -729,15 +728,15 @@
         QueryText: str = ...,
         QueryScopes: Sequence[SearchQueryScopeTypeType] = ...,
         OrganizationId: str = ...,
         AdditionalResponseFields: Sequence[Literal["WEBURL"]] = ...,
         Filters: FiltersTypeDef = ...,
         OrderBy: Sequence[SearchSortResultTypeDef] = ...,
         Limit: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> SearchResourcesResponseTypeDef:
         """
         Searches metadata and the content of folders, documents, document versions, and
         comments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.search_resources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/client/#search_resources)
@@ -746,30 +745,30 @@
     async def update_document(
         self,
         *,
         DocumentId: str,
         AuthenticationToken: str = ...,
         Name: str = ...,
         ParentFolderId: str = ...,
-        ResourceState: ResourceStateTypeType = ...
+        ResourceState: ResourceStateTypeType = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates the specified attributes of a document.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.update_document)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/client/#update_document)
         """
 
     async def update_document_version(
         self,
         *,
         DocumentId: str,
         VersionId: str,
         AuthenticationToken: str = ...,
-        VersionStatus: Literal["ACTIVE"] = ...
+        VersionStatus: Literal["ACTIVE"] = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Changes the status of the document version to ACTIVE.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.update_document_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/client/#update_document_version)
         """
@@ -777,15 +776,15 @@
     async def update_folder(
         self,
         *,
         FolderId: str,
         AuthenticationToken: str = ...,
         Name: str = ...,
         ParentFolderId: str = ...,
-        ResourceState: ResourceStateTypeType = ...
+        ResourceState: ResourceStateTypeType = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates the specified attributes of the specified folder.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.update_folder)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/client/#update_folder)
         """
@@ -797,15 +796,15 @@
         AuthenticationToken: str = ...,
         GivenName: str = ...,
         Surname: str = ...,
         Type: UserTypeType = ...,
         StorageRule: StorageRuleTypeTypeDef = ...,
         TimeZoneId: str = ...,
         Locale: LocaleTypeType = ...,
-        GrantPoweruserPrivileges: BooleanEnumTypeType = ...
+        GrantPoweruserPrivileges: BooleanEnumTypeType = ...,
     ) -> UpdateUserResponseTypeDef:
         """
         Updates the specified attributes of the specified user, and grants or revokes
         administrative privileges to the Amazon WorkDocs
         site.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.update_user)
```

### Comparing `types-aiobotocore-workdocs-2.9.0/types_aiobotocore_workdocs/client.pyi` & `types-aiobotocore-workdocs-2.9.1/types_aiobotocore_workdocs/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -166,15 +166,15 @@
 
     async def add_resource_permissions(
         self,
         *,
         ResourceId: str,
         Principals: Sequence[SharePrincipalTypeDef],
         AuthenticationToken: str = ...,
-        NotificationOptions: NotificationOptionsTypeDef = ...
+        NotificationOptions: NotificationOptionsTypeDef = ...,
     ) -> AddResourcePermissionsResponseTypeDef:
         """
         Creates a set of permissions for the specified folder or document.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.add_resource_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/client/#add_resource_permissions)
         """
@@ -201,30 +201,30 @@
         DocumentId: str,
         VersionId: str,
         Text: str,
         AuthenticationToken: str = ...,
         ParentId: str = ...,
         ThreadId: str = ...,
         Visibility: CommentVisibilityTypeType = ...,
-        NotifyCollaborators: bool = ...
+        NotifyCollaborators: bool = ...,
     ) -> CreateCommentResponseTypeDef:
         """
         Adds a new comment to the specified document version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.create_comment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/client/#create_comment)
         """
 
     async def create_custom_metadata(
         self,
         *,
         ResourceId: str,
         CustomMetadata: Mapping[str, str],
         AuthenticationToken: str = ...,
-        VersionId: str = ...
+        VersionId: str = ...,
     ) -> Dict[str, Any]:
         """
         Adds one or more custom properties to the specified resource (a folder,
         document, or
         version).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.create_custom_metadata)
@@ -255,15 +255,15 @@
 
     async def create_notification_subscription(
         self,
         *,
         OrganizationId: str,
         Endpoint: str,
         Protocol: SubscriptionProtocolTypeType,
-        SubscriptionType: Literal["ALL"]
+        SubscriptionType: Literal["ALL"],
     ) -> CreateNotificationSubscriptionResponseTypeDef:
         """
         Configure Amazon WorkDocs to use Amazon SNS notifications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.create_notification_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/client/#create_notification_subscription)
         """
@@ -275,15 +275,15 @@
         GivenName: str,
         Surname: str,
         Password: str,
         OrganizationId: str = ...,
         EmailAddress: str = ...,
         TimeZoneId: str = ...,
         StorageRule: StorageRuleTypeTypeDef = ...,
-        AuthenticationToken: str = ...
+        AuthenticationToken: str = ...,
     ) -> CreateUserResponseTypeDef:
         """
         Creates a user in a Simple AD or Microsoft AD directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.create_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/client/#create_user)
         """
@@ -312,15 +312,15 @@
     async def delete_custom_metadata(
         self,
         *,
         ResourceId: str,
         AuthenticationToken: str = ...,
         VersionId: str = ...,
         Keys: Sequence[str] = ...,
-        DeleteAll: bool = ...
+        DeleteAll: bool = ...,
     ) -> Dict[str, Any]:
         """
         Deletes custom metadata from the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.delete_custom_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/client/#delete_custom_metadata)
         """
@@ -337,15 +337,15 @@
 
     async def delete_document_version(
         self,
         *,
         DocumentId: str,
         VersionId: str,
         DeletePriorVersions: bool,
-        AuthenticationToken: str = ...
+        AuthenticationToken: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a specific version of a document.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.delete_document_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/client/#delete_document_version)
         """
@@ -372,15 +372,15 @@
 
     async def delete_labels(
         self,
         *,
         ResourceId: str,
         AuthenticationToken: str = ...,
         Labels: Sequence[str] = ...,
-        DeleteAll: bool = ...
+        DeleteAll: bool = ...,
     ) -> Dict[str, Any]:
         """
         Deletes the specified list of labels from a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.delete_labels)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/client/#delete_labels)
         """
@@ -413,15 +413,15 @@
         EndTime: TimestampTypeDef = ...,
         OrganizationId: str = ...,
         ActivityTypes: str = ...,
         ResourceId: str = ...,
         UserId: str = ...,
         IncludeIndirectActivities: bool = ...,
         Limit: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DescribeActivitiesResponseTypeDef:
         """
         Describes the user activities in a specified time period.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.describe_activities)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/client/#describe_activities)
         """
@@ -429,15 +429,15 @@
     async def describe_comments(
         self,
         *,
         DocumentId: str,
         VersionId: str,
         AuthenticationToken: str = ...,
         Limit: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DescribeCommentsResponseTypeDef:
         """
         List all the comments for the specified document version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.describe_comments)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/client/#describe_comments)
         """
@@ -446,15 +446,15 @@
         self,
         *,
         DocumentId: str,
         AuthenticationToken: str = ...,
         Marker: str = ...,
         Limit: int = ...,
         Include: str = ...,
-        Fields: str = ...
+        Fields: str = ...,
     ) -> DescribeDocumentVersionsResponseTypeDef:
         """
         Retrieves the document versions for the specified document.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.describe_document_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/client/#describe_document_versions)
         """
@@ -465,15 +465,15 @@
         FolderId: str,
         AuthenticationToken: str = ...,
         Sort: ResourceSortTypeType = ...,
         Order: OrderTypeType = ...,
         Limit: int = ...,
         Marker: str = ...,
         Type: FolderContentTypeType = ...,
-        Include: str = ...
+        Include: str = ...,
     ) -> DescribeFolderContentsResponseTypeDef:
         """
         Describes the contents of the specified folder, including its documents and
         subfolders.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.describe_folder_contents)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/client/#describe_folder_contents)
@@ -482,15 +482,15 @@
     async def describe_groups(
         self,
         *,
         SearchQuery: str,
         AuthenticationToken: str = ...,
         OrganizationId: str = ...,
         Marker: str = ...,
-        Limit: int = ...
+        Limit: int = ...,
     ) -> DescribeGroupsResponseTypeDef:
         """
         Describes the groups specified by the query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.describe_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/client/#describe_groups)
         """
@@ -508,15 +508,15 @@
     async def describe_resource_permissions(
         self,
         *,
         ResourceId: str,
         AuthenticationToken: str = ...,
         PrincipalId: str = ...,
         Limit: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DescribeResourcePermissionsResponseTypeDef:
         """
         Describes the permissions of a specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.describe_resource_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/client/#describe_resource_permissions)
         """
@@ -540,15 +540,15 @@
         UserIds: str = ...,
         Query: str = ...,
         Include: UserFilterTypeType = ...,
         Order: OrderTypeType = ...,
         Sort: UserSortTypeType = ...,
         Marker: str = ...,
         Limit: int = ...,
-        Fields: str = ...
+        Fields: str = ...,
     ) -> DescribeUsersResponseTypeDef:
         """
         Describes the specified users.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.describe_users)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/client/#describe_users)
         """
@@ -589,15 +589,15 @@
     async def get_document_path(
         self,
         *,
         DocumentId: str,
         AuthenticationToken: str = ...,
         Limit: int = ...,
         Fields: str = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> GetDocumentPathResponseTypeDef:
         """
         Retrieves the path information (the hierarchy from the root folder) for the
         requested
         document.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.get_document_path)
@@ -607,15 +607,15 @@
     async def get_document_version(
         self,
         *,
         DocumentId: str,
         VersionId: str,
         AuthenticationToken: str = ...,
         Fields: str = ...,
-        IncludeCustomMetadata: bool = ...
+        IncludeCustomMetadata: bool = ...,
     ) -> GetDocumentVersionResponseTypeDef:
         """
         Retrieves version metadata for the specified document.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.get_document_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/client/#get_document_version)
         """
@@ -633,15 +633,15 @@
     async def get_folder_path(
         self,
         *,
         FolderId: str,
         AuthenticationToken: str = ...,
         Limit: int = ...,
         Fields: str = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> GetFolderPathResponseTypeDef:
         """
         Retrieves the path information (the hierarchy from the root folder) for the
         specified
         folder.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.get_folder_path)
@@ -651,15 +651,15 @@
     async def get_resources(
         self,
         *,
         AuthenticationToken: str = ...,
         UserId: str = ...,
         CollectionType: Literal["SHARED_WITH_ME"] = ...,
         Limit: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> GetResourcesResponseTypeDef:
         """
         Retrieves a collection of resources, including folders and documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.get_resources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/client/#get_resources)
         """
@@ -670,15 +670,15 @@
         AuthenticationToken: str = ...,
         Id: str = ...,
         Name: str = ...,
         ContentCreatedTimestamp: TimestampTypeDef = ...,
         ContentModifiedTimestamp: TimestampTypeDef = ...,
         ContentType: str = ...,
         DocumentSizeInBytes: int = ...,
-        ParentFolderId: str = ...
+        ParentFolderId: str = ...,
     ) -> InitiateDocumentVersionUploadResponseTypeDef:
         """
         Creates a new document object and version object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.initiate_document_version_upload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/client/#initiate_document_version_upload)
         """
@@ -695,15 +695,15 @@
 
     async def remove_resource_permission(
         self,
         *,
         ResourceId: str,
         PrincipalId: str,
         AuthenticationToken: str = ...,
-        PrincipalType: PrincipalTypeType = ...
+        PrincipalType: PrincipalTypeType = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Removes the permission for the specified principal from the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.remove_resource_permission)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/client/#remove_resource_permission)
         """
@@ -725,15 +725,15 @@
         QueryText: str = ...,
         QueryScopes: Sequence[SearchQueryScopeTypeType] = ...,
         OrganizationId: str = ...,
         AdditionalResponseFields: Sequence[Literal["WEBURL"]] = ...,
         Filters: FiltersTypeDef = ...,
         OrderBy: Sequence[SearchSortResultTypeDef] = ...,
         Limit: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> SearchResourcesResponseTypeDef:
         """
         Searches metadata and the content of folders, documents, document versions, and
         comments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.search_resources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/client/#search_resources)
@@ -742,30 +742,30 @@
     async def update_document(
         self,
         *,
         DocumentId: str,
         AuthenticationToken: str = ...,
         Name: str = ...,
         ParentFolderId: str = ...,
-        ResourceState: ResourceStateTypeType = ...
+        ResourceState: ResourceStateTypeType = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates the specified attributes of a document.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.update_document)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/client/#update_document)
         """
 
     async def update_document_version(
         self,
         *,
         DocumentId: str,
         VersionId: str,
         AuthenticationToken: str = ...,
-        VersionStatus: Literal["ACTIVE"] = ...
+        VersionStatus: Literal["ACTIVE"] = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Changes the status of the document version to ACTIVE.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.update_document_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/client/#update_document_version)
         """
@@ -773,15 +773,15 @@
     async def update_folder(
         self,
         *,
         FolderId: str,
         AuthenticationToken: str = ...,
         Name: str = ...,
         ParentFolderId: str = ...,
-        ResourceState: ResourceStateTypeType = ...
+        ResourceState: ResourceStateTypeType = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates the specified attributes of the specified folder.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.update_folder)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/client/#update_folder)
         """
@@ -793,15 +793,15 @@
         AuthenticationToken: str = ...,
         GivenName: str = ...,
         Surname: str = ...,
         Type: UserTypeType = ...,
         StorageRule: StorageRuleTypeTypeDef = ...,
         TimeZoneId: str = ...,
         Locale: LocaleTypeType = ...,
-        GrantPoweruserPrivileges: BooleanEnumTypeType = ...
+        GrantPoweruserPrivileges: BooleanEnumTypeType = ...,
     ) -> UpdateUserResponseTypeDef:
         """
         Updates the specified attributes of the specified user, and grants or revokes
         administrative privileges to the Amazon WorkDocs
         site.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.update_user)
```

### Comparing `types-aiobotocore-workdocs-2.9.0/types_aiobotocore_workdocs/literals.py` & `types-aiobotocore-workdocs-2.9.1/types_aiobotocore_workdocs/literals.py`

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
     "ActivityTypeType",
     "AdditionalResponseFieldTypeType",
     "BooleanEnumTypeType",
     "CommentStatusTypeType",
     "CommentVisibilityTypeType",
     "ContentCategoryTypeType",
@@ -70,15 +69,14 @@
     "WorkDocsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ActivityTypeType = Literal[
     "DOCUMENT_ANNOTATION_ADDED",
     "DOCUMENT_ANNOTATION_DELETED",
     "DOCUMENT_CHECKED_IN",
     "DOCUMENT_CHECKED_OUT",
     "DOCUMENT_COMMENT_ADDED",
     "DOCUMENT_COMMENT_DELETED",
```

### Comparing `types-aiobotocore-workdocs-2.9.0/types_aiobotocore_workdocs/literals.pyi` & `types-aiobotocore-workdocs-2.9.1/types_aiobotocore_workdocs/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workdocs-2.9.0/types_aiobotocore_workdocs/paginator.py` & `types-aiobotocore-workdocs-2.9.1/types_aiobotocore_workdocs/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,29 +71,27 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "DescribeActivitiesPaginator",
     "DescribeCommentsPaginator",
     "DescribeDocumentVersionsPaginator",
     "DescribeFolderContentsPaginator",
     "DescribeGroupsPaginator",
     "DescribeNotificationSubscriptionsPaginator",
     "DescribeResourcePermissionsPaginator",
     "DescribeRootFoldersPaginator",
     "DescribeUsersPaginator",
     "SearchResourcesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -113,15 +111,15 @@
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         OrganizationId: str = ...,
         ActivityTypes: str = ...,
         ResourceId: str = ...,
         UserId: str = ...,
         IncludeIndirectActivities: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeActivitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeActivities.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/paginators/#describeactivitiespaginator)
         """
 
 
@@ -133,15 +131,15 @@
 
     def paginate(
         self,
         *,
         DocumentId: str,
         VersionId: str,
         AuthenticationToken: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeCommentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeComments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/paginators/#describecommentspaginator)
         """
 
 
@@ -154,15 +152,15 @@
     def paginate(
         self,
         *,
         DocumentId: str,
         AuthenticationToken: str = ...,
         Include: str = ...,
         Fields: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeDocumentVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeDocumentVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/paginators/#describedocumentversionspaginator)
         """
 
 
@@ -177,15 +175,15 @@
         *,
         FolderId: str,
         AuthenticationToken: str = ...,
         Sort: ResourceSortTypeType = ...,
         Order: OrderTypeType = ...,
         Type: FolderContentTypeType = ...,
         Include: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeFolderContentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeFolderContents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/paginators/#describefoldercontentspaginator)
         """
 
 
@@ -197,15 +195,15 @@
 
     def paginate(
         self,
         *,
         SearchQuery: str,
         AuthenticationToken: str = ...,
         OrganizationId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/paginators/#describegroupspaginator)
         """
 
 
@@ -232,15 +230,15 @@
 
     def paginate(
         self,
         *,
         ResourceId: str,
         AuthenticationToken: str = ...,
         PrincipalId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeResourcePermissionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeResourcePermissions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/paginators/#describeresourcepermissionspaginator)
         """
 
 
@@ -272,15 +270,15 @@
         OrganizationId: str = ...,
         UserIds: str = ...,
         Query: str = ...,
         Include: UserFilterTypeType = ...,
         Order: OrderTypeType = ...,
         Sort: UserSortTypeType = ...,
         Fields: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeUsers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/paginators/#describeuserspaginator)
         """
 
 
@@ -296,13 +294,13 @@
         AuthenticationToken: str = ...,
         QueryText: str = ...,
         QueryScopes: Sequence[SearchQueryScopeTypeType] = ...,
         OrganizationId: str = ...,
         AdditionalResponseFields: Sequence[Literal["WEBURL"]] = ...,
         Filters: FiltersTypeDef = ...,
         OrderBy: Sequence[SearchSortResultTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.SearchResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/paginators/#searchresourcespaginator)
         """
```

### Comparing `types-aiobotocore-workdocs-2.9.0/types_aiobotocore_workdocs/paginator.pyi` & `types-aiobotocore-workdocs-2.9.1/types_aiobotocore_workdocs/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         OrganizationId: str = ...,
         ActivityTypes: str = ...,
         ResourceId: str = ...,
         UserId: str = ...,
         IncludeIndirectActivities: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeActivitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeActivities.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/paginators/#describeactivitiespaginator)
         """
 
 class DescribeCommentsPaginator(AioPaginator):
@@ -128,15 +128,15 @@
 
     def paginate(
         self,
         *,
         DocumentId: str,
         VersionId: str,
         AuthenticationToken: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeCommentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeComments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/paginators/#describecommentspaginator)
         """
 
 class DescribeDocumentVersionsPaginator(AioPaginator):
@@ -148,15 +148,15 @@
     def paginate(
         self,
         *,
         DocumentId: str,
         AuthenticationToken: str = ...,
         Include: str = ...,
         Fields: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeDocumentVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeDocumentVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/paginators/#describedocumentversionspaginator)
         """
 
 class DescribeFolderContentsPaginator(AioPaginator):
@@ -170,15 +170,15 @@
         *,
         FolderId: str,
         AuthenticationToken: str = ...,
         Sort: ResourceSortTypeType = ...,
         Order: OrderTypeType = ...,
         Type: FolderContentTypeType = ...,
         Include: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeFolderContentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeFolderContents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/paginators/#describefoldercontentspaginator)
         """
 
 class DescribeGroupsPaginator(AioPaginator):
@@ -189,15 +189,15 @@
 
     def paginate(
         self,
         *,
         SearchQuery: str,
         AuthenticationToken: str = ...,
         OrganizationId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/paginators/#describegroupspaginator)
         """
 
 class DescribeNotificationSubscriptionsPaginator(AioPaginator):
@@ -222,15 +222,15 @@
 
     def paginate(
         self,
         *,
         ResourceId: str,
         AuthenticationToken: str = ...,
         PrincipalId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeResourcePermissionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeResourcePermissions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/paginators/#describeresourcepermissionspaginator)
         """
 
 class DescribeRootFoldersPaginator(AioPaginator):
@@ -260,15 +260,15 @@
         OrganizationId: str = ...,
         UserIds: str = ...,
         Query: str = ...,
         Include: UserFilterTypeType = ...,
         Order: OrderTypeType = ...,
         Sort: UserSortTypeType = ...,
         Fields: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeUsers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/paginators/#describeuserspaginator)
         """
 
 class SearchResourcesPaginator(AioPaginator):
@@ -283,13 +283,13 @@
         AuthenticationToken: str = ...,
         QueryText: str = ...,
         QueryScopes: Sequence[SearchQueryScopeTypeType] = ...,
         OrganizationId: str = ...,
         AdditionalResponseFields: Sequence[Literal["WEBURL"]] = ...,
         Filters: FiltersTypeDef = ...,
         OrderBy: Sequence[SearchSortResultTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.SearchResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/paginators/#searchresourcespaginator)
         """
```

### Comparing `types-aiobotocore-workdocs-2.9.0/types_aiobotocore_workdocs/type_defs.py` & `types-aiobotocore-workdocs-2.9.1/types_aiobotocore_workdocs/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AbortDocumentVersionUploadRequestRequestTypeDef",
     "ActivateUserRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "UserMetadataTypeDef",
     "NotificationOptionsTypeDef",
     "SharePrincipalTypeDef",
```

### Comparing `types-aiobotocore-workdocs-2.9.0/types_aiobotocore_workdocs/type_defs.pyi` & `types-aiobotocore-workdocs-2.9.1/types_aiobotocore_workdocs/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workdocs-2.9.0/types_aiobotocore_workdocs.egg-info/PKG-INFO` & `types-aiobotocore-workdocs-2.9.1/types_aiobotocore_workdocs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-workdocs
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.WorkDocs 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.WorkDocs 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/
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
 
 <a id="types-aiobotocore-workdocs"></a>
 
 # types-aiobotocore-workdocs
 
 [![PyPI - types-aiobotocore-workdocs](https://img.shields.io/pypi/v/types-aiobotocore-workdocs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-workdocs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-workdocs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-workdocs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-workdocs)](https://pepy.tech/project/types-aiobotocore-workdocs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.WorkDocs 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs)
+[aiobotocore.WorkDocs 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs)
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
 [types-aiobotocore-workdocs docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-workdocs-2.9.0/types_aiobotocore_workdocs.egg-info/SOURCES.txt` & `types-aiobotocore-workdocs-2.9.1/types_aiobotocore_workdocs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

