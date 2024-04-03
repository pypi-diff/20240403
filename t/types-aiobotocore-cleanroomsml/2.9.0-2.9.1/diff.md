# Comparing `tmp/types-aiobotocore-cleanroomsml-2.9.0.tar.gz` & `tmp/types-aiobotocore-cleanroomsml-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cleanroomsml-2.9.0.tar", last modified: Wed Dec 13 19:58:47 2023, max compression
+gzip compressed data, was "types-aiobotocore-cleanroomsml-2.9.1.tar", last modified: Thu Jan 18 01:20:14 2024, max compression
```

## Comparing `types-aiobotocore-cleanroomsml-2.9.0.tar` & `types-aiobotocore-cleanroomsml-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:47.349990 types-aiobotocore-cleanroomsml-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:42:11.000000 types-aiobotocore-cleanroomsml-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14026 2023-12-13 19:58:47.349990 types-aiobotocore-cleanroomsml-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12443 2023-12-13 19:42:11.000000 types-aiobotocore-cleanroomsml-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:47.349990 types-aiobotocore-cleanroomsml-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2023-12-13 19:42:11.000000 types-aiobotocore-cleanroomsml-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:47.349990 types-aiobotocore-cleanroomsml-2.9.0/types_aiobotocore_cleanroomsml/
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2023-12-13 19:42:11.000000 types-aiobotocore-cleanroomsml-2.9.0/types_aiobotocore_cleanroomsml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2023-12-13 19:42:11.000000 types-aiobotocore-cleanroomsml-2.9.0/types_aiobotocore_cleanroomsml/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      952 2023-12-13 19:42:11.000000 types-aiobotocore-cleanroomsml-2.9.0/types_aiobotocore_cleanroomsml/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24126 2023-12-13 19:42:11.000000 types-aiobotocore-cleanroomsml-2.9.0/types_aiobotocore_cleanroomsml/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    24122 2023-12-13 19:42:11.000000 types-aiobotocore-cleanroomsml-2.9.0/types_aiobotocore_cleanroomsml/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10473 2023-12-13 19:42:11.000000 types-aiobotocore-cleanroomsml-2.9.0/types_aiobotocore_cleanroomsml/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10471 2023-12-13 19:42:11.000000 types-aiobotocore-cleanroomsml-2.9.0/types_aiobotocore_cleanroomsml/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7096 2023-12-13 19:42:11.000000 types-aiobotocore-cleanroomsml-2.9.0/types_aiobotocore_cleanroomsml/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7089 2023-12-13 19:42:11.000000 types-aiobotocore-cleanroomsml-2.9.0/types_aiobotocore_cleanroomsml/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:42:11.000000 types-aiobotocore-cleanroomsml-2.9.0/types_aiobotocore_cleanroomsml/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    22522 2023-12-13 19:42:12.000000 types-aiobotocore-cleanroomsml-2.9.0/types_aiobotocore_cleanroomsml/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    22521 2023-12-13 19:42:12.000000 types-aiobotocore-cleanroomsml-2.9.0/types_aiobotocore_cleanroomsml/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:42:11.000000 types-aiobotocore-cleanroomsml-2.9.0/types_aiobotocore_cleanroomsml/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:47.349990 types-aiobotocore-cleanroomsml-2.9.0/types_aiobotocore_cleanroomsml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14026 2023-12-13 19:58:47.000000 types-aiobotocore-cleanroomsml-2.9.0/types_aiobotocore_cleanroomsml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      908 2023-12-13 19:58:47.000000 types-aiobotocore-cleanroomsml-2.9.0/types_aiobotocore_cleanroomsml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:47.000000 types-aiobotocore-cleanroomsml-2.9.0/types_aiobotocore_cleanroomsml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:47.000000 types-aiobotocore-cleanroomsml-2.9.0/types_aiobotocore_cleanroomsml.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:47.000000 types-aiobotocore-cleanroomsml-2.9.0/types_aiobotocore_cleanroomsml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-13 19:58:47.000000 types-aiobotocore-cleanroomsml-2.9.0/types_aiobotocore_cleanroomsml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:14.285471 types-aiobotocore-cleanroomsml-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:04:08.000000 types-aiobotocore-cleanroomsml-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14046 2024-01-18 01:20:14.285471 types-aiobotocore-cleanroomsml-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12443 2024-01-18 01:04:08.000000 types-aiobotocore-cleanroomsml-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:14.285471 types-aiobotocore-cleanroomsml-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-01-18 01:04:08.000000 types-aiobotocore-cleanroomsml-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:14.285471 types-aiobotocore-cleanroomsml-2.9.1/types_aiobotocore_cleanroomsml/
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-01-18 01:04:08.000000 types-aiobotocore-cleanroomsml-2.9.1/types_aiobotocore_cleanroomsml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-01-18 01:04:08.000000 types-aiobotocore-cleanroomsml-2.9.1/types_aiobotocore_cleanroomsml/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-01-18 01:04:08.000000 types-aiobotocore-cleanroomsml-2.9.1/types_aiobotocore_cleanroomsml/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24133 2024-01-18 01:04:09.000000 types-aiobotocore-cleanroomsml-2.9.1/types_aiobotocore_cleanroomsml/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24130 2024-01-18 01:04:09.000000 types-aiobotocore-cleanroomsml-2.9.1/types_aiobotocore_cleanroomsml/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-01-18 01:04:09.000000 types-aiobotocore-cleanroomsml-2.9.1/types_aiobotocore_cleanroomsml/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-01-18 01:04:09.000000 types-aiobotocore-cleanroomsml-2.9.1/types_aiobotocore_cleanroomsml/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7096 2024-01-18 01:04:09.000000 types-aiobotocore-cleanroomsml-2.9.1/types_aiobotocore_cleanroomsml/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7090 2024-01-18 01:04:09.000000 types-aiobotocore-cleanroomsml-2.9.1/types_aiobotocore_cleanroomsml/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:04:08.000000 types-aiobotocore-cleanroomsml-2.9.1/types_aiobotocore_cleanroomsml/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    22521 2024-01-18 01:04:09.000000 types-aiobotocore-cleanroomsml-2.9.1/types_aiobotocore_cleanroomsml/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22521 2024-01-18 01:04:09.000000 types-aiobotocore-cleanroomsml-2.9.1/types_aiobotocore_cleanroomsml/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:04:08.000000 types-aiobotocore-cleanroomsml-2.9.1/types_aiobotocore_cleanroomsml/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:14.285471 types-aiobotocore-cleanroomsml-2.9.1/types_aiobotocore_cleanroomsml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14046 2024-01-18 01:20:14.000000 types-aiobotocore-cleanroomsml-2.9.1/types_aiobotocore_cleanroomsml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-01-18 01:20:14.000000 types-aiobotocore-cleanroomsml-2.9.1/types_aiobotocore_cleanroomsml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:14.000000 types-aiobotocore-cleanroomsml-2.9.1/types_aiobotocore_cleanroomsml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:14.000000 types-aiobotocore-cleanroomsml-2.9.1/types_aiobotocore_cleanroomsml.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:14.000000 types-aiobotocore-cleanroomsml-2.9.1/types_aiobotocore_cleanroomsml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-01-18 01:20:14.000000 types-aiobotocore-cleanroomsml-2.9.1/types_aiobotocore_cleanroomsml.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cleanroomsml-2.9.0/LICENSE` & `types-aiobotocore-cleanroomsml-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-cleanroomsml-2.9.0/PKG-INFO` & `types-aiobotocore-cleanroomsml-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cleanroomsml
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CleanRoomsML 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CleanRoomsML 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanroomsml/
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
 
 <a id="types-aiobotocore-cleanroomsml"></a>
 
 # types-aiobotocore-cleanroomsml
 
 [![PyPI - types-aiobotocore-cleanroomsml](https://img.shields.io/pypi/v/types-aiobotocore-cleanroomsml.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cleanroomsml)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cleanroomsml.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cleanroomsml)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanroomsml/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cleanroomsml)](https://pepy.tech/project/types-aiobotocore-cleanroomsml)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CleanRoomsML 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML)
+[aiobotocore.CleanRoomsML 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML)
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
 [types-aiobotocore-cleanroomsml docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanroomsml/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-cleanroomsml-2.9.0/README.md` & `types-aiobotocore-cleanroomsml-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cleanroomsml.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cleanroomsml)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanroomsml/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cleanroomsml)](https://pepy.tech/project/types-aiobotocore-cleanroomsml)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CleanRoomsML 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML)
+[aiobotocore.CleanRoomsML 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML)
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
 [types-aiobotocore-cleanroomsml docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanroomsml/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-cleanroomsml-2.9.0/setup.py` & `types-aiobotocore-cleanroomsml-2.9.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cleanroomsml",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_cleanroomsml"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CleanRoomsML 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.CleanRoomsML 2.9.1 service generated with"
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
     keywords="aiobotocore cleanroomsml type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_cleanroomsml": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanroomsml/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-cleanroomsml-2.9.0/types_aiobotocore_cleanroomsml/__init__.py` & `types-aiobotocore-cleanroomsml-2.9.1/types_aiobotocore_cleanroomsml/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     ListAudienceModelsPaginator,
     ListConfiguredAudienceModelsPaginator,
     ListTrainingDatasetsPaginator,
 )
 
 Client = CleanRoomsMLClient
 
-
 __all__ = (
     "CleanRoomsMLClient",
     "Client",
     "ListAudienceExportJobsPaginator",
     "ListAudienceGenerationJobsPaginator",
     "ListAudienceModelsPaginator",
     "ListConfiguredAudienceModelsPaginator",
```

### Comparing `types-aiobotocore-cleanroomsml-2.9.0/types_aiobotocore_cleanroomsml/__init__.pyi` & `types-aiobotocore-cleanroomsml-2.9.1/types_aiobotocore_cleanroomsml/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cleanroomsml-2.9.0/types_aiobotocore_cleanroomsml/__main__.py` & `types-aiobotocore-cleanroomsml-2.9.1/types_aiobotocore_cleanroomsml/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CleanRoomsML 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.CleanRoomsML 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanroomsml//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML\nOther"
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

### Comparing `types-aiobotocore-cleanroomsml-2.9.0/types_aiobotocore_cleanroomsml/client.py` & `types-aiobotocore-cleanroomsml-2.9.1/types_aiobotocore_cleanroomsml/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("CleanRoomsMLClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -120,15 +119,15 @@
         *,
         name: str,
         trainingDatasetArn: str,
         description: str = ...,
         kmsKeyArn: str = ...,
         tags: Mapping[str, str] = ...,
         trainingDataEndTime: TimestampTypeDef = ...,
-        trainingDataStartTime: TimestampTypeDef = ...
+        trainingDataStartTime: TimestampTypeDef = ...,
     ) -> CreateAudienceModelResponseTypeDef:
         """
         Defines the information necessary to create an audience model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.create_audience_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanroomsml/client/#create_audience_model)
         """
@@ -140,15 +139,15 @@
         name: str,
         outputConfig: ConfiguredAudienceModelOutputConfigTypeDef,
         sharedAudienceMetrics: Sequence[SharedAudienceMetricsType],
         audienceSizeConfig: AudienceSizeConfigTypeDef = ...,
         childResourceTagOnCreatePolicy: TagOnCreatePolicyType = ...,
         description: str = ...,
         minMatchingSeedSize: int = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateConfiguredAudienceModelResponseTypeDef:
         """
         Defines the information necessary to create a configured audience model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.create_configured_audience_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanroomsml/client/#create_configured_audience_model)
         """
@@ -156,15 +155,15 @@
     async def create_training_dataset(
         self,
         *,
         name: str,
         roleArn: str,
         trainingData: Sequence[DatasetTypeDef],
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateTrainingDatasetResponseTypeDef:
         """
         Defines the information necessary to create a training dataset, or seed
         audience.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.create_training_dataset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanroomsml/client/#create_training_dataset)
@@ -295,15 +294,15 @@
 
     async def list_audience_generation_jobs(
         self,
         *,
         collaborationId: str = ...,
         configuredAudienceModelArn: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListAudienceGenerationJobsResponseTypeDef:
         """
         Returns a list of audience generation jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.list_audience_generation_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanroomsml/client/#list_audience_generation_jobs)
         """
@@ -350,30 +349,30 @@
 
     async def put_configured_audience_model_policy(
         self,
         *,
         configuredAudienceModelArn: str,
         configuredAudienceModelPolicy: str,
         policyExistenceCondition: PolicyExistenceConditionType = ...,
-        previousPolicyHash: str = ...
+        previousPolicyHash: str = ...,
     ) -> PutConfiguredAudienceModelPolicyResponseTypeDef:
         """
         Create or update the resource policy for a configured audience model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.put_configured_audience_model_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanroomsml/client/#put_configured_audience_model_policy)
         """
 
     async def start_audience_export_job(
         self,
         *,
         audienceGenerationJobArn: str,
         audienceSize: AudienceSizeTypeDef,
         name: str,
-        description: str = ...
+        description: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Export an audience of a specified size after you have generated an audience.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.start_audience_export_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanroomsml/client/#start_audience_export_job)
         """
@@ -383,15 +382,15 @@
         *,
         configuredAudienceModelArn: str,
         name: str,
         seedAudience: AudienceGenerationJobDataSourceTypeDef,
         collaborationId: str = ...,
         description: str = ...,
         includeSeedInOutput: bool = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> StartAudienceGenerationJobResponseTypeDef:
         """
         Information necessary to start the audience generation job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.start_audience_generation_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanroomsml/client/#start_audience_generation_job)
         """
@@ -417,15 +416,15 @@
         *,
         configuredAudienceModelArn: str,
         audienceModelArn: str = ...,
         audienceSizeConfig: AudienceSizeConfigTypeDef = ...,
         description: str = ...,
         minMatchingSeedSize: int = ...,
         outputConfig: ConfiguredAudienceModelOutputConfigTypeDef = ...,
-        sharedAudienceMetrics: Sequence[SharedAudienceMetricsType] = ...
+        sharedAudienceMetrics: Sequence[SharedAudienceMetricsType] = ...,
     ) -> UpdateConfiguredAudienceModelResponseTypeDef:
         """
         Provides the information necessary to update a configured audience model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.update_configured_audience_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanroomsml/client/#update_configured_audience_model)
         """
```

### Comparing `types-aiobotocore-cleanroomsml-2.9.0/types_aiobotocore_cleanroomsml/client.pyi` & `types-aiobotocore-cleanroomsml-2.9.1/types_aiobotocore_cleanroomsml/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,15 @@
         *,
         name: str,
         trainingDatasetArn: str,
         description: str = ...,
         kmsKeyArn: str = ...,
         tags: Mapping[str, str] = ...,
         trainingDataEndTime: TimestampTypeDef = ...,
-        trainingDataStartTime: TimestampTypeDef = ...
+        trainingDataStartTime: TimestampTypeDef = ...,
     ) -> CreateAudienceModelResponseTypeDef:
         """
         Defines the information necessary to create an audience model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.create_audience_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanroomsml/client/#create_audience_model)
         """
