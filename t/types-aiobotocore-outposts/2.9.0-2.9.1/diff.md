# Comparing `tmp/types-aiobotocore-outposts-2.9.0.tar.gz` & `tmp/types-aiobotocore-outposts-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-outposts-2.9.0.tar", last modified: Wed Dec 13 20:00:05 2023, max compression
+gzip compressed data, was "types-aiobotocore-outposts-2.9.1.tar", last modified: Thu Jan 18 01:21:26 2024, max compression
```

## Comparing `types-aiobotocore-outposts-2.9.0.tar` & `types-aiobotocore-outposts-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:05.593353 types-aiobotocore-outposts-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:51:21.000000 types-aiobotocore-outposts-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13636 2023-12-13 20:00:05.593353 types-aiobotocore-outposts-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12069 2023-12-13 19:51:21.000000 types-aiobotocore-outposts-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:05.593353 types-aiobotocore-outposts-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2023-12-13 19:51:21.000000 types-aiobotocore-outposts-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:05.589353 types-aiobotocore-outposts-2.9.0/types_aiobotocore_outposts/
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2023-12-13 19:51:21.000000 types-aiobotocore-outposts-2.9.0/types_aiobotocore_outposts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2023-12-13 19:51:21.000000 types-aiobotocore-outposts-2.9.0/types_aiobotocore_outposts/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      936 2023-12-13 19:51:21.000000 types-aiobotocore-outposts-2.9.0/types_aiobotocore_outposts/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23135 2023-12-13 19:51:21.000000 types-aiobotocore-outposts-2.9.0/types_aiobotocore_outposts/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    23131 2023-12-13 19:51:21.000000 types-aiobotocore-outposts-2.9.0/types_aiobotocore_outposts/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12132 2023-12-13 19:51:21.000000 types-aiobotocore-outposts-2.9.0/types_aiobotocore_outposts/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    12130 2023-12-13 19:51:21.000000 types-aiobotocore-outposts-2.9.0/types_aiobotocore_outposts/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8136 2023-12-13 19:51:21.000000 types-aiobotocore-outposts-2.9.0/types_aiobotocore_outposts/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8128 2023-12-13 19:51:21.000000 types-aiobotocore-outposts-2.9.0/types_aiobotocore_outposts/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:51:21.000000 types-aiobotocore-outposts-2.9.0/types_aiobotocore_outposts/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    22923 2023-12-13 19:51:22.000000 types-aiobotocore-outposts-2.9.0/types_aiobotocore_outposts/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    22922 2023-12-13 19:51:22.000000 types-aiobotocore-outposts-2.9.0/types_aiobotocore_outposts/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:51:21.000000 types-aiobotocore-outposts-2.9.0/types_aiobotocore_outposts/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:05.593353 types-aiobotocore-outposts-2.9.0/types_aiobotocore_outposts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13636 2023-12-13 20:00:05.000000 types-aiobotocore-outposts-2.9.0/types_aiobotocore_outposts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      832 2023-12-13 20:00:05.000000 types-aiobotocore-outposts-2.9.0/types_aiobotocore_outposts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:05.000000 types-aiobotocore-outposts-2.9.0/types_aiobotocore_outposts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:05.000000 types-aiobotocore-outposts-2.9.0/types_aiobotocore_outposts.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:05.000000 types-aiobotocore-outposts-2.9.0/types_aiobotocore_outposts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-13 20:00:05.000000 types-aiobotocore-outposts-2.9.0/types_aiobotocore_outposts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:26.337135 types-aiobotocore-outposts-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:13:01.000000 types-aiobotocore-outposts-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13656 2024-01-18 01:21:26.337135 types-aiobotocore-outposts-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12069 2024-01-18 01:13:01.000000 types-aiobotocore-outposts-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:26.337135 types-aiobotocore-outposts-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-01-18 01:13:01.000000 types-aiobotocore-outposts-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:26.337135 types-aiobotocore-outposts-2.9.1/types_aiobotocore_outposts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-01-18 01:13:01.000000 types-aiobotocore-outposts-2.9.1/types_aiobotocore_outposts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-01-18 01:13:01.000000 types-aiobotocore-outposts-2.9.1/types_aiobotocore_outposts/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-01-18 01:13:01.000000 types-aiobotocore-outposts-2.9.1/types_aiobotocore_outposts/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23144 2024-01-18 01:13:01.000000 types-aiobotocore-outposts-2.9.1/types_aiobotocore_outposts/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23141 2024-01-18 01:13:01.000000 types-aiobotocore-outposts-2.9.1/types_aiobotocore_outposts/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12130 2024-01-18 01:13:02.000000 types-aiobotocore-outposts-2.9.1/types_aiobotocore_outposts/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12130 2024-01-18 01:13:02.000000 types-aiobotocore-outposts-2.9.1/types_aiobotocore_outposts/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8139 2024-01-18 01:13:01.000000 types-aiobotocore-outposts-2.9.1/types_aiobotocore_outposts/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8132 2024-01-18 01:13:01.000000 types-aiobotocore-outposts-2.9.1/types_aiobotocore_outposts/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:13:01.000000 types-aiobotocore-outposts-2.9.1/types_aiobotocore_outposts/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    22922 2024-01-18 01:13:02.000000 types-aiobotocore-outposts-2.9.1/types_aiobotocore_outposts/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22922 2024-01-18 01:13:02.000000 types-aiobotocore-outposts-2.9.1/types_aiobotocore_outposts/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:13:01.000000 types-aiobotocore-outposts-2.9.1/types_aiobotocore_outposts/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:26.337135 types-aiobotocore-outposts-2.9.1/types_aiobotocore_outposts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13656 2024-01-18 01:21:26.000000 types-aiobotocore-outposts-2.9.1/types_aiobotocore_outposts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-01-18 01:21:26.000000 types-aiobotocore-outposts-2.9.1/types_aiobotocore_outposts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:26.000000 types-aiobotocore-outposts-2.9.1/types_aiobotocore_outposts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:26.000000 types-aiobotocore-outposts-2.9.1/types_aiobotocore_outposts.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:26.000000 types-aiobotocore-outposts-2.9.1/types_aiobotocore_outposts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-18 01:21:26.000000 types-aiobotocore-outposts-2.9.1/types_aiobotocore_outposts.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-outposts-2.9.0/LICENSE` & `types-aiobotocore-outposts-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-outposts-2.9.0/PKG-INFO` & `types-aiobotocore-outposts-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-outposts
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Outposts 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Outposts 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/
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
 
 <a id="types-aiobotocore-outposts"></a>
 
 # types-aiobotocore-outposts
 
 [![PyPI - types-aiobotocore-outposts](https://img.shields.io/pypi/v/types-aiobotocore-outposts.svg?color=blue)](https://pypi.org/project/types-aiobotocore-outposts)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-outposts.svg?color=blue)](https://pypi.org/project/types-aiobotocore-outposts)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-outposts)](https://pepy.tech/project/types-aiobotocore-outposts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Outposts 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts)
+[aiobotocore.Outposts 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts)
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
 [types-aiobotocore-outposts docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-outposts-2.9.0/README.md` & `types-aiobotocore-outposts-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-outposts.svg?color=blue)](https://pypi.org/project/types-aiobotocore-outposts)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-outposts)](https://pepy.tech/project/types-aiobotocore-outposts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Outposts 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts)
+[aiobotocore.Outposts 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts)
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
 [types-aiobotocore-outposts docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-outposts-2.9.0/setup.py` & `types-aiobotocore-outposts-2.9.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-outposts",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_outposts"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Outposts 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.Outposts 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore outposts type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_outposts": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-outposts-2.9.0/types_aiobotocore_outposts/__init__.py` & `types-aiobotocore-outposts-2.9.1/types_aiobotocore_outposts/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,14 @@
     ListOrdersPaginator,
     ListOutpostsPaginator,
     ListSitesPaginator,
 )
 
 Client = OutpostsClient
 
-
 __all__ = (
     "Client",
     "GetOutpostInstanceTypesPaginator",
     "ListAssetsPaginator",
     "ListCatalogItemsPaginator",
     "ListOrdersPaginator",
     "ListOutpostsPaginator",
```

### Comparing `types-aiobotocore-outposts-2.9.0/types_aiobotocore_outposts/__init__.pyi` & `types-aiobotocore-outposts-2.9.1/types_aiobotocore_outposts/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-outposts-2.9.0/types_aiobotocore_outposts/__main__.py` & `types-aiobotocore-outposts-2.9.1/types_aiobotocore_outposts/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Outposts 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Outposts 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts\nOther"
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

### Comparing `types-aiobotocore-outposts-2.9.0/types_aiobotocore_outposts/client.py` & `types-aiobotocore-outposts-2.9.1/types_aiobotocore_outposts/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -75,36 +75,32 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("OutpostsClient",)
 
-
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     NotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class OutpostsClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/client/)
     """
 
     meta: ClientMeta
@@ -144,15 +140,15 @@
 
     async def create_order(
         self,
         *,
         OutpostIdentifier: str,
         LineItems: Sequence[LineItemRequestTypeDef],
         PaymentOption: PaymentOptionType,
-        PaymentTerm: PaymentTermType = ...
+        PaymentTerm: PaymentTermType = ...,
     ) -> CreateOrderOutputTypeDef:
         """
         Creates an order for an Outpost.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.create_order)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/client/#create_order)
         """
@@ -162,15 +158,15 @@
         *,
         Name: str,
         SiteId: str,
         Description: str = ...,
         AvailabilityZone: str = ...,
         AvailabilityZoneId: str = ...,
         Tags: Mapping[str, str] = ...,
-        SupportedHardwareType: SupportedHardwareTypeType = ...
+        SupportedHardwareType: SupportedHardwareTypeType = ...,
     ) -> CreateOutpostOutputTypeDef:
         """
         Creates an Outpost.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.create_outpost)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/client/#create_outpost)
         """
@@ -180,15 +176,15 @@
         *,
         Name: str,
         Description: str = ...,
         Notes: str = ...,
         Tags: Mapping[str, str] = ...,
         OperatingAddress: AddressTypeDef = ...,
         ShippingAddress: AddressTypeDef = ...,
-        RackPhysicalProperties: RackPhysicalPropertiesTypeDef = ...
+        RackPhysicalProperties: RackPhysicalPropertiesTypeDef = ...,
     ) -> CreateSiteOutputTypeDef:
         """
         Creates a site for an Outpost.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.create_site)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/client/#create_site)
         """
@@ -286,15 +282,15 @@
     async def list_assets(
         self,
         *,
         OutpostIdentifier: str,
         HostIdFilter: Sequence[str] = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        StatusFilter: Sequence[AssetStateType] = ...
+        StatusFilter: Sequence[AssetStateType] = ...,
     ) -> ListAssetsOutputTypeDef:
         """
         Lists the hardware assets for the specified Outpost.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.list_assets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/client/#list_assets)
         """
@@ -302,15 +298,15 @@
     async def list_catalog_items(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         ItemClassFilter: Sequence[CatalogItemClassType] = ...,
         SupportedStorageFilter: Sequence[SupportedStorageEnumType] = ...,
-        EC2FamilyFilter: Sequence[str] = ...
+        EC2FamilyFilter: Sequence[str] = ...,
     ) -> ListCatalogItemsOutputTypeDef:
         """
         Lists the items in the catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.list_catalog_items)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/client/#list_catalog_items)
         """
@@ -328,15 +324,15 @@
     async def list_outposts(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         LifeCycleStatusFilter: Sequence[str] = ...,
         AvailabilityZoneFilter: Sequence[str] = ...,
-        AvailabilityZoneIdFilter: Sequence[str] = ...
+        AvailabilityZoneIdFilter: Sequence[str] = ...,
     ) -> ListOutpostsOutputTypeDef:
         """
         Lists the Outposts for your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.list_outposts)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/client/#list_outposts)
         """
@@ -344,15 +340,15 @@
     async def list_sites(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         OperatingAddressCountryCodeFilter: Sequence[str] = ...,
         OperatingAddressStateOrRegionFilter: Sequence[str] = ...,
-        OperatingAddressCityFilter: Sequence[str] = ...
+        OperatingAddressCityFilter: Sequence[str] = ...,
     ) -> ListSitesOutputTypeDef:
         """
         Lists the Outpost sites for your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.list_sites)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/client/#list_sites)
         """
@@ -369,15 +365,15 @@
 
     async def start_connection(
         self,
         *,
         DeviceSerialNumber: str,
         AssetId: str,
         ClientPublicKey: str,
-        NetworkInterfaceDeviceIndex: int
+        NetworkInterfaceDeviceIndex: int,
     ) -> StartConnectionResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.start_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/client/#start_connection)
         """
