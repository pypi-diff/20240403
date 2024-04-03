# Comparing `tmp/types-aiobotocore-codepipeline-2.9.0.tar.gz` & `tmp/types-aiobotocore-codepipeline-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-codepipeline-2.9.0.tar", last modified: Wed Dec 13 19:58:55 2023, max compression
+gzip compressed data, was "types-aiobotocore-codepipeline-2.9.1.tar", last modified: Thu Jan 18 01:20:21 2024, max compression
```

## Comparing `types-aiobotocore-codepipeline-2.9.0.tar` & `types-aiobotocore-codepipeline-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:55.581924 types-aiobotocore-codepipeline-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:42:57.000000 types-aiobotocore-codepipeline-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14022 2023-12-13 19:58:55.577924 types-aiobotocore-codepipeline-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12439 2023-12-13 19:42:57.000000 types-aiobotocore-codepipeline-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:55.581924 types-aiobotocore-codepipeline-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2023-12-13 19:42:57.000000 types-aiobotocore-codepipeline-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:55.577924 types-aiobotocore-codepipeline-2.9.0/types_aiobotocore_codepipeline/
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2023-12-13 19:42:57.000000 types-aiobotocore-codepipeline-2.9.0/types_aiobotocore_codepipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2023-12-13 19:42:57.000000 types-aiobotocore-codepipeline-2.9.0/types_aiobotocore_codepipeline/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      952 2023-12-13 19:42:57.000000 types-aiobotocore-codepipeline-2.9.0/types_aiobotocore_codepipeline/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34728 2023-12-13 19:42:57.000000 types-aiobotocore-codepipeline-2.9.0/types_aiobotocore_codepipeline/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    34724 2023-12-13 19:42:57.000000 types-aiobotocore-codepipeline-2.9.0/types_aiobotocore_codepipeline/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11800 2023-12-13 19:42:58.000000 types-aiobotocore-codepipeline-2.9.0/types_aiobotocore_codepipeline/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11798 2023-12-13 19:42:58.000000 types-aiobotocore-codepipeline-2.9.0/types_aiobotocore_codepipeline/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7997 2023-12-13 19:42:57.000000 types-aiobotocore-codepipeline-2.9.0/types_aiobotocore_codepipeline/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7989 2023-12-13 19:42:57.000000 types-aiobotocore-codepipeline-2.9.0/types_aiobotocore_codepipeline/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:42:57.000000 types-aiobotocore-codepipeline-2.9.0/types_aiobotocore_codepipeline/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    41576 2023-12-13 19:42:59.000000 types-aiobotocore-codepipeline-2.9.0/types_aiobotocore_codepipeline/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    41575 2023-12-13 19:42:58.000000 types-aiobotocore-codepipeline-2.9.0/types_aiobotocore_codepipeline/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:42:57.000000 types-aiobotocore-codepipeline-2.9.0/types_aiobotocore_codepipeline/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:55.577924 types-aiobotocore-codepipeline-2.9.0/types_aiobotocore_codepipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14022 2023-12-13 19:58:55.000000 types-aiobotocore-codepipeline-2.9.0/types_aiobotocore_codepipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      908 2023-12-13 19:58:55.000000 types-aiobotocore-codepipeline-2.9.0/types_aiobotocore_codepipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:55.000000 types-aiobotocore-codepipeline-2.9.0/types_aiobotocore_codepipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:55.000000 types-aiobotocore-codepipeline-2.9.0/types_aiobotocore_codepipeline.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:55.000000 types-aiobotocore-codepipeline-2.9.0/types_aiobotocore_codepipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-13 19:58:55.000000 types-aiobotocore-codepipeline-2.9.0/types_aiobotocore_codepipeline.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:21.837436 types-aiobotocore-codepipeline-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:04:53.000000 types-aiobotocore-codepipeline-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14042 2024-01-18 01:20:21.837436 types-aiobotocore-codepipeline-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12439 2024-01-18 01:04:53.000000 types-aiobotocore-codepipeline-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:21.837436 types-aiobotocore-codepipeline-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-01-18 01:04:53.000000 types-aiobotocore-codepipeline-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:21.837436 types-aiobotocore-codepipeline-2.9.1/types_aiobotocore_codepipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-01-18 01:04:53.000000 types-aiobotocore-codepipeline-2.9.1/types_aiobotocore_codepipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-01-18 01:04:53.000000 types-aiobotocore-codepipeline-2.9.1/types_aiobotocore_codepipeline/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-01-18 01:04:53.000000 types-aiobotocore-codepipeline-2.9.1/types_aiobotocore_codepipeline/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34738 2024-01-18 01:04:54.000000 types-aiobotocore-codepipeline-2.9.1/types_aiobotocore_codepipeline/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34735 2024-01-18 01:04:53.000000 types-aiobotocore-codepipeline-2.9.1/types_aiobotocore_codepipeline/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11798 2024-01-18 01:04:54.000000 types-aiobotocore-codepipeline-2.9.1/types_aiobotocore_codepipeline/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11798 2024-01-18 01:04:54.000000 types-aiobotocore-codepipeline-2.9.1/types_aiobotocore_codepipeline/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7998 2024-01-18 01:04:54.000000 types-aiobotocore-codepipeline-2.9.1/types_aiobotocore_codepipeline/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7991 2024-01-18 01:04:54.000000 types-aiobotocore-codepipeline-2.9.1/types_aiobotocore_codepipeline/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:04:53.000000 types-aiobotocore-codepipeline-2.9.1/types_aiobotocore_codepipeline/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    41575 2024-01-18 01:04:55.000000 types-aiobotocore-codepipeline-2.9.1/types_aiobotocore_codepipeline/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41575 2024-01-18 01:04:55.000000 types-aiobotocore-codepipeline-2.9.1/types_aiobotocore_codepipeline/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:04:53.000000 types-aiobotocore-codepipeline-2.9.1/types_aiobotocore_codepipeline/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:21.837436 types-aiobotocore-codepipeline-2.9.1/types_aiobotocore_codepipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14042 2024-01-18 01:20:21.000000 types-aiobotocore-codepipeline-2.9.1/types_aiobotocore_codepipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-01-18 01:20:21.000000 types-aiobotocore-codepipeline-2.9.1/types_aiobotocore_codepipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:21.000000 types-aiobotocore-codepipeline-2.9.1/types_aiobotocore_codepipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:21.000000 types-aiobotocore-codepipeline-2.9.1/types_aiobotocore_codepipeline.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:21.000000 types-aiobotocore-codepipeline-2.9.1/types_aiobotocore_codepipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-01-18 01:20:21.000000 types-aiobotocore-codepipeline-2.9.1/types_aiobotocore_codepipeline.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-codepipeline-2.9.0/LICENSE` & `types-aiobotocore-codepipeline-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-codepipeline-2.9.0/PKG-INFO` & `types-aiobotocore-codepipeline-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codepipeline
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CodePipeline 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CodePipeline 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/
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
 
 <a id="types-aiobotocore-codepipeline"></a>
 
 # types-aiobotocore-codepipeline
 
 [![PyPI - types-aiobotocore-codepipeline](https://img.shields.io/pypi/v/types-aiobotocore-codepipeline.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codepipeline)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codepipeline.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codepipeline)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codepipeline)](https://pepy.tech/project/types-aiobotocore-codepipeline)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodePipeline 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
+[aiobotocore.CodePipeline 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
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
 [types-aiobotocore-codepipeline docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-codepipeline-2.9.0/README.md` & `types-aiobotocore-codepipeline-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codepipeline.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codepipeline)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codepipeline)](https://pepy.tech/project/types-aiobotocore-codepipeline)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodePipeline 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
+[aiobotocore.CodePipeline 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
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
 [types-aiobotocore-codepipeline docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-codepipeline-2.9.0/setup.py` & `types-aiobotocore-codepipeline-2.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-codepipeline",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_codepipeline"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CodePipeline 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.CodePipeline 2.9.1 service generated with"
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
     keywords="aiobotocore codepipeline type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_codepipeline": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-codepipeline-2.9.0/types_aiobotocore_codepipeline/__init__.py` & `types-aiobotocore-codepipeline-2.9.1/types_aiobotocore_codepipeline/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,14 @@
     ListPipelinesPaginator,
     ListTagsForResourcePaginator,
     ListWebhooksPaginator,
 )
 
 Client = CodePipelineClient
 
-
 __all__ = (
     "Client",
     "CodePipelineClient",
     "ListActionExecutionsPaginator",
     "ListActionTypesPaginator",
     "ListPipelineExecutionsPaginator",
     "ListPipelinesPaginator",
```

### Comparing `types-aiobotocore-codepipeline-2.9.0/types_aiobotocore_codepipeline/__init__.pyi` & `types-aiobotocore-codepipeline-2.9.1/types_aiobotocore_codepipeline/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codepipeline-2.9.0/types_aiobotocore_codepipeline/__main__.py` & `types-aiobotocore-codepipeline-2.9.1/types_aiobotocore_codepipeline/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CodePipeline 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.CodePipeline 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline\nOther"
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

### Comparing `types-aiobotocore-codepipeline-2.9.0/types_aiobotocore_codepipeline/client.py` & `types-aiobotocore-codepipeline-2.9.1/types_aiobotocore_codepipeline/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,15 +81,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("CodePipelineClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -197,15 +196,15 @@
         category: ActionCategoryType,
         provider: str,
         version: str,
         inputArtifactDetails: ArtifactDetailsTypeDef,
         outputArtifactDetails: ArtifactDetailsTypeDef,
         settings: ActionTypeSettingsTypeDef = ...,
         configurationProperties: Sequence[ActionConfigurationPropertyTypeDef] = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateCustomActionTypeOutputTypeDef:
         """
         Creates a new custom action that can be used in all pipelines associated with
         the Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.create_custom_action_type)
@@ -262,15 +261,15 @@
 
     async def disable_stage_transition(
         self,
         *,
         pipelineName: str,
         stageName: str,
         transitionType: StageTransitionTypeType,
-        reason: str
+        reason: str,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Prevents artifacts in a pipeline from transitioning to the next stage in the
         pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.disable_stage_transition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/client/#disable_stage_transition)
@@ -361,29 +360,29 @@
 
     async def list_action_executions(
         self,
         *,
         pipelineName: str,
         filter: ActionExecutionFilterTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListActionExecutionsOutputTypeDef:
         """
         Lists the action executions that have occurred in a pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.list_action_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/client/#list_action_executions)
         """
 
     async def list_action_types(
         self,
         *,
         actionOwnerFilter: ActionOwnerType = ...,
         nextToken: str = ...,
-        regionFilter: str = ...
+        regionFilter: str = ...,
     ) -> ListActionTypesOutputTypeDef:
         """
         Gets a summary of all CodePipeline action types associated with your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.list_action_types)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/client/#list_action_types)
         """
@@ -430,15 +429,15 @@
         """
 
     async def poll_for_jobs(
         self,
         *,
         actionTypeId: ActionTypeIdTypeDef,
         maxBatchSize: int = ...,
-        queryParam: Mapping[str, str] = ...
+        queryParam: Mapping[str, str] = ...,
     ) -> PollForJobsOutputTypeDef:
         """
         Returns information about any jobs for CodePipeline to act on.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.poll_for_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/client/#poll_for_jobs)
         """
@@ -455,15 +454,15 @@
 
     async def put_action_revision(
         self,
         *,
         pipelineName: str,
         stageName: str,
         actionName: str,
-        actionRevision: ActionRevisionTypeDef
+        actionRevision: ActionRevisionTypeDef,
     ) -> PutActionRevisionOutputTypeDef:
         """
         Provides information to CodePipeline about new revisions to a source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.put_action_revision)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/client/#put_action_revision)
         """
@@ -471,15 +470,15 @@
     async def put_approval_result(
         self,
         *,
         pipelineName: str,
         stageName: str,
         actionName: str,
         result: ApprovalResultTypeDef,
-        token: str
+        token: str,
     ) -> PutApprovalResultOutputTypeDef:
         """
         Provides the response to a manual approval request to CodePipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.put_approval_result)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/client/#put_approval_result)
         """
@@ -497,15 +496,15 @@
     async def put_job_success_result(
         self,
         *,
         jobId: str,
         currentRevision: CurrentRevisionTypeDef = ...,
         continuationToken: str = ...,
         executionDetails: ExecutionDetailsTypeDef = ...,
-        outputVariables: Mapping[str, str] = ...
+        outputVariables: Mapping[str, str] = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Represents the success of a job as returned to the pipeline by a job worker.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.put_job_success_result)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/client/#put_job_success_result)
         """
@@ -525,15 +524,15 @@
     async def put_third_party_job_success_result(
         self,
         *,
         jobId: str,
         clientToken: str,
         currentRevision: CurrentRevisionTypeDef = ...,
         continuationToken: str = ...,
-        executionDetails: ExecutionDetailsTypeDef = ...
+        executionDetails: ExecutionDetailsTypeDef = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Represents the success of a third party job as returned to the pipeline by a
         job
         worker.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.put_third_party_job_success_result)
@@ -562,15 +561,15 @@
 
     async def retry_stage_execution(
         self,
         *,
         pipelineName: str,
         stageName: str,
         pipelineExecutionId: str,
-        retryMode: StageRetryModeType
+        retryMode: StageRetryModeType,
     ) -> RetryStageExecutionOutputTypeDef:
         """
         You can retry a stage that has failed without having to run a pipeline again
         from the
         beginning.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.retry_stage_execution)
@@ -579,15 +578,15 @@
 
     async def start_pipeline_execution(
         self,
         *,
         name: str,
         variables: Sequence[PipelineVariableTypeDef] = ...,
         clientRequestToken: str = ...,
-        sourceRevisions: Sequence[SourceRevisionOverrideTypeDef] = ...
+        sourceRevisions: Sequence[SourceRevisionOverrideTypeDef] = ...,
     ) -> StartPipelineExecutionOutputTypeDef:
         """
         Starts the specified pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.start_pipeline_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/client/#start_pipeline_execution)
         """
```

### Comparing `types-aiobotocore-codepipeline-2.9.0/types_aiobotocore_codepipeline/client.pyi` & `types-aiobotocore-codepipeline-2.9.1/types_aiobotocore_codepipeline/client.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -193,15 +193,15 @@
         category: ActionCategoryType,
         provider: str,
         version: str,
         inputArtifactDetails: ArtifactDetailsTypeDef,
         outputArtifactDetails: ArtifactDetailsTypeDef,
         settings: ActionTypeSettingsTypeDef = ...,
         configurationProperties: Sequence[ActionConfigurationPropertyTypeDef] = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateCustomActionTypeOutputTypeDef:
         """
         Creates a new custom action that can be used in all pipelines associated with
         the Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.create_custom_action_type)
@@ -258,15 +258,15 @@
 
     async def disable_stage_transition(
         self,
         *,
         pipelineName: str,
         stageName: str,
         transitionType: StageTransitionTypeType,
-        reason: str
+        reason: str,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Prevents artifacts in a pipeline from transitioning to the next stage in the
         pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.disable_stage_transition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/client/#disable_stage_transition)
@@ -357,29 +357,29 @@
 
     async def list_action_executions(
         self,
         *,
         pipelineName: str,
         filter: ActionExecutionFilterTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListActionExecutionsOutputTypeDef:
         """
         Lists the action executions that have occurred in a pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.list_action_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/client/#list_action_executions)
         """
 
     async def list_action_types(
         self,
         *,
         actionOwnerFilter: ActionOwnerType = ...,
         nextToken: str = ...,
-        regionFilter: str = ...
+        regionFilter: str = ...,
     ) -> ListActionTypesOutputTypeDef:
         """
         Gets a summary of all CodePipeline action types associated with your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.list_action_types)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/client/#list_action_types)
         """
@@ -426,15 +426,15 @@
         """
 
     async def poll_for_jobs(
         self,
         *,
         actionTypeId: ActionTypeIdTypeDef,
         maxBatchSize: int = ...,
-        queryParam: Mapping[str, str] = ...
+        queryParam: Mapping[str, str] = ...,
     ) -> PollForJobsOutputTypeDef:
         """
         Returns information about any jobs for CodePipeline to act on.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.poll_for_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/client/#poll_for_jobs)
         """
@@ -451,15 +451,15 @@
 
     async def put_action_revision(
         self,
         *,
         pipelineName: str,
         stageName: str,
         actionName: str,
-        actionRevision: ActionRevisionTypeDef
+        actionRevision: ActionRevisionTypeDef,
     ) -> PutActionRevisionOutputTypeDef:
         """
         Provides information to CodePipeline about new revisions to a source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.put_action_revision)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/client/#put_action_revision)
         """
@@ -467,15 +467,15 @@
     async def put_approval_result(
         self,
         *,
         pipelineName: str,
         stageName: str,
         actionName: str,
         result: ApprovalResultTypeDef,
-        token: str
+        token: str,
     ) -> PutApprovalResultOutputTypeDef:
         """
         Provides the response to a manual approval request to CodePipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.put_approval_result)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/client/#put_approval_result)
         """
@@ -493,15 +493,15 @@
     async def put_job_success_result(
         self,
         *,
         jobId: str,
         currentRevision: CurrentRevisionTypeDef = ...,
         continuationToken: str = ...,
         executionDetails: ExecutionDetailsTypeDef = ...,
-        outputVariables: Mapping[str, str] = ...
+        outputVariables: Mapping[str, str] = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Represents the success of a job as returned to the pipeline by a job worker.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.put_job_success_result)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/client/#put_job_success_result)
         """
@@ -521,15 +521,15 @@
     async def put_third_party_job_success_result(
         self,
         *,
         jobId: str,
         clientToken: str,
         currentRevision: CurrentRevisionTypeDef = ...,
         continuationToken: str = ...,
-        executionDetails: ExecutionDetailsTypeDef = ...
+        executionDetails: ExecutionDetailsTypeDef = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Represents the success of a third party job as returned to the pipeline by a
         job
         worker.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.put_third_party_job_success_result)
@@ -558,15 +558,15 @@
 
     async def retry_stage_execution(
         self,
         *,
         pipelineName: str,
         stageName: str,
         pipelineExecutionId: str,
-        retryMode: StageRetryModeType
+        retryMode: StageRetryModeType,
     ) -> RetryStageExecutionOutputTypeDef:
         """
         You can retry a stage that has failed without having to run a pipeline again
         from the
         beginning.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.retry_stage_execution)
