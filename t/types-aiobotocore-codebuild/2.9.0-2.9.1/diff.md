# Comparing `tmp/types-aiobotocore-codebuild-2.9.0.tar.gz` & `tmp/types-aiobotocore-codebuild-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-codebuild-2.9.0.tar", last modified: Wed Dec 13 19:58:52 2023, max compression
+gzip compressed data, was "types-aiobotocore-codebuild-2.9.1.tar", last modified: Thu Jan 18 01:20:19 2024, max compression
```

## Comparing `types-aiobotocore-codebuild-2.9.0.tar` & `types-aiobotocore-codebuild-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:52.953946 types-aiobotocore-codebuild-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:42:43.000000 types-aiobotocore-codebuild-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14833 2023-12-13 19:58:52.953946 types-aiobotocore-codebuild-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13262 2023-12-13 19:42:43.000000 types-aiobotocore-codebuild-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:52.953946 types-aiobotocore-codebuild-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2023-12-13 19:42:43.000000 types-aiobotocore-codebuild-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:52.953946 types-aiobotocore-codebuild-2.9.0/types_aiobotocore_codebuild/
--rw-r--r--   0 runner    (1001) docker     (127)     3084 2023-12-13 19:42:43.000000 types-aiobotocore-codebuild-2.9.0/types_aiobotocore_codebuild/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2023-12-13 19:42:43.000000 types-aiobotocore-codebuild-2.9.0/types_aiobotocore_codebuild/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      940 2023-12-13 19:42:43.000000 types-aiobotocore-codebuild-2.9.0/types_aiobotocore_codebuild/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43813 2023-12-13 19:42:43.000000 types-aiobotocore-codebuild-2.9.0/types_aiobotocore_codebuild/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    43809 2023-12-13 19:42:43.000000 types-aiobotocore-codebuild-2.9.0/types_aiobotocore_codebuild/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14875 2023-12-13 19:42:43.000000 types-aiobotocore-codebuild-2.9.0/types_aiobotocore_codebuild/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    14873 2023-12-13 19:42:43.000000 types-aiobotocore-codebuild-2.9.0/types_aiobotocore_codebuild/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    15951 2023-12-13 19:42:43.000000 types-aiobotocore-codebuild-2.9.0/types_aiobotocore_codebuild/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    15937 2023-12-13 19:42:43.000000 types-aiobotocore-codebuild-2.9.0/types_aiobotocore_codebuild/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:42:43.000000 types-aiobotocore-codebuild-2.9.0/types_aiobotocore_codebuild/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    53209 2023-12-13 19:42:44.000000 types-aiobotocore-codebuild-2.9.0/types_aiobotocore_codebuild/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    53208 2023-12-13 19:42:44.000000 types-aiobotocore-codebuild-2.9.0/types_aiobotocore_codebuild/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:42:43.000000 types-aiobotocore-codebuild-2.9.0/types_aiobotocore_codebuild/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:52.953946 types-aiobotocore-codebuild-2.9.0/types_aiobotocore_codebuild.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14833 2023-12-13 19:58:52.000000 types-aiobotocore-codebuild-2.9.0/types_aiobotocore_codebuild.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      851 2023-12-13 19:58:52.000000 types-aiobotocore-codebuild-2.9.0/types_aiobotocore_codebuild.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:52.000000 types-aiobotocore-codebuild-2.9.0/types_aiobotocore_codebuild.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:52.000000 types-aiobotocore-codebuild-2.9.0/types_aiobotocore_codebuild.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:52.000000 types-aiobotocore-codebuild-2.9.0/types_aiobotocore_codebuild.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-12-13 19:58:52.000000 types-aiobotocore-codebuild-2.9.0/types_aiobotocore_codebuild.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:19.437447 types-aiobotocore-codebuild-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:04:39.000000 types-aiobotocore-codebuild-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14853 2024-01-18 01:20:19.437447 types-aiobotocore-codebuild-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13262 2024-01-18 01:04:39.000000 types-aiobotocore-codebuild-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:19.441447 types-aiobotocore-codebuild-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-01-18 01:04:39.000000 types-aiobotocore-codebuild-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:19.437447 types-aiobotocore-codebuild-2.9.1/types_aiobotocore_codebuild/
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-01-18 01:04:39.000000 types-aiobotocore-codebuild-2.9.1/types_aiobotocore_codebuild/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-01-18 01:04:39.000000 types-aiobotocore-codebuild-2.9.1/types_aiobotocore_codebuild/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-01-18 01:04:39.000000 types-aiobotocore-codebuild-2.9.1/types_aiobotocore_codebuild/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43834 2024-01-18 01:04:40.000000 types-aiobotocore-codebuild-2.9.1/types_aiobotocore_codebuild/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43831 2024-01-18 01:04:40.000000 types-aiobotocore-codebuild-2.9.1/types_aiobotocore_codebuild/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14873 2024-01-18 01:04:40.000000 types-aiobotocore-codebuild-2.9.1/types_aiobotocore_codebuild/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14873 2024-01-18 01:04:40.000000 types-aiobotocore-codebuild-2.9.1/types_aiobotocore_codebuild/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    15961 2024-01-18 01:04:40.000000 types-aiobotocore-codebuild-2.9.1/types_aiobotocore_codebuild/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15948 2024-01-18 01:04:40.000000 types-aiobotocore-codebuild-2.9.1/types_aiobotocore_codebuild/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:04:39.000000 types-aiobotocore-codebuild-2.9.1/types_aiobotocore_codebuild/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    53208 2024-01-18 01:04:41.000000 types-aiobotocore-codebuild-2.9.1/types_aiobotocore_codebuild/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53208 2024-01-18 01:04:41.000000 types-aiobotocore-codebuild-2.9.1/types_aiobotocore_codebuild/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:04:39.000000 types-aiobotocore-codebuild-2.9.1/types_aiobotocore_codebuild/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:19.437447 types-aiobotocore-codebuild-2.9.1/types_aiobotocore_codebuild.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14853 2024-01-18 01:20:19.000000 types-aiobotocore-codebuild-2.9.1/types_aiobotocore_codebuild.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-01-18 01:20:19.000000 types-aiobotocore-codebuild-2.9.1/types_aiobotocore_codebuild.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:19.000000 types-aiobotocore-codebuild-2.9.1/types_aiobotocore_codebuild.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:19.000000 types-aiobotocore-codebuild-2.9.1/types_aiobotocore_codebuild.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:19.000000 types-aiobotocore-codebuild-2.9.1/types_aiobotocore_codebuild.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-18 01:20:19.000000 types-aiobotocore-codebuild-2.9.1/types_aiobotocore_codebuild.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-codebuild-2.9.0/LICENSE` & `types-aiobotocore-codebuild-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-codebuild-2.9.0/PKG-INFO` & `types-aiobotocore-codebuild-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codebuild
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CodeBuild 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CodeBuild 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/
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
 
 <a id="types-aiobotocore-codebuild"></a>
 
 # types-aiobotocore-codebuild
 
 [![PyPI - types-aiobotocore-codebuild](https://img.shields.io/pypi/v/types-aiobotocore-codebuild.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codebuild)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codebuild.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codebuild)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codebuild)](https://pepy.tech/project/types-aiobotocore-codebuild)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeBuild 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild)
+[aiobotocore.CodeBuild 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild)
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
 [types-aiobotocore-codebuild docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-codebuild-2.9.0/README.md` & `types-aiobotocore-codebuild-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codebuild.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codebuild)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codebuild)](https://pepy.tech/project/types-aiobotocore-codebuild)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeBuild 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild)
+[aiobotocore.CodeBuild 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild)
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
 [types-aiobotocore-codebuild docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-codebuild-2.9.0/setup.py` & `types-aiobotocore-codebuild-2.9.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-codebuild",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_codebuild"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CodeBuild 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.CodeBuild 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore codebuild type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_codebuild": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-codebuild-2.9.0/types_aiobotocore_codebuild/__init__.py` & `types-aiobotocore-codebuild-2.9.1/types_aiobotocore_codebuild/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,14 @@
     ListReportsPaginator,
     ListSharedProjectsPaginator,
     ListSharedReportGroupsPaginator,
 )
 
 Client = CodeBuildClient
 
-
 __all__ = (
     "Client",
     "CodeBuildClient",
     "DescribeCodeCoveragesPaginator",
     "DescribeTestCasesPaginator",
     "ListBuildBatchesForProjectPaginator",
     "ListBuildBatchesPaginator",
```

### Comparing `types-aiobotocore-codebuild-2.9.0/types_aiobotocore_codebuild/__init__.pyi` & `types-aiobotocore-codebuild-2.9.1/types_aiobotocore_codebuild/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codebuild-2.9.0/types_aiobotocore_codebuild/__main__.py` & `types-aiobotocore-codebuild-2.9.1/types_aiobotocore_codebuild/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CodeBuild 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.CodeBuild 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild\nOther"
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

### Comparing `types-aiobotocore-codebuild-2.9.0/types_aiobotocore_codebuild/client.py` & `types-aiobotocore-codebuild-2.9.1/types_aiobotocore_codebuild/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("CodeBuildClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -245,45 +244,45 @@
         encryptionKey: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         vpcConfig: VpcConfigTypeDef = ...,
         badgeEnabled: bool = ...,
         logsConfig: LogsConfigTypeDef = ...,
         fileSystemLocations: Sequence[ProjectFileSystemLocationTypeDef] = ...,
         buildBatchConfig: ProjectBuildBatchConfigTypeDef = ...,
-        concurrentBuildLimit: int = ...
+        concurrentBuildLimit: int = ...,
     ) -> CreateProjectOutputTypeDef:
         """
         Creates a build project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.create_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/client/#create_project)
         """
 
     async def create_report_group(
         self,
         *,
         name: str,
         type: ReportTypeType,
         exportConfig: ReportExportConfigTypeDef,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateReportGroupOutputTypeDef:
         """
         Creates a report group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.create_report_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/client/#create_report_group)
         """
 
     async def create_webhook(
         self,
         *,
         projectName: str,
         branchFilter: str = ...,
         filterGroups: Sequence[Sequence[WebhookFilterTypeDef]] = ...,
-        buildType: WebhookBuildTypeType = ...
+        buildType: WebhookBuildTypeType = ...,
     ) -> CreateWebhookOutputTypeDef:
         """
         For an existing CodeBuild build project that has its source code stored in a
         GitHub or Bitbucket repository, enables CodeBuild to start rebuilding the
         source code every time a code change is pushed to the
         repository.
 
@@ -355,30 +354,30 @@
         *,
         reportArn: str,
         nextToken: str = ...,
         maxResults: int = ...,
         sortOrder: SortOrderTypeType = ...,
         sortBy: ReportCodeCoverageSortByTypeType = ...,
         minLineCoveragePercentage: float = ...,
-        maxLineCoveragePercentage: float = ...
+        maxLineCoveragePercentage: float = ...,
     ) -> DescribeCodeCoveragesOutputTypeDef:
         """
         Retrieves one or more code coverage reports.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.describe_code_coverages)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/client/#describe_code_coverages)
         """
 
     async def describe_test_cases(
         self,
         *,
         reportArn: str,
         nextToken: str = ...,
         maxResults: int = ...,
-        filter: TestCaseFilterTypeDef = ...
+        filter: TestCaseFilterTypeDef = ...,
     ) -> DescribeTestCasesOutputTypeDef:
         """
         Returns a list of details about test cases for a report.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.describe_test_cases)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/client/#describe_test_cases)
         """
@@ -398,15 +397,15 @@
         """
 
     async def get_report_group_trend(
         self,
         *,
         reportGroupArn: str,
         trendField: ReportGroupTrendFieldTypeType,
-        numOfReports: int = ...
+        numOfReports: int = ...,
     ) -> GetReportGroupTrendOutputTypeDef:
         """
         Analyzes and accumulates test report values for the specified test reports.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.get_report_group_trend)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/client/#get_report_group_trend)
         """
