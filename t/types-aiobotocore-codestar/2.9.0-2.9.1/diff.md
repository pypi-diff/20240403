# Comparing `tmp/types-aiobotocore-codestar-2.9.0.tar.gz` & `tmp/types-aiobotocore-codestar-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-codestar-2.9.0.tar", last modified: Wed Dec 13 19:58:56 2023, max compression
+gzip compressed data, was "types-aiobotocore-codestar-2.9.1.tar", last modified: Thu Jan 18 01:20:22 2024, max compression
```

## Comparing `types-aiobotocore-codestar-2.9.0.tar` & `types-aiobotocore-codestar-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:56.701915 types-aiobotocore-codestar-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:43:00.000000 types-aiobotocore-codestar-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13470 2023-12-13 19:58:56.701915 types-aiobotocore-codestar-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11903 2023-12-13 19:43:00.000000 types-aiobotocore-codestar-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:56.701915 types-aiobotocore-codestar-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2023-12-13 19:43:00.000000 types-aiobotocore-codestar-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:56.697915 types-aiobotocore-codestar-2.9.0/types_aiobotocore_codestar/
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2023-12-13 19:43:00.000000 types-aiobotocore-codestar-2.9.0/types_aiobotocore_codestar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2023-12-13 19:43:00.000000 types-aiobotocore-codestar-2.9.0/types_aiobotocore_codestar/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      936 2023-12-13 19:43:00.000000 types-aiobotocore-codestar-2.9.0/types_aiobotocore_codestar/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17222 2023-12-13 19:43:00.000000 types-aiobotocore-codestar-2.9.0/types_aiobotocore_codestar/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    17218 2023-12-13 19:43:00.000000 types-aiobotocore-codestar-2.9.0/types_aiobotocore_codestar/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8903 2023-12-13 19:43:00.000000 types-aiobotocore-codestar-2.9.0/types_aiobotocore_codestar/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8901 2023-12-13 19:43:00.000000 types-aiobotocore-codestar-2.9.0/types_aiobotocore_codestar/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5224 2023-12-13 19:43:00.000000 types-aiobotocore-codestar-2.9.0/types_aiobotocore_codestar/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5218 2023-12-13 19:43:00.000000 types-aiobotocore-codestar-2.9.0/types_aiobotocore_codestar/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:43:00.000000 types-aiobotocore-codestar-2.9.0/types_aiobotocore_codestar/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    13608 2023-12-13 19:43:00.000000 types-aiobotocore-codestar-2.9.0/types_aiobotocore_codestar/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    13607 2023-12-13 19:43:00.000000 types-aiobotocore-codestar-2.9.0/types_aiobotocore_codestar/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:43:00.000000 types-aiobotocore-codestar-2.9.0/types_aiobotocore_codestar/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:56.701915 types-aiobotocore-codestar-2.9.0/types_aiobotocore_codestar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13470 2023-12-13 19:58:56.000000 types-aiobotocore-codestar-2.9.0/types_aiobotocore_codestar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      832 2023-12-13 19:58:56.000000 types-aiobotocore-codestar-2.9.0/types_aiobotocore_codestar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:56.000000 types-aiobotocore-codestar-2.9.0/types_aiobotocore_codestar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:56.000000 types-aiobotocore-codestar-2.9.0/types_aiobotocore_codestar.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:56.000000 types-aiobotocore-codestar-2.9.0/types_aiobotocore_codestar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-13 19:58:56.000000 types-aiobotocore-codestar-2.9.0/types_aiobotocore_codestar.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:22.849431 types-aiobotocore-codestar-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:04:56.000000 types-aiobotocore-codestar-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13490 2024-01-18 01:20:22.849431 types-aiobotocore-codestar-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11903 2024-01-18 01:04:56.000000 types-aiobotocore-codestar-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:22.849431 types-aiobotocore-codestar-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-01-18 01:04:55.000000 types-aiobotocore-codestar-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:22.845431 types-aiobotocore-codestar-2.9.1/types_aiobotocore_codestar/
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-01-18 01:04:56.000000 types-aiobotocore-codestar-2.9.1/types_aiobotocore_codestar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-01-18 01:04:56.000000 types-aiobotocore-codestar-2.9.1/types_aiobotocore_codestar/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-01-18 01:04:56.000000 types-aiobotocore-codestar-2.9.1/types_aiobotocore_codestar/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17225 2024-01-18 01:04:56.000000 types-aiobotocore-codestar-2.9.1/types_aiobotocore_codestar/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17222 2024-01-18 01:04:56.000000 types-aiobotocore-codestar-2.9.1/types_aiobotocore_codestar/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8901 2024-01-18 01:04:56.000000 types-aiobotocore-codestar-2.9.1/types_aiobotocore_codestar/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8901 2024-01-18 01:04:56.000000 types-aiobotocore-codestar-2.9.1/types_aiobotocore_codestar/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5223 2024-01-18 01:04:56.000000 types-aiobotocore-codestar-2.9.1/types_aiobotocore_codestar/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-01-18 01:04:56.000000 types-aiobotocore-codestar-2.9.1/types_aiobotocore_codestar/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:04:56.000000 types-aiobotocore-codestar-2.9.1/types_aiobotocore_codestar/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    13607 2024-01-18 01:04:56.000000 types-aiobotocore-codestar-2.9.1/types_aiobotocore_codestar/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13607 2024-01-18 01:04:56.000000 types-aiobotocore-codestar-2.9.1/types_aiobotocore_codestar/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:04:56.000000 types-aiobotocore-codestar-2.9.1/types_aiobotocore_codestar/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:22.849431 types-aiobotocore-codestar-2.9.1/types_aiobotocore_codestar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13490 2024-01-18 01:20:22.000000 types-aiobotocore-codestar-2.9.1/types_aiobotocore_codestar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-01-18 01:20:22.000000 types-aiobotocore-codestar-2.9.1/types_aiobotocore_codestar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:22.000000 types-aiobotocore-codestar-2.9.1/types_aiobotocore_codestar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:22.000000 types-aiobotocore-codestar-2.9.1/types_aiobotocore_codestar.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:22.000000 types-aiobotocore-codestar-2.9.1/types_aiobotocore_codestar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-18 01:20:22.000000 types-aiobotocore-codestar-2.9.1/types_aiobotocore_codestar.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-codestar-2.9.0/LICENSE` & `types-aiobotocore-codestar-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-codestar-2.9.0/PKG-INFO` & `types-aiobotocore-codestar-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codestar
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CodeStar 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CodeStar 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/
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
 
 <a id="types-aiobotocore-codestar"></a>
 
 # types-aiobotocore-codestar
 
 [![PyPI - types-aiobotocore-codestar](https://img.shields.io/pypi/v/types-aiobotocore-codestar.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codestar)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codestar.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codestar)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codestar)](https://pepy.tech/project/types-aiobotocore-codestar)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeStar 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar)
+[aiobotocore.CodeStar 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar)
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
 [types-aiobotocore-codestar docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-codestar-2.9.0/README.md` & `types-aiobotocore-codestar-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codestar.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codestar)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codestar)](https://pepy.tech/project/types-aiobotocore-codestar)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeStar 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar)
+[aiobotocore.CodeStar 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar)
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
 [types-aiobotocore-codestar docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-codestar-2.9.0/setup.py` & `types-aiobotocore-codestar-2.9.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-codestar",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_codestar"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CodeStar 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.CodeStar 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore codestar type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_codestar": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-codestar-2.9.0/types_aiobotocore_codestar/__init__.py` & `types-aiobotocore-codestar-2.9.1/types_aiobotocore_codestar/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     ListResourcesPaginator,
     ListTeamMembersPaginator,
     ListUserProfilesPaginator,
 )
 
 Client = CodeStarClient
 
-
 __all__ = (
     "Client",
     "CodeStarClient",
     "ListProjectsPaginator",
     "ListResourcesPaginator",
     "ListTeamMembersPaginator",
     "ListUserProfilesPaginator",
```

### Comparing `types-aiobotocore-codestar-2.9.0/types_aiobotocore_codestar/__init__.pyi` & `types-aiobotocore-codestar-2.9.1/types_aiobotocore_codestar/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-2.9.0/types_aiobotocore_codestar/__main__.py` & `types-aiobotocore-codestar-2.9.1/types_aiobotocore_codestar/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CodeStar 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.CodeStar 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar\nOther"
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

### Comparing `types-aiobotocore-codestar-2.9.0/types_aiobotocore_codestar/client.py` & `types-aiobotocore-codestar-2.9.1/types_aiobotocore_codestar/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("CodeStarClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -101,15 +100,15 @@
     async def associate_team_member(
         self,
         *,
         projectId: str,
         userArn: str,
         projectRole: str,
         clientRequestToken: str = ...,
-        remoteAccessAllowed: bool = ...
+        remoteAccessAllowed: bool = ...,
     ) -> AssociateTeamMemberResultTypeDef:
         """
         Adds an IAM user to the team for an AWS CodeStar project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Client.associate_team_member)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/client/#associate_team_member)
         """
@@ -135,15 +134,15 @@
         *,
         name: str,
         id: str,
         description: str = ...,
         clientRequestToken: str = ...,
         sourceCode: Sequence[CodeTypeDef] = ...,
         toolchain: ToolchainTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateProjectResultTypeDef:
         """
         Creates a project, including project resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Client.create_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/client/#create_project)
         """
@@ -296,30 +295,30 @@
 
     async def update_team_member(
         self,
         *,
         projectId: str,
         userArn: str,
         projectRole: str = ...,
-        remoteAccessAllowed: bool = ...
+        remoteAccessAllowed: bool = ...,
     ) -> UpdateTeamMemberResultTypeDef:
         """
         Updates a team member's attributes in an AWS CodeStar project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Client.update_team_member)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/client/#update_team_member)
         """
 
     async def update_user_profile(
         self,
         *,
         userArn: str,
         displayName: str = ...,
         emailAddress: str = ...,
-        sshPublicKey: str = ...
+        sshPublicKey: str = ...,
     ) -> UpdateUserProfileResultTypeDef:
         """
         Updates a user's profile in AWS CodeStar.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Client.update_user_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/client/#update_user_profile)
         """
```

### Comparing `types-aiobotocore-codestar-2.9.0/types_aiobotocore_codestar/client.pyi` & `types-aiobotocore-codestar-2.9.1/types_aiobotocore_codestar/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     async def associate_team_member(
         self,
         *,
         projectId: str,
         userArn: str,
         projectRole: str,
         clientRequestToken: str = ...,
-        remoteAccessAllowed: bool = ...
+        remoteAccessAllowed: bool = ...,
     ) -> AssociateTeamMemberResultTypeDef:
         """
         Adds an IAM user to the team for an AWS CodeStar project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Client.associate_team_member)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/client/#associate_team_member)
         """
@@ -131,15 +131,15 @@
         *,
         name: str,
         id: str,
         description: str = ...,
         clientRequestToken: str = ...,
         sourceCode: Sequence[CodeTypeDef] = ...,
         toolchain: ToolchainTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateProjectResultTypeDef:
         """
         Creates a project, including project resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Client.create_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/client/#create_project)
         """
@@ -292,30 +292,30 @@
 
     async def update_team_member(
         self,
         *,
         projectId: str,
         userArn: str,
         projectRole: str = ...,
-        remoteAccessAllowed: bool = ...
+        remoteAccessAllowed: bool = ...,
     ) -> UpdateTeamMemberResultTypeDef:
         """
         Updates a team member's attributes in an AWS CodeStar project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Client.update_team_member)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/client/#update_team_member)
         """
 
     async def update_user_profile(
         self,
         *,
         userArn: str,
         displayName: str = ...,
         emailAddress: str = ...,
-        sshPublicKey: str = ...
+        sshPublicKey: str = ...,
     ) -> UpdateUserProfileResultTypeDef:
         """
         Updates a user's profile in AWS CodeStar.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Client.update_user_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/client/#update_user_profile)
         """
```

### Comparing `types-aiobotocore-codestar-2.9.0/types_aiobotocore_codestar/literals.py` & `types-aiobotocore-codestar-2.9.1/types_aiobotocore_codestar/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,28 +15,26 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ListProjectsPaginatorName",
     "ListResourcesPaginatorName",
     "ListTeamMembersPaginatorName",
     "ListUserProfilesPaginatorName",
     "CodeStarServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ListProjectsPaginatorName = Literal["list_projects"]
 ListResourcesPaginatorName = Literal["list_resources"]
 ListTeamMembersPaginatorName = Literal["list_team_members"]
 ListUserProfilesPaginatorName = Literal["list_user_profiles"]
 CodeStarServiceName = Literal["codestar"]
 ServiceName = Literal[
     "accessanalyzer",
```

### Comparing `types-aiobotocore-codestar-2.9.0/types_aiobotocore_codestar/literals.pyi` & `types-aiobotocore-codestar-2.9.1/types_aiobotocore_codestar/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-2.9.0/types_aiobotocore_codestar/paginator.py` & `types-aiobotocore-codestar-2.9.1/types_aiobotocore_codestar/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 __all__ = (
     "ListProjectsPaginator",
     "ListResourcesPaginator",
     "ListTeamMembersPaginator",
     "ListUserProfilesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
```

### Comparing `types-aiobotocore-codestar-2.9.0/types_aiobotocore_codestar/paginator.pyi` & `types-aiobotocore-codestar-2.9.1/types_aiobotocore_codestar/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-2.9.0/types_aiobotocore_codestar/type_defs.py` & `types-aiobotocore-codestar-2.9.1/types_aiobotocore_codestar/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AssociateTeamMemberRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CodeCommitCodeDestinationTypeDef",
     "GitHubCodeDestinationTypeDef",
     "S3LocationTypeDef",
     "CreateUserProfileRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-codestar-2.9.0/types_aiobotocore_codestar/type_defs.pyi` & `types-aiobotocore-codestar-2.9.1/types_aiobotocore_codestar/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-2.9.0/types_aiobotocore_codestar.egg-info/PKG-INFO` & `types-aiobotocore-codestar-2.9.1/types_aiobotocore_codestar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codestar
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CodeStar 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CodeStar 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/
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
 
 <a id="types-aiobotocore-codestar"></a>
 
 # types-aiobotocore-codestar
 
 [![PyPI - types-aiobotocore-codestar](https://img.shields.io/pypi/v/types-aiobotocore-codestar.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codestar)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codestar.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codestar)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codestar)](https://pepy.tech/project/types-aiobotocore-codestar)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeStar 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar)
+[aiobotocore.CodeStar 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar)
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
 [types-aiobotocore-codestar docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-codestar-2.9.0/types_aiobotocore_codestar.egg-info/SOURCES.txt` & `types-aiobotocore-codestar-2.9.1/types_aiobotocore_codestar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