@@ -575,15 +575,15 @@
 
     async def start_pipeline_execution(
         self,
         *,
         name: str,
         variables: Sequence[PipelineVariableTypeDef] = ...,
         clientRequestToken: str = ...,
-        sourceRevisions: Sequence[SourceRevisionOverrideTypeDef] = ...
+        sourceRevisions: Sequence[SourceRevisionOverrideTypeDef] = ...,
     ) -> StartPipelineExecutionOutputTypeDef:
         """
         Starts the specified pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.start_pipeline_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/client/#start_pipeline_execution)
         """
```

### Comparing `types-aiobotocore-codepipeline-2.9.0/types_aiobotocore_codepipeline/literals.py` & `types-aiobotocore-codepipeline-2.9.1/types_aiobotocore_codepipeline/literals.py`

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
     "ActionCategoryType",
     "ActionConfigurationPropertyTypeType",
     "ActionExecutionStatusType",
     "ActionOwnerType",
     "ApprovalStatusType",
     "ArtifactLocationTypeType",
@@ -51,15 +50,14 @@
     "CodePipelineServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ActionCategoryType = Literal["Approval", "Build", "Deploy", "Invoke", "Source", "Test"]
 ActionConfigurationPropertyTypeType = Literal["Boolean", "Number", "String"]
 ActionExecutionStatusType = Literal["Abandoned", "Failed", "InProgress", "Succeeded"]
 ActionOwnerType = Literal["AWS", "Custom", "ThirdParty"]
 ApprovalStatusType = Literal["Approved", "Rejected"]
 ArtifactLocationTypeType = Literal["S3"]
 ArtifactStoreTypeType = Literal["S3"]
```