@@ -422,15 +421,15 @@
     async def import_source_credentials(
         self,
         *,
         token: str,
         serverType: ServerTypeType,
         authType: AuthTypeType,
         username: str = ...,
-        shouldOverwrite: bool = ...
+        shouldOverwrite: bool = ...,
     ) -> ImportSourceCredentialsOutputTypeDef:
         """
         Imports the source repository credentials for an CodeBuild project that has its
         source code stored in a GitHub, GitHub Enterprise, or Bitbucket
         repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.import_source_credentials)
@@ -447,15 +446,15 @@
 
     async def list_build_batches(
         self,
         *,
         filter: BuildBatchFilterTypeDef = ...,
         maxResults: int = ...,
         sortOrder: SortOrderTypeType = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListBuildBatchesOutputTypeDef:
         """
         Retrieves the identifiers of your build batches in the current region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.list_build_batches)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/client/#list_build_batches)
         """
@@ -463,15 +462,15 @@
     async def list_build_batches_for_project(
         self,
         *,
         projectName: str = ...,
         filter: BuildBatchFilterTypeDef = ...,
         maxResults: int = ...,
         sortOrder: SortOrderTypeType = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListBuildBatchesForProjectOutputTypeDef:
         """
         Retrieves the identifiers of the build batches for a specific project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.list_build_batches_for_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/client/#list_build_batches_for_project)
         """
@@ -507,15 +506,15 @@
         """
 
     async def list_projects(
         self,
         *,
         sortBy: ProjectSortByTypeType = ...,
         sortOrder: SortOrderTypeType = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListProjectsOutputTypeDef:
         """
         Gets a list of build project names, with each build project name representing a
         single build
         project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.list_projects)
@@ -524,15 +523,15 @@
 
     async def list_report_groups(
         self,
         *,
         sortOrder: SortOrderTypeType = ...,
         sortBy: ReportGroupSortByTypeType = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListReportGroupsOutputTypeDef:
         """
         Gets a list ARNs for the report groups in the current Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.list_report_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/client/#list_report_groups)
@@ -540,15 +539,15 @@
 
     async def list_reports(
         self,
         *,
         sortOrder: SortOrderTypeType = ...,
         nextToken: str = ...,
         maxResults: int = ...,
-        filter: ReportFilterTypeDef = ...
+        filter: ReportFilterTypeDef = ...,
     ) -> ListReportsOutputTypeDef:
         """
         Returns a list of ARNs for the reports in the current Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.list_reports)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/client/#list_reports)
@@ -557,30 +556,30 @@
     async def list_reports_for_report_group(
         self,
         *,
         reportGroupArn: str,
         nextToken: str = ...,
         sortOrder: SortOrderTypeType = ...,
         maxResults: int = ...,
-        filter: ReportFilterTypeDef = ...
+        filter: ReportFilterTypeDef = ...,
     ) -> ListReportsForReportGroupOutputTypeDef:
         """
         Returns a list of ARNs for the reports that belong to a `ReportGroup`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.list_reports_for_report_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/client/#list_reports_for_report_group)
         """
 
     async def list_shared_projects(
         self,
         *,
         sortBy: SharedResourceSortByTypeType = ...,
         sortOrder: SortOrderTypeType = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListSharedProjectsOutputTypeDef:
         """
         Gets a list of projects that are shared with other Amazon Web Services accounts
         or
         users.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.list_shared_projects)