@@ -136,15 +136,15 @@
         name: str,
         outputConfig: ConfiguredAudienceModelOutputConfigTypeDef,
         sharedAudienceMetrics: Sequence[SharedAudienceMetricsType],
         audienceSizeConfig: AudienceSizeConfigTypeDef = ...,
         childResourceTagOnCreatePolicy: TagOnCreatePolicyType = ...,
         description: str = ...,
         minMatchingSeedSize: int = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateConfiguredAudienceModelResponseTypeDef:
         """
         Defines the information necessary to create a configured audience model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.create_configured_audience_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanroomsml/client/#create_configured_audience_model)
         """
@@ -152,15 +152,15 @@
     async def create_training_dataset(
         self,
         *,
         name: str,
         roleArn: str,
         trainingData: Sequence[DatasetTypeDef],
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateTrainingDatasetResponseTypeDef:
         """
         Defines the information necessary to create a training dataset, or seed
         audience.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.create_training_dataset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanroomsml/client/#create_training_dataset)
@@ -291,15 +291,15 @@
 
     async def list_audience_generation_jobs(
         self,
         *,
         collaborationId: str = ...,
         configuredAudienceModelArn: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListAudienceGenerationJobsResponseTypeDef:
         """
         Returns a list of audience generation jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.list_audience_generation_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanroomsml/client/#list_audience_generation_jobs)
         """
@@ -346,30 +346,30 @@
 
     async def put_configured_audience_model_policy(
         self,
         *,
         configuredAudienceModelArn: str,
         configuredAudienceModelPolicy: str,
         policyExistenceCondition: PolicyExistenceConditionType = ...,
-        previousPolicyHash: str = ...
+        previousPolicyHash: str = ...,
     ) -> PutConfiguredAudienceModelPolicyResponseTypeDef:
         """
         Create or update the resource policy for a configured audience model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.put_configured_audience_model_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanroomsml/client/#put_configured_audience_model_policy)
         """
 
     async def start_audience_export_job(
         self,
         *,
         audienceGenerationJobArn: str,
         audienceSize: AudienceSizeTypeDef,
         name: str,
-        description: str = ...
+        description: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Export an audience of a specified size after you have generated an audience.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.start_audience_export_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanroomsml/client/#start_audience_export_job)
         """
@@ -379,15 +379,15 @@
         *,
         configuredAudienceModelArn: str,
         name: str,
         seedAudience: AudienceGenerationJobDataSourceTypeDef,
         collaborationId: str = ...,
         description: str = ...,
         includeSeedInOutput: bool = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> StartAudienceGenerationJobResponseTypeDef:
         """
         Information necessary to start the audience generation job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.start_audience_generation_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanroomsml/client/#start_audience_generation_job)
         """
@@ -413,15 +413,15 @@
         *,
         configuredAudienceModelArn: str,
         audienceModelArn: str = ...,
         audienceSizeConfig: AudienceSizeConfigTypeDef = ...,
         description: str = ...,
         minMatchingSeedSize: int = ...,
         outputConfig: ConfiguredAudienceModelOutputConfigTypeDef = ...,
-        sharedAudienceMetrics: Sequence[SharedAudienceMetricsType] = ...
+        sharedAudienceMetrics: Sequence[SharedAudienceMetricsType] = ...,
     ) -> UpdateConfiguredAudienceModelResponseTypeDef:
         """
         Provides the information necessary to update a configured audience model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.update_configured_audience_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanroomsml/client/#update_configured_audience_model)
         """
