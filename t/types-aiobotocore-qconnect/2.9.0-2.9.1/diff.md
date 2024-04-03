# Comparing `tmp/types-aiobotocore-qconnect-2.9.0.tar.gz` & `tmp/types-aiobotocore-qconnect-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-qconnect-2.9.0.tar", last modified: Wed Dec 13 20:00:12 2023, max compression
+gzip compressed data, was "types-aiobotocore-qconnect-2.9.1.tar", last modified: Thu Jan 18 01:21:32 2024, max compression
```

## Comparing `types-aiobotocore-qconnect-2.9.0.tar` & `types-aiobotocore-qconnect-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:12.749292 types-aiobotocore-qconnect-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:52:04.000000 types-aiobotocore-qconnect-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14362 2023-12-13 20:00:12.749292 types-aiobotocore-qconnect-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12795 2023-12-13 19:52:04.000000 types-aiobotocore-qconnect-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:12.749292 types-aiobotocore-qconnect-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2023-12-13 19:52:04.000000 types-aiobotocore-qconnect-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:12.749292 types-aiobotocore-qconnect-2.9.0/types_aiobotocore_qconnect/
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2023-12-13 19:52:04.000000 types-aiobotocore-qconnect-2.9.0/types_aiobotocore_qconnect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2531 2023-12-13 19:52:04.000000 types-aiobotocore-qconnect-2.9.0/types_aiobotocore_qconnect/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      936 2023-12-13 19:52:04.000000 types-aiobotocore-qconnect-2.9.0/types_aiobotocore_qconnect/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35959 2023-12-13 19:52:04.000000 types-aiobotocore-qconnect-2.9.0/types_aiobotocore_qconnect/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    35955 2023-12-13 19:52:04.000000 types-aiobotocore-qconnect-2.9.0/types_aiobotocore_qconnect/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12380 2023-12-13 19:52:05.000000 types-aiobotocore-qconnect-2.9.0/types_aiobotocore_qconnect/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    12378 2023-12-13 19:52:05.000000 types-aiobotocore-qconnect-2.9.0/types_aiobotocore_qconnect/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12603 2023-12-13 19:52:04.000000 types-aiobotocore-qconnect-2.9.0/types_aiobotocore_qconnect/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12591 2023-12-13 19:52:04.000000 types-aiobotocore-qconnect-2.9.0/types_aiobotocore_qconnect/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:52:04.000000 types-aiobotocore-qconnect-2.9.0/types_aiobotocore_qconnect/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    48885 2023-12-13 19:52:07.000000 types-aiobotocore-qconnect-2.9.0/types_aiobotocore_qconnect/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    48884 2023-12-13 19:52:07.000000 types-aiobotocore-qconnect-2.9.0/types_aiobotocore_qconnect/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:52:04.000000 types-aiobotocore-qconnect-2.9.0/types_aiobotocore_qconnect/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:12.749292 types-aiobotocore-qconnect-2.9.0/types_aiobotocore_qconnect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14362 2023-12-13 20:00:12.000000 types-aiobotocore-qconnect-2.9.0/types_aiobotocore_qconnect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      832 2023-12-13 20:00:12.000000 types-aiobotocore-qconnect-2.9.0/types_aiobotocore_qconnect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:12.000000 types-aiobotocore-qconnect-2.9.0/types_aiobotocore_qconnect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:12.000000 types-aiobotocore-qconnect-2.9.0/types_aiobotocore_qconnect.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:12.000000 types-aiobotocore-qconnect-2.9.0/types_aiobotocore_qconnect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-13 20:00:12.000000 types-aiobotocore-qconnect-2.9.0/types_aiobotocore_qconnect.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:32.773105 types-aiobotocore-qconnect-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:13:42.000000 types-aiobotocore-qconnect-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14382 2024-01-18 01:21:32.773105 types-aiobotocore-qconnect-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12795 2024-01-18 01:13:42.000000 types-aiobotocore-qconnect-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:32.773105 types-aiobotocore-qconnect-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-01-18 01:13:42.000000 types-aiobotocore-qconnect-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:32.773105 types-aiobotocore-qconnect-2.9.1/types_aiobotocore_qconnect/
+-rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-01-18 01:13:42.000000 types-aiobotocore-qconnect-2.9.1/types_aiobotocore_qconnect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-01-18 01:13:42.000000 types-aiobotocore-qconnect-2.9.1/types_aiobotocore_qconnect/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-01-18 01:13:42.000000 types-aiobotocore-qconnect-2.9.1/types_aiobotocore_qconnect/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35972 2024-01-18 01:13:42.000000 types-aiobotocore-qconnect-2.9.1/types_aiobotocore_qconnect/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35969 2024-01-18 01:13:42.000000 types-aiobotocore-qconnect-2.9.1/types_aiobotocore_qconnect/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12378 2024-01-18 01:13:42.000000 types-aiobotocore-qconnect-2.9.1/types_aiobotocore_qconnect/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12378 2024-01-18 01:13:42.000000 types-aiobotocore-qconnect-2.9.1/types_aiobotocore_qconnect/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12606 2024-01-18 01:13:42.000000 types-aiobotocore-qconnect-2.9.1/types_aiobotocore_qconnect/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12595 2024-01-18 01:13:42.000000 types-aiobotocore-qconnect-2.9.1/types_aiobotocore_qconnect/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:13:42.000000 types-aiobotocore-qconnect-2.9.1/types_aiobotocore_qconnect/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    48884 2024-01-18 01:13:43.000000 types-aiobotocore-qconnect-2.9.1/types_aiobotocore_qconnect/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48884 2024-01-18 01:13:43.000000 types-aiobotocore-qconnect-2.9.1/types_aiobotocore_qconnect/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:13:42.000000 types-aiobotocore-qconnect-2.9.1/types_aiobotocore_qconnect/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:32.773105 types-aiobotocore-qconnect-2.9.1/types_aiobotocore_qconnect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14382 2024-01-18 01:21:32.000000 types-aiobotocore-qconnect-2.9.1/types_aiobotocore_qconnect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-01-18 01:21:32.000000 types-aiobotocore-qconnect-2.9.1/types_aiobotocore_qconnect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:32.000000 types-aiobotocore-qconnect-2.9.1/types_aiobotocore_qconnect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:32.000000 types-aiobotocore-qconnect-2.9.1/types_aiobotocore_qconnect.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:32.000000 types-aiobotocore-qconnect-2.9.1/types_aiobotocore_qconnect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-18 01:21:32.000000 types-aiobotocore-qconnect-2.9.1/types_aiobotocore_qconnect.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-qconnect-2.9.0/LICENSE` & `types-aiobotocore-qconnect-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-qconnect-2.9.0/PKG-INFO` & `types-aiobotocore-qconnect-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-qconnect
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.QConnect 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.QConnect 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qconnect/
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
 
 <a id="types-aiobotocore-qconnect"></a>
 
 # types-aiobotocore-qconnect
 
 [![PyPI - types-aiobotocore-qconnect](https://img.shields.io/pypi/v/types-aiobotocore-qconnect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-qconnect)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-qconnect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-qconnect)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qconnect/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-qconnect)](https://pepy.tech/project/types-aiobotocore-qconnect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.QConnect 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect)
+[aiobotocore.QConnect 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect)
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
 [types-aiobotocore-qconnect docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qconnect/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-qconnect-2.9.0/README.md` & `types-aiobotocore-qconnect-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-qconnect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-qconnect)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qconnect/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-qconnect)](https://pepy.tech/project/types-aiobotocore-qconnect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.QConnect 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect)
+[aiobotocore.QConnect 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect)
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
 [types-aiobotocore-qconnect docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qconnect/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-qconnect-2.9.0/setup.py` & `types-aiobotocore-qconnect-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-qconnect",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_qconnect"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.QConnect 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.QConnect 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore qconnect type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_qconnect": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qconnect/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-qconnect-2.9.0/types_aiobotocore_qconnect/__init__.py` & `types-aiobotocore-qconnect-2.9.1/types_aiobotocore_qconnect/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,14 @@
     SearchContentPaginator,
     SearchQuickResponsesPaginator,
     SearchSessionsPaginator,
 )
 
 Client = QConnectClient
 
-
 __all__ = (
     "Client",
     "ListAssistantAssociationsPaginator",
     "ListAssistantsPaginator",
     "ListContentsPaginator",
     "ListImportJobsPaginator",
     "ListKnowledgeBasesPaginator",
```

### Comparing `types-aiobotocore-qconnect-2.9.0/types_aiobotocore_qconnect/__init__.pyi` & `types-aiobotocore-qconnect-2.9.1/types_aiobotocore_qconnect/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-qconnect-2.9.0/types_aiobotocore_qconnect/__main__.py` & `types-aiobotocore-qconnect-2.9.1/types_aiobotocore_qconnect/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.QConnect 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.QConnect 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qconnect//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect\nOther"
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

### Comparing `types-aiobotocore-qconnect-2.9.0/types_aiobotocore_qconnect/client.py` & `types-aiobotocore-qconnect-2.9.1/types_aiobotocore_qconnect/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("QConnectClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -147,15 +146,15 @@
         self,
         *,
         name: str,
         type: Literal["AGENT"],
         clientToken: str = ...,
         description: str = ...,
         serverSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateAssistantResponseTypeDef:
         """
         Creates an Amazon Q in Connect assistant.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Client.create_assistant)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qconnect/client/#create_assistant)
         """
@@ -163,15 +162,15 @@
     async def create_assistant_association(
         self,
         *,
         assistantId: str,
         association: AssistantAssociationInputDataTypeDef,
         associationType: Literal["KNOWLEDGE_BASE"],
         clientToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateAssistantAssociationResponseTypeDef:
         """
         Creates an association between an Amazon Q in Connect assistant and another
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Client.create_assistant_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qconnect/client/#create_assistant_association)
@@ -183,15 +182,15 @@
         knowledgeBaseId: str,
         name: str,
         uploadId: str,
         clientToken: str = ...,
         metadata: Mapping[str, str] = ...,
         overrideLinkOutUri: str = ...,
         tags: Mapping[str, str] = ...,
-        title: str = ...
+        title: str = ...,
     ) -> CreateContentResponseTypeDef:
         """
         Creates Amazon Q content.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Client.create_content)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qconnect/client/#create_content)
         """
@@ -202,15 +201,15 @@
         knowledgeBaseType: KnowledgeBaseTypeType,
         name: str,
         clientToken: str = ...,
         description: str = ...,
         renderingConfiguration: RenderingConfigurationTypeDef = ...,
         serverSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef = ...,
         sourceConfiguration: SourceConfigurationTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateKnowledgeBaseResponseTypeDef:
         """
         Creates a knowledge base.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Client.create_knowledge_base)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qconnect/client/#create_knowledge_base)
         """
@@ -225,15 +224,15 @@
         clientToken: str = ...,
         contentType: str = ...,
         description: str = ...,
         groupingConfiguration: GroupingConfigurationTypeDef = ...,
         isActive: bool = ...,
         language: str = ...,
         shortcutKey: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateQuickResponseResponseTypeDef:
         """
         Creates an Amazon Q quick response.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Client.create_quick_response)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qconnect/client/#create_quick_response)
         """
@@ -241,15 +240,15 @@
     async def create_session(
         self,
         *,
         assistantId: str,
         name: str,
         clientToken: str = ...,
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateSessionResponseTypeDef:
         """
         Creates a session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Client.create_session)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qconnect/client/#create_session)
         """
@@ -488,15 +487,15 @@
 
     async def put_feedback(
         self,
         *,
         assistantId: str,
         contentFeedback: ContentFeedbackDataTypeDef,
         targetId: str,
-        targetType: TargetTypeType
+        targetType: TargetTypeType,
     ) -> PutFeedbackResponseTypeDef:
         """
         Provides feedback against the specified assistant for the specified target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Client.put_feedback)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qconnect/client/#put_feedback)
         """
@@ -505,15 +504,15 @@
         self,
         *,
         assistantId: str,
         queryText: str,
         maxResults: int = ...,
         nextToken: str = ...,
         queryCondition: Sequence[QueryConditionTypeDef] = ...,
-        sessionId: str = ...
+        sessionId: str = ...,
     ) -> QueryAssistantResponseTypeDef:
         """
         Performs a manual search against the specified assistant.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Client.query_assistant)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qconnect/client/#query_assistant)
         """
@@ -528,15 +527,15 @@
 
     async def search_content(
         self,
         *,
         knowledgeBaseId: str,
         searchExpression: SearchExpressionTypeDef,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> SearchContentResponseTypeDef:
         """
         Searches for content in a specified knowledge base.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Client.search_content)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qconnect/client/#search_content)
         """
@@ -544,30 +543,30 @@
     async def search_quick_responses(
         self,
         *,
         knowledgeBaseId: str,
         searchExpression: QuickResponseSearchExpressionTypeDef,
         attributes: Mapping[str, str] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> SearchQuickResponsesResponseTypeDef:
         """
         Searches existing Amazon Q quick responses in an Amazon Q knowledge base.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Client.search_quick_responses)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qconnect/client/#search_quick_responses)
         """
 
     async def search_sessions(
         self,
         *,
         assistantId: str,
         searchExpression: SearchExpressionTypeDef,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> SearchSessionsResponseTypeDef:
         """
         Searches for sessions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Client.search_sessions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qconnect/client/#search_sessions)
         """
@@ -586,15 +585,15 @@
         self,
         *,
         importJobType: Literal["QUICK_RESPONSES"],
         knowledgeBaseId: str,
         uploadId: str,
         clientToken: str = ...,
         externalSourceConfiguration: ExternalSourceConfigurationTypeDef = ...,
-        metadata: Mapping[str, str] = ...
+        metadata: Mapping[str, str] = ...,
     ) -> StartImportJobResponseTypeDef:
         """
         Start an asynchronous job to import Amazon Q resources from an uploaded source
         file.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Client.start_import_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qconnect/client/#start_import_job)
