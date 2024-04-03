# Comparing `tmp/types-aiobotocore-mediapackage-2.9.0.tar.gz` & `tmp/types-aiobotocore-mediapackage-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-mediapackage-2.9.0.tar", last modified: Wed Dec 13 19:59:53 2023, max compression
+gzip compressed data, was "types-aiobotocore-mediapackage-2.9.1.tar", last modified: Thu Jan 18 01:21:15 2024, max compression
```

## Comparing `types-aiobotocore-mediapackage-2.9.0.tar` & `types-aiobotocore-mediapackage-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:53.489460 types-aiobotocore-mediapackage-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:50:14.000000 types-aiobotocore-mediapackage-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13532 2023-12-13 19:59:53.489460 types-aiobotocore-mediapackage-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11949 2023-12-13 19:50:14.000000 types-aiobotocore-mediapackage-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:53.489460 types-aiobotocore-mediapackage-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2023-12-13 19:50:14.000000 types-aiobotocore-mediapackage-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:53.485460 types-aiobotocore-mediapackage-2.9.0/types_aiobotocore_mediapackage/
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2023-12-13 19:50:14.000000 types-aiobotocore-mediapackage-2.9.0/types_aiobotocore_mediapackage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2023-12-13 19:50:14.000000 types-aiobotocore-mediapackage-2.9.0/types_aiobotocore_mediapackage/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      952 2023-12-13 19:50:14.000000 types-aiobotocore-mediapackage-2.9.0/types_aiobotocore_mediapackage/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18430 2023-12-13 19:50:14.000000 types-aiobotocore-mediapackage-2.9.0/types_aiobotocore_mediapackage/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    18426 2023-12-13 19:50:14.000000 types-aiobotocore-mediapackage-2.9.0/types_aiobotocore_mediapackage/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10869 2023-12-13 19:50:14.000000 types-aiobotocore-mediapackage-2.9.0/types_aiobotocore_mediapackage/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10867 2023-12-13 19:50:14.000000 types-aiobotocore-mediapackage-2.9.0/types_aiobotocore_mediapackage/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4404 2023-12-13 19:50:14.000000 types-aiobotocore-mediapackage-2.9.0/types_aiobotocore_mediapackage/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4399 2023-12-13 19:50:14.000000 types-aiobotocore-mediapackage-2.9.0/types_aiobotocore_mediapackage/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:50:14.000000 types-aiobotocore-mediapackage-2.9.0/types_aiobotocore_mediapackage/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    29923 2023-12-13 19:50:15.000000 types-aiobotocore-mediapackage-2.9.0/types_aiobotocore_mediapackage/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    29922 2023-12-13 19:50:14.000000 types-aiobotocore-mediapackage-2.9.0/types_aiobotocore_mediapackage/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:50:14.000000 types-aiobotocore-mediapackage-2.9.0/types_aiobotocore_mediapackage/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:53.489460 types-aiobotocore-mediapackage-2.9.0/types_aiobotocore_mediapackage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13532 2023-12-13 19:59:53.000000 types-aiobotocore-mediapackage-2.9.0/types_aiobotocore_mediapackage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      908 2023-12-13 19:59:53.000000 types-aiobotocore-mediapackage-2.9.0/types_aiobotocore_mediapackage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:53.000000 types-aiobotocore-mediapackage-2.9.0/types_aiobotocore_mediapackage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:53.000000 types-aiobotocore-mediapackage-2.9.0/types_aiobotocore_mediapackage.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:53.000000 types-aiobotocore-mediapackage-2.9.0/types_aiobotocore_mediapackage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-13 19:59:53.000000 types-aiobotocore-mediapackage-2.9.0/types_aiobotocore_mediapackage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:15.385185 types-aiobotocore-mediapackage-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:11:57.000000 types-aiobotocore-mediapackage-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13552 2024-01-18 01:21:15.385185 types-aiobotocore-mediapackage-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11949 2024-01-18 01:11:57.000000 types-aiobotocore-mediapackage-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:15.385185 types-aiobotocore-mediapackage-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-01-18 01:11:57.000000 types-aiobotocore-mediapackage-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:15.385185 types-aiobotocore-mediapackage-2.9.1/types_aiobotocore_mediapackage/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-01-18 01:11:57.000000 types-aiobotocore-mediapackage-2.9.1/types_aiobotocore_mediapackage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-01-18 01:11:57.000000 types-aiobotocore-mediapackage-2.9.1/types_aiobotocore_mediapackage/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-01-18 01:11:57.000000 types-aiobotocore-mediapackage-2.9.1/types_aiobotocore_mediapackage/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18434 2024-01-18 01:11:57.000000 types-aiobotocore-mediapackage-2.9.1/types_aiobotocore_mediapackage/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18431 2024-01-18 01:11:57.000000 types-aiobotocore-mediapackage-2.9.1/types_aiobotocore_mediapackage/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10867 2024-01-18 01:11:57.000000 types-aiobotocore-mediapackage-2.9.1/types_aiobotocore_mediapackage/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10867 2024-01-18 01:11:57.000000 types-aiobotocore-mediapackage-2.9.1/types_aiobotocore_mediapackage/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-01-18 01:11:57.000000 types-aiobotocore-mediapackage-2.9.1/types_aiobotocore_mediapackage/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-01-18 01:11:57.000000 types-aiobotocore-mediapackage-2.9.1/types_aiobotocore_mediapackage/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:11:57.000000 types-aiobotocore-mediapackage-2.9.1/types_aiobotocore_mediapackage/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    29922 2024-01-18 01:11:58.000000 types-aiobotocore-mediapackage-2.9.1/types_aiobotocore_mediapackage/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29922 2024-01-18 01:11:58.000000 types-aiobotocore-mediapackage-2.9.1/types_aiobotocore_mediapackage/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:11:57.000000 types-aiobotocore-mediapackage-2.9.1/types_aiobotocore_mediapackage/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:15.385185 types-aiobotocore-mediapackage-2.9.1/types_aiobotocore_mediapackage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13552 2024-01-18 01:21:15.000000 types-aiobotocore-mediapackage-2.9.1/types_aiobotocore_mediapackage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-01-18 01:21:15.000000 types-aiobotocore-mediapackage-2.9.1/types_aiobotocore_mediapackage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:15.000000 types-aiobotocore-mediapackage-2.9.1/types_aiobotocore_mediapackage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:15.000000 types-aiobotocore-mediapackage-2.9.1/types_aiobotocore_mediapackage.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:15.000000 types-aiobotocore-mediapackage-2.9.1/types_aiobotocore_mediapackage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-01-18 01:21:15.000000 types-aiobotocore-mediapackage-2.9.1/types_aiobotocore_mediapackage.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-mediapackage-2.9.0/LICENSE` & `types-aiobotocore-mediapackage-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-mediapackage-2.9.0/PKG-INFO` & `types-aiobotocore-mediapackage-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mediapackage
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.MediaPackage 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.MediaPackage 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage/
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
 
 <a id="types-aiobotocore-mediapackage"></a>
 
 # types-aiobotocore-mediapackage
 
 [![PyPI - types-aiobotocore-mediapackage](https://img.shields.io/pypi/v/types-aiobotocore-mediapackage.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediapackage)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mediapackage.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediapackage)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mediapackage)](https://pepy.tech/project/types-aiobotocore-mediapackage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MediaPackage 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage)
+[aiobotocore.MediaPackage 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage)
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
 [types-aiobotocore-mediapackage docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-mediapackage-2.9.0/README.md` & `types-aiobotocore-mediapackage-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mediapackage.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediapackage)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mediapackage)](https://pepy.tech/project/types-aiobotocore-mediapackage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MediaPackage 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage)
+[aiobotocore.MediaPackage 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage)
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
 [types-aiobotocore-mediapackage docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-mediapackage-2.9.0/setup.py` & `types-aiobotocore-mediapackage-2.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-mediapackage",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_mediapackage"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.MediaPackage 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.MediaPackage 2.9.1 service generated with"
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
     keywords="aiobotocore mediapackage type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_mediapackage": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-mediapackage-2.9.0/types_aiobotocore_mediapackage/__init__.py` & `types-aiobotocore-mediapackage-2.9.1/types_aiobotocore_mediapackage/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 """
 
 from .client import MediaPackageClient
 from .paginator import ListChannelsPaginator, ListHarvestJobsPaginator, ListOriginEndpointsPaginator
 
 Client = MediaPackageClient
 
-
 __all__ = (
     "Client",
     "ListChannelsPaginator",
     "ListHarvestJobsPaginator",
     "ListOriginEndpointsPaginator",
     "MediaPackageClient",
 )
```

### Comparing `types-aiobotocore-mediapackage-2.9.0/types_aiobotocore_mediapackage/__init__.pyi` & `types-aiobotocore-mediapackage-2.9.1/types_aiobotocore_mediapackage/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediapackage-2.9.0/types_aiobotocore_mediapackage/__main__.py` & `types-aiobotocore-mediapackage-2.9.1/types_aiobotocore_mediapackage/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.MediaPackage 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.MediaPackage 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage\nOther"
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

### Comparing `types-aiobotocore-mediapackage-2.9.0/types_aiobotocore_mediapackage/client.py` & `types-aiobotocore-mediapackage-2.9.1/types_aiobotocore_mediapackage/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("MediaPackageClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -111,15 +110,15 @@
         """
 
     async def configure_logs(
         self,
         *,
         Id: str,
         EgressAccessLogs: EgressAccessLogsTypeDef = ...,
-        IngressAccessLogs: IngressAccessLogsTypeDef = ...
+        IngressAccessLogs: IngressAccessLogsTypeDef = ...,
     ) -> ConfigureLogsResponseTypeDef:
         """
         Changes the Channel's properities to configure log subscription See also: [AWS
         API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/mediapackage-2017-10-12/ConfigureLogs).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client.configure_logs)
@@ -139,15 +138,15 @@
     async def create_harvest_job(
         self,
         *,
         EndTime: str,
         Id: str,
         OriginEndpointId: str,
         S3Destination: S3DestinationTypeDef,
-        StartTime: str
+        StartTime: str,
     ) -> CreateHarvestJobResponseTypeDef:
         """
         Creates a new HarvestJob record.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client.create_harvest_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage/client/#create_harvest_job)
         """
@@ -164,15 +163,15 @@
         HlsPackage: HlsPackageTypeDef = ...,
         ManifestName: str = ...,
         MssPackage: MssPackageTypeDef = ...,
         Origination: OriginationType = ...,
         StartoverWindowSeconds: int = ...,
         Tags: Mapping[str, str] = ...,
         TimeDelaySeconds: int = ...,
-        Whitelist: Sequence[str] = ...
+        Whitelist: Sequence[str] = ...,
     ) -> CreateOriginEndpointResponseTypeDef:
         """
         Creates a new OriginEndpoint record.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client.create_origin_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage/client/#create_origin_endpoint)
         """
@@ -243,15 +242,15 @@
 
     async def list_harvest_jobs(
         self,
         *,
         IncludeChannelId: str = ...,
         IncludeStatus: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListHarvestJobsResponseTypeDef:
         """
         Returns a collection of HarvestJob records.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client.list_harvest_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage/client/#list_harvest_jobs)
         """
@@ -341,15 +340,15 @@
         Description: str = ...,
         HlsPackage: HlsPackageTypeDef = ...,
         ManifestName: str = ...,
         MssPackage: MssPackageTypeDef = ...,
         Origination: OriginationType = ...,
         StartoverWindowSeconds: int = ...,
         TimeDelaySeconds: int = ...,
-        Whitelist: Sequence[str] = ...
+        Whitelist: Sequence[str] = ...,
     ) -> UpdateOriginEndpointResponseTypeDef:
         """
         Updates an existing OriginEndpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client.update_origin_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage/client/#update_origin_endpoint)
         """
```

### Comparing `types-aiobotocore-mediapackage-2.9.0/types_aiobotocore_mediapackage/client.pyi` & `types-aiobotocore-mediapackage-2.9.1/types_aiobotocore_mediapackage/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         """
 
     async def configure_logs(
         self,
         *,
         Id: str,
         EgressAccessLogs: EgressAccessLogsTypeDef = ...,
-        IngressAccessLogs: IngressAccessLogsTypeDef = ...
+        IngressAccessLogs: IngressAccessLogsTypeDef = ...,
     ) -> ConfigureLogsResponseTypeDef:
         """
         Changes the Channel's properities to configure log subscription See also: [AWS
         API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/mediapackage-2017-10-12/ConfigureLogs).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client.configure_logs)
@@ -135,15 +135,15 @@
     async def create_harvest_job(
         self,
         *,
         EndTime: str,
         Id: str,
         OriginEndpointId: str,
         S3Destination: S3DestinationTypeDef,
-        StartTime: str
+        StartTime: str,
     ) -> CreateHarvestJobResponseTypeDef:
         """
         Creates a new HarvestJob record.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client.create_harvest_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage/client/#create_harvest_job)
         """
@@ -160,15 +160,15 @@
         HlsPackage: HlsPackageTypeDef = ...,
         ManifestName: str = ...,
         MssPackage: MssPackageTypeDef = ...,
         Origination: OriginationType = ...,
         StartoverWindowSeconds: int = ...,
         Tags: Mapping[str, str] = ...,
         TimeDelaySeconds: int = ...,
-        Whitelist: Sequence[str] = ...
+        Whitelist: Sequence[str] = ...,
     ) -> CreateOriginEndpointResponseTypeDef:
         """
         Creates a new OriginEndpoint record.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client.create_origin_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage/client/#create_origin_endpoint)
         """
@@ -239,15 +239,15 @@
 
     async def list_harvest_jobs(
         self,
         *,
         IncludeChannelId: str = ...,
         IncludeStatus: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListHarvestJobsResponseTypeDef:
         """
         Returns a collection of HarvestJob records.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client.list_harvest_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage/client/#list_harvest_jobs)
         """
@@ -337,15 +337,15 @@
         Description: str = ...,
         HlsPackage: HlsPackageTypeDef = ...,
         ManifestName: str = ...,
         MssPackage: MssPackageTypeDef = ...,
         Origination: OriginationType = ...,
         StartoverWindowSeconds: int = ...,
         TimeDelaySeconds: int = ...,
-        Whitelist: Sequence[str] = ...
+        Whitelist: Sequence[str] = ...,
     ) -> UpdateOriginEndpointResponseTypeDef:
         """
         Updates an existing OriginEndpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client.update_origin_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage/client/#update_origin_endpoint)
         """
```

### Comparing `types-aiobotocore-mediapackage-2.9.0/types_aiobotocore_mediapackage/literals.py` & `types-aiobotocore-mediapackage-2.9.1/types_aiobotocore_mediapackage/literals.py`

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
     "AdMarkersType",
     "AdTriggersElementType",
     "AdsOnDeliveryRestrictionsType",
     "CmafEncryptionMethodType",
     "EncryptionMethodType",
     "ListChannelsPaginatorName",
@@ -43,15 +42,14 @@
     "MediaPackageServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AdMarkersType = Literal["DATERANGE", "NONE", "PASSTHROUGH", "SCTE35_ENHANCED"]
 AdTriggersElementType = Literal[
     "BREAK",
     "DISTRIBUTOR_ADVERTISEMENT",
     "DISTRIBUTOR_OVERLAY_PLACEMENT_OPPORTUNITY",
     "DISTRIBUTOR_PLACEMENT_OPPORTUNITY",
     "PROVIDER_ADVERTISEMENT",
```

### Comparing `types-aiobotocore-mediapackage-2.9.0/types_aiobotocore_mediapackage/literals.pyi` & `types-aiobotocore-mediapackage-2.9.1/types_aiobotocore_mediapackage/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediapackage-2.9.0/types_aiobotocore_mediapackage/paginator.py` & `types-aiobotocore-mediapackage-2.9.1/types_aiobotocore_mediapackage/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,14 @@
     ListHarvestJobsResponseTypeDef,
     ListOriginEndpointsResponsePaginatorTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("ListChannelsPaginator", "ListHarvestJobsPaginator", "ListOriginEndpointsPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -72,15 +71,15 @@
     """
 
     def paginate(
         self,
         *,
         IncludeChannelId: str = ...,
         IncludeStatus: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListHarvestJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Paginator.ListHarvestJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage/paginators/#listharvestjobspaginator)
         """
```

### Comparing `types-aiobotocore-mediapackage-2.9.0/types_aiobotocore_mediapackage/paginator.pyi` & `types-aiobotocore-mediapackage-2.9.1/types_aiobotocore_mediapackage/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     """
 
     def paginate(
         self,
         *,
         IncludeChannelId: str = ...,
         IncludeStatus: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListHarvestJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Paginator.ListHarvestJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage/paginators/#listharvestjobspaginator)
         """
 
 class ListOriginEndpointsPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-mediapackage-2.9.0/types_aiobotocore_mediapackage/type_defs.py` & `types-aiobotocore-mediapackage-2.9.1/types_aiobotocore_mediapackage/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AuthorizationTypeDef",
     "EgressAccessLogsTypeDef",
     "IngressAccessLogsTypeDef",
     "HlsManifestCreateOrUpdateParametersTypeDef",
     "StreamSelectionTypeDef",
     "HlsManifestTypeDef",
```

### Comparing `types-aiobotocore-mediapackage-2.9.0/types_aiobotocore_mediapackage/type_defs.pyi` & `types-aiobotocore-mediapackage-2.9.1/types_aiobotocore_mediapackage/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediapackage-2.9.0/types_aiobotocore_mediapackage.egg-info/PKG-INFO` & `types-aiobotocore-mediapackage-2.9.1/types_aiobotocore_mediapackage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mediapackage
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.MediaPackage 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.MediaPackage 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage/
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
 
 <a id="types-aiobotocore-mediapackage"></a>
 
 # types-aiobotocore-mediapackage
 
 [![PyPI - types-aiobotocore-mediapackage](https://img.shields.io/pypi/v/types-aiobotocore-mediapackage.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediapackage)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mediapackage.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediapackage)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mediapackage)](https://pepy.tech/project/types-aiobotocore-mediapackage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MediaPackage 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage)
+[aiobotocore.MediaPackage 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage)
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
 [types-aiobotocore-mediapackage docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-mediapackage-2.9.0/types_aiobotocore_mediapackage.egg-info/SOURCES.txt` & `types-aiobotocore-mediapackage-2.9.1/types_aiobotocore_mediapackage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

