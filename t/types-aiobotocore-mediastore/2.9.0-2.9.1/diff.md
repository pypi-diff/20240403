# Comparing `tmp/types-aiobotocore-mediastore-2.9.0.tar.gz` & `tmp/types-aiobotocore-mediastore-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-mediastore-2.9.0.tar", last modified: Wed Dec 13 19:59:54 2023, max compression
+gzip compressed data, was "types-aiobotocore-mediastore-2.9.1.tar", last modified: Thu Jan 18 01:21:16 2024, max compression
```

## Comparing `types-aiobotocore-mediastore-2.9.0.tar` & `types-aiobotocore-mediastore-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:54.965446 types-aiobotocore-mediastore-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:50:19.000000 types-aiobotocore-mediastore-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13121 2023-12-13 19:59:54.965446 types-aiobotocore-mediastore-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11546 2023-12-13 19:50:19.000000 types-aiobotocore-mediastore-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:54.965446 types-aiobotocore-mediastore-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2023-12-13 19:50:19.000000 types-aiobotocore-mediastore-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:54.961446 types-aiobotocore-mediastore-2.9.0/types_aiobotocore_mediastore/
--rw-r--r--   0 runner    (1001) docker     (127)      672 2023-12-13 19:50:19.000000 types-aiobotocore-mediastore-2.9.0/types_aiobotocore_mediastore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2023-12-13 19:50:19.000000 types-aiobotocore-mediastore-2.9.0/types_aiobotocore_mediastore/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      944 2023-12-13 19:50:19.000000 types-aiobotocore-mediastore-2.9.0/types_aiobotocore_mediastore/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16141 2023-12-13 19:50:19.000000 types-aiobotocore-mediastore-2.9.0/types_aiobotocore_mediastore/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    16137 2023-12-13 19:50:19.000000 types-aiobotocore-mediastore-2.9.0/types_aiobotocore_mediastore/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8753 2023-12-13 19:50:19.000000 types-aiobotocore-mediastore-2.9.0/types_aiobotocore_mediastore/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8751 2023-12-13 19:50:19.000000 types-aiobotocore-mediastore-2.9.0/types_aiobotocore_mediastore/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2023-12-13 19:50:19.000000 types-aiobotocore-mediastore-2.9.0/types_aiobotocore_mediastore/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2023-12-13 19:50:19.000000 types-aiobotocore-mediastore-2.9.0/types_aiobotocore_mediastore/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:50:19.000000 types-aiobotocore-mediastore-2.9.0/types_aiobotocore_mediastore/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     8619 2023-12-13 19:50:19.000000 types-aiobotocore-mediastore-2.9.0/types_aiobotocore_mediastore/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8618 2023-12-13 19:50:19.000000 types-aiobotocore-mediastore-2.9.0/types_aiobotocore_mediastore/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:50:19.000000 types-aiobotocore-mediastore-2.9.0/types_aiobotocore_mediastore/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:54.965446 types-aiobotocore-mediastore-2.9.0/types_aiobotocore_mediastore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13121 2023-12-13 19:59:54.000000 types-aiobotocore-mediastore-2.9.0/types_aiobotocore_mediastore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      870 2023-12-13 19:59:54.000000 types-aiobotocore-mediastore-2.9.0/types_aiobotocore_mediastore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:54.000000 types-aiobotocore-mediastore-2.9.0/types_aiobotocore_mediastore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:54.000000 types-aiobotocore-mediastore-2.9.0/types_aiobotocore_mediastore.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:54.000000 types-aiobotocore-mediastore-2.9.0/types_aiobotocore_mediastore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-13 19:59:54.000000 types-aiobotocore-mediastore-2.9.0/types_aiobotocore_mediastore.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:16.749179 types-aiobotocore-mediastore-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:12:02.000000 types-aiobotocore-mediastore-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13141 2024-01-18 01:21:16.749179 types-aiobotocore-mediastore-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11546 2024-01-18 01:12:02.000000 types-aiobotocore-mediastore-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:16.749179 types-aiobotocore-mediastore-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-01-18 01:12:02.000000 types-aiobotocore-mediastore-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:16.749179 types-aiobotocore-mediastore-2.9.1/types_aiobotocore_mediastore/
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-01-18 01:12:02.000000 types-aiobotocore-mediastore-2.9.1/types_aiobotocore_mediastore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-01-18 01:12:02.000000 types-aiobotocore-mediastore-2.9.1/types_aiobotocore_mediastore/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-01-18 01:12:02.000000 types-aiobotocore-mediastore-2.9.1/types_aiobotocore_mediastore/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16140 2024-01-18 01:12:02.000000 types-aiobotocore-mediastore-2.9.1/types_aiobotocore_mediastore/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16137 2024-01-18 01:12:02.000000 types-aiobotocore-mediastore-2.9.1/types_aiobotocore_mediastore/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8751 2024-01-18 01:12:03.000000 types-aiobotocore-mediastore-2.9.1/types_aiobotocore_mediastore/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8751 2024-01-18 01:12:02.000000 types-aiobotocore-mediastore-2.9.1/types_aiobotocore_mediastore/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-01-18 01:12:02.000000 types-aiobotocore-mediastore-2.9.1/types_aiobotocore_mediastore/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-01-18 01:12:02.000000 types-aiobotocore-mediastore-2.9.1/types_aiobotocore_mediastore/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:12:02.000000 types-aiobotocore-mediastore-2.9.1/types_aiobotocore_mediastore/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     8618 2024-01-18 01:12:03.000000 types-aiobotocore-mediastore-2.9.1/types_aiobotocore_mediastore/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8618 2024-01-18 01:12:03.000000 types-aiobotocore-mediastore-2.9.1/types_aiobotocore_mediastore/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:12:02.000000 types-aiobotocore-mediastore-2.9.1/types_aiobotocore_mediastore/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:16.749179 types-aiobotocore-mediastore-2.9.1/types_aiobotocore_mediastore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13141 2024-01-18 01:21:16.000000 types-aiobotocore-mediastore-2.9.1/types_aiobotocore_mediastore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-01-18 01:21:16.000000 types-aiobotocore-mediastore-2.9.1/types_aiobotocore_mediastore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:16.000000 types-aiobotocore-mediastore-2.9.1/types_aiobotocore_mediastore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:16.000000 types-aiobotocore-mediastore-2.9.1/types_aiobotocore_mediastore.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:16.000000 types-aiobotocore-mediastore-2.9.1/types_aiobotocore_mediastore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-01-18 01:21:16.000000 types-aiobotocore-mediastore-2.9.1/types_aiobotocore_mediastore.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-mediastore-2.9.0/LICENSE` & `types-aiobotocore-mediastore-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-mediastore-2.9.0/PKG-INFO` & `types-aiobotocore-mediastore-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mediastore
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.MediaStore 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.MediaStore 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore/
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
 
 <a id="types-aiobotocore-mediastore"></a>
 
 # types-aiobotocore-mediastore
 
 [![PyPI - types-aiobotocore-mediastore](https://img.shields.io/pypi/v/types-aiobotocore-mediastore.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediastore)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mediastore.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediastore)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mediastore)](https://pepy.tech/project/types-aiobotocore-mediastore)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MediaStore 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore)
+[aiobotocore.MediaStore 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore)
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
 [types-aiobotocore-mediastore docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-mediastore-2.9.0/README.md` & `types-aiobotocore-mediastore-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mediastore.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediastore)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mediastore)](https://pepy.tech/project/types-aiobotocore-mediastore)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MediaStore 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore)
+[aiobotocore.MediaStore 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore)
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
 [types-aiobotocore-mediastore docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-mediastore-2.9.0/setup.py` & `types-aiobotocore-mediastore-2.9.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-mediastore",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_mediastore"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.MediaStore 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.MediaStore 2.9.1 service generated with"
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
     keywords="aiobotocore mediastore type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_mediastore": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-mediastore-2.9.0/types_aiobotocore_mediastore/__init__.py` & `types-aiobotocore-mediastore-2.9.1/types_aiobotocore_mediastore/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,9 +22,8 @@
 """
 
 from .client import MediaStoreClient
 from .paginator import ListContainersPaginator
 
 Client = MediaStoreClient
 
-
 __all__ = ("Client", "ListContainersPaginator", "MediaStoreClient")
```

### Comparing `types-aiobotocore-mediastore-2.9.0/types_aiobotocore_mediastore/__init__.pyi` & `types-aiobotocore-mediastore-2.9.1/types_aiobotocore_mediastore/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediastore-2.9.0/types_aiobotocore_mediastore/__main__.py` & `types-aiobotocore-mediastore-2.9.1/types_aiobotocore_mediastore/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.MediaStore 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.MediaStore 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore\nOther"
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

### Comparing `types-aiobotocore-mediastore-2.9.0/types_aiobotocore_mediastore/client.py` & `types-aiobotocore-mediastore-2.9.1/types_aiobotocore_mediastore/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("MediaStoreClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
```

### Comparing `types-aiobotocore-mediastore-2.9.0/types_aiobotocore_mediastore/client.pyi` & `types-aiobotocore-mediastore-2.9.1/types_aiobotocore_mediastore/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediastore-2.9.0/types_aiobotocore_mediastore/literals.py` & `types-aiobotocore-mediastore-2.9.1/types_aiobotocore_mediastore/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,28 +15,26 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ContainerLevelMetricsType",
     "ContainerStatusType",
     "ListContainersPaginatorName",
     "MethodNameType",
     "MediaStoreServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ContainerLevelMetricsType = Literal["DISABLED", "ENABLED"]
 ContainerStatusType = Literal["ACTIVE", "CREATING", "DELETING"]
 ListContainersPaginatorName = Literal["list_containers"]
 MethodNameType = Literal["DELETE", "GET", "HEAD", "PUT"]
 MediaStoreServiceName = Literal["mediastore"]
 ServiceName = Literal[
     "accessanalyzer",
```

### Comparing `types-aiobotocore-mediastore-2.9.0/types_aiobotocore_mediastore/literals.pyi` & `types-aiobotocore-mediastore-2.9.1/types_aiobotocore_mediastore/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediastore-2.9.0/types_aiobotocore_mediastore/paginator.py` & `types-aiobotocore-mediastore-2.9.1/types_aiobotocore_mediastore/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .type_defs import ListContainersOutputTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListContainersPaginator",)
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
```

### Comparing `types-aiobotocore-mediastore-2.9.0/types_aiobotocore_mediastore/paginator.pyi` & `types-aiobotocore-mediastore-2.9.1/types_aiobotocore_mediastore/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediastore-2.9.0/types_aiobotocore_mediastore/type_defs.py` & `types-aiobotocore-mediastore-2.9.1/types_aiobotocore_mediastore/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ContainerTypeDef",
     "CorsRuleTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteContainerInputRequestTypeDef",
     "DeleteContainerPolicyInputRequestTypeDef",
```

### Comparing `types-aiobotocore-mediastore-2.9.0/types_aiobotocore_mediastore/type_defs.pyi` & `types-aiobotocore-mediastore-2.9.1/types_aiobotocore_mediastore/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediastore-2.9.0/types_aiobotocore_mediastore.egg-info/PKG-INFO` & `types-aiobotocore-mediastore-2.9.1/types_aiobotocore_mediastore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mediastore
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.MediaStore 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.MediaStore 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore/
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
 
 <a id="types-aiobotocore-mediastore"></a>
 
 # types-aiobotocore-mediastore
 
 [![PyPI - types-aiobotocore-mediastore](https://img.shields.io/pypi/v/types-aiobotocore-mediastore.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediastore)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mediastore.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediastore)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mediastore)](https://pepy.tech/project/types-aiobotocore-mediastore)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MediaStore 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore)
+[aiobotocore.MediaStore 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore)
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
 [types-aiobotocore-mediastore docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-mediastore-2.9.0/types_aiobotocore_mediastore.egg-info/SOURCES.txt` & `types-aiobotocore-mediastore-2.9.1/types_aiobotocore_mediastore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