@@ -622,15 +621,15 @@
         contentId: str,
         knowledgeBaseId: str,
         metadata: Mapping[str, str] = ...,
         overrideLinkOutUri: str = ...,
         removeOverrideLinkOutUri: bool = ...,
         revisionId: str = ...,
         title: str = ...,
-        uploadId: str = ...
+        uploadId: str = ...,
     ) -> UpdateContentResponseTypeDef:
         """
         Updates information about the content.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Client.update_content)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qconnect/client/#update_content)
         """
@@ -657,15 +656,15 @@
         groupingConfiguration: GroupingConfigurationTypeDef = ...,
         isActive: bool = ...,
         language: str = ...,
         name: str = ...,
         removeDescription: bool = ...,
         removeGroupingConfiguration: bool = ...,
         removeShortcutKey: bool = ...,
-        shortcutKey: str = ...
+        shortcutKey: str = ...,
     ) -> UpdateQuickResponseResponseTypeDef:
         """
         Updates an existing Amazon Q quick response.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Client.update_quick_response)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qconnect/client/#update_quick_response)
         """
```

### Comparing `types-aiobotocore-qconnect-2.9.0/types_aiobotocore_qconnect/client.pyi` & `types-aiobotocore-qconnect-2.9.1/types_aiobotocore_qconnect/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,15 @@
         self,
         *,
         name: str,
         type: Literal["AGENT"],
         clientToken: str = ...,
         description: str = ...,
         serverSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateAssistantResponseTypeDef:
         """
         Creates an Amazon Q in Connect assistant.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Client.create_assistant)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qconnect/client/#create_assistant)
         """
