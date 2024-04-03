# Comparing `tmp/types-aiobotocore-lex-models-2.9.0.tar.gz` & `tmp/types-aiobotocore-lex-models-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-lex-models-2.9.0.tar", last modified: Wed Dec 13 19:59:43 2023, max compression
+gzip compressed data, was "types-aiobotocore-lex-models-2.9.1.tar", last modified: Thu Jan 18 01:21:06 2024, max compression
```

## Comparing `types-aiobotocore-lex-models-2.9.0.tar` & `types-aiobotocore-lex-models-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:43.697542 types-aiobotocore-lex-models-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:48:51.000000 types-aiobotocore-lex-models-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14527 2023-12-13 19:59:43.697542 types-aiobotocore-lex-models-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12939 2023-12-13 19:48:51.000000 types-aiobotocore-lex-models-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:43.697542 types-aiobotocore-lex-models-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2023-12-13 19:48:50.000000 types-aiobotocore-lex-models-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:43.697542 types-aiobotocore-lex-models-2.9.0/types_aiobotocore_lex_models/
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2023-12-13 19:48:51.000000 types-aiobotocore-lex-models-2.9.0/types_aiobotocore_lex_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2023-12-13 19:48:51.000000 types-aiobotocore-lex-models-2.9.0/types_aiobotocore_lex_models/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      970 2023-12-13 19:48:51.000000 types-aiobotocore-lex-models-2.9.0/types_aiobotocore_lex_models/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37367 2023-12-13 19:48:52.000000 types-aiobotocore-lex-models-2.9.0/types_aiobotocore_lex_models/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    37363 2023-12-13 19:48:52.000000 types-aiobotocore-lex-models-2.9.0/types_aiobotocore_lex_models/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11718 2023-12-13 19:48:53.000000 types-aiobotocore-lex-models-2.9.0/types_aiobotocore_lex_models/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11716 2023-12-13 19:48:53.000000 types-aiobotocore-lex-models-2.9.0/types_aiobotocore_lex_models/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12668 2023-12-13 19:48:52.000000 types-aiobotocore-lex-models-2.9.0/types_aiobotocore_lex_models/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12656 2023-12-13 19:48:52.000000 types-aiobotocore-lex-models-2.9.0/types_aiobotocore_lex_models/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:48:51.000000 types-aiobotocore-lex-models-2.9.0/types_aiobotocore_lex_models/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    39800 2023-12-13 19:48:53.000000 types-aiobotocore-lex-models-2.9.0/types_aiobotocore_lex_models/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    39799 2023-12-13 19:48:53.000000 types-aiobotocore-lex-models-2.9.0/types_aiobotocore_lex_models/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:48:51.000000 types-aiobotocore-lex-models-2.9.0/types_aiobotocore_lex_models/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:43.697542 types-aiobotocore-lex-models-2.9.0/types_aiobotocore_lex_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14527 2023-12-13 19:59:43.000000 types-aiobotocore-lex-models-2.9.0/types_aiobotocore_lex_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      870 2023-12-13 19:59:43.000000 types-aiobotocore-lex-models-2.9.0/types_aiobotocore_lex_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:43.000000 types-aiobotocore-lex-models-2.9.0/types_aiobotocore_lex_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:43.000000 types-aiobotocore-lex-models-2.9.0/types_aiobotocore_lex_models.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:43.000000 types-aiobotocore-lex-models-2.9.0/types_aiobotocore_lex_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-13 19:59:43.000000 types-aiobotocore-lex-models-2.9.0/types_aiobotocore_lex_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:06.333226 types-aiobotocore-lex-models-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:10:38.000000 types-aiobotocore-lex-models-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14547 2024-01-18 01:21:06.333226 types-aiobotocore-lex-models-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12939 2024-01-18 01:10:38.000000 types-aiobotocore-lex-models-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:06.333226 types-aiobotocore-lex-models-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-01-18 01:10:38.000000 types-aiobotocore-lex-models-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:06.333226 types-aiobotocore-lex-models-2.9.1/types_aiobotocore_lex_models/
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-01-18 01:10:38.000000 types-aiobotocore-lex-models-2.9.1/types_aiobotocore_lex_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-01-18 01:10:38.000000 types-aiobotocore-lex-models-2.9.1/types_aiobotocore_lex_models/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-01-18 01:10:38.000000 types-aiobotocore-lex-models-2.9.1/types_aiobotocore_lex_models/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37376 2024-01-18 01:10:38.000000 types-aiobotocore-lex-models-2.9.1/types_aiobotocore_lex_models/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37373 2024-01-18 01:10:38.000000 types-aiobotocore-lex-models-2.9.1/types_aiobotocore_lex_models/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11716 2024-01-18 01:10:38.000000 types-aiobotocore-lex-models-2.9.1/types_aiobotocore_lex_models/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11716 2024-01-18 01:10:38.000000 types-aiobotocore-lex-models-2.9.1/types_aiobotocore_lex_models/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12671 2024-01-18 01:10:38.000000 types-aiobotocore-lex-models-2.9.1/types_aiobotocore_lex_models/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12660 2024-01-18 01:10:38.000000 types-aiobotocore-lex-models-2.9.1/types_aiobotocore_lex_models/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:10:38.000000 types-aiobotocore-lex-models-2.9.1/types_aiobotocore_lex_models/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    39799 2024-01-18 01:10:39.000000 types-aiobotocore-lex-models-2.9.1/types_aiobotocore_lex_models/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39799 2024-01-18 01:10:39.000000 types-aiobotocore-lex-models-2.9.1/types_aiobotocore_lex_models/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:10:38.000000 types-aiobotocore-lex-models-2.9.1/types_aiobotocore_lex_models/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:06.333226 types-aiobotocore-lex-models-2.9.1/types_aiobotocore_lex_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14547 2024-01-18 01:21:06.000000 types-aiobotocore-lex-models-2.9.1/types_aiobotocore_lex_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-01-18 01:21:06.000000 types-aiobotocore-lex-models-2.9.1/types_aiobotocore_lex_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:06.000000 types-aiobotocore-lex-models-2.9.1/types_aiobotocore_lex_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:06.000000 types-aiobotocore-lex-models-2.9.1/types_aiobotocore_lex_models.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:06.000000 types-aiobotocore-lex-models-2.9.1/types_aiobotocore_lex_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-01-18 01:21:06.000000 types-aiobotocore-lex-models-2.9.1/types_aiobotocore_lex_models.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-lex-models-2.9.0/LICENSE` & `types-aiobotocore-lex-models-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-lex-models-2.9.0/PKG-INFO` & `types-aiobotocore-lex-models-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-lex-models
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.LexModelBuildingService 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.LexModelBuildingService 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/
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
 
 <a id="types-aiobotocore-lex-models"></a>
 
 # types-aiobotocore-lex-models
 
 [![PyPI - types-aiobotocore-lex-models](https://img.shields.io/pypi/v/types-aiobotocore-lex-models.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lex-models)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lex-models.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lex-models)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lex-models)](https://pepy.tech/project/types-aiobotocore-lex-models)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LexModelBuildingService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService)
+[aiobotocore.LexModelBuildingService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService)
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
 [types-aiobotocore-lex-models docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-lex-models-2.9.0/README.md` & `types-aiobotocore-lex-models-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lex-models.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lex-models)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lex-models)](https://pepy.tech/project/types-aiobotocore-lex-models)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LexModelBuildingService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService)
+[aiobotocore.LexModelBuildingService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService)
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
 [types-aiobotocore-lex-models docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-lex-models-2.9.0/setup.py` & `types-aiobotocore-lex-models-2.9.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-lex-models",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_lex_models"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.LexModelBuildingService 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.LexModelBuildingService 2.9.1 service generated with"
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
     keywords="aiobotocore lex-models type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_lex_models": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-lex-models-2.9.0/types_aiobotocore_lex_models/__init__.py` & `types-aiobotocore-lex-models-2.9.1/types_aiobotocore_lex_models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,14 @@
     GetIntentVersionsPaginator,
     GetSlotTypesPaginator,
     GetSlotTypeVersionsPaginator,
 )
 
 Client = LexModelBuildingServiceClient
 
-
 __all__ = (
     "Client",
     "GetBotAliasesPaginator",
     "GetBotChannelAssociationsPaginator",
     "GetBotVersionsPaginator",
     "GetBotsPaginator",
     "GetBuiltinIntentsPaginator",
```

### Comparing `types-aiobotocore-lex-models-2.9.0/types_aiobotocore_lex_models/__init__.pyi` & `types-aiobotocore-lex-models-2.9.1/types_aiobotocore_lex_models/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-models-2.9.0/types_aiobotocore_lex_models/__main__.py` & `types-aiobotocore-lex-models-2.9.1/types_aiobotocore_lex_models/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.LexModelBuildingService 2.9.0\nVersion:        "
-        " 2.9.0\nBuilder version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.LexModelBuildingService 2.9.1\nVersion:        "
+        " 2.9.1\nBuilder version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService\nOther"
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

### Comparing `types-aiobotocore-lex-models-2.9.0/types_aiobotocore_lex_models/client.py` & `types-aiobotocore-lex-models-2.9.1/types_aiobotocore_lex_models/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("LexModelBuildingServiceClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -323,15 +322,15 @@
     async def get_bot_channel_associations(
         self,
         *,
         botName: str,
         botAlias: str,
         nextToken: str = ...,
         maxResults: int = ...,
-        nameContains: str = ...
+        nameContains: str = ...,
     ) -> GetBotChannelAssociationsResponseTypeDef:
         """
         Returns a list of all of the channels associated with the specified bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Client.get_bot_channel_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/client/#get_bot_channel_associations)
         """
@@ -369,30 +368,30 @@
 
     async def get_builtin_intents(
         self,
         *,
         locale: LocaleType = ...,
         signatureContains: str = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> GetBuiltinIntentsResponseTypeDef:
         """
         Gets a list of built-in intents that meet the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Client.get_builtin_intents)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/client/#get_builtin_intents)
         """
 
     async def get_builtin_slot_types(
         self,
         *,
         locale: LocaleType = ...,
         signatureContains: str = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> GetBuiltinSlotTypesResponseTypeDef:
         """
         Gets a list of built-in slot types that meet the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Client.get_builtin_slot_types)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/client/#get_builtin_slot_types)
         """
@@ -459,15 +458,15 @@
         self,
         *,
         sortByAttribute: MigrationSortAttributeType = ...,
         sortByOrder: SortOrderType = ...,
         v1BotNameContains: str = ...,
         migrationStatusEquals: MigrationStatusType = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> GetMigrationsResponseTypeDef:
         """
         Gets a list of migrations between Amazon Lex V1 and Amazon Lex V2.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Client.get_migrations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/client/#get_migrations)
         """
@@ -539,15 +538,15 @@
         abortStatement: StatementTypeDef = ...,
         idleSessionTTLInSeconds: int = ...,
         voiceId: str = ...,
         checksum: str = ...,
         processBehavior: ProcessBehaviorType = ...,
         detectSentiment: bool = ...,
         createVersion: bool = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> PutBotResponseTypeDef:
         """
         Creates an Amazon Lex conversational bot or replaces an existing bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Client.put_bot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/client/#put_bot)
         """
@@ -557,15 +556,15 @@
         *,
         name: str,
         botVersion: str,
         botName: str,
         description: str = ...,
         checksum: str = ...,
         conversationLogs: ConversationLogsRequestTypeDef = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> PutBotAliasResponseTypeDef:
         """
         Creates an alias for the specified version of the bot or replaces an alias for
         the specified
         bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Client.put_bot_alias)
@@ -586,15 +585,15 @@
         dialogCodeHook: CodeHookTypeDef = ...,
         fulfillmentActivity: FulfillmentActivityTypeDef = ...,
         parentIntentSignature: str = ...,
         checksum: str = ...,
         createVersion: bool = ...,
         kendraConfiguration: KendraConfigurationTypeDef = ...,
         inputContexts: Sequence[InputContextTypeDef] = ...,
-        outputContexts: Sequence[OutputContextTypeDef] = ...
+        outputContexts: Sequence[OutputContextTypeDef] = ...,
     ) -> PutIntentResponseTypeDef:
         """
         Creates an intent or replaces an existing intent.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Client.put_intent)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/client/#put_intent)
         """
@@ -605,30 +604,30 @@
         name: str,
         description: str = ...,
         enumerationValues: Sequence[EnumerationValueTypeDef] = ...,
         checksum: str = ...,
         valueSelectionStrategy: SlotValueSelectionStrategyType = ...,
         createVersion: bool = ...,
         parentSlotTypeSignature: str = ...,
-        slotTypeConfigurations: Sequence[SlotTypeConfigurationTypeDef] = ...
+        slotTypeConfigurations: Sequence[SlotTypeConfigurationTypeDef] = ...,
     ) -> PutSlotTypeResponseTypeDef:
         """
         Creates a custom slot type or replaces an existing custom slot type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Client.put_slot_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/client/#put_slot_type)
         """
 
     async def start_import(
         self,
         *,
         payload: BlobTypeDef,
         resourceType: ResourceTypeType,
         mergeStrategy: MergeStrategyType,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> StartImportResponseTypeDef:
         """
         Starts a job to import a resource to Amazon Lex.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Client.start_import)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/client/#start_import)
         """
@@ -636,15 +635,15 @@
     async def start_migration(
         self,
         *,
         v1BotName: str,
         v1BotVersion: str,
         v2BotName: str,
         v2BotRole: str,
-        migrationStrategy: MigrationStrategyType
+        migrationStrategy: MigrationStrategyType,
     ) -> StartMigrationResponseTypeDef:
         """
         Starts migrating a bot from Amazon Lex V1 to Amazon Lex V2.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Client.start_migration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/client/#start_migration)
         """
```

### Comparing `types-aiobotocore-lex-models-2.9.0/types_aiobotocore_lex_models/client.pyi` & `types-aiobotocore-lex-models-2.9.1/types_aiobotocore_lex_models/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -319,15 +319,15 @@
     async def get_bot_channel_associations(
         self,
         *,
         botName: str,
         botAlias: str,
         nextToken: str = ...,
         maxResults: int = ...,
-        nameContains: str = ...
+        nameContains: str = ...,
     ) -> GetBotChannelAssociationsResponseTypeDef:
         """
         Returns a list of all of the channels associated with the specified bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Client.get_bot_channel_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/client/#get_bot_channel_associations)
         """
@@ -365,30 +365,30 @@
 
     async def get_builtin_intents(
         self,
         *,
         locale: LocaleType = ...,
         signatureContains: str = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> GetBuiltinIntentsResponseTypeDef:
         """
         Gets a list of built-in intents that meet the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Client.get_builtin_intents)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/client/#get_builtin_intents)
         """
 
     async def get_builtin_slot_types(
         self,
         *,
         locale: LocaleType = ...,
         signatureContains: str = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> GetBuiltinSlotTypesResponseTypeDef:
         """
         Gets a list of built-in slot types that meet the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Client.get_builtin_slot_types)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/client/#get_builtin_slot_types)
         """
@@ -455,15 +455,15 @@
         self,
         *,
         sortByAttribute: MigrationSortAttributeType = ...,
         sortByOrder: SortOrderType = ...,
         v1BotNameContains: str = ...,
         migrationStatusEquals: MigrationStatusType = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> GetMigrationsResponseTypeDef:
         """
         Gets a list of migrations between Amazon Lex V1 and Amazon Lex V2.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Client.get_migrations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/client/#get_migrations)
         """
@@ -535,15 +535,15 @@
         abortStatement: StatementTypeDef = ...,
         idleSessionTTLInSeconds: int = ...,
         voiceId: str = ...,
         checksum: str = ...,
         processBehavior: ProcessBehaviorType = ...,
         detectSentiment: bool = ...,
         createVersion: bool = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> PutBotResponseTypeDef:
         """
         Creates an Amazon Lex conversational bot or replaces an existing bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Client.put_bot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/client/#put_bot)
         """
@@ -553,15 +553,15 @@
         *,
         name: str,
         botVersion: str,
         botName: str,
         description: str = ...,
         checksum: str = ...,
         conversationLogs: ConversationLogsRequestTypeDef = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> PutBotAliasResponseTypeDef:
         """
         Creates an alias for the specified version of the bot or replaces an alias for
         the specified
         bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Client.put_bot_alias)
