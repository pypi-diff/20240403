# Comparing `tmp/types-aiobotocore-codestar-connections-2.9.0.tar.gz` & `tmp/types-aiobotocore-codestar-connections-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-codestar-connections-2.9.0.tar", last modified: Wed Dec 13 19:58:55 2023, max compression
+gzip compressed data, was "types-aiobotocore-codestar-connections-2.9.1.tar", last modified: Thu Jan 18 01:20:22 2024, max compression
```

## Comparing `types-aiobotocore-codestar-connections-2.9.0.tar` & `types-aiobotocore-codestar-connections-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:55.953921 types-aiobotocore-codestar-connections-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:43:00.000000 types-aiobotocore-codestar-connections-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12899 2023-12-13 19:58:55.953921 types-aiobotocore-codestar-connections-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11285 2023-12-13 19:43:00.000000 types-aiobotocore-codestar-connections-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:55.953921 types-aiobotocore-codestar-connections-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2023-12-13 19:43:00.000000 types-aiobotocore-codestar-connections-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:55.953921 types-aiobotocore-codestar-connections-2.9.0/types_aiobotocore_codestar_connections/
--rw-r--r--   0 runner    (1001) docker     (127)      542 2023-12-13 19:43:00.000000 types-aiobotocore-codestar-connections-2.9.0/types_aiobotocore_codestar_connections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2023-12-13 19:43:00.000000 types-aiobotocore-codestar-connections-2.9.0/types_aiobotocore_codestar_connections/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      982 2023-12-13 19:43:00.000000 types-aiobotocore-codestar-connections-2.9.0/types_aiobotocore_codestar_connections/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23103 2023-12-13 19:43:01.000000 types-aiobotocore-codestar-connections-2.9.0/types_aiobotocore_codestar_connections/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    23099 2023-12-13 19:43:00.000000 types-aiobotocore-codestar-connections-2.9.0/types_aiobotocore_codestar_connections/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9189 2023-12-13 19:43:01.000000 types-aiobotocore-codestar-connections-2.9.0/types_aiobotocore_codestar_connections/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9187 2023-12-13 19:43:01.000000 types-aiobotocore-codestar-connections-2.9.0/types_aiobotocore_codestar_connections/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:43:00.000000 types-aiobotocore-codestar-connections-2.9.0/types_aiobotocore_codestar_connections/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    17686 2023-12-13 19:43:01.000000 types-aiobotocore-codestar-connections-2.9.0/types_aiobotocore_codestar_connections/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    17685 2023-12-13 19:43:01.000000 types-aiobotocore-codestar-connections-2.9.0/types_aiobotocore_codestar_connections/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:43:00.000000 types-aiobotocore-codestar-connections-2.9.0/types_aiobotocore_codestar_connections/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:55.953921 types-aiobotocore-codestar-connections-2.9.0/types_aiobotocore_codestar_connections.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12899 2023-12-13 19:58:55.000000 types-aiobotocore-codestar-connections-2.9.0/types_aiobotocore_codestar_connections.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      955 2023-12-13 19:58:55.000000 types-aiobotocore-codestar-connections-2.9.0/types_aiobotocore_codestar_connections.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:55.000000 types-aiobotocore-codestar-connections-2.9.0/types_aiobotocore_codestar_connections.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:55.000000 types-aiobotocore-codestar-connections-2.9.0/types_aiobotocore_codestar_connections.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:55.000000 types-aiobotocore-codestar-connections-2.9.0/types_aiobotocore_codestar_connections.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-12-13 19:58:55.000000 types-aiobotocore-codestar-connections-2.9.0/types_aiobotocore_codestar_connections.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:22.181434 types-aiobotocore-codestar-connections-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:04:56.000000 types-aiobotocore-codestar-connections-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12919 2024-01-18 01:20:22.181434 types-aiobotocore-codestar-connections-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11285 2024-01-18 01:04:56.000000 types-aiobotocore-codestar-connections-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:22.181434 types-aiobotocore-codestar-connections-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-01-18 01:04:56.000000 types-aiobotocore-codestar-connections-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:22.181434 types-aiobotocore-codestar-connections-2.9.1/types_aiobotocore_codestar_connections/
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-01-18 01:04:56.000000 types-aiobotocore-codestar-connections-2.9.1/types_aiobotocore_codestar_connections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-01-18 01:04:56.000000 types-aiobotocore-codestar-connections-2.9.1/types_aiobotocore_codestar_connections/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-01-18 01:04:56.000000 types-aiobotocore-codestar-connections-2.9.1/types_aiobotocore_codestar_connections/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23111 2024-01-18 01:04:57.000000 types-aiobotocore-codestar-connections-2.9.1/types_aiobotocore_codestar_connections/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23108 2024-01-18 01:04:56.000000 types-aiobotocore-codestar-connections-2.9.1/types_aiobotocore_codestar_connections/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9187 2024-01-18 01:04:57.000000 types-aiobotocore-codestar-connections-2.9.1/types_aiobotocore_codestar_connections/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9187 2024-01-18 01:04:57.000000 types-aiobotocore-codestar-connections-2.9.1/types_aiobotocore_codestar_connections/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:04:56.000000 types-aiobotocore-codestar-connections-2.9.1/types_aiobotocore_codestar_connections/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    17685 2024-01-18 01:04:57.000000 types-aiobotocore-codestar-connections-2.9.1/types_aiobotocore_codestar_connections/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17685 2024-01-18 01:04:57.000000 types-aiobotocore-codestar-connections-2.9.1/types_aiobotocore_codestar_connections/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:04:56.000000 types-aiobotocore-codestar-connections-2.9.1/types_aiobotocore_codestar_connections/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:22.181434 types-aiobotocore-codestar-connections-2.9.1/types_aiobotocore_codestar_connections.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12919 2024-01-18 01:20:22.000000 types-aiobotocore-codestar-connections-2.9.1/types_aiobotocore_codestar_connections.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-01-18 01:20:22.000000 types-aiobotocore-codestar-connections-2.9.1/types_aiobotocore_codestar_connections.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:22.000000 types-aiobotocore-codestar-connections-2.9.1/types_aiobotocore_codestar_connections.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:22.000000 types-aiobotocore-codestar-connections-2.9.1/types_aiobotocore_codestar_connections.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:22.000000 types-aiobotocore-codestar-connections-2.9.1/types_aiobotocore_codestar_connections.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-01-18 01:20:22.000000 types-aiobotocore-codestar-connections-2.9.1/types_aiobotocore_codestar_connections.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-codestar-connections-2.9.0/LICENSE` & `types-aiobotocore-codestar-connections-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-codestar-connections-2.9.0/PKG-INFO` & `types-aiobotocore-codestar-connections-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codestar-connections
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CodeStarconnections 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CodeStarconnections 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/
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
 
 <a id="types-aiobotocore-codestar-connections"></a>
 
 # types-aiobotocore-codestar-connections
 
 [![PyPI - types-aiobotocore-codestar-connections](https://img.shields.io/pypi/v/types-aiobotocore-codestar-connections.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codestar-connections)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codestar-connections.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codestar-connections)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codestar-connections)](https://pepy.tech/project/types-aiobotocore-codestar-connections)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeStarconnections 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections)
+[aiobotocore.CodeStarconnections 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections)
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
 [types-aiobotocore-codestar-connections docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-codestar-connections-2.9.0/README.md` & `types-aiobotocore-codestar-connections-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codestar-connections.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codestar-connections)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codestar-connections)](https://pepy.tech/project/types-aiobotocore-codestar-connections)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeStarconnections 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections)
+[aiobotocore.CodeStarconnections 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections)
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
 [types-aiobotocore-codestar-connections docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-codestar-connections-2.9.0/setup.py` & `types-aiobotocore-codestar-connections-2.9.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,50 +7,49 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-codestar-connections",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_codestar_connections"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CodeStarconnections 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.CodeStarconnections 2.9.1 service generated with"
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
     keywords=(
         "aiobotocore codestar-connections type-annotations botocore mypy typeshed autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_codestar_connections": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-codestar-connections-2.9.0/types_aiobotocore_codestar_connections/__init__.py` & `types-aiobotocore-codestar-connections-2.9.1/types_aiobotocore_codestar_connections/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,9 +18,8 @@
     ```
 """
 
 from .client import CodeStarconnectionsClient
 
 Client = CodeStarconnectionsClient
 
-
 __all__ = ("Client", "CodeStarconnectionsClient")
```

### Comparing `types-aiobotocore-codestar-connections-2.9.0/types_aiobotocore_codestar_connections/__init__.pyi` & `types-aiobotocore-codestar-connections-2.9.1/types_aiobotocore_codestar_connections/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-connections-2.9.0/types_aiobotocore_codestar_connections/__main__.py` & `types-aiobotocore-codestar-connections-2.9.1/types_aiobotocore_codestar_connections/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CodeStarconnections 2.9.0\nVersion:        "
-        " 2.9.0\nBuilder version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.CodeStarconnections 2.9.1\nVersion:        "
+        " 2.9.1\nBuilder version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections\nOther"
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

### Comparing `types-aiobotocore-codestar-connections-2.9.0/types_aiobotocore_codestar_connections/client.py` & `types-aiobotocore-codestar-connections-2.9.1/types_aiobotocore_codestar_connections/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("CodeStarconnectionsClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -120,15 +119,15 @@
 
     async def create_connection(
         self,
         *,
         ConnectionName: str,
         ProviderType: ProviderTypeType = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        HostArn: str = ...
+        HostArn: str = ...,
     ) -> CreateConnectionOutputTypeDef:
         """
         Creates a connection that can then be given to other Amazon Web Services
         services like CodePipeline so that it can access third-party code
         repositories.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.create_connection)
@@ -138,15 +137,15 @@
     async def create_host(
         self,
         *,
         Name: str,
         ProviderType: ProviderTypeType,
         ProviderEndpoint: str,
         VpcConfiguration: VpcConfigurationTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateHostOutputTypeDef:
         """
         Creates a resource that represents the infrastructure where a third-party
         provider is
         installed.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.create_host)
@@ -156,15 +155,15 @@
     async def create_repository_link(
         self,
         *,
         ConnectionArn: str,
         OwnerId: str,
         RepositoryName: str,
         EncryptionKeyArn: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateRepositoryLinkOutputTypeDef:
         """
         Creates a link to a specified external Git repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.create_repository_link)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/#create_repository_link)
         """
@@ -173,15 +172,15 @@
         self,
         *,
         Branch: str,
         ConfigFile: str,
         RepositoryLinkId: str,
         ResourceName: str,
         RoleArn: str,
-        SyncType: Literal["CFN_STACK_SYNC"]
+        SyncType: Literal["CFN_STACK_SYNC"],
     ) -> CreateSyncConfigurationOutputTypeDef:
         """
         Creates a sync configuration which allows Amazon Web Services to sync content
         from a Git repository to update a specified Amazon Web Services
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.create_sync_configuration)
@@ -309,15 +308,15 @@
 
     async def list_connections(
         self,
         *,
         ProviderTypeFilter: ProviderTypeType = ...,
         HostArnFilter: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListConnectionsOutputTypeDef:
         """
         Lists the connections associated with your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.list_connections)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/#list_connections)
         """
@@ -354,15 +353,15 @@
 
     async def list_sync_configurations(
         self,
         *,
         RepositoryLinkId: str,
         SyncType: Literal["CFN_STACK_SYNC"],
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListSyncConfigurationsOutputTypeDef:
         """
         Returns a list of sync configurations for a specified repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.list_sync_configurations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/#list_sync_configurations)
         """
@@ -392,15 +391,15 @@
         """
 
     async def update_host(
         self,
         *,
         HostArn: str,
         ProviderEndpoint: str = ...,
-        VpcConfiguration: VpcConfigurationTypeDef = ...
+        VpcConfiguration: VpcConfigurationTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates a specified host with the provided configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.update_host)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/#update_host)
         """
@@ -418,15 +417,15 @@
 
     async def update_sync_blocker(
         self,
         *,
         Id: str,
         SyncType: Literal["CFN_STACK_SYNC"],
         ResourceName: str,
-        ResolvedReason: str
+        ResolvedReason: str,
     ) -> UpdateSyncBlockerOutputTypeDef:
         """
         Allows you to update the status of a sync blocker, resolving the blocker and
         allowing syncing to
         continue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.update_sync_blocker)