@@ -159,15 +159,15 @@
     async def create_assistant_association(
         self,
         *,
         assistantId: str,
         association: AssistantAssociationInputDataTypeDef,
         associationType: Literal["KNOWLEDGE_BASE"],
         clientToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateAssistantAssociationResponseTypeDef:
         """
         Creates an association between an Amazon Q in Connect assistant and another
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Client.create_assistant_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qconnect/client/#create_assistant_association)
@@ -179,15 +179,15 @@
         knowledgeBaseId: str,
         name: str,
         uploadId: str,
         clientToken: str = ...,
         metadata: Mapping[str, str] = ...,
         overrideLinkOutUri: str = ...,
         tags: Mapping[str, str] = ...,
-        title: str = ...
+        title: str = ...,
     ) -> CreateContentResponseTypeDef:
         """
         Creates Amazon Q content.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Client.create_content)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qconnect/client/#create_content)
         """
@@ -198,15 +198,15 @@
         knowledgeBaseType: KnowledgeBaseTypeType,
         name: str,
         clientToken: str = ...,
         description: str = ...,
         renderingConfiguration: RenderingConfigurationTypeDef = ...,
         serverSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef = ...,
         sourceConfiguration: SourceConfigurationTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateKnowledgeBaseResponseTypeDef:
         """
         Creates a knowledge base.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Client.create_knowledge_base)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qconnect/client/#create_knowledge_base)
         """
@@ -221,15 +221,15 @@
         clientToken: str = ...,
         contentType: str = ...,
         description: str = ...,
         groupingConfiguration: GroupingConfigurationTypeDef = ...,
         isActive: bool = ...,
         language: str = ...,
         shortcutKey: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateQuickResponseResponseTypeDef:
         """
         Creates an Amazon Q quick response.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Client.create_quick_response)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qconnect/client/#create_quick_response)
         """
@@ -237,15 +237,15 @@
     async def create_session(
         self,
         *,
         assistantId: str,
         name: str,
         clientToken: str = ...,
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateSessionResponseTypeDef:
         """
         Creates a session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Client.create_session)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qconnect/client/#create_session)
         """
@@ -484,15 +484,15 @@
 
     async def put_feedback(
         self,
         *,
         assistantId: str,
         contentFeedback: ContentFeedbackDataTypeDef,
         targetId: str,
-        targetType: TargetTypeType
+        targetType: TargetTypeType,
     ) -> PutFeedbackResponseTypeDef:
         """
         Provides feedback against the specified assistant for the specified target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Client.put_feedback)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qconnect/client/#put_feedback)
         """
@@ -501,15 +501,15 @@
         self,
         *,
         assistantId: str,
         queryText: str,
         maxResults: int = ...,
         nextToken: str = ...,
         queryCondition: Sequence[QueryConditionTypeDef] = ...,
-        sessionId: str = ...
+        sessionId: str = ...,
     ) -> QueryAssistantResponseTypeDef:
         """
         Performs a manual search against the specified assistant.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Client.query_assistant)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qconnect/client/#query_assistant)
         """
@@ -524,15 +524,15 @@
 
     async def search_content(
         self,
         *,
         knowledgeBaseId: str,
         searchExpression: SearchExpressionTypeDef,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> SearchContentResponseTypeDef:
         """
         Searches for content in a specified knowledge base.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Client.search_content)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qconnect/client/#search_content)
         """
@@ -540,30 +540,30 @@
     async def search_quick_responses(
         self,
         *,
         knowledgeBaseId: str,
         searchExpression: QuickResponseSearchExpressionTypeDef,
         attributes: Mapping[str, str] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> SearchQuickResponsesResponseTypeDef:
         """
         Searches existing Amazon Q quick responses in an Amazon Q knowledge base.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Client.search_quick_responses)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qconnect/client/#search_quick_responses)
         """
 
     async def search_sessions(
         self,
         *,
         assistantId: str,
         searchExpression: SearchExpressionTypeDef,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> SearchSessionsResponseTypeDef:
         """
         Searches for sessions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Client.search_sessions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qconnect/client/#search_sessions)
         """
@@ -582,15 +582,15 @@
         self,
         *,
         importJobType: Literal["QUICK_RESPONSES"],
         knowledgeBaseId: str,
         uploadId: str,
         clientToken: str = ...,
         externalSourceConfiguration: ExternalSourceConfigurationTypeDef = ...,
-        metadata: Mapping[str, str] = ...
+        metadata: Mapping[str, str] = ...,
     ) -> StartImportJobResponseTypeDef:
         """
         Start an asynchronous job to import Amazon Q resources from an uploaded source
         file.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Client.start_import_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qconnect/client/#start_import_job)
