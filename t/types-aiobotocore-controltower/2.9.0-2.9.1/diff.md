# Comparing `tmp/types-aiobotocore-controltower-2.9.0.tar.gz` & `tmp/types-aiobotocore-controltower-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-controltower-2.9.0.tar", last modified: Wed Dec 13 19:59:01 2023, max compression
+gzip compressed data, was "types-aiobotocore-controltower-2.9.1.tar", last modified: Thu Jan 18 01:20:27 2024, max compression
```

## Comparing `types-aiobotocore-controltower-2.9.0.tar` & `types-aiobotocore-controltower-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:01.613875 types-aiobotocore-controltower-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:43:36.000000 types-aiobotocore-controltower-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13450 2023-12-13 19:59:01.613875 types-aiobotocore-controltower-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11867 2023-12-13 19:43:36.000000 types-aiobotocore-controltower-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:01.613875 types-aiobotocore-controltower-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2023-12-13 19:43:36.000000 types-aiobotocore-controltower-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:01.613875 types-aiobotocore-controltower-2.9.0/types_aiobotocore_controltower/
--rw-r--r--   0 runner    (1001) docker     (127)      935 2023-12-13 19:43:36.000000 types-aiobotocore-controltower-2.9.0/types_aiobotocore_controltower/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2023-12-13 19:43:36.000000 types-aiobotocore-controltower-2.9.0/types_aiobotocore_controltower/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      952 2023-12-13 19:43:36.000000 types-aiobotocore-controltower-2.9.0/types_aiobotocore_controltower/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14824 2023-12-13 19:43:36.000000 types-aiobotocore-controltower-2.9.0/types_aiobotocore_controltower/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14820 2023-12-13 19:43:36.000000 types-aiobotocore-controltower-2.9.0/types_aiobotocore_controltower/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9861 2023-12-13 19:43:36.000000 types-aiobotocore-controltower-2.9.0/types_aiobotocore_controltower/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9859 2023-12-13 19:43:36.000000 types-aiobotocore-controltower-2.9.0/types_aiobotocore_controltower/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3244 2023-12-13 19:43:36.000000 types-aiobotocore-controltower-2.9.0/types_aiobotocore_controltower/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3240 2023-12-13 19:43:36.000000 types-aiobotocore-controltower-2.9.0/types_aiobotocore_controltower/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:43:36.000000 types-aiobotocore-controltower-2.9.0/types_aiobotocore_controltower/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    12350 2023-12-13 19:43:36.000000 types-aiobotocore-controltower-2.9.0/types_aiobotocore_controltower/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12349 2023-12-13 19:43:36.000000 types-aiobotocore-controltower-2.9.0/types_aiobotocore_controltower/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:43:36.000000 types-aiobotocore-controltower-2.9.0/types_aiobotocore_controltower/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:01.613875 types-aiobotocore-controltower-2.9.0/types_aiobotocore_controltower.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13450 2023-12-13 19:59:01.000000 types-aiobotocore-controltower-2.9.0/types_aiobotocore_controltower.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      908 2023-12-13 19:59:01.000000 types-aiobotocore-controltower-2.9.0/types_aiobotocore_controltower.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:01.000000 types-aiobotocore-controltower-2.9.0/types_aiobotocore_controltower.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:01.000000 types-aiobotocore-controltower-2.9.0/types_aiobotocore_controltower.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:01.000000 types-aiobotocore-controltower-2.9.0/types_aiobotocore_controltower.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-13 19:59:01.000000 types-aiobotocore-controltower-2.9.0/types_aiobotocore_controltower.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:27.381410 types-aiobotocore-controltower-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:05:31.000000 types-aiobotocore-controltower-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13470 2024-01-18 01:20:27.381410 types-aiobotocore-controltower-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11867 2024-01-18 01:05:31.000000 types-aiobotocore-controltower-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:27.381410 types-aiobotocore-controltower-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-01-18 01:05:31.000000 types-aiobotocore-controltower-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:27.377411 types-aiobotocore-controltower-2.9.1/types_aiobotocore_controltower/
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-01-18 01:05:31.000000 types-aiobotocore-controltower-2.9.1/types_aiobotocore_controltower/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-01-18 01:05:31.000000 types-aiobotocore-controltower-2.9.1/types_aiobotocore_controltower/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-01-18 01:05:31.000000 types-aiobotocore-controltower-2.9.1/types_aiobotocore_controltower/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14824 2024-01-18 01:05:31.000000 types-aiobotocore-controltower-2.9.1/types_aiobotocore_controltower/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14821 2024-01-18 01:05:31.000000 types-aiobotocore-controltower-2.9.1/types_aiobotocore_controltower/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9859 2024-01-18 01:05:31.000000 types-aiobotocore-controltower-2.9.1/types_aiobotocore_controltower/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9859 2024-01-18 01:05:31.000000 types-aiobotocore-controltower-2.9.1/types_aiobotocore_controltower/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-01-18 01:05:31.000000 types-aiobotocore-controltower-2.9.1/types_aiobotocore_controltower/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-01-18 01:05:31.000000 types-aiobotocore-controltower-2.9.1/types_aiobotocore_controltower/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:05:31.000000 types-aiobotocore-controltower-2.9.1/types_aiobotocore_controltower/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    12349 2024-01-18 01:05:32.000000 types-aiobotocore-controltower-2.9.1/types_aiobotocore_controltower/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12349 2024-01-18 01:05:32.000000 types-aiobotocore-controltower-2.9.1/types_aiobotocore_controltower/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:05:31.000000 types-aiobotocore-controltower-2.9.1/types_aiobotocore_controltower/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:27.381410 types-aiobotocore-controltower-2.9.1/types_aiobotocore_controltower.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13470 2024-01-18 01:20:27.000000 types-aiobotocore-controltower-2.9.1/types_aiobotocore_controltower.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-01-18 01:20:27.000000 types-aiobotocore-controltower-2.9.1/types_aiobotocore_controltower.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:27.000000 types-aiobotocore-controltower-2.9.1/types_aiobotocore_controltower.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:27.000000 types-aiobotocore-controltower-2.9.1/types_aiobotocore_controltower.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:27.000000 types-aiobotocore-controltower-2.9.1/types_aiobotocore_controltower.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-01-18 01:20:27.000000 types-aiobotocore-controltower-2.9.1/types_aiobotocore_controltower.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-controltower-2.9.0/LICENSE` & `types-aiobotocore-controltower-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-controltower-2.9.0/PKG-INFO` & `types-aiobotocore-controltower-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-controltower
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ControlTower 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ControlTower 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_controltower/
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
 
 <a id="types-aiobotocore-controltower"></a>
 
 # types-aiobotocore-controltower
 
 [![PyPI - types-aiobotocore-controltower](https://img.shields.io/pypi/v/types-aiobotocore-controltower.svg?color=blue)](https://pypi.org/project/types-aiobotocore-controltower)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-controltower.svg?color=blue)](https://pypi.org/project/types-aiobotocore-controltower)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_controltower/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-controltower)](https://pepy.tech/project/types-aiobotocore-controltower)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ControlTower 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower)
+[aiobotocore.ControlTower 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower)
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
 [types-aiobotocore-controltower docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_controltower/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-controltower-2.9.0/README.md` & `types-aiobotocore-controltower-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-controltower.svg?color=blue)](https://pypi.org/project/types-aiobotocore-controltower)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_controltower/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-controltower)](https://pepy.tech/project/types-aiobotocore-controltower)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ControlTower 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower)
+[aiobotocore.ControlTower 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower)
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
 [types-aiobotocore-controltower docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_controltower/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-controltower-2.9.0/setup.py` & `types-aiobotocore-controltower-2.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-controltower",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_controltower"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ControlTower 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.ControlTower 2.9.1 service generated with"
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
     keywords="aiobotocore controltower type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_controltower": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_controltower/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-controltower-2.9.0/types_aiobotocore_controltower/__init__.py` & `types-aiobotocore-controltower-2.9.1/types_aiobotocore_controltower/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,13 @@
 """
 
 from .client import ControlTowerClient
 from .paginator import ListEnabledControlsPaginator, ListLandingZonesPaginator
 
 Client = ControlTowerClient
 
-
 __all__ = (
     "Client",
     "ControlTowerClient",
     "ListEnabledControlsPaginator",
     "ListLandingZonesPaginator",
 )
```

### Comparing `types-aiobotocore-controltower-2.9.0/types_aiobotocore_controltower/__init__.pyi` & `types-aiobotocore-controltower-2.9.1/types_aiobotocore_controltower/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-controltower-2.9.0/types_aiobotocore_controltower/__main__.py` & `types-aiobotocore-controltower-2.9.1/types_aiobotocore_controltower/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ControlTower 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.ControlTower 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_controltower//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower\nOther"
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

### Comparing `types-aiobotocore-controltower-2.9.0/types_aiobotocore_controltower/client.py` & `types-aiobotocore-controltower-2.9.1/types_aiobotocore_controltower/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ControlTowerClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -133,15 +132,15 @@
 
     async def enable_control(
         self,
         *,
         controlIdentifier: str,
         targetIdentifier: str,
         parameters: Sequence[EnabledControlParameterTypeDef] = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> EnableControlOutputTypeDef:
         """
         This API call activates a control.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.enable_control)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_controltower/client/#enable_control)
         """
```

### Comparing `types-aiobotocore-controltower-2.9.0/types_aiobotocore_controltower/client.pyi` & `types-aiobotocore-controltower-2.9.1/types_aiobotocore_controltower/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
 
     async def enable_control(
         self,
         *,
         controlIdentifier: str,
         targetIdentifier: str,
         parameters: Sequence[EnabledControlParameterTypeDef] = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> EnableControlOutputTypeDef:
         """
         This API call activates a control.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.enable_control)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_controltower/client/#enable_control)
         """
```

### Comparing `types-aiobotocore-controltower-2.9.0/types_aiobotocore_controltower/literals.py` & `types-aiobotocore-controltower-2.9.1/types_aiobotocore_controltower/literals.py`

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
     "ControlOperationStatusType",
     "ControlOperationTypeType",
     "DriftStatusType",
     "EnablementStatusType",
     "LandingZoneDriftStatusType",
     "LandingZoneOperationStatusType",
@@ -34,15 +33,14 @@
     "ControlTowerServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ControlOperationStatusType = Literal["FAILED", "IN_PROGRESS", "SUCCEEDED"]
 ControlOperationTypeType = Literal["DISABLE_CONTROL", "ENABLE_CONTROL", "UPDATE_ENABLED_CONTROL"]
 DriftStatusType = Literal["DRIFTED", "IN_SYNC", "NOT_CHECKING", "UNKNOWN"]
 EnablementStatusType = Literal["FAILED", "SUCCEEDED", "UNDER_CHANGE"]
 LandingZoneDriftStatusType = Literal["DRIFTED", "IN_SYNC"]
 LandingZoneOperationStatusType = Literal["FAILED", "IN_PROGRESS", "SUCCEEDED"]
 LandingZoneOperationTypeType = Literal["CREATE", "DELETE", "RESET", "UPDATE"]
```

### Comparing `types-aiobotocore-controltower-2.9.0/types_aiobotocore_controltower/literals.pyi` & `types-aiobotocore-controltower-2.9.1/types_aiobotocore_controltower/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-controltower-2.9.0/types_aiobotocore_controltower/paginator.py` & `types-aiobotocore-controltower-2.9.1/types_aiobotocore_controltower/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,14 @@
     ListEnabledControlsOutputTypeDef,
     ListLandingZonesOutputTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("ListEnabledControlsPaginator", "ListLandingZonesPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
```

### Comparing `types-aiobotocore-controltower-2.9.0/types_aiobotocore_controltower/paginator.pyi` & `types-aiobotocore-controltower-2.9.1/types_aiobotocore_controltower/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-controltower-2.9.0/types_aiobotocore_controltower/type_defs.py` & `types-aiobotocore-controltower-2.9.1/types_aiobotocore_controltower/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ControlOperationTypeDef",
     "CreateLandingZoneInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteLandingZoneInputRequestTypeDef",
     "DisableControlInputRequestTypeDef",
     "DriftStatusSummaryTypeDef",
```

### Comparing `types-aiobotocore-controltower-2.9.0/types_aiobotocore_controltower/type_defs.pyi` & `types-aiobotocore-controltower-2.9.1/types_aiobotocore_controltower/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-controltower-2.9.0/types_aiobotocore_controltower.egg-info/PKG-INFO` & `types-aiobotocore-controltower-2.9.1/types_aiobotocore_controltower.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-controltower
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ControlTower 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ControlTower 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_controltower/
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
 
 <a id="types-aiobotocore-controltower"></a>
 
 # types-aiobotocore-controltower
 
 [![PyPI - types-aiobotocore-controltower](https://img.shields.io/pypi/v/types-aiobotocore-controltower.svg?color=blue)](https://pypi.org/project/types-aiobotocore-controltower)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-controltower.svg?color=blue)](https://pypi.org/project/types-aiobotocore-controltower)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_controltower/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-controltower)](https://pepy.tech/project/types-aiobotocore-controltower)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ControlTower 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower)
+[aiobotocore.ControlTower 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower)
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
 [types-aiobotocore-controltower docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_controltower/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-controltower-2.9.0/types_aiobotocore_controltower.egg-info/SOURCES.txt` & `types-aiobotocore-controltower-2.9.1/types_aiobotocore_controltower.egg-info/SOURCES.txt`

 * *Files identical despite different names*