@@ -589,15 +588,15 @@
 
     async def list_shared_report_groups(
         self,
         *,
         sortOrder: SortOrderTypeType = ...,
         sortBy: SharedResourceSortByTypeType = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListSharedReportGroupsOutputTypeDef:
         """
         Gets a list of report groups that are shared with other Amazon Web Services
         accounts or
         users.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.list_shared_report_groups)
@@ -633,15 +632,15 @@
         """
 
     async def retry_build_batch(
         self,
         *,
         id: str = ...,
         idempotencyToken: str = ...,
-        retryType: RetryBuildBatchTypeType = ...
+        retryType: RetryBuildBatchTypeType = ...,
     ) -> RetryBuildBatchOutputTypeDef:
         """
         Restarts a failed batch build.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.retry_build_batch)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/client/#retry_build_batch)
         """
@@ -675,15 +674,15 @@
         timeoutInMinutesOverride: int = ...,
         queuedTimeoutInMinutesOverride: int = ...,
         encryptionKeyOverride: str = ...,
         idempotencyToken: str = ...,
         logsConfigOverride: LogsConfigTypeDef = ...,
         registryCredentialOverride: RegistryCredentialTypeDef = ...,
         imagePullCredentialsTypeOverride: ImagePullCredentialsTypeType = ...,
-        debugSessionEnabled: bool = ...
+        debugSessionEnabled: bool = ...,
     ) -> StartBuildOutputTypeDef:
         """
         Starts running a build.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.start_build)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/client/#start_build)
         """