@@ -618,15 +618,15 @@
         contentId: str,
         knowledgeBaseId: str,
         metadata: Mapping[str, str] = ...,
         overrideLinkOutUri: str = ...,
         removeOverrideLinkOutUri: bool = ...,
         revisionId: str = ...,
         title: str = ...,
-        uploadId: str = ...
+        uploadId: str = ...,
     ) -> UpdateContentResponseTypeDef:
         """
         Updates information about the content.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Client.update_content)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qconnect/client/#update_content)
         """
@@ -653,15 +653,15 @@
         groupingConfiguration: GroupingConfigurationTypeDef = ...,
         isActive: bool = ...,
         language: str = ...,
         name: str = ...,
         removeDescription: bool = ...,
         removeGroupingConfiguration: bool = ...,
         removeShortcutKey: bool = ...,
-        shortcutKey: str = ...
+        shortcutKey: str = ...,
     ) -> UpdateQuickResponseResponseTypeDef:
         """
         Updates an existing Amazon Q quick response.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Client.update_quick_response)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qconnect/client/#update_quick_response)
         """
```

### Comparing `types-aiobotocore-qconnect-2.9.0/types_aiobotocore_qconnect/literals.py` & `types-aiobotocore-qconnect-2.9.1/types_aiobotocore_qconnect/literals.py`

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
     "AssistantCapabilityTypeType",
     "AssistantStatusType",
     "AssistantTypeType",
     "AssociationTypeType",
     "ContentStatusType",
     "ExternalSourceType",
@@ -61,15 +60,14 @@
     "QConnectServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AssistantCapabilityTypeType = Literal["V1", "V2"]
 AssistantStatusType = Literal[
     "ACTIVE",
     "CREATE_FAILED",
     "CREATE_IN_PROGRESS",
     "DELETED",
     "DELETE_FAILED",
```