@@ -437,15 +436,15 @@
         self,
         *,
         ResourceName: str,
         SyncType: Literal["CFN_STACK_SYNC"],
         Branch: str = ...,
         ConfigFile: str = ...,
         RepositoryLinkId: str = ...,
-        RoleArn: str = ...
+        RoleArn: str = ...,
     ) -> UpdateSyncConfigurationOutputTypeDef:
         """
         Updates the sync configuration for your connection and a specified external Git
         repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.update_sync_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/#update_sync_configuration)
```

### Comparing `types-aiobotocore-codestar-connections-2.9.0/types_aiobotocore_codestar_connections/client.pyi` & `types-aiobotocore-codestar-connections-2.9.1/types_aiobotocore_codestar_connections/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,15 @@
 
     async def create_connection(
         self,
         *,
         ConnectionName: str,
         ProviderType: ProviderTypeType = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        HostArn: str = ...
+        HostArn: str = ...,
     ) -> CreateConnectionOutputTypeDef:
         """
         Creates a connection that can then be given to other Amazon Web Services
         services like CodePipeline so that it can access third-party code
         repositories.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.create_connection)
@@ -134,15 +134,15 @@
     async def create_host(
         self,
         *,
         Name: str,
         ProviderType: ProviderTypeType,
         ProviderEndpoint: str,
         VpcConfiguration: VpcConfigurationTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateHostOutputTypeDef:
         """
         Creates a resource that represents the infrastructure where a third-party
         provider is
         installed.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.create_host)
@@ -152,15 +152,15 @@
     async def create_repository_link(
         self,
         *,
         ConnectionArn: str,
         OwnerId: str,
         RepositoryName: str,
         EncryptionKeyArn: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateRepositoryLinkOutputTypeDef:
         """
         Creates a link to a specified external Git repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.create_repository_link)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/#create_repository_link)
         """
@@ -169,15 +169,15 @@
         self,
         *,
         Branch: str,
         ConfigFile: str,
         RepositoryLinkId: str,
         ResourceName: str,
         RoleArn: str,
-        SyncType: Literal["CFN_STACK_SYNC"]
+        SyncType: Literal["CFN_STACK_SYNC"],
     ) -> CreateSyncConfigurationOutputTypeDef:
         """
         Creates a sync configuration which allows Amazon Web Services to sync content
         from a Git repository to update a specified Amazon Web Services
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.create_sync_configuration)
@@ -305,15 +305,15 @@
 
     async def list_connections(
         self,
         *,
         ProviderTypeFilter: ProviderTypeType = ...,
         HostArnFilter: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListConnectionsOutputTypeDef:
         """
         Lists the connections associated with your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.list_connections)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/#list_connections)
         """
@@ -350,15 +350,15 @@
 
     async def list_sync_configurations(
         self,
         *,
         RepositoryLinkId: str,
         SyncType: Literal["CFN_STACK_SYNC"],
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListSyncConfigurationsOutputTypeDef:
         """
         Returns a list of sync configurations for a specified repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.list_sync_configurations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/#list_sync_configurations)
         """
@@ -388,15 +388,15 @@
         """
 
     async def update_host(
         self,
         *,
         HostArn: str,
         ProviderEndpoint: str = ...,
-        VpcConfiguration: VpcConfigurationTypeDef = ...
+        VpcConfiguration: VpcConfigurationTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates a specified host with the provided configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.update_host)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/#update_host)
         """
@@ -414,15 +414,15 @@
 
     async def update_sync_blocker(
         self,
         *,
         Id: str,
         SyncType: Literal["CFN_STACK_SYNC"],
         ResourceName: str,
-        ResolvedReason: str
+        ResolvedReason: str,
     ) -> UpdateSyncBlockerOutputTypeDef:
         """
         Allows you to update the status of a sync blocker, resolving the blocker and
         allowing syncing to
         continue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.update_sync_blocker)
@@ -433,15 +433,15 @@
         self,
         *,
         ResourceName: str,
         SyncType: Literal["CFN_STACK_SYNC"],
         Branch: str = ...,
         ConfigFile: str = ...,
         RepositoryLinkId: str = ...,
-        RoleArn: str = ...
+        RoleArn: str = ...,
     ) -> UpdateSyncConfigurationOutputTypeDef:
         """
         Updates the sync configuration for your connection and a specified external Git
         repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.update_sync_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/#update_sync_configuration)
```

### Comparing `types-aiobotocore-codestar-connections-2.9.0/types_aiobotocore_codestar_connections/literals.py` & `types-aiobotocore-codestar-connections-2.9.1/types_aiobotocore_codestar_connections/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,30 +15,28 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "BlockerStatusType",
     "BlockerTypeType",
     "ConnectionStatusType",
     "ProviderTypeType",
     "RepositorySyncStatusType",
     "ResourceSyncStatusType",
     "SyncConfigurationTypeType",
     "CodeStarconnectionsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 BlockerStatusType = Literal["ACTIVE", "RESOLVED"]
 BlockerTypeType = Literal["AUTOMATED"]
 ConnectionStatusType = Literal["AVAILABLE", "ERROR", "PENDING"]
 ProviderTypeType = Literal["Bitbucket", "GitHub", "GitHubEnterpriseServer", "GitLab"]
 RepositorySyncStatusType = Literal["FAILED", "INITIATED", "IN_PROGRESS", "QUEUED", "SUCCEEDED"]
 ResourceSyncStatusType = Literal["FAILED", "INITIATED", "IN_PROGRESS", "SUCCEEDED"]
 SyncConfigurationTypeType = Literal["CFN_STACK_SYNC"]
```

### Comparing `types-aiobotocore-codestar-connections-2.9.0/types_aiobotocore_codestar_connections/literals.pyi` & `types-aiobotocore-codestar-connections-2.9.1/types_aiobotocore_codestar_connections/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-connections-2.9.0/types_aiobotocore_codestar_connections/type_defs.py` & `types-aiobotocore-codestar-connections-2.9.1/types_aiobotocore_codestar_connections/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ConnectionTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "VpcConfigurationTypeDef",
     "RepositoryLinkInfoTypeDef",
     "CreateSyncConfigurationInputRequestTypeDef",
```

### Comparing `types-aiobotocore-codestar-connections-2.9.0/types_aiobotocore_codestar_connections/type_defs.pyi` & `types-aiobotocore-codestar-connections-2.9.1/types_aiobotocore_codestar_connections/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-connections-2.9.0/types_aiobotocore_codestar_connections.egg-info/PKG-INFO` & `types-aiobotocore-codestar-connections-2.9.1/types_aiobotocore_codestar_connections.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codestar-connections
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CodeStarconnections 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CodeStarconnections 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/
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
 
 <a id="types-aiobotocore-codestar-connections"></a>
 
 # types-aiobotocore-codestar-connections
 
 [![PyPI - types-aiobotocore-codestar-connections](https://img.shields.io/pypi/v/types-aiobotocore-codestar-connections.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codestar-connections)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codestar-connections.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codestar-connections)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codestar-connections)](https://pepy.tech/project/types-aiobotocore-codestar-connections)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeStarconnections 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections)
+[aiobotocore.CodeStarconnections 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections)
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
 [types-aiobotocore-codestar-connections docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-codestar-connections-2.9.0/types_aiobotocore_codestar_connections.egg-info/SOURCES.txt` & `types-aiobotocore-codestar-connections-2.9.1/types_aiobotocore_codestar_connections.egg-info/SOURCES.txt`

 * *Files identical despite different names*