@@ -582,15 +582,15 @@
         dialogCodeHook: CodeHookTypeDef = ...,
         fulfillmentActivity: FulfillmentActivityTypeDef = ...,
         parentIntentSignature: str = ...,
         checksum: str = ...,
         createVersion: bool = ...,
         kendraConfiguration: KendraConfigurationTypeDef = ...,
         inputContexts: Sequence[InputContextTypeDef] = ...,
-        outputContexts: Sequence[OutputContextTypeDef] = ...
+        outputContexts: Sequence[OutputContextTypeDef] = ...,
     ) -> PutIntentResponseTypeDef:
         """
         Creates an intent or replaces an existing intent.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Client.put_intent)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/client/#put_intent)
         """
@@ -601,30 +601,30 @@
         name: str,
         description: str = ...,
         enumerationValues: Sequence[EnumerationValueTypeDef] = ...,
         checksum: str = ...,
         valueSelectionStrategy: SlotValueSelectionStrategyType = ...,
         createVersion: bool = ...,
         parentSlotTypeSignature: str = ...,
-        slotTypeConfigurations: Sequence[SlotTypeConfigurationTypeDef] = ...
+        slotTypeConfigurations: Sequence[SlotTypeConfigurationTypeDef] = ...,
     ) -> PutSlotTypeResponseTypeDef:
         """
         Creates a custom slot type or replaces an existing custom slot type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Client.put_slot_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/client/#put_slot_type)
         """
 
     async def start_import(
         self,
         *,
         payload: BlobTypeDef,
         resourceType: ResourceTypeType,
         mergeStrategy: MergeStrategyType,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> StartImportResponseTypeDef:
         """
         Starts a job to import a resource to Amazon Lex.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Client.start_import)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/client/#start_import)
         """
@@ -632,15 +632,15 @@
     async def start_migration(
         self,
         *,
         v1BotName: str,
         v1BotVersion: str,
         v2BotName: str,
         v2BotRole: str,
-        migrationStrategy: MigrationStrategyType
+        migrationStrategy: MigrationStrategyType,
     ) -> StartMigrationResponseTypeDef:
         """
         Starts migrating a bot from Amazon Lex V1 to Amazon Lex V2.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Client.start_migration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/client/#start_migration)
         """
```

### Comparing `types-aiobotocore-lex-models-2.9.0/types_aiobotocore_lex_models/literals.py` & `types-aiobotocore-lex-models-2.9.1/types_aiobotocore_lex_models/literals.py`

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
     "ChannelStatusType",
     "ChannelTypeType",
     "ContentTypeType",
     "DestinationType",
     "ExportStatusType",
     "ExportTypeType",
@@ -57,15 +56,14 @@
     "LexModelBuildingServiceServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ChannelStatusType = Literal["CREATED", "FAILED", "IN_PROGRESS"]
 ChannelTypeType = Literal["Facebook", "Kik", "Slack", "Twilio-Sms"]
 ContentTypeType = Literal["CustomPayload", "PlainText", "SSML"]
 DestinationType = Literal["CLOUDWATCH_LOGS", "S3"]
 ExportStatusType = Literal["FAILED", "IN_PROGRESS", "READY"]
 ExportTypeType = Literal["ALEXA_SKILLS_KIT", "LEX"]
 FulfillmentActivityTypeType = Literal["CodeHook", "ReturnIntent"]
```

### Comparing `types-aiobotocore-lex-models-2.9.0/types_aiobotocore_lex_models/literals.pyi` & `types-aiobotocore-lex-models-2.9.1/types_aiobotocore_lex_models/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-models-2.9.0/types_aiobotocore_lex_models/paginator.py` & `types-aiobotocore-lex-models-2.9.1/types_aiobotocore_lex_models/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,14 @@
     "GetBuiltinSlotTypesPaginator",
     "GetIntentVersionsPaginator",
     "GetIntentsPaginator",
     "GetSlotTypeVersionsPaginator",
     "GetSlotTypesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -90,15 +89,15 @@
     """
 
     def paginate(
         self,
         *,
         botName: str,
         nameContains: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetBotAliasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBotAliases.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/paginators/#getbotaliasespaginator)
         """
 
 
@@ -110,15 +109,15 @@
 
     def paginate(
         self,
         *,
         botName: str,
         botAlias: str,
         nameContains: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetBotChannelAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBotChannelAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/paginators/#getbotchannelassociationspaginator)
         """
 
 
@@ -159,15 +158,15 @@
     """
 
     def paginate(
         self,
         *,
         locale: LocaleType = ...,
         signatureContains: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetBuiltinIntentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBuiltinIntents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/paginators/#getbuiltinintentspaginator)
         """
 
 
@@ -178,15 +177,15 @@
     """
 
     def paginate(
         self,
         *,
         locale: LocaleType = ...,
         signatureContains: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetBuiltinSlotTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBuiltinSlotTypes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/paginators/#getbuiltinslottypespaginator)
         """
```

### Comparing `types-aiobotocore-lex-models-2.9.0/types_aiobotocore_lex_models/paginator.pyi` & `types-aiobotocore-lex-models-2.9.1/types_aiobotocore_lex_models/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
     """
 
     def paginate(
         self,
         *,
         botName: str,
         nameContains: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetBotAliasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBotAliases.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/paginators/#getbotaliasespaginator)
         """
 
 class GetBotChannelAssociationsPaginator(AioPaginator):
@@ -106,15 +106,15 @@
 
     def paginate(
         self,
         *,
         botName: str,
         botAlias: str,
         nameContains: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetBotChannelAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBotChannelAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/paginators/#getbotchannelassociationspaginator)
         """
 
 class GetBotVersionsPaginator(AioPaginator):
@@ -152,15 +152,15 @@
     """
 
     def paginate(
         self,
         *,
         locale: LocaleType = ...,
         signatureContains: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetBuiltinIntentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBuiltinIntents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/paginators/#getbuiltinintentspaginator)
         """
 
 class GetBuiltinSlotTypesPaginator(AioPaginator):
@@ -170,15 +170,15 @@
     """
 
     def paginate(
         self,
         *,
         locale: LocaleType = ...,
         signatureContains: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetBuiltinSlotTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBuiltinSlotTypes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/paginators/#getbuiltinslottypespaginator)
         """
 
 class GetIntentVersionsPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-lex-models-2.9.0/types_aiobotocore_lex_models/type_defs.py` & `types-aiobotocore-lex-models-2.9.1/types_aiobotocore_lex_models/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "BlobTypeDef",
     "BotChannelAssociationTypeDef",
     "BotMetadataTypeDef",
     "BuiltinIntentMetadataTypeDef",
     "BuiltinIntentSlotTypeDef",
     "BuiltinSlotTypeMetadataTypeDef",
```

### Comparing `types-aiobotocore-lex-models-2.9.0/types_aiobotocore_lex_models/type_defs.pyi` & `types-aiobotocore-lex-models-2.9.1/types_aiobotocore_lex_models/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-models-2.9.0/types_aiobotocore_lex_models.egg-info/PKG-INFO` & `types-aiobotocore-lex-models-2.9.1/types_aiobotocore_lex_models.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-lex-models
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.LexModelBuildingService 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.LexModelBuildingService 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/
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
 
 <a id="types-aiobotocore-lex-models"></a>
 
 # types-aiobotocore-lex-models
 
 [![PyPI - types-aiobotocore-lex-models](https://img.shields.io/pypi/v/types-aiobotocore-lex-models.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lex-models)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lex-models.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lex-models)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lex-models)](https://pepy.tech/project/types-aiobotocore-lex-models)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LexModelBuildingService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService)
+[aiobotocore.LexModelBuildingService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService)
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
 [types-aiobotocore-lex-models docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-lex-models-2.9.0/types_aiobotocore_lex_models.egg-info/SOURCES.txt` & `types-aiobotocore-lex-models-2.9.1/types_aiobotocore_lex_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