```

### Comparing `types-aiobotocore-cleanroomsml-2.9.0/types_aiobotocore_cleanroomsml/literals.py` & `types-aiobotocore-cleanroomsml-2.9.1/types_aiobotocore_cleanroomsml/literals.py`

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
     "AudienceExportJobStatusType",
     "AudienceGenerationJobStatusType",
     "AudienceModelMetricTypeType",
     "AudienceModelStatusType",
     "AudienceSizeTypeType",
     "ColumnTypeType",
@@ -40,15 +39,14 @@
     "TrainingDatasetStatusType",
     "CleanRoomsMLServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 AudienceExportJobStatusType = Literal[
     "ACTIVE", "CREATE_FAILED", "CREATE_IN_PROGRESS", "CREATE_PENDING"
 ]
 AudienceGenerationJobStatusType = Literal[
     "ACTIVE",
     "CREATE_FAILED",
     "CREATE_IN_PROGRESS",
```

### Comparing `types-aiobotocore-cleanroomsml-2.9.0/types_aiobotocore_cleanroomsml/literals.pyi` & `types-aiobotocore-cleanroomsml-2.9.1/types_aiobotocore_cleanroomsml/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cleanroomsml-2.9.0/types_aiobotocore_cleanroomsml/paginator.py` & `types-aiobotocore-cleanroomsml-2.9.1/types_aiobotocore_cleanroomsml/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,14 @@
     "ListAudienceExportJobsPaginator",
     "ListAudienceGenerationJobsPaginator",
     "ListAudienceModelsPaginator",
     "ListConfiguredAudienceModelsPaginator",
     "ListTrainingDatasetsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -84,15 +83,15 @@
     """
 
     def paginate(
         self,
         *,
         collaborationId: str = ...,
         configuredAudienceModelArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAudienceGenerationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Paginator.ListAudienceGenerationJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanroomsml/paginators/#listaudiencegenerationjobspaginator)
         """
