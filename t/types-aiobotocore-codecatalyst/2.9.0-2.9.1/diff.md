# Comparing `tmp/types-aiobotocore-codecatalyst-2.9.0.tar.gz` & `tmp/types-aiobotocore-codecatalyst-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-codecatalyst-2.9.0.tar", last modified: Wed Dec 13 19:58:53 2023, max compression
+gzip compressed data, was "types-aiobotocore-codecatalyst-2.9.1.tar", last modified: Thu Jan 18 01:20:19 2024, max compression
```

## Comparing `types-aiobotocore-codecatalyst-2.9.0.tar` & `types-aiobotocore-codecatalyst-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:53.333943 types-aiobotocore-codecatalyst-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:42:45.000000 types-aiobotocore-codecatalyst-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14640 2023-12-13 19:58:53.333943 types-aiobotocore-codecatalyst-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13057 2023-12-13 19:42:45.000000 types-aiobotocore-codecatalyst-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:53.333943 types-aiobotocore-codecatalyst-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2023-12-13 19:42:45.000000 types-aiobotocore-codecatalyst-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:53.333943 types-aiobotocore-codecatalyst-2.9.0/types_aiobotocore_codecatalyst/
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2023-12-13 19:42:45.000000 types-aiobotocore-codecatalyst-2.9.0/types_aiobotocore_codecatalyst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2023-12-13 19:42:45.000000 types-aiobotocore-codecatalyst-2.9.0/types_aiobotocore_codecatalyst/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      952 2023-12-13 19:42:45.000000 types-aiobotocore-codecatalyst-2.9.0/types_aiobotocore_codecatalyst/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33971 2023-12-13 19:42:46.000000 types-aiobotocore-codecatalyst-2.9.0/types_aiobotocore_codecatalyst/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    33967 2023-12-13 19:42:45.000000 types-aiobotocore-codecatalyst-2.9.0/types_aiobotocore_codecatalyst/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10640 2023-12-13 19:42:46.000000 types-aiobotocore-codecatalyst-2.9.0/types_aiobotocore_codecatalyst/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10638 2023-12-13 19:42:46.000000 types-aiobotocore-codecatalyst-2.9.0/types_aiobotocore_codecatalyst/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13247 2023-12-13 19:42:46.000000 types-aiobotocore-codecatalyst-2.9.0/types_aiobotocore_codecatalyst/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    13235 2023-12-13 19:42:46.000000 types-aiobotocore-codecatalyst-2.9.0/types_aiobotocore_codecatalyst/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:42:45.000000 types-aiobotocore-codecatalyst-2.9.0/types_aiobotocore_codecatalyst/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    34372 2023-12-13 19:42:47.000000 types-aiobotocore-codecatalyst-2.9.0/types_aiobotocore_codecatalyst/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    34371 2023-12-13 19:42:46.000000 types-aiobotocore-codecatalyst-2.9.0/types_aiobotocore_codecatalyst/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:42:45.000000 types-aiobotocore-codecatalyst-2.9.0/types_aiobotocore_codecatalyst/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:53.333943 types-aiobotocore-codecatalyst-2.9.0/types_aiobotocore_codecatalyst.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14640 2023-12-13 19:58:53.000000 types-aiobotocore-codecatalyst-2.9.0/types_aiobotocore_codecatalyst.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      908 2023-12-13 19:58:53.000000 types-aiobotocore-codecatalyst-2.9.0/types_aiobotocore_codecatalyst.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:53.000000 types-aiobotocore-codecatalyst-2.9.0/types_aiobotocore_codecatalyst.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:53.000000 types-aiobotocore-codecatalyst-2.9.0/types_aiobotocore_codecatalyst.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:53.000000 types-aiobotocore-codecatalyst-2.9.0/types_aiobotocore_codecatalyst.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-13 19:58:53.000000 types-aiobotocore-codecatalyst-2.9.0/types_aiobotocore_codecatalyst.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:19.785446 types-aiobotocore-codecatalyst-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:04:41.000000 types-aiobotocore-codecatalyst-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14660 2024-01-18 01:20:19.785446 types-aiobotocore-codecatalyst-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13057 2024-01-18 01:04:41.000000 types-aiobotocore-codecatalyst-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:19.785446 types-aiobotocore-codecatalyst-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-01-18 01:04:41.000000 types-aiobotocore-codecatalyst-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:19.785446 types-aiobotocore-codecatalyst-2.9.1/types_aiobotocore_codecatalyst/
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-01-18 01:04:41.000000 types-aiobotocore-codecatalyst-2.9.1/types_aiobotocore_codecatalyst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-01-18 01:04:41.000000 types-aiobotocore-codecatalyst-2.9.1/types_aiobotocore_codecatalyst/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-01-18 01:04:41.000000 types-aiobotocore-codecatalyst-2.9.1/types_aiobotocore_codecatalyst/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33982 2024-01-18 01:04:42.000000 types-aiobotocore-codecatalyst-2.9.1/types_aiobotocore_codecatalyst/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33979 2024-01-18 01:04:41.000000 types-aiobotocore-codecatalyst-2.9.1/types_aiobotocore_codecatalyst/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10638 2024-01-18 01:04:43.000000 types-aiobotocore-codecatalyst-2.9.1/types_aiobotocore_codecatalyst/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10638 2024-01-18 01:04:43.000000 types-aiobotocore-codecatalyst-2.9.1/types_aiobotocore_codecatalyst/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13253 2024-01-18 01:04:42.000000 types-aiobotocore-codecatalyst-2.9.1/types_aiobotocore_codecatalyst/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13242 2024-01-18 01:04:42.000000 types-aiobotocore-codecatalyst-2.9.1/types_aiobotocore_codecatalyst/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:04:41.000000 types-aiobotocore-codecatalyst-2.9.1/types_aiobotocore_codecatalyst/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    34371 2024-01-18 01:04:43.000000 types-aiobotocore-codecatalyst-2.9.1/types_aiobotocore_codecatalyst/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34371 2024-01-18 01:04:43.000000 types-aiobotocore-codecatalyst-2.9.1/types_aiobotocore_codecatalyst/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:04:41.000000 types-aiobotocore-codecatalyst-2.9.1/types_aiobotocore_codecatalyst/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:19.785446 types-aiobotocore-codecatalyst-2.9.1/types_aiobotocore_codecatalyst.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14660 2024-01-18 01:20:19.000000 types-aiobotocore-codecatalyst-2.9.1/types_aiobotocore_codecatalyst.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-01-18 01:20:19.000000 types-aiobotocore-codecatalyst-2.9.1/types_aiobotocore_codecatalyst.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:19.000000 types-aiobotocore-codecatalyst-2.9.1/types_aiobotocore_codecatalyst.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:19.000000 types-aiobotocore-codecatalyst-2.9.1/types_aiobotocore_codecatalyst.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:19.000000 types-aiobotocore-codecatalyst-2.9.1/types_aiobotocore_codecatalyst.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-01-18 01:20:19.000000 types-aiobotocore-codecatalyst-2.9.1/types_aiobotocore_codecatalyst.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-codecatalyst-2.9.0/LICENSE` & `types-aiobotocore-codecatalyst-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-codecatalyst-2.9.0/PKG-INFO` & `types-aiobotocore-codecatalyst-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codecatalyst
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CodeCatalyst 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CodeCatalyst 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/
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
 
 <a id="types-aiobotocore-codecatalyst"></a>
 
 # types-aiobotocore-codecatalyst
 
 [![PyPI - types-aiobotocore-codecatalyst](https://img.shields.io/pypi/v/types-aiobotocore-codecatalyst.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codecatalyst)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codecatalyst.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codecatalyst)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codecatalyst)](https://pepy.tech/project/types-aiobotocore-codecatalyst)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeCatalyst 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst)
+[aiobotocore.CodeCatalyst 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst)
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
 [types-aiobotocore-codecatalyst docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-codecatalyst-2.9.0/README.md` & `types-aiobotocore-codecatalyst-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codecatalyst.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codecatalyst)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codecatalyst)](https://pepy.tech/project/types-aiobotocore-codecatalyst)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeCatalyst 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst)
+[aiobotocore.CodeCatalyst 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst)
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
 [types-aiobotocore-codecatalyst docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-codecatalyst-2.9.0/setup.py` & `types-aiobotocore-codecatalyst-2.9.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-codecatalyst",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_codecatalyst"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CodeCatalyst 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.CodeCatalyst 2.9.1 service generated with"
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
     keywords="aiobotocore codecatalyst type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_codecatalyst": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-codecatalyst-2.9.0/types_aiobotocore_codecatalyst/__init__.py` & `types-aiobotocore-codecatalyst-2.9.1/types_aiobotocore_codecatalyst/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,14 @@
     ListSpacesPaginator,
     ListWorkflowRunsPaginator,
     ListWorkflowsPaginator,
 )
 
 Client = CodeCatalystClient
 
-
 __all__ = (
     "Client",
     "CodeCatalystClient",
     "ListAccessTokensPaginator",
     "ListDevEnvironmentSessionsPaginator",
     "ListDevEnvironmentsPaginator",
     "ListEventLogsPaginator",
```

### Comparing `types-aiobotocore-codecatalyst-2.9.0/types_aiobotocore_codecatalyst/__init__.pyi` & `types-aiobotocore-codecatalyst-2.9.1/types_aiobotocore_codecatalyst/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codecatalyst-2.9.0/types_aiobotocore_codecatalyst/__main__.py` & `types-aiobotocore-codecatalyst-2.9.1/types_aiobotocore_codecatalyst/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CodeCatalyst 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.CodeCatalyst 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst\nOther"
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

### Comparing `types-aiobotocore-codecatalyst-2.9.0/types_aiobotocore_codecatalyst/client.py` & `types-aiobotocore-codecatalyst-2.9.1/types_aiobotocore_codecatalyst/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("CodeCatalystClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -159,15 +158,15 @@
         instanceType: InstanceTypeType,
         persistentStorage: PersistentStorageConfigurationTypeDef,
         repositories: Sequence[RepositoryInputTypeDef] = ...,
         clientToken: str = ...,
         alias: str = ...,
         ides: Sequence[IdeConfigurationTypeDef] = ...,
         inactivityTimeoutMinutes: int = ...,
-        vpcConnectionName: str = ...
+        vpcConnectionName: str = ...,
     ) -> CreateDevEnvironmentResponseTypeDef:
         """
         Creates a Dev Environment in Amazon CodeCatalyst, a cloud-based development
         environment that you can use to quickly work on the code stored in the source
         repositories of your
         project.
 
@@ -198,15 +197,15 @@
     async def create_source_repository_branch(
         self,
         *,
         spaceName: str,
         projectName: str,
         sourceRepositoryName: str,
         name: str,
-        headCommitId: str = ...
+        headCommitId: str = ...,
     ) -> CreateSourceRepositoryBranchResponseTypeDef:
         """
         Creates a branch in a specified source repository in Amazon CodeCatalyst.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.create_source_repository_branch)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/client/#create_source_repository_branch)
         """
@@ -372,15 +371,15 @@
     async def list_dev_environment_sessions(
         self,
         *,
         spaceName: str,
         projectName: str,
         devEnvironmentId: str,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListDevEnvironmentSessionsResponseTypeDef:
         """
         Retrieves a list of active sessions for a Dev Environment in a project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.list_dev_environment_sessions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/client/#list_dev_environment_sessions)
         """
@@ -388,15 +387,15 @@
     async def list_dev_environments(
         self,
         *,
         spaceName: str,
         projectName: str = ...,
         filters: Sequence[FilterTypeDef] = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListDevEnvironmentsResponseTypeDef:
         """
         Retrieves a list of Dev Environments in a project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.list_dev_environments)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/client/#list_dev_environments)
         """
@@ -405,30 +404,30 @@
         self,
         *,
         spaceName: str,
         startTime: TimestampTypeDef,
         endTime: TimestampTypeDef,
         eventName: str = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListEventLogsResponseTypeDef:
         """
         Retrieves a list of events that occurred during a specific time in a space.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.list_event_logs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/client/#list_event_logs)
         """
 
     async def list_projects(
         self,
         *,
         spaceName: str,
         nextToken: str = ...,
         maxResults: int = ...,
-        filters: Sequence[ProjectListFilterTypeDef] = ...
+        filters: Sequence[ProjectListFilterTypeDef] = ...,
     ) -> ListProjectsResponseTypeDef:
         """
         Retrieves a list of projects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.list_projects)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/client/#list_projects)
         """
@@ -446,15 +445,15 @@
     async def list_source_repository_branches(
         self,
         *,
         spaceName: str,
         projectName: str,
         sourceRepositoryName: str,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListSourceRepositoryBranchesResponseTypeDef:
         """
         Retrieves a list of branches in a specified source repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.list_source_repository_branches)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/client/#list_source_repository_branches)
         """
@@ -471,15 +470,15 @@
         self,
         *,
         spaceName: str,
         projectName: str,
         workflowId: str = ...,
         nextToken: str = ...,
         maxResults: int = ...,
-        sortBy: Sequence[Mapping[str, Any]] = ...
+        sortBy: Sequence[Mapping[str, Any]] = ...,
     ) -> ListWorkflowRunsResponseTypeDef:
         """
         Retrieves a list of workflow runs of a specified workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.list_workflow_runs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/client/#list_workflow_runs)
         """
@@ -487,15 +486,15 @@
     async def list_workflows(
         self,
         *,
         spaceName: str,
         projectName: str,
         nextToken: str = ...,
         maxResults: int = ...,
-        sortBy: Sequence[Mapping[str, Any]] = ...
+        sortBy: Sequence[Mapping[str, Any]] = ...,
     ) -> ListWorkflowsResponseTypeDef:
         """
         Retrieves a list of workflows in a specified project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.list_workflows)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/client/#list_workflows)
         """
@@ -504,30 +503,30 @@
         self,
         *,
         spaceName: str,
         projectName: str,
         id: str,
         ides: Sequence[IdeConfigurationTypeDef] = ...,
         instanceType: InstanceTypeType = ...,
-        inactivityTimeoutMinutes: int = ...
+        inactivityTimeoutMinutes: int = ...,
     ) -> StartDevEnvironmentResponseTypeDef:
         """
         Starts a specified Dev Environment and puts it into an active state.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.start_dev_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/client/#start_dev_environment)
         """
 
     async def start_dev_environment_session(
         self,
         *,
         spaceName: str,
         projectName: str,
         id: str,
-        sessionConfiguration: DevEnvironmentSessionConfigurationTypeDef
+        sessionConfiguration: DevEnvironmentSessionConfigurationTypeDef,
     ) -> StartDevEnvironmentSessionResponseTypeDef:
         """
         Starts a session for a specified Dev Environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.start_dev_environment_session)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/client/#start_dev_environment_session)
         """
@@ -568,15 +567,15 @@
         spaceName: str,
         projectName: str,
         id: str,
         alias: str = ...,
         ides: Sequence[IdeConfigurationTypeDef] = ...,
         instanceType: InstanceTypeType = ...,
         inactivityTimeoutMinutes: int = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> UpdateDevEnvironmentResponseTypeDef:
         """
         Changes one or more values for a Dev Environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.update_dev_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/client/#update_dev_environment)
         """
```

### Comparing `types-aiobotocore-codecatalyst-2.9.0/types_aiobotocore_codecatalyst/client.pyi` & `types-aiobotocore-codecatalyst-2.9.1/types_aiobotocore_codecatalyst/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,15 @@
         instanceType: InstanceTypeType,
         persistentStorage: PersistentStorageConfigurationTypeDef,
         repositories: Sequence[RepositoryInputTypeDef] = ...,
         clientToken: str = ...,
         alias: str = ...,
         ides: Sequence[IdeConfigurationTypeDef] = ...,
         inactivityTimeoutMinutes: int = ...,
-        vpcConnectionName: str = ...
+        vpcConnectionName: str = ...,
     ) -> CreateDevEnvironmentResponseTypeDef:
         """
         Creates a Dev Environment in Amazon CodeCatalyst, a cloud-based development
         environment that you can use to quickly work on the code stored in the source
         repositories of your
         project.
 