### Comparing `types-aiobotocore-codepipeline-2.9.0/types_aiobotocore_codepipeline/literals.pyi` & `types-aiobotocore-codepipeline-2.9.1/types_aiobotocore_codepipeline/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codepipeline-2.9.0/types_aiobotocore_codepipeline/paginator.py` & `types-aiobotocore-codepipeline-2.9.1/types_aiobotocore_codepipeline/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,14 @@
     "ListActionTypesPaginator",
     "ListPipelineExecutionsPaginator",
     "ListPipelinesPaginator",
     "ListTagsForResourcePaginator",
     "ListWebhooksPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -75,15 +74,15 @@
     """
 
     def paginate(
         self,
         *,
         pipelineName: str,
         filter: ActionExecutionFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListActionExecutionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListActionExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/paginators/#listactionexecutionspaginator)
         """
 
 
@@ -94,15 +93,15 @@
     """
 
     def paginate(
         self,
         *,
         actionOwnerFilter: ActionOwnerType = ...,
         regionFilter: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListActionTypesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListActionTypes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/paginators/#listactiontypespaginator)
         """
```

### Comparing `types-aiobotocore-codepipeline-2.9.0/types_aiobotocore_codepipeline/paginator.pyi` & `types-aiobotocore-codepipeline-2.9.1/types_aiobotocore_codepipeline/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     """
 
     def paginate(
         self,
         *,
         pipelineName: str,
         filter: ActionExecutionFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListActionExecutionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListActionExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/paginators/#listactionexecutionspaginator)
         """
 
 class ListActionTypesPaginator(AioPaginator):