@@ -400,15 +396,15 @@
 
     async def update_outpost(
         self,
         *,
         OutpostId: str,
         Name: str = ...,
         Description: str = ...,
-        SupportedHardwareType: SupportedHardwareTypeType = ...
+        SupportedHardwareType: SupportedHardwareTypeType = ...,
     ) -> UpdateOutpostOutputTypeDef:
         """
         Updates an Outpost.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.update_outpost)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/client/#update_outpost)
         """
@@ -441,15 +437,15 @@
         PowerPhase: PowerPhaseType = ...,
         PowerConnector: PowerConnectorType = ...,
         PowerFeedDrop: PowerFeedDropType = ...,
         UplinkGbps: UplinkGbpsType = ...,
         UplinkCount: UplinkCountType = ...,
         FiberOpticCableType: FiberOpticCableTypeType = ...,
         OpticalStandard: OpticalStandardType = ...,
-        MaximumSupportedWeightLbs: MaximumSupportedWeightLbsType = ...
+        MaximumSupportedWeightLbs: MaximumSupportedWeightLbsType = ...,
     ) -> UpdateSiteRackPhysicalPropertiesOutputTypeDef:
         """
         Update the physical and logistical details for a rack at a site.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.update_site_rack_physical_properties)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/client/#update_site_rack_physical_properties)
         """