@@ -194,15 +194,15 @@
     async def create_source_repository_branch(
         self,
         *,
         spaceName: str,
         projectName: str,
         sourceRepositoryName: str,
         name: str,
-        headCommitId: str = ...
+        headCommitId: str = ...,
     ) -> CreateSourceRepositoryBranchResponseTypeDef:
         """
         Creates a branch in a specified source repository in Amazon CodeCatalyst.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.create_source_repository_branch)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/client/#create_source_repository_branch)
         """
@@ -368,15 +368,15 @@
     async def list_dev_environment_sessions(
         self,
         *,
         spaceName: str,
         projectName: str,
         devEnvironmentId: str,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListDevEnvironmentSessionsResponseTypeDef:
         """
         Retrieves a list of active sessions for a Dev Environment in a project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.list_dev_environment_sessions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/client/#list_dev_environment_sessions)
         """
@@ -384,15 +384,15 @@
     async def list_dev_environments(
         self,
         *,
         spaceName: str,
         projectName: str = ...,
         filters: Sequence[FilterTypeDef] = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListDevEnvironmentsResponseTypeDef:
         """
         Retrieves a list of Dev Environments in a project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.list_dev_environments)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/client/#list_dev_environments)
         """
@@ -401,30 +401,30 @@
         self,
         *,
         spaceName: str,
         startTime: TimestampTypeDef,
         endTime: TimestampTypeDef,
         eventName: str = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListEventLogsResponseTypeDef:
         """
         Retrieves a list of events that occurred during a specific time in a space.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.list_event_logs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/client/#list_event_logs)
         """
 
     async def list_projects(
         self,
         *,
         spaceName: str,
         nextToken: str = ...,
         maxResults: int = ...,
-        filters: Sequence[ProjectListFilterTypeDef] = ...
+        filters: Sequence[ProjectListFilterTypeDef] = ...,
     ) -> ListProjectsResponseTypeDef:
         """
         Retrieves a list of projects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.list_projects)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/client/#list_projects)
         """
@@ -442,15 +442,15 @@
     async def list_source_repository_branches(
         self,
         *,
         spaceName: str,
         projectName: str,
         sourceRepositoryName: str,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListSourceRepositoryBranchesResponseTypeDef:
         """
         Retrieves a list of branches in a specified source repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.list_source_repository_branches)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/client/#list_source_repository_branches)
         """
@@ -467,15 +467,15 @@
         self,
         *,
         spaceName: str,
         projectName: str,
         workflowId: str = ...,
         nextToken: str = ...,
         maxResults: int = ...,
-        sortBy: Sequence[Mapping[str, Any]] = ...
+        sortBy: Sequence[Mapping[str, Any]] = ...,
     ) -> ListWorkflowRunsResponseTypeDef:
         """
         Retrieves a list of workflow runs of a specified workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.list_workflow_runs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/client/#list_workflow_runs)
         """
@@ -483,15 +483,15 @@
     async def list_workflows(
         self,
         *,
         spaceName: str,
         projectName: str,
         nextToken: str = ...,
         maxResults: int = ...,
-        sortBy: Sequence[Mapping[str, Any]] = ...
+        sortBy: Sequence[Mapping[str, Any]] = ...,
     ) -> ListWorkflowsResponseTypeDef:
         """
         Retrieves a list of workflows in a specified project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.list_workflows)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/client/#list_workflows)
         """
@@ -500,30 +500,30 @@
         self,
         *,
         spaceName: str,
         projectName: str,
         id: str,
         ides: Sequence[IdeConfigurationTypeDef] = ...,
         instanceType: InstanceTypeType = ...,
-        inactivityTimeoutMinutes: int = ...
+        inactivityTimeoutMinutes: int = ...,
     ) -> StartDevEnvironmentResponseTypeDef:
         """
         Starts a specified Dev Environment and puts it into an active state.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.start_dev_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/client/#start_dev_environment)
         """
 
     async def start_dev_environment_session(
         self,
         *,
         spaceName: str,
         projectName: str,
         id: str,
-        sessionConfiguration: DevEnvironmentSessionConfigurationTypeDef
+        sessionConfiguration: DevEnvironmentSessionConfigurationTypeDef,
     ) -> StartDevEnvironmentSessionResponseTypeDef:
         """
         Starts a session for a specified Dev Environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.start_dev_environment_session)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/client/#start_dev_environment_session)
         """
@@ -564,15 +564,15 @@
         spaceName: str,
         projectName: str,
         id: str,
         alias: str = ...,
         ides: Sequence[IdeConfigurationTypeDef] = ...,
         instanceType: InstanceTypeType = ...,
         inactivityTimeoutMinutes: int = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> UpdateDevEnvironmentResponseTypeDef:
         """
         Changes one or more values for a Dev Environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.update_dev_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/client/#update_dev_environment)
         """
```

### Comparing `types-aiobotocore-codecatalyst-2.9.0/types_aiobotocore_codecatalyst/literals.py` & `types-aiobotocore-codecatalyst-2.9.1/types_aiobotocore_codecatalyst/literals.py`

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
     "ComparisonOperatorType",
     "DevEnvironmentSessionTypeType",
     "DevEnvironmentStatusType",
     "FilterKeyType",
     "InstanceTypeType",
     "ListAccessTokensPaginatorName",
@@ -43,15 +42,14 @@
     "WorkflowStatusType",
     "CodeCatalystServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 ComparisonOperatorType = Literal["BEGINS_WITH", "EQ", "GE", "GT", "LE", "LT"]
 DevEnvironmentSessionTypeType = Literal["SSH", "SSM"]
 DevEnvironmentStatusType = Literal[
     "DELETED", "DELETING", "FAILED", "PENDING", "RUNNING", "STARTING", "STOPPED", "STOPPING"
 ]
 FilterKeyType = Literal["hasAccessTo", "name"]
 InstanceTypeType = Literal[
```

### Comparing `types-aiobotocore-codecatalyst-2.9.0/types_aiobotocore_codecatalyst/literals.pyi` & `types-aiobotocore-codecatalyst-2.9.1/types_aiobotocore_codecatalyst/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codecatalyst-2.9.0/types_aiobotocore_codecatalyst/paginator.py` & `types-aiobotocore-codecatalyst-2.9.1/types_aiobotocore_codecatalyst/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,14 @@
     "ListSourceRepositoriesPaginator",
     "ListSourceRepositoryBranchesPaginator",
     "ListSpacesPaginator",
     "ListWorkflowRunsPaginator",
     "ListWorkflowsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -108,15 +107,15 @@
 
     def paginate(
         self,
         *,
         spaceName: str,
         projectName: str,
         devEnvironmentId: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDevEnvironmentSessionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListDevEnvironmentSessions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/paginators/#listdevenvironmentsessionspaginator)
         """
 
 
@@ -128,15 +127,15 @@
 
     def paginate(
         self,
         *,
         spaceName: str,
         projectName: str = ...,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDevEnvironmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListDevEnvironments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/paginators/#listdevenvironmentspaginator)
         """
 
 
@@ -149,15 +148,15 @@
     def paginate(
         self,
         *,
         spaceName: str,
         startTime: TimestampTypeDef,
         endTime: TimestampTypeDef,
         eventName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEventLogsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListEventLogs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/paginators/#listeventlogspaginator)
         """
 
 
@@ -168,15 +167,15 @@
     """
 
     def paginate(
         self,
         *,
         spaceName: str,
         filters: Sequence[ProjectListFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListProjectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListProjects.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/paginators/#listprojectspaginator)
         """
 
 
@@ -203,15 +202,15 @@
 
     def paginate(
         self,
         *,
         spaceName: str,
         projectName: str,
         sourceRepositoryName: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSourceRepositoryBranchesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListSourceRepositoryBranches.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/paginators/#listsourcerepositorybranchespaginator)
         """
 
 
@@ -239,15 +238,15 @@
     def paginate(
         self,
         *,
         spaceName: str,
         projectName: str,
         workflowId: str = ...,
         sortBy: Sequence[Mapping[str, Any]] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListWorkflowRunsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListWorkflowRuns.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/paginators/#listworkflowrunspaginator)
         """
 
 
@@ -259,13 +258,13 @@
 
     def paginate(
         self,
         *,
         spaceName: str,
         projectName: str,
         sortBy: Sequence[Mapping[str, Any]] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListWorkflowsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListWorkflows.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/paginators/#listworkflowspaginator)
         """
```

### Comparing `types-aiobotocore-codecatalyst-2.9.0/types_aiobotocore_codecatalyst/paginator.pyi` & `types-aiobotocore-codecatalyst-2.9.1/types_aiobotocore_codecatalyst/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 
     def paginate(
         self,
         *,
         spaceName: str,
         projectName: str,
         devEnvironmentId: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDevEnvironmentSessionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListDevEnvironmentSessions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/paginators/#listdevenvironmentsessionspaginator)
         """
 
 class ListDevEnvironmentsPaginator(AioPaginator):
@@ -123,15 +123,15 @@
 
     def paginate(
         self,
         *,
         spaceName: str,
         projectName: str = ...,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDevEnvironmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListDevEnvironments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/paginators/#listdevenvironmentspaginator)
         """
 
 class ListEventLogsPaginator(AioPaginator):
@@ -143,15 +143,15 @@
     def paginate(
         self,
         *,
         spaceName: str,
         startTime: TimestampTypeDef,
         endTime: TimestampTypeDef,
         eventName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEventLogsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListEventLogs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/paginators/#listeventlogspaginator)
         """
 
 class ListProjectsPaginator(AioPaginator):
@@ -161,15 +161,15 @@
     """
 
     def paginate(
         self,
         *,
         spaceName: str,
         filters: Sequence[ProjectListFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListProjectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListProjects.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/paginators/#listprojectspaginator)
         """
 
 class ListSourceRepositoriesPaginator(AioPaginator):
@@ -194,15 +194,15 @@
 
     def paginate(
         self,
         *,
         spaceName: str,
         projectName: str,
         sourceRepositoryName: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSourceRepositoryBranchesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListSourceRepositoryBranches.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/paginators/#listsourcerepositorybranchespaginator)
         """
 
 class ListSpacesPaginator(AioPaginator):
@@ -228,15 +228,15 @@
     def paginate(
         self,
         *,
         spaceName: str,
         projectName: str,
         workflowId: str = ...,
         sortBy: Sequence[Mapping[str, Any]] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListWorkflowRunsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListWorkflowRuns.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/paginators/#listworkflowrunspaginator)
         """
 
 class ListWorkflowsPaginator(AioPaginator):
@@ -247,13 +247,13 @@
 
     def paginate(
         self,
         *,
         spaceName: str,
         projectName: str,
         sortBy: Sequence[Mapping[str, Any]] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListWorkflowsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListWorkflows.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/paginators/#listworkflowspaginator)
         """
```

### Comparing `types-aiobotocore-codecatalyst-2.9.0/types_aiobotocore_codecatalyst/type_defs.py` & `types-aiobotocore-codecatalyst-2.9.1/types_aiobotocore_codecatalyst/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccessTokenSummaryTypeDef",
     "TimestampTypeDef",
     "ResponseMetadataTypeDef",
     "IdeConfigurationTypeDef",
     "PersistentStorageConfigurationTypeDef",
     "RepositoryInputTypeDef",
```

### Comparing `types-aiobotocore-codecatalyst-2.9.0/types_aiobotocore_codecatalyst/type_defs.pyi` & `types-aiobotocore-codecatalyst-2.9.1/types_aiobotocore_codecatalyst/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codecatalyst-2.9.0/types_aiobotocore_codecatalyst.egg-info/PKG-INFO` & `types-aiobotocore-codecatalyst-2.9.1/types_aiobotocore_codecatalyst.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codecatalyst
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CodeCatalyst 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CodeCatalyst 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/
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
 
 <a id="types-aiobotocore-codecatalyst"></a>
 
 # types-aiobotocore-codecatalyst
 
 [![PyPI - types-aiobotocore-codecatalyst](https://img.shields.io/pypi/v/types-aiobotocore-codecatalyst.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codecatalyst)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codecatalyst.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codecatalyst)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codecatalyst)](https://pepy.tech/project/types-aiobotocore-codecatalyst)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeCatalyst 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst)
+[aiobotocore.CodeCatalyst 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst)
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
 [types-aiobotocore-codecatalyst docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-codecatalyst-2.9.0/types_aiobotocore_codecatalyst.egg-info/SOURCES.txt` & `types-aiobotocore-codecatalyst-2.9.1/types_aiobotocore_codecatalyst.egg-info/SOURCES.txt`

 * *Files identical despite different names*