@@ -90,15 +90,15 @@
     """
 
     def paginate(
         self,
         *,
         actionOwnerFilter: ActionOwnerType = ...,
         regionFilter: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListActionTypesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListActionTypes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/paginators/#listactiontypespaginator)
         """
 
 class ListPipelineExecutionsPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-codepipeline-2.9.0/types_aiobotocore_codepipeline/type_defs.py` & `types-aiobotocore-codepipeline-2.9.1/types_aiobotocore_codepipeline/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AWSSessionCredentialsTypeDef",
     "AcknowledgeJobInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AcknowledgeThirdPartyJobInputRequestTypeDef",
     "ActionConfigurationPropertyTypeDef",
     "ActionConfigurationTypeDef",
```

### Comparing `types-aiobotocore-codepipeline-2.9.0/types_aiobotocore_codepipeline/type_defs.pyi` & `types-aiobotocore-codepipeline-2.9.1/types_aiobotocore_codepipeline/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codepipeline-2.9.0/types_aiobotocore_codepipeline.egg-info/PKG-INFO` & `types-aiobotocore-codepipeline-2.9.1/types_aiobotocore_codepipeline.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codepipeline
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CodePipeline 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CodePipeline 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/
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
 
 <a id="types-aiobotocore-codepipeline"></a>
 
 # types-aiobotocore-codepipeline
 
 [![PyPI - types-aiobotocore-codepipeline](https://img.shields.io/pypi/v/types-aiobotocore-codepipeline.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codepipeline)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codepipeline.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codepipeline)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codepipeline)](https://pepy.tech/project/types-aiobotocore-codepipeline)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodePipeline 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
+[aiobotocore.CodePipeline 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
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
 [types-aiobotocore-codepipeline docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-codepipeline-2.9.0/types_aiobotocore_codepipeline.egg-info/SOURCES.txt` & `types-aiobotocore-codepipeline-2.9.1/types_aiobotocore_codepipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