### Comparing `types-aiobotocore-qconnect-2.9.0/types_aiobotocore_qconnect/literals.pyi` & `types-aiobotocore-qconnect-2.9.1/types_aiobotocore_qconnect/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-qconnect-2.9.0/types_aiobotocore_qconnect/paginator.py` & `types-aiobotocore-qconnect-2.9.1/types_aiobotocore_qconnect/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,14 @@
     "ListQuickResponsesPaginator",
     "QueryAssistantPaginator",
     "SearchContentPaginator",
     "SearchQuickResponsesPaginator",
     "SearchSessionsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -184,15 +183,15 @@
     def paginate(
         self,
         *,
         assistantId: str,
         queryText: str,
         queryCondition: Sequence[QueryConditionTypeDef] = ...,
         sessionId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[QueryAssistantResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Paginator.QueryAssistant.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qconnect/paginators/#queryassistantpaginator)
         """
 
 
@@ -203,15 +202,15 @@
     """
 
     def paginate(
         self,
         *,
         knowledgeBaseId: str,
         searchExpression: SearchExpressionTypeDef,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchContentResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Paginator.SearchContent.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qconnect/paginators/#searchcontentpaginator)
         """
 
 
@@ -223,15 +222,15 @@
 
     def paginate(
         self,
         *,
         knowledgeBaseId: str,
         searchExpression: QuickResponseSearchExpressionTypeDef,
         attributes: Mapping[str, str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchQuickResponsesResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Paginator.SearchQuickResponses.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qconnect/paginators/#searchquickresponsespaginator)
         """
 
 
@@ -242,13 +241,13 @@
     """
 
     def paginate(
         self,
         *,
         assistantId: str,
         searchExpression: SearchExpressionTypeDef,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchSessionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Paginator.SearchSessions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qconnect/paginators/#searchsessionspaginator)
         """
```

### Comparing `types-aiobotocore-qconnect-2.9.0/types_aiobotocore_qconnect/paginator.pyi` & `types-aiobotocore-qconnect-2.9.1/types_aiobotocore_qconnect/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,15 @@
     def paginate(
         self,
         *,
         assistantId: str,
         queryText: str,
         queryCondition: Sequence[QueryConditionTypeDef] = ...,
         sessionId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[QueryAssistantResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Paginator.QueryAssistant.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qconnect/paginators/#queryassistantpaginator)
         """
 
 class SearchContentPaginator(AioPaginator):
@@ -193,15 +193,15 @@
     """
 
     def paginate(
         self,
         *,
         knowledgeBaseId: str,
         searchExpression: SearchExpressionTypeDef,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchContentResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Paginator.SearchContent.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qconnect/paginators/#searchcontentpaginator)
         """
 
 class SearchQuickResponsesPaginator(AioPaginator):
@@ -212,15 +212,15 @@
 
     def paginate(
         self,
         *,
         knowledgeBaseId: str,
         searchExpression: QuickResponseSearchExpressionTypeDef,
         attributes: Mapping[str, str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchQuickResponsesResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Paginator.SearchQuickResponses.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qconnect/paginators/#searchquickresponsespaginator)
         """
 
 class SearchSessionsPaginator(AioPaginator):
@@ -230,13 +230,13 @@
     """
 
     def paginate(
         self,
         *,
         assistantId: str,
         searchExpression: SearchExpressionTypeDef,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchSessionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Paginator.SearchSessions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qconnect/paginators/#searchsessionspaginator)
         """
```

### Comparing `types-aiobotocore-qconnect-2.9.0/types_aiobotocore_qconnect/type_defs.py` & `types-aiobotocore-qconnect-2.9.1/types_aiobotocore_qconnect/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AppIntegrationsConfigurationPaginatorTypeDef",
     "AppIntegrationsConfigurationTypeDef",
     "AssistantAssociationInputDataTypeDef",
     "KnowledgeBaseAssociationDataTypeDef",
     "AssistantCapabilityConfigurationTypeDef",
     "AssistantIntegrationConfigurationTypeDef",
```

### Comparing `types-aiobotocore-qconnect-2.9.0/types_aiobotocore_qconnect/type_defs.pyi` & `types-aiobotocore-qconnect-2.9.1/types_aiobotocore_qconnect/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-qconnect-2.9.0/types_aiobotocore_qconnect.egg-info/PKG-INFO` & `types-aiobotocore-qconnect-2.9.1/types_aiobotocore_qconnect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-qconnect
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.QConnect 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.QConnect 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qconnect/
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
 
 <a id="types-aiobotocore-qconnect"></a>
 
 # types-aiobotocore-qconnect
 
 [![PyPI - types-aiobotocore-qconnect](https://img.shields.io/pypi/v/types-aiobotocore-qconnect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-qconnect)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-qconnect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-qconnect)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qconnect/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-qconnect)](https://pepy.tech/project/types-aiobotocore-qconnect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.QConnect 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect)
+[aiobotocore.QConnect 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect)
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
 [types-aiobotocore-qconnect docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qconnect/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-qconnect-2.9.0/types_aiobotocore_qconnect.egg-info/SOURCES.txt` & `types-aiobotocore-qconnect-2.9.1/types_aiobotocore_qconnect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