```

### Comparing `types-aiobotocore-outposts-2.9.0/types_aiobotocore_outposts/client.pyi` & `types-aiobotocore-outposts-2.9.1/types_aiobotocore_outposts/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,30 +77,33 @@
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = ("OutpostsClient",)
 
+
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     NotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class OutpostsClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/client/)
     """
 
     meta: ClientMeta
@@ -140,15 +143,15 @@
 
     async def create_order(
         self,
         *,
         OutpostIdentifier: str,
         LineItems: Sequence[LineItemRequestTypeDef],
         PaymentOption: PaymentOptionType,
-        PaymentTerm: PaymentTermType = ...
+        PaymentTerm: PaymentTermType = ...,
     ) -> CreateOrderOutputTypeDef:
         """
         Creates an order for an Outpost.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.create_order)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/client/#create_order)
         """
@@ -158,15 +161,15 @@
         *,
         Name: str,
         SiteId: str,
         Description: str = ...,
         AvailabilityZone: str = ...,
         AvailabilityZoneId: str = ...,
         Tags: Mapping[str, str] = ...,
-        SupportedHardwareType: SupportedHardwareTypeType = ...
+        SupportedHardwareType: SupportedHardwareTypeType = ...,
     ) -> CreateOutpostOutputTypeDef:
         """
         Creates an Outpost.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.create_outpost)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/client/#create_outpost)
         """
@@ -176,15 +179,15 @@
         *,
         Name: str,
         Description: str = ...,
         Notes: str = ...,
         Tags: Mapping[str, str] = ...,
         OperatingAddress: AddressTypeDef = ...,
         ShippingAddress: AddressTypeDef = ...,
-        RackPhysicalProperties: RackPhysicalPropertiesTypeDef = ...
+        RackPhysicalProperties: RackPhysicalPropertiesTypeDef = ...,
     ) -> CreateSiteOutputTypeDef:
         """
         Creates a site for an Outpost.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.create_site)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/client/#create_site)
         """
@@ -282,15 +285,15 @@
     async def list_assets(
         self,
         *,
         OutpostIdentifier: str,
         HostIdFilter: Sequence[str] = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        StatusFilter: Sequence[AssetStateType] = ...
+        StatusFilter: Sequence[AssetStateType] = ...,
     ) -> ListAssetsOutputTypeDef:
         """
         Lists the hardware assets for the specified Outpost.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.list_assets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/client/#list_assets)
         """
@@ -298,15 +301,15 @@
     async def list_catalog_items(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         ItemClassFilter: Sequence[CatalogItemClassType] = ...,
         SupportedStorageFilter: Sequence[SupportedStorageEnumType] = ...,
-        EC2FamilyFilter: Sequence[str] = ...
+        EC2FamilyFilter: Sequence[str] = ...,
     ) -> ListCatalogItemsOutputTypeDef:
         """
         Lists the items in the catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.list_catalog_items)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/client/#list_catalog_items)
         """
@@ -324,15 +327,15 @@
     async def list_outposts(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         LifeCycleStatusFilter: Sequence[str] = ...,
         AvailabilityZoneFilter: Sequence[str] = ...,
-        AvailabilityZoneIdFilter: Sequence[str] = ...
+        AvailabilityZoneIdFilter: Sequence[str] = ...,
     ) -> ListOutpostsOutputTypeDef:
         """
         Lists the Outposts for your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.list_outposts)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/client/#list_outposts)
         """
@@ -340,15 +343,15 @@
     async def list_sites(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         OperatingAddressCountryCodeFilter: Sequence[str] = ...,
         OperatingAddressStateOrRegionFilter: Sequence[str] = ...,
-        OperatingAddressCityFilter: Sequence[str] = ...
+        OperatingAddressCityFilter: Sequence[str] = ...,
     ) -> ListSitesOutputTypeDef:
         """
         Lists the Outpost sites for your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.list_sites)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/client/#list_sites)
         """
@@ -365,15 +368,15 @@
 
     async def start_connection(
         self,
         *,
         DeviceSerialNumber: str,
         AssetId: str,
         ClientPublicKey: str,
-        NetworkInterfaceDeviceIndex: int
+        NetworkInterfaceDeviceIndex: int,
     ) -> StartConnectionResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.start_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/client/#start_connection)
         """