```

### Comparing `types-aiobotocore-cleanroomsml-2.9.0/types_aiobotocore_cleanroomsml/paginator.pyi` & `types-aiobotocore-cleanroomsml-2.9.1/types_aiobotocore_cleanroomsml/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     """
 
     def paginate(
         self,
         *,
         collaborationId: str = ...,
         configuredAudienceModelArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAudienceGenerationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Paginator.ListAudienceGenerationJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanroomsml/paginators/#listaudiencegenerationjobspaginator)
         """
 
 class ListAudienceModelsPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-cleanroomsml-2.9.0/types_aiobotocore_cleanroomsml/type_defs.py` & `types-aiobotocore-cleanroomsml-2.9.1/types_aiobotocore_cleanroomsml/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "S3ConfigMapTypeDef",
     "AudienceSizeTypeDef",
     "StatusDetailsTypeDef",
     "AudienceGenerationJobSummaryTypeDef",
     "AudienceModelMetricTypeDef",
     "AudienceModelSummaryTypeDef",
```

### Comparing `types-aiobotocore-cleanroomsml-2.9.0/types_aiobotocore_cleanroomsml/type_defs.pyi` & `types-aiobotocore-cleanroomsml-2.9.1/types_aiobotocore_cleanroomsml/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cleanroomsml-2.9.0/types_aiobotocore_cleanroomsml.egg-info/PKG-INFO` & `types-aiobotocore-cleanroomsml-2.9.1/types_aiobotocore_cleanroomsml.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cleanroomsml
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CleanRoomsML 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CleanRoomsML 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanroomsml/
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
 
 <a id="types-aiobotocore-cleanroomsml"></a>
 
 # types-aiobotocore-cleanroomsml
 
 [![PyPI - types-aiobotocore-cleanroomsml](https://img.shields.io/pypi/v/types-aiobotocore-cleanroomsml.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cleanroomsml)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cleanroomsml.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cleanroomsml)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanroomsml/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cleanroomsml)](https://pepy.tech/project/types-aiobotocore-cleanroomsml)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CleanRoomsML 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML)
+[aiobotocore.CleanRoomsML 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML)
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
 [types-aiobotocore-cleanroomsml docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanroomsml/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-cleanroomsml-2.9.0/types_aiobotocore_cleanroomsml.egg-info/SOURCES.txt` & `types-aiobotocore-cleanroomsml-2.9.1/types_aiobotocore_cleanroomsml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

