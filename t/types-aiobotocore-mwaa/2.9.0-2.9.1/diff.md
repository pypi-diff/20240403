# Comparing `tmp/types-aiobotocore-mwaa-2.9.0.tar.gz` & `tmp/types-aiobotocore-mwaa-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-mwaa-2.9.0.tar", last modified: Wed Dec 13 20:00:00 2023, max compression
+gzip compressed data, was "types-aiobotocore-mwaa-2.9.1.tar", last modified: Thu Jan 18 01:21:21 2024, max compression
```

## Comparing `types-aiobotocore-mwaa-2.9.0.tar` & `types-aiobotocore-mwaa-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:00.205400 types-aiobotocore-mwaa-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:50:44.000000 types-aiobotocore-mwaa-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12819 2023-12-13 20:00:00.205400 types-aiobotocore-mwaa-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11268 2023-12-13 19:50:44.000000 types-aiobotocore-mwaa-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:00.205400 types-aiobotocore-mwaa-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2023-12-13 19:50:44.000000 types-aiobotocore-mwaa-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:00.205400 types-aiobotocore-mwaa-2.9.0/types_aiobotocore_mwaa/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2023-12-13 19:50:44.000000 types-aiobotocore-mwaa-2.9.0/types_aiobotocore_mwaa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2023-12-13 19:50:44.000000 types-aiobotocore-mwaa-2.9.0/types_aiobotocore_mwaa/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      909 2023-12-13 19:50:44.000000 types-aiobotocore-mwaa-2.9.0/types_aiobotocore_mwaa/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12396 2023-12-13 19:50:44.000000 types-aiobotocore-mwaa-2.9.0/types_aiobotocore_mwaa/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    12392 2023-12-13 19:50:44.000000 types-aiobotocore-mwaa-2.9.0/types_aiobotocore_mwaa/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9735 2023-12-13 19:50:44.000000 types-aiobotocore-mwaa-2.9.0/types_aiobotocore_mwaa/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9733 2023-12-13 19:50:44.000000 types-aiobotocore-mwaa-2.9.0/types_aiobotocore_mwaa/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2023-12-13 19:50:44.000000 types-aiobotocore-mwaa-2.9.0/types_aiobotocore_mwaa/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2023-12-13 19:50:44.000000 types-aiobotocore-mwaa-2.9.0/types_aiobotocore_mwaa/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:50:44.000000 types-aiobotocore-mwaa-2.9.0/types_aiobotocore_mwaa/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    12355 2023-12-13 19:50:44.000000 types-aiobotocore-mwaa-2.9.0/types_aiobotocore_mwaa/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12354 2023-12-13 19:50:44.000000 types-aiobotocore-mwaa-2.9.0/types_aiobotocore_mwaa/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:50:44.000000 types-aiobotocore-mwaa-2.9.0/types_aiobotocore_mwaa/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:00.205400 types-aiobotocore-mwaa-2.9.0/types_aiobotocore_mwaa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12819 2023-12-13 20:00:00.000000 types-aiobotocore-mwaa-2.9.0/types_aiobotocore_mwaa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      756 2023-12-13 20:00:00.000000 types-aiobotocore-mwaa-2.9.0/types_aiobotocore_mwaa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:00.000000 types-aiobotocore-mwaa-2.9.0/types_aiobotocore_mwaa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:00.000000 types-aiobotocore-mwaa-2.9.0/types_aiobotocore_mwaa.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:00.000000 types-aiobotocore-mwaa-2.9.0/types_aiobotocore_mwaa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-13 20:00:00.000000 types-aiobotocore-mwaa-2.9.0/types_aiobotocore_mwaa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:21.485157 types-aiobotocore-mwaa-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:12:23.000000 types-aiobotocore-mwaa-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12839 2024-01-18 01:21:21.481157 types-aiobotocore-mwaa-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11268 2024-01-18 01:12:23.000000 types-aiobotocore-mwaa-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:21.485157 types-aiobotocore-mwaa-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-01-18 01:12:23.000000 types-aiobotocore-mwaa-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:21.481157 types-aiobotocore-mwaa-2.9.1/types_aiobotocore_mwaa/
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-01-18 01:12:23.000000 types-aiobotocore-mwaa-2.9.1/types_aiobotocore_mwaa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-01-18 01:12:23.000000 types-aiobotocore-mwaa-2.9.1/types_aiobotocore_mwaa/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-01-18 01:12:23.000000 types-aiobotocore-mwaa-2.9.1/types_aiobotocore_mwaa/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12397 2024-01-18 01:12:23.000000 types-aiobotocore-mwaa-2.9.1/types_aiobotocore_mwaa/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12394 2024-01-18 01:12:23.000000 types-aiobotocore-mwaa-2.9.1/types_aiobotocore_mwaa/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9733 2024-01-18 01:12:24.000000 types-aiobotocore-mwaa-2.9.1/types_aiobotocore_mwaa/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9733 2024-01-18 01:12:24.000000 types-aiobotocore-mwaa-2.9.1/types_aiobotocore_mwaa/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-01-18 01:12:23.000000 types-aiobotocore-mwaa-2.9.1/types_aiobotocore_mwaa/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-01-18 01:12:23.000000 types-aiobotocore-mwaa-2.9.1/types_aiobotocore_mwaa/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:12:23.000000 types-aiobotocore-mwaa-2.9.1/types_aiobotocore_mwaa/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    12354 2024-01-18 01:12:24.000000 types-aiobotocore-mwaa-2.9.1/types_aiobotocore_mwaa/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12354 2024-01-18 01:12:24.000000 types-aiobotocore-mwaa-2.9.1/types_aiobotocore_mwaa/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:12:23.000000 types-aiobotocore-mwaa-2.9.1/types_aiobotocore_mwaa/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:21.481157 types-aiobotocore-mwaa-2.9.1/types_aiobotocore_mwaa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12839 2024-01-18 01:21:21.000000 types-aiobotocore-mwaa-2.9.1/types_aiobotocore_mwaa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-01-18 01:21:21.000000 types-aiobotocore-mwaa-2.9.1/types_aiobotocore_mwaa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:21.000000 types-aiobotocore-mwaa-2.9.1/types_aiobotocore_mwaa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:21.000000 types-aiobotocore-mwaa-2.9.1/types_aiobotocore_mwaa.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:21.000000 types-aiobotocore-mwaa-2.9.1/types_aiobotocore_mwaa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-01-18 01:21:21.000000 types-aiobotocore-mwaa-2.9.1/types_aiobotocore_mwaa.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-mwaa-2.9.0/LICENSE` & `types-aiobotocore-mwaa-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-mwaa-2.9.0/PKG-INFO` & `types-aiobotocore-mwaa-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mwaa
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.MWAA 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.MWAA 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mwaa/
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
 
 <a id="types-aiobotocore-mwaa"></a>
 
 # types-aiobotocore-mwaa
 
 [![PyPI - types-aiobotocore-mwaa](https://img.shields.io/pypi/v/types-aiobotocore-mwaa.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mwaa)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mwaa.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mwaa)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mwaa/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mwaa)](https://pepy.tech/project/types-aiobotocore-mwaa)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MWAA 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA)
+[aiobotocore.MWAA 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA)
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
 [types-aiobotocore-mwaa docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mwaa/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-mwaa-2.9.0/README.md` & `types-aiobotocore-mwaa-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mwaa.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mwaa)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mwaa/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mwaa)](https://pepy.tech/project/types-aiobotocore-mwaa)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MWAA 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA)
+[aiobotocore.MWAA 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA)
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
 [types-aiobotocore-mwaa docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mwaa/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-mwaa-2.9.0/setup.py` & `types-aiobotocore-mwaa-2.9.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-mwaa",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_mwaa"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.MWAA 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.MWAA 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore mwaa type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_mwaa": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mwaa/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-mwaa-2.9.0/types_aiobotocore_mwaa/__init__.py` & `types-aiobotocore-mwaa-2.9.1/types_aiobotocore_mwaa/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,9 +22,8 @@
 """
 
 from .client import MWAAClient
 from .paginator import ListEnvironmentsPaginator
 
 Client = MWAAClient
 
-
 __all__ = ("Client", "ListEnvironmentsPaginator", "MWAAClient")
```

### Comparing `types-aiobotocore-mwaa-2.9.0/types_aiobotocore_mwaa/__init__.pyi` & `types-aiobotocore-mwaa-2.9.1/types_aiobotocore_mwaa/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mwaa-2.9.0/types_aiobotocore_mwaa/__main__.py` & `types-aiobotocore-mwaa-2.9.1/types_aiobotocore_mwaa/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.MWAA 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.MWAA 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mwaa//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA\nOther"
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

### Comparing `types-aiobotocore-mwaa-2.9.0/types_aiobotocore_mwaa/client.py` & `types-aiobotocore-mwaa-2.9.1/types_aiobotocore_mwaa/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("MWAAClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -124,15 +123,15 @@
         RequirementsS3ObjectVersion: str = ...,
         RequirementsS3Path: str = ...,
         Schedulers: int = ...,
         StartupScriptS3ObjectVersion: str = ...,
         StartupScriptS3Path: str = ...,
         Tags: Mapping[str, str] = ...,
         WebserverAccessMode: WebserverAccessModeType = ...,
-        WeeklyMaintenanceWindowStart: str = ...
+        WeeklyMaintenanceWindowStart: str = ...,
     ) -> CreateEnvironmentOutputTypeDef:
         """
         Creates an Amazon Managed Workflows for Apache Airflow (MWAA) environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA.Client.create_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mwaa/client/#create_environment)
         """
@@ -243,15 +242,15 @@
         RequirementsS3ObjectVersion: str = ...,
         RequirementsS3Path: str = ...,
         Schedulers: int = ...,
         SourceBucketArn: str = ...,
         StartupScriptS3ObjectVersion: str = ...,
         StartupScriptS3Path: str = ...,
         WebserverAccessMode: WebserverAccessModeType = ...,
-        WeeklyMaintenanceWindowStart: str = ...
+        WeeklyMaintenanceWindowStart: str = ...,
     ) -> UpdateEnvironmentOutputTypeDef:
         """
         Updates an Amazon Managed Workflows for Apache Airflow (MWAA) environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA.Client.update_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mwaa/client/#update_environment)
         """
```

### Comparing `types-aiobotocore-mwaa-2.9.0/types_aiobotocore_mwaa/client.pyi` & `types-aiobotocore-mwaa-2.9.1/types_aiobotocore_mwaa/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -120,15 +120,15 @@
         RequirementsS3ObjectVersion: str = ...,
         RequirementsS3Path: str = ...,
         Schedulers: int = ...,
         StartupScriptS3ObjectVersion: str = ...,
         StartupScriptS3Path: str = ...,
         Tags: Mapping[str, str] = ...,
         WebserverAccessMode: WebserverAccessModeType = ...,
-        WeeklyMaintenanceWindowStart: str = ...
+        WeeklyMaintenanceWindowStart: str = ...,
     ) -> CreateEnvironmentOutputTypeDef:
         """
         Creates an Amazon Managed Workflows for Apache Airflow (MWAA) environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA.Client.create_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mwaa/client/#create_environment)
         """
@@ -239,15 +239,15 @@
         RequirementsS3ObjectVersion: str = ...,
         RequirementsS3Path: str = ...,
         Schedulers: int = ...,
         SourceBucketArn: str = ...,
         StartupScriptS3ObjectVersion: str = ...,
         StartupScriptS3Path: str = ...,
         WebserverAccessMode: WebserverAccessModeType = ...,
-        WeeklyMaintenanceWindowStart: str = ...
+        WeeklyMaintenanceWindowStart: str = ...,
     ) -> UpdateEnvironmentOutputTypeDef:
         """
         Updates an Amazon Managed Workflows for Apache Airflow (MWAA) environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA.Client.update_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mwaa/client/#update_environment)
         """
```

### Comparing `types-aiobotocore-mwaa-2.9.0/types_aiobotocore_mwaa/literals.py` & `types-aiobotocore-mwaa-2.9.1/types_aiobotocore_mwaa/literals.py`

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
     "EndpointManagementType",
     "EnvironmentStatusType",
     "ListEnvironmentsPaginatorName",
     "LoggingLevelType",
     "UnitType",
     "UpdateStatusType",
@@ -31,15 +30,14 @@
     "MWAAServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 EndpointManagementType = Literal["CUSTOMER", "SERVICE"]
 EnvironmentStatusType = Literal[
     "AVAILABLE",
     "CREATE_FAILED",
     "CREATING",
     "CREATING_SNAPSHOT",
     "DELETED",
```

### Comparing `types-aiobotocore-mwaa-2.9.0/types_aiobotocore_mwaa/literals.pyi` & `types-aiobotocore-mwaa-2.9.1/types_aiobotocore_mwaa/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mwaa-2.9.0/types_aiobotocore_mwaa/paginator.py` & `types-aiobotocore-mwaa-2.9.1/types_aiobotocore_mwaa/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -26,25 +26,22 @@
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .type_defs import ListEnvironmentsOutputTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListEnvironmentsPaginator",)
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListEnvironmentsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA.Paginator.ListEnvironments)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mwaa/paginators/#listenvironmentspaginator)
     """
 
     def paginate(
```

### Comparing `types-aiobotocore-mwaa-2.9.0/types_aiobotocore_mwaa/paginator.pyi` & `types-aiobotocore-mwaa-2.9.1/types_aiobotocore_mwaa/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,20 +28,22 @@
 
 from .type_defs import ListEnvironmentsOutputTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListEnvironmentsPaginator",)
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListEnvironmentsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA.Paginator.ListEnvironments)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mwaa/paginators/#listenvironmentspaginator)
     """
 
     def paginate(
```

### Comparing `types-aiobotocore-mwaa-2.9.0/types_aiobotocore_mwaa/type_defs.py` & `types-aiobotocore-mwaa-2.9.1/types_aiobotocore_mwaa/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CreateCliTokenRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "NetworkConfigurationTypeDef",
     "CreateWebLoginTokenRequestRequestTypeDef",
     "DeleteEnvironmentInputRequestTypeDef",
     "DimensionTypeDef",
```

### Comparing `types-aiobotocore-mwaa-2.9.0/types_aiobotocore_mwaa/type_defs.pyi` & `types-aiobotocore-mwaa-2.9.1/types_aiobotocore_mwaa/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mwaa-2.9.0/types_aiobotocore_mwaa.egg-info/PKG-INFO` & `types-aiobotocore-mwaa-2.9.1/types_aiobotocore_mwaa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mwaa
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.MWAA 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.MWAA 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mwaa/
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
 
 <a id="types-aiobotocore-mwaa"></a>
 
 # types-aiobotocore-mwaa
 
 [![PyPI - types-aiobotocore-mwaa](https://img.shields.io/pypi/v/types-aiobotocore-mwaa.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mwaa)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mwaa.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mwaa)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mwaa/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mwaa)](https://pepy.tech/project/types-aiobotocore-mwaa)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MWAA 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA)
+[aiobotocore.MWAA 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA)
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
 [types-aiobotocore-mwaa docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mwaa/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-mwaa-2.9.0/types_aiobotocore_mwaa.egg-info/SOURCES.txt` & `types-aiobotocore-mwaa-2.9.1/types_aiobotocore_mwaa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