@@ -396,15 +399,15 @@
 
     async def update_outpost(
         self,
         *,
         OutpostId: str,
         Name: str = ...,
         Description: str = ...,
-        SupportedHardwareType: SupportedHardwareTypeType = ...
+        SupportedHardwareType: SupportedHardwareTypeType = ...,
     ) -> UpdateOutpostOutputTypeDef:
         """
         Updates an Outpost.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.update_outpost)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/client/#update_outpost)
         """
@@ -437,15 +440,15 @@
         PowerPhase: PowerPhaseType = ...,
         PowerConnector: PowerConnectorType = ...,
         PowerFeedDrop: PowerFeedDropType = ...,
         UplinkGbps: UplinkGbpsType = ...,
         UplinkCount: UplinkCountType = ...,
         FiberOpticCableType: FiberOpticCableTypeType = ...,
         OpticalStandard: OpticalStandardType = ...,
-        MaximumSupportedWeightLbs: MaximumSupportedWeightLbsType = ...
+        MaximumSupportedWeightLbs: MaximumSupportedWeightLbsType = ...,
     ) -> UpdateSiteRackPhysicalPropertiesOutputTypeDef:
         """
         Update the physical and logistical details for a rack at a site.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.update_site_rack_physical_properties)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/client/#update_site_rack_physical_properties)
         """