@@ -717,15 +716,15 @@
         queuedTimeoutInMinutesOverride: int = ...,
         encryptionKeyOverride: str = ...,
         idempotencyToken: str = ...,
         logsConfigOverride: LogsConfigTypeDef = ...,
         registryCredentialOverride: RegistryCredentialTypeDef = ...,
         imagePullCredentialsTypeOverride: ImagePullCredentialsTypeType = ...,
         buildBatchConfigOverride: ProjectBuildBatchConfigTypeDef = ...,
-        debugSessionEnabled: bool = ...
+        debugSessionEnabled: bool = ...,
     ) -> StartBuildBatchOutputTypeDef:
         """
         Starts a batch build for a project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.start_build_batch)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/client/#start_build_batch)
         """
@@ -765,43 +764,43 @@
         encryptionKey: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         vpcConfig: VpcConfigTypeDef = ...,
         badgeEnabled: bool = ...,
         logsConfig: LogsConfigTypeDef = ...,
         fileSystemLocations: Sequence[ProjectFileSystemLocationTypeDef] = ...,
         buildBatchConfig: ProjectBuildBatchConfigTypeDef = ...,
-        concurrentBuildLimit: int = ...
+        concurrentBuildLimit: int = ...,
     ) -> UpdateProjectOutputTypeDef:
         """
         Changes the settings of a build project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.update_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/client/#update_project)
         """
 
     async def update_project_visibility(
         self,
         *,
         projectArn: str,
         projectVisibility: ProjectVisibilityTypeType,
-        resourceAccessRole: str = ...
+        resourceAccessRole: str = ...,
     ) -> UpdateProjectVisibilityOutputTypeDef:
         """
         Changes the public visibility for a project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.update_project_visibility)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/client/#update_project_visibility)
         """
 
     async def update_report_group(
         self,
         *,
         arn: str,
         exportConfig: ReportExportConfigTypeDef = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> UpdateReportGroupOutputTypeDef:
         """
         Updates a report group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.update_report_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/client/#update_report_group)
         """
@@ -809,15 +808,15 @@
     async def update_webhook(
         self,
         *,
         projectName: str,
         branchFilter: str = ...,
         rotateSecret: bool = ...,
         filterGroups: Sequence[Sequence[WebhookFilterTypeDef]] = ...,
-        buildType: WebhookBuildTypeType = ...
+        buildType: WebhookBuildTypeType = ...,
     ) -> UpdateWebhookOutputTypeDef:
         """
         Updates the webhook associated with an CodeBuild build project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.update_webhook)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/client/#update_webhook)
         """
```

### Comparing `types-aiobotocore-codebuild-2.9.0/types_aiobotocore_codebuild/client.pyi` & `types-aiobotocore-codebuild-2.9.1/types_aiobotocore_codebuild/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -241,45 +241,45 @@
         encryptionKey: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         vpcConfig: VpcConfigTypeDef = ...,
         badgeEnabled: bool = ...,
         logsConfig: LogsConfigTypeDef = ...,
         fileSystemLocations: Sequence[ProjectFileSystemLocationTypeDef] = ...,
         buildBatchConfig: ProjectBuildBatchConfigTypeDef = ...,
-        concurrentBuildLimit: int = ...
+        concurrentBuildLimit: int = ...,
     ) -> CreateProjectOutputTypeDef:
         """
         Creates a build project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.create_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/client/#create_project)
         """
 
     async def create_report_group(
         self,
         *,
         name: str,
         type: ReportTypeType,
         exportConfig: ReportExportConfigTypeDef,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateReportGroupOutputTypeDef:
         """
         Creates a report group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.create_report_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/client/#create_report_group)
         """
 
     async def create_webhook(
         self,
         *,
         projectName: str,
         branchFilter: str = ...,
         filterGroups: Sequence[Sequence[WebhookFilterTypeDef]] = ...,
-        buildType: WebhookBuildTypeType = ...
+        buildType: WebhookBuildTypeType = ...,
     ) -> CreateWebhookOutputTypeDef:
         """
         For an existing CodeBuild build project that has its source code stored in a
         GitHub or Bitbucket repository, enables CodeBuild to start rebuilding the
         source code every time a code change is pushed to the
         repository.
 
@@ -351,30 +351,30 @@
         *,
         reportArn: str,
         nextToken: str = ...,
         maxResults: int = ...,
         sortOrder: SortOrderTypeType = ...,
         sortBy: ReportCodeCoverageSortByTypeType = ...,
         minLineCoveragePercentage: float = ...,
-        maxLineCoveragePercentage: float = ...
+        maxLineCoveragePercentage: float = ...,
     ) -> DescribeCodeCoveragesOutputTypeDef:
         """
         Retrieves one or more code coverage reports.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.describe_code_coverages)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/client/#describe_code_coverages)
         """
 
     async def describe_test_cases(
         self,
         *,
         reportArn: str,
         nextToken: str = ...,
         maxResults: int = ...,
-        filter: TestCaseFilterTypeDef = ...
+        filter: TestCaseFilterTypeDef = ...,
     ) -> DescribeTestCasesOutputTypeDef:
         """
         Returns a list of details about test cases for a report.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.describe_test_cases)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/client/#describe_test_cases)
         """
@@ -394,15 +394,15 @@
         """
 
     async def get_report_group_trend(
         self,
         *,
         reportGroupArn: str,
         trendField: ReportGroupTrendFieldTypeType,
-        numOfReports: int = ...
+        numOfReports: int = ...,
     ) -> GetReportGroupTrendOutputTypeDef:
         """
         Analyzes and accumulates test report values for the specified test reports.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.get_report_group_trend)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/client/#get_report_group_trend)
         """