```

### Comparing `types-aiobotocore-outposts-2.9.0/types_aiobotocore_outposts/literals.py` & `types-aiobotocore-outposts-2.9.1/types_aiobotocore_outposts/literals.py`

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
     "AddressTypeType",
     "AssetStateType",
     "AssetTypeType",
     "CatalogItemClassType",
     "CatalogItemStatusType",
     "ComputeAssetStateType",
@@ -53,15 +52,14 @@
     "OutpostsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AddressTypeType = Literal["OPERATING_ADDRESS", "SHIPPING_ADDRESS"]
 AssetStateType = Literal["ACTIVE", "ISOLATED", "RETIRING"]
 AssetTypeType = Literal["COMPUTE"]
 CatalogItemClassType = Literal["RACK", "SERVER"]
 CatalogItemStatusType = Literal["AVAILABLE", "DISCONTINUED"]
 ComputeAssetStateType = Literal["ACTIVE", "ISOLATED", "RETIRING"]
 FiberOpticCableTypeType = Literal["MULTI_MODE", "SINGLE_MODE"]
```

### Comparing `types-aiobotocore-outposts-2.9.0/types_aiobotocore_outposts/literals.pyi` & `types-aiobotocore-outposts-2.9.1/types_aiobotocore_outposts/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-outposts-2.9.0/types_aiobotocore_outposts/paginator.py` & `types-aiobotocore-outposts-2.9.1/types_aiobotocore_outposts/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,14 @@
     "ListAssetsPaginator",
     "ListCatalogItemsPaginator",
     "ListOrdersPaginator",
     "ListOutpostsPaginator",
     "ListSitesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -90,15 +89,15 @@
 
     def paginate(
         self,
         *,
         OutpostIdentifier: str,
         HostIdFilter: Sequence[str] = ...,
         StatusFilter: Sequence[AssetStateType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAssetsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Paginator.ListAssets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/paginators/#listassetspaginator)
         """
 
 
@@ -110,15 +109,15 @@
 
     def paginate(
         self,
         *,
         ItemClassFilter: Sequence[CatalogItemClassType] = ...,
         SupportedStorageFilter: Sequence[SupportedStorageEnumType] = ...,
         EC2FamilyFilter: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCatalogItemsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Paginator.ListCatalogItems.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/paginators/#listcatalogitemspaginator)
         """
 
 
@@ -145,15 +144,15 @@
 
     def paginate(
         self,
         *,
         LifeCycleStatusFilter: Sequence[str] = ...,
         AvailabilityZoneFilter: Sequence[str] = ...,
         AvailabilityZoneIdFilter: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListOutpostsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Paginator.ListOutposts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/paginators/#listoutpostspaginator)
         """
 
 
@@ -165,13 +164,13 @@
 
     def paginate(
         self,
         *,
         OperatingAddressCountryCodeFilter: Sequence[str] = ...,
         OperatingAddressStateOrRegionFilter: Sequence[str] = ...,
         OperatingAddressCityFilter: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSitesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Paginator.ListSites.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/paginators/#listsitespaginator)
         """
```

### Comparing `types-aiobotocore-outposts-2.9.0/types_aiobotocore_outposts/paginator.pyi` & `types-aiobotocore-outposts-2.9.1/types_aiobotocore_outposts/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 
     def paginate(
         self,
         *,
         OutpostIdentifier: str,
         HostIdFilter: Sequence[str] = ...,
         StatusFilter: Sequence[AssetStateType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAssetsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Paginator.ListAssets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/paginators/#listassetspaginator)
         """
 
 class ListCatalogItemsPaginator(AioPaginator):
@@ -105,15 +105,15 @@
 
     def paginate(
         self,
         *,
         ItemClassFilter: Sequence[CatalogItemClassType] = ...,
         SupportedStorageFilter: Sequence[SupportedStorageEnumType] = ...,
         EC2FamilyFilter: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCatalogItemsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Paginator.ListCatalogItems.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/paginators/#listcatalogitemspaginator)
         """
 
 class ListOrdersPaginator(AioPaginator):
@@ -138,15 +138,15 @@
 
     def paginate(
         self,
         *,
         LifeCycleStatusFilter: Sequence[str] = ...,
         AvailabilityZoneFilter: Sequence[str] = ...,
         AvailabilityZoneIdFilter: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListOutpostsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Paginator.ListOutposts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/paginators/#listoutpostspaginator)
         """
 
 class ListSitesPaginator(AioPaginator):
@@ -157,13 +157,13 @@
 
     def paginate(
         self,
         *,
         OperatingAddressCountryCodeFilter: Sequence[str] = ...,
         OperatingAddressStateOrRegionFilter: Sequence[str] = ...,
         OperatingAddressCityFilter: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSitesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Paginator.ListSites.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/paginators/#listsitespaginator)
         """
```

### Comparing `types-aiobotocore-outposts-2.9.0/types_aiobotocore_outposts/type_defs.py` & `types-aiobotocore-outposts-2.9.1/types_aiobotocore_outposts/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AddressTypeDef",
     "AssetLocationTypeDef",
     "ComputeAttributesTypeDef",
     "CancelOrderInputRequestTypeDef",
     "EC2CapacityTypeDef",
     "ConnectionDetailsTypeDef",
```

### Comparing `types-aiobotocore-outposts-2.9.0/types_aiobotocore_outposts/type_defs.pyi` & `types-aiobotocore-outposts-2.9.1/types_aiobotocore_outposts/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-outposts-2.9.0/types_aiobotocore_outposts.egg-info/PKG-INFO` & `types-aiobotocore-outposts-2.9.1/types_aiobotocore_outposts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-outposts
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Outposts 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Outposts 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/
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
 
 <a id="types-aiobotocore-outposts"></a>
 
 # types-aiobotocore-outposts
 
 [![PyPI - types-aiobotocore-outposts](https://img.shields.io/pypi/v/types-aiobotocore-outposts.svg?color=blue)](https://pypi.org/project/types-aiobotocore-outposts)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-outposts.svg?color=blue)](https://pypi.org/project/types-aiobotocore-outposts)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-outposts)](https://pepy.tech/project/types-aiobotocore-outposts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Outposts 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts)
+[aiobotocore.Outposts 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts)
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
 [types-aiobotocore-outposts docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-outposts-2.9.0/types_aiobotocore_outposts.egg-info/SOURCES.txt` & `types-aiobotocore-outposts-2.9.1/types_aiobotocore_outposts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