@@ -418,15 +418,15 @@
     async def import_source_credentials(
         self,
         *,
         token: str,
         serverType: ServerTypeType,
         authType: AuthTypeType,
         username: str = ...,
-        shouldOverwrite: bool = ...
+        shouldOverwrite: bool = ...,
     ) -> ImportSourceCredentialsOutputTypeDef:
         """
         Imports the source repository credentials for an CodeBuild project that has its
         source code stored in a GitHub, GitHub Enterprise, or Bitbucket
         repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.import_source_credentials)
@@ -443,15 +443,15 @@
 
     async def list_build_batches(
         self,
         *,
         filter: BuildBatchFilterTypeDef = ...,
         maxResults: int = ...,
         sortOrder: SortOrderTypeType = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListBuildBatchesOutputTypeDef:
         """
         Retrieves the identifiers of your build batches in the current region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.list_build_batches)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/client/#list_build_batches)
         """
@@ -459,15 +459,15 @@
     async def list_build_batches_for_project(
         self,
         *,
         projectName: str = ...,
         filter: BuildBatchFilterTypeDef = ...,
         maxResults: int = ...,
         sortOrder: SortOrderTypeType = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListBuildBatchesForProjectOutputTypeDef:
         """
         Retrieves the identifiers of the build batches for a specific project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.list_build_batches_for_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/client/#list_build_batches_for_project)
         """
@@ -503,15 +503,15 @@
         """
 
     async def list_projects(
         self,
         *,
         sortBy: ProjectSortByTypeType = ...,
         sortOrder: SortOrderTypeType = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListProjectsOutputTypeDef:
         """
         Gets a list of build project names, with each build project name representing a
         single build
         project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.list_projects)
@@ -520,15 +520,15 @@
 
     async def list_report_groups(
         self,
         *,
         sortOrder: SortOrderTypeType = ...,
         sortBy: ReportGroupSortByTypeType = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListReportGroupsOutputTypeDef:
         """
         Gets a list ARNs for the report groups in the current Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.list_report_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/client/#list_report_groups)
@@ -536,15 +536,15 @@
 
     async def list_reports(
         self,
         *,
         sortOrder: SortOrderTypeType = ...,
         nextToken: str = ...,
         maxResults: int = ...,
-        filter: ReportFilterTypeDef = ...
+        filter: ReportFilterTypeDef = ...,
     ) -> ListReportsOutputTypeDef:
         """
         Returns a list of ARNs for the reports in the current Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.list_reports)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/client/#list_reports)
@@ -553,30 +553,30 @@
     async def list_reports_for_report_group(
         self,
         *,
         reportGroupArn: str,
         nextToken: str = ...,
         sortOrder: SortOrderTypeType = ...,
         maxResults: int = ...,
-        filter: ReportFilterTypeDef = ...
+        filter: ReportFilterTypeDef = ...,
     ) -> ListReportsForReportGroupOutputTypeDef:
         """
         Returns a list of ARNs for the reports that belong to a `ReportGroup`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.list_reports_for_report_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/client/#list_reports_for_report_group)
         """
 
     async def list_shared_projects(
         self,
         *,
         sortBy: SharedResourceSortByTypeType = ...,
         sortOrder: SortOrderTypeType = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListSharedProjectsOutputTypeDef:
         """
         Gets a list of projects that are shared with other Amazon Web Services accounts
         or
         users.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.list_shared_projects)
@@ -585,15 +585,15 @@
 
     async def list_shared_report_groups(
         self,
         *,
         sortOrder: SortOrderTypeType = ...,
         sortBy: SharedResourceSortByTypeType = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListSharedReportGroupsOutputTypeDef:
         """
         Gets a list of report groups that are shared with other Amazon Web Services
         accounts or
         users.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.list_shared_report_groups)
@@ -629,15 +629,15 @@
         """
 
     async def retry_build_batch(
         self,
         *,
         id: str = ...,
         idempotencyToken: str = ...,
-        retryType: RetryBuildBatchTypeType = ...
+        retryType: RetryBuildBatchTypeType = ...,
     ) -> RetryBuildBatchOutputTypeDef:
         """
         Restarts a failed batch build.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.retry_build_batch)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/client/#retry_build_batch)
         """
@@ -671,15 +671,15 @@
         timeoutInMinutesOverride: int = ...,
         queuedTimeoutInMinutesOverride: int = ...,
         encryptionKeyOverride: str = ...,
         idempotencyToken: str = ...,
         logsConfigOverride: LogsConfigTypeDef = ...,
         registryCredentialOverride: RegistryCredentialTypeDef = ...,
         imagePullCredentialsTypeOverride: ImagePullCredentialsTypeType = ...,
-        debugSessionEnabled: bool = ...
+        debugSessionEnabled: bool = ...,
     ) -> StartBuildOutputTypeDef:
         """
         Starts running a build.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.start_build)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/client/#start_build)
         """
@@ -713,15 +713,15 @@
         queuedTimeoutInMinutesOverride: int = ...,
         encryptionKeyOverride: str = ...,
         idempotencyToken: str = ...,
         logsConfigOverride: LogsConfigTypeDef = ...,
         registryCredentialOverride: RegistryCredentialTypeDef = ...,
         imagePullCredentialsTypeOverride: ImagePullCredentialsTypeType = ...,
         buildBatchConfigOverride: ProjectBuildBatchConfigTypeDef = ...,
-        debugSessionEnabled: bool = ...
+        debugSessionEnabled: bool = ...,
     ) -> StartBuildBatchOutputTypeDef:
         """
         Starts a batch build for a project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.start_build_batch)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/client/#start_build_batch)
         """
@@ -761,43 +761,43 @@
         encryptionKey: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         vpcConfig: VpcConfigTypeDef = ...,
         badgeEnabled: bool = ...,
         logsConfig: LogsConfigTypeDef = ...,
         fileSystemLocations: Sequence[ProjectFileSystemLocationTypeDef] = ...,
         buildBatchConfig: ProjectBuildBatchConfigTypeDef = ...,
-        concurrentBuildLimit: int = ...
+        concurrentBuildLimit: int = ...,
     ) -> UpdateProjectOutputTypeDef:
         """
         Changes the settings of a build project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.update_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/client/#update_project)
         """
 
     async def update_project_visibility(
         self,
         *,
         projectArn: str,
         projectVisibility: ProjectVisibilityTypeType,
-        resourceAccessRole: str = ...
+        resourceAccessRole: str = ...,
     ) -> UpdateProjectVisibilityOutputTypeDef:
         """
         Changes the public visibility for a project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.update_project_visibility)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/client/#update_project_visibility)
         """
 
     async def update_report_group(
         self,
         *,
         arn: str,
         exportConfig: ReportExportConfigTypeDef = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> UpdateReportGroupOutputTypeDef:
         """
         Updates a report group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.update_report_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/client/#update_report_group)
         """
@@ -805,15 +805,15 @@
     async def update_webhook(
         self,
         *,
         projectName: str,
         branchFilter: str = ...,
         rotateSecret: bool = ...,
         filterGroups: Sequence[Sequence[WebhookFilterTypeDef]] = ...,
-        buildType: WebhookBuildTypeType = ...
+        buildType: WebhookBuildTypeType = ...,
     ) -> UpdateWebhookOutputTypeDef:
         """
         Updates the webhook associated with an CodeBuild build project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.update_webhook)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/client/#update_webhook)
         """
```

### Comparing `types-aiobotocore-codebuild-2.9.0/types_aiobotocore_codebuild/literals.py` & `types-aiobotocore-codebuild-2.9.1/types_aiobotocore_codebuild/literals.py`

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
     "ArtifactNamespaceType",
     "ArtifactPackagingType",
     "ArtifactsTypeType",
     "AuthTypeType",
     "BatchReportModeTypeType",
     "BucketOwnerAccessType",
@@ -74,15 +73,14 @@
     "CodeBuildServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ArtifactNamespaceType = Literal["BUILD_ID", "NONE"]
 ArtifactPackagingType = Literal["NONE", "ZIP"]
 ArtifactsTypeType = Literal["CODEPIPELINE", "NO_ARTIFACTS", "S3"]
 AuthTypeType = Literal["BASIC_AUTH", "OAUTH", "PERSONAL_ACCESS_TOKEN"]
 BatchReportModeTypeType = Literal["REPORT_AGGREGATED_BATCH", "REPORT_INDIVIDUAL_BUILDS"]
 BucketOwnerAccessType = Literal["FULL", "NONE", "READ_ONLY"]
 BuildBatchPhaseTypeType = Literal[
```

### Comparing `types-aiobotocore-codebuild-2.9.0/types_aiobotocore_codebuild/literals.pyi` & `types-aiobotocore-codebuild-2.9.1/types_aiobotocore_codebuild/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codebuild-2.9.0/types_aiobotocore_codebuild/paginator.py` & `types-aiobotocore-codebuild-2.9.1/types_aiobotocore_codebuild/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,14 @@
     "ListReportGroupsPaginator",
     "ListReportsPaginator",
     "ListReportsForReportGroupPaginator",
     "ListSharedProjectsPaginator",
     "ListSharedReportGroupsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -110,15 +109,15 @@
         self,
         *,
         reportArn: str,
         sortOrder: SortOrderTypeType = ...,
         sortBy: ReportCodeCoverageSortByTypeType = ...,
         minLineCoveragePercentage: float = ...,
         maxLineCoveragePercentage: float = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeCodeCoveragesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.DescribeCodeCoverages.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/paginators/#describecodecoveragespaginator)
         """
 
 
@@ -129,15 +128,15 @@
     """
 
     def paginate(
         self,
         *,
         reportArn: str,
         filter: TestCaseFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeTestCasesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.DescribeTestCases.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/paginators/#describetestcasespaginator)
         """
 
 
@@ -148,15 +147,15 @@
     """
 
     def paginate(
         self,
         *,
         filter: BuildBatchFilterTypeDef = ...,
         sortOrder: SortOrderTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListBuildBatchesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListBuildBatches.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/paginators/#listbuildbatchespaginator)
         """
 
 
@@ -168,15 +167,15 @@
 
     def paginate(
         self,
         *,
         projectName: str = ...,
         filter: BuildBatchFilterTypeDef = ...,
         sortOrder: SortOrderTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListBuildBatchesForProjectOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListBuildBatchesForProject.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/paginators/#listbuildbatchesforprojectpaginator)
         """
 
 
@@ -202,15 +201,15 @@
     """
 
     def paginate(
         self,
         *,
         projectName: str,
         sortOrder: SortOrderTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListBuildsForProjectOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListBuildsForProject.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/paginators/#listbuildsforprojectpaginator)
         """
 
 
@@ -221,15 +220,15 @@
     """
 
     def paginate(
         self,
         *,
         sortBy: ProjectSortByTypeType = ...,
         sortOrder: SortOrderTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListProjectsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListProjects.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/paginators/#listprojectspaginator)
         """
 
 
@@ -240,15 +239,15 @@
     """
 
     def paginate(
         self,
         *,
         sortOrder: SortOrderTypeType = ...,
         sortBy: ReportGroupSortByTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListReportGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListReportGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/paginators/#listreportgroupspaginator)
         """
 
 
@@ -259,15 +258,15 @@
     """
 
     def paginate(
         self,
         *,
         sortOrder: SortOrderTypeType = ...,
         filter: ReportFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListReportsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListReports.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/paginators/#listreportspaginator)
         """
 
 
@@ -279,15 +278,15 @@
 
     def paginate(
         self,
         *,
         reportGroupArn: str,
         sortOrder: SortOrderTypeType = ...,
         filter: ReportFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListReportsForReportGroupOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListReportsForReportGroup.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/paginators/#listreportsforreportgrouppaginator)
         """
 
 
@@ -298,15 +297,15 @@
     """
 
     def paginate(
         self,
         *,
         sortBy: SharedResourceSortByTypeType = ...,
         sortOrder: SortOrderTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSharedProjectsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListSharedProjects.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/paginators/#listsharedprojectspaginator)
         """
 
 
@@ -317,13 +316,13 @@
     """
 
     def paginate(
         self,
         *,
         sortOrder: SortOrderTypeType = ...,
         sortBy: SharedResourceSortByTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSharedReportGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListSharedReportGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/paginators/#listsharedreportgroupspaginator)
         """
```

### Comparing `types-aiobotocore-codebuild-2.9.0/types_aiobotocore_codebuild/paginator.pyi` & `types-aiobotocore-codebuild-2.9.1/types_aiobotocore_codebuild/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         self,
         *,
         reportArn: str,
         sortOrder: SortOrderTypeType = ...,
         sortBy: ReportCodeCoverageSortByTypeType = ...,
         minLineCoveragePercentage: float = ...,
         maxLineCoveragePercentage: float = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeCodeCoveragesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.DescribeCodeCoverages.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/paginators/#describecodecoveragespaginator)
         """
 
 class DescribeTestCasesPaginator(AioPaginator):
@@ -125,15 +125,15 @@
     """
 
     def paginate(
         self,
         *,
         reportArn: str,
         filter: TestCaseFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeTestCasesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.DescribeTestCases.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/paginators/#describetestcasespaginator)
         """
 
 class ListBuildBatchesPaginator(AioPaginator):
@@ -143,15 +143,15 @@
     """
 
     def paginate(
         self,
         *,
         filter: BuildBatchFilterTypeDef = ...,
         sortOrder: SortOrderTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListBuildBatchesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListBuildBatches.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/paginators/#listbuildbatchespaginator)
         """
 
 class ListBuildBatchesForProjectPaginator(AioPaginator):
@@ -162,15 +162,15 @@
 
     def paginate(
         self,
         *,
         projectName: str = ...,
         filter: BuildBatchFilterTypeDef = ...,
         sortOrder: SortOrderTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListBuildBatchesForProjectOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListBuildBatchesForProject.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/paginators/#listbuildbatchesforprojectpaginator)
         """
 
 class ListBuildsPaginator(AioPaginator):
@@ -194,15 +194,15 @@
     """
 
     def paginate(
         self,
         *,
         projectName: str,
         sortOrder: SortOrderTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListBuildsForProjectOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListBuildsForProject.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/paginators/#listbuildsforprojectpaginator)
         """
 
 class ListProjectsPaginator(AioPaginator):
@@ -212,15 +212,15 @@
     """
 
     def paginate(
         self,
         *,
         sortBy: ProjectSortByTypeType = ...,
         sortOrder: SortOrderTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListProjectsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListProjects.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/paginators/#listprojectspaginator)
         """
 
 class ListReportGroupsPaginator(AioPaginator):
@@ -230,15 +230,15 @@
     """
 
     def paginate(
         self,
         *,
         sortOrder: SortOrderTypeType = ...,
         sortBy: ReportGroupSortByTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListReportGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListReportGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/paginators/#listreportgroupspaginator)
         """
 
 class ListReportsPaginator(AioPaginator):
@@ -248,15 +248,15 @@
     """
 
     def paginate(
         self,
         *,
         sortOrder: SortOrderTypeType = ...,
         filter: ReportFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListReportsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListReports.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/paginators/#listreportspaginator)
         """
 
 class ListReportsForReportGroupPaginator(AioPaginator):
@@ -267,15 +267,15 @@
 
     def paginate(
         self,
         *,
         reportGroupArn: str,
         sortOrder: SortOrderTypeType = ...,
         filter: ReportFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListReportsForReportGroupOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListReportsForReportGroup.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/paginators/#listreportsforreportgrouppaginator)
         """
 
 class ListSharedProjectsPaginator(AioPaginator):
@@ -285,15 +285,15 @@
     """
 
     def paginate(
         self,
         *,
         sortBy: SharedResourceSortByTypeType = ...,
         sortOrder: SortOrderTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSharedProjectsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListSharedProjects.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/paginators/#listsharedprojectspaginator)
         """
 
 class ListSharedReportGroupsPaginator(AioPaginator):
@@ -303,13 +303,13 @@
     """
 
     def paginate(
         self,
         *,
         sortOrder: SortOrderTypeType = ...,
         sortBy: SharedResourceSortByTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSharedReportGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListSharedReportGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/paginators/#listsharedreportgroupspaginator)
         """
```

### Comparing `types-aiobotocore-codebuild-2.9.0/types_aiobotocore_codebuild/type_defs.py` & `types-aiobotocore-codebuild-2.9.1/types_aiobotocore_codebuild/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "BatchDeleteBuildsInputRequestTypeDef",
     "BuildNotDeletedTypeDef",
     "ResponseMetadataTypeDef",
     "BatchGetBuildBatchesInputRequestTypeDef",
     "BatchGetBuildsInputRequestTypeDef",
     "BatchGetProjectsInputRequestTypeDef",
```

### Comparing `types-aiobotocore-codebuild-2.9.0/types_aiobotocore_codebuild/type_defs.pyi` & `types-aiobotocore-codebuild-2.9.1/types_aiobotocore_codebuild/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codebuild-2.9.0/types_aiobotocore_codebuild.egg-info/PKG-INFO` & `types-aiobotocore-codebuild-2.9.1/types_aiobotocore_codebuild.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codebuild
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CodeBuild 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CodeBuild 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/
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
 
 <a id="types-aiobotocore-codebuild"></a>
 
 # types-aiobotocore-codebuild
 
 [![PyPI - types-aiobotocore-codebuild](https://img.shields.io/pypi/v/types-aiobotocore-codebuild.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codebuild)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codebuild.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codebuild)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codebuild)](https://pepy.tech/project/types-aiobotocore-codebuild)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeBuild 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild)
+[aiobotocore.CodeBuild 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild)
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
 [types-aiobotocore-codebuild docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-codebuild-2.9.0/types_aiobotocore_codebuild.egg-info/SOURCES.txt` & `types-aiobotocore-codebuild-2.9.1/types_aiobotocore_codebuild.egg-info/SOURCES.txt`

 * *Files identical despite different names*

