# Comparing `tmp/types-aiobotocore-b2bi-2.9.0.tar.gz` & `tmp/types-aiobotocore-b2bi-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-b2bi-2.9.0.tar", last modified: Wed Dec 13 19:58:39 2023, max compression
+gzip compressed data, was "types-aiobotocore-b2bi-2.9.1.tar", last modified: Thu Jan 18 01:20:07 2024, max compression
```

## Comparing `types-aiobotocore-b2bi-2.9.0.tar` & `types-aiobotocore-b2bi-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:39.482054 types-aiobotocore-b2bi-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:41:30.000000 types-aiobotocore-b2bi-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13212 2023-12-13 19:58:39.482054 types-aiobotocore-b2bi-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11661 2023-12-13 19:41:30.000000 types-aiobotocore-b2bi-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:39.482054 types-aiobotocore-b2bi-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2023-12-13 19:41:30.000000 types-aiobotocore-b2bi-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:39.482054 types-aiobotocore-b2bi-2.9.0/types_aiobotocore_b2bi/
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2023-12-13 19:41:30.000000 types-aiobotocore-b2bi-2.9.0/types_aiobotocore_b2bi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2023-12-13 19:41:30.000000 types-aiobotocore-b2bi-2.9.0/types_aiobotocore_b2bi/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      909 2023-12-13 19:41:30.000000 types-aiobotocore-b2bi-2.9.0/types_aiobotocore_b2bi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22669 2023-12-13 19:41:30.000000 types-aiobotocore-b2bi-2.9.0/types_aiobotocore_b2bi/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    22665 2023-12-13 19:41:30.000000 types-aiobotocore-b2bi-2.9.0/types_aiobotocore_b2bi/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9483 2023-12-13 19:41:31.000000 types-aiobotocore-b2bi-2.9.0/types_aiobotocore_b2bi/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9481 2023-12-13 19:41:31.000000 types-aiobotocore-b2bi-2.9.0/types_aiobotocore_b2bi/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5150 2023-12-13 19:41:30.000000 types-aiobotocore-b2bi-2.9.0/types_aiobotocore_b2bi/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5144 2023-12-13 19:41:30.000000 types-aiobotocore-b2bi-2.9.0/types_aiobotocore_b2bi/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:41:30.000000 types-aiobotocore-b2bi-2.9.0/types_aiobotocore_b2bi/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    20234 2023-12-13 19:41:31.000000 types-aiobotocore-b2bi-2.9.0/types_aiobotocore_b2bi/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    20233 2023-12-13 19:41:31.000000 types-aiobotocore-b2bi-2.9.0/types_aiobotocore_b2bi/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:41:30.000000 types-aiobotocore-b2bi-2.9.0/types_aiobotocore_b2bi/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:39.482054 types-aiobotocore-b2bi-2.9.0/types_aiobotocore_b2bi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13212 2023-12-13 19:58:39.000000 types-aiobotocore-b2bi-2.9.0/types_aiobotocore_b2bi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      756 2023-12-13 19:58:39.000000 types-aiobotocore-b2bi-2.9.0/types_aiobotocore_b2bi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:39.000000 types-aiobotocore-b2bi-2.9.0/types_aiobotocore_b2bi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:39.000000 types-aiobotocore-b2bi-2.9.0/types_aiobotocore_b2bi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:39.000000 types-aiobotocore-b2bi-2.9.0/types_aiobotocore_b2bi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-13 19:58:39.000000 types-aiobotocore-b2bi-2.9.0/types_aiobotocore_b2bi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:07.173499 types-aiobotocore-b2bi-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:03:29.000000 types-aiobotocore-b2bi-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13232 2024-01-18 01:20:07.173499 types-aiobotocore-b2bi-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11661 2024-01-18 01:03:29.000000 types-aiobotocore-b2bi-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:07.173499 types-aiobotocore-b2bi-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-01-18 01:03:29.000000 types-aiobotocore-b2bi-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:07.169499 types-aiobotocore-b2bi-2.9.1/types_aiobotocore_b2bi/
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-01-18 01:03:29.000000 types-aiobotocore-b2bi-2.9.1/types_aiobotocore_b2bi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-01-18 01:03:29.000000 types-aiobotocore-b2bi-2.9.1/types_aiobotocore_b2bi/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-01-18 01:03:29.000000 types-aiobotocore-b2bi-2.9.1/types_aiobotocore_b2bi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22676 2024-01-18 01:03:29.000000 types-aiobotocore-b2bi-2.9.1/types_aiobotocore_b2bi/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22673 2024-01-18 01:03:29.000000 types-aiobotocore-b2bi-2.9.1/types_aiobotocore_b2bi/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9481 2024-01-18 01:03:29.000000 types-aiobotocore-b2bi-2.9.1/types_aiobotocore_b2bi/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9481 2024-01-18 01:03:29.000000 types-aiobotocore-b2bi-2.9.1/types_aiobotocore_b2bi/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5149 2024-01-18 01:03:29.000000 types-aiobotocore-b2bi-2.9.1/types_aiobotocore_b2bi/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-01-18 01:03:29.000000 types-aiobotocore-b2bi-2.9.1/types_aiobotocore_b2bi/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:03:29.000000 types-aiobotocore-b2bi-2.9.1/types_aiobotocore_b2bi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    20233 2024-01-18 01:03:30.000000 types-aiobotocore-b2bi-2.9.1/types_aiobotocore_b2bi/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20233 2024-01-18 01:03:30.000000 types-aiobotocore-b2bi-2.9.1/types_aiobotocore_b2bi/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:03:29.000000 types-aiobotocore-b2bi-2.9.1/types_aiobotocore_b2bi/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:07.173499 types-aiobotocore-b2bi-2.9.1/types_aiobotocore_b2bi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13232 2024-01-18 01:20:07.000000 types-aiobotocore-b2bi-2.9.1/types_aiobotocore_b2bi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-01-18 01:20:07.000000 types-aiobotocore-b2bi-2.9.1/types_aiobotocore_b2bi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:07.000000 types-aiobotocore-b2bi-2.9.1/types_aiobotocore_b2bi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:07.000000 types-aiobotocore-b2bi-2.9.1/types_aiobotocore_b2bi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:07.000000 types-aiobotocore-b2bi-2.9.1/types_aiobotocore_b2bi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-01-18 01:20:07.000000 types-aiobotocore-b2bi-2.9.1/types_aiobotocore_b2bi.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-b2bi-2.9.0/LICENSE` & `types-aiobotocore-b2bi-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-b2bi-2.9.0/PKG-INFO` & `types-aiobotocore-b2bi-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-b2bi
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.B2BI 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.B2BI 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_b2bi/
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
 
 <a id="types-aiobotocore-b2bi"></a>
 
 # types-aiobotocore-b2bi
 
 [![PyPI - types-aiobotocore-b2bi](https://img.shields.io/pypi/v/types-aiobotocore-b2bi.svg?color=blue)](https://pypi.org/project/types-aiobotocore-b2bi)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-b2bi.svg?color=blue)](https://pypi.org/project/types-aiobotocore-b2bi)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_b2bi/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-b2bi)](https://pepy.tech/project/types-aiobotocore-b2bi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.B2BI 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/b2bi.html#B2BI)
+[aiobotocore.B2BI 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/b2bi.html#B2BI)
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
 [types-aiobotocore-b2bi docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_b2bi/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-b2bi-2.9.0/README.md` & `types-aiobotocore-b2bi-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-b2bi.svg?color=blue)](https://pypi.org/project/types-aiobotocore-b2bi)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_b2bi/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-b2bi)](https://pepy.tech/project/types-aiobotocore-b2bi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.B2BI 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/b2bi.html#B2BI)
+[aiobotocore.B2BI 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/b2bi.html#B2BI)
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
 [types-aiobotocore-b2bi docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_b2bi/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-b2bi-2.9.0/setup.py` & `types-aiobotocore-b2bi-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-b2bi",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_b2bi"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.B2BI 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.B2BI 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore b2bi type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_b2bi": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_b2bi/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-b2bi-2.9.0/types_aiobotocore_b2bi/__init__.py` & `types-aiobotocore-b2bi-2.9.1/types_aiobotocore_b2bi/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     ListPartnershipsPaginator,
     ListProfilesPaginator,
     ListTransformersPaginator,
 )
 
 Client = B2BIClient
 
-
 __all__ = (
     "B2BIClient",
     "Client",
     "ListCapabilitiesPaginator",
     "ListPartnershipsPaginator",
     "ListProfilesPaginator",
     "ListTransformersPaginator",
```

### Comparing `types-aiobotocore-b2bi-2.9.0/types_aiobotocore_b2bi/__init__.pyi` & `types-aiobotocore-b2bi-2.9.1/types_aiobotocore_b2bi/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-b2bi-2.9.0/types_aiobotocore_b2bi/__main__.py` & `types-aiobotocore-b2bi-2.9.1/types_aiobotocore_b2bi/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.B2BI 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.B2BI 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_b2bi//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/b2bi.html#B2BI\nOther"
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

### Comparing `types-aiobotocore-b2bi-2.9.0/types_aiobotocore_b2bi/client.py` & `types-aiobotocore-b2bi-2.9.1/types_aiobotocore_b2bi/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("B2BIClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -122,15 +121,15 @@
         self,
         *,
         name: str,
         type: Literal["edi"],
         configuration: CapabilityConfigurationTypeDef,
         instructionsDocuments: Sequence[S3LocationTypeDef] = ...,
         clientToken: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateCapabilityResponseTypeDef:
         """
         Instantiates a capability based on the specified parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/b2bi.html#B2BI.Client.create_capability)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_b2bi/client/#create_capability)
         """
@@ -140,15 +139,15 @@
         *,
         profileId: str,
         name: str,
         email: str,
         phone: str = ...,
         capabilities: Sequence[str] = ...,
         clientToken: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreatePartnershipResponseTypeDef:
         """
         Creates a partnership between a customer and a trading partner, based on the
         supplied
         parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/b2bi.html#B2BI.Client.create_partnership)
@@ -160,15 +159,15 @@
         *,
         name: str,
         phone: str,
         businessName: str,
         logging: LoggingType,
         email: str = ...,
         clientToken: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateProfileResponseTypeDef:
         """
         Creates a customer profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/b2bi.html#B2BI.Client.create_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_b2bi/client/#create_profile)
         """
@@ -178,15 +177,15 @@
         *,
         name: str,
         fileFormat: FileFormatType,
         mappingTemplate: str,
         ediType: EdiTypeTypeDef,
         sampleDocument: str = ...,
         clientToken: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateTransformerResponseTypeDef:
         """
         Creates a transformer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/b2bi.html#B2BI.Client.create_transformer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_b2bi/client/#create_transformer)
         """
@@ -339,15 +338,15 @@
 
     async def start_transformer_job(
         self,
         *,
         inputFile: S3LocationTypeDef,
         outputLocation: S3LocationTypeDef,
         transformerId: str,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> StartTransformerJobResponseTypeDef:
         """
         Runs a job, using a transformer, to parse input EDI (electronic data
         interchange) file into the output structures used by Amazon Web Services B2BI
         Data
         Interchange.
 
@@ -401,15 +400,15 @@
 
     async def update_capability(
         self,
         *,
         capabilityId: str,
         name: str = ...,
         configuration: CapabilityConfigurationTypeDef = ...,
-        instructionsDocuments: Sequence[S3LocationTypeDef] = ...
+        instructionsDocuments: Sequence[S3LocationTypeDef] = ...,
     ) -> UpdateCapabilityResponseTypeDef:
         """
         Updates some of the parameters for a capability, based on the specified
         parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/b2bi.html#B2BI.Client.update_capability)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_b2bi/client/#update_capability)
@@ -429,15 +428,15 @@
     async def update_profile(
         self,
         *,
         profileId: str,
         name: str = ...,
         email: str = ...,
         phone: str = ...,
-        businessName: str = ...
+        businessName: str = ...,
     ) -> UpdateProfileResponseTypeDef:
         """
         Updates the specified parameters for a profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/b2bi.html#B2BI.Client.update_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_b2bi/client/#update_profile)
         """
@@ -447,15 +446,15 @@
         *,
         transformerId: str,
         name: str = ...,
         fileFormat: FileFormatType = ...,
         mappingTemplate: str = ...,
         status: TransformerStatusType = ...,
         ediType: EdiTypeTypeDef = ...,
-        sampleDocument: str = ...
+        sampleDocument: str = ...,
     ) -> UpdateTransformerResponseTypeDef:
         """
         Updates the specified parameters for a transformer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/b2bi.html#B2BI.Client.update_transformer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_b2bi/client/#update_transformer)
         """
```

### Comparing `types-aiobotocore-b2bi-2.9.0/types_aiobotocore_b2bi/client.pyi` & `types-aiobotocore-b2bi-2.9.1/types_aiobotocore_b2bi/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
         self,
         *,
         name: str,
         type: Literal["edi"],
         configuration: CapabilityConfigurationTypeDef,
         instructionsDocuments: Sequence[S3LocationTypeDef] = ...,
         clientToken: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateCapabilityResponseTypeDef:
         """
         Instantiates a capability based on the specified parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/b2bi.html#B2BI.Client.create_capability)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_b2bi/client/#create_capability)
         """
@@ -136,15 +136,15 @@
         *,
         profileId: str,
         name: str,
         email: str,
         phone: str = ...,
         capabilities: Sequence[str] = ...,
         clientToken: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreatePartnershipResponseTypeDef:
         """
         Creates a partnership between a customer and a trading partner, based on the
         supplied
         parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/b2bi.html#B2BI.Client.create_partnership)
@@ -156,15 +156,15 @@
         *,
         name: str,
         phone: str,
         businessName: str,
         logging: LoggingType,
         email: str = ...,
         clientToken: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateProfileResponseTypeDef:
         """
         Creates a customer profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/b2bi.html#B2BI.Client.create_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_b2bi/client/#create_profile)
         """
@@ -174,15 +174,15 @@
         *,
         name: str,
         fileFormat: FileFormatType,
         mappingTemplate: str,
         ediType: EdiTypeTypeDef,
         sampleDocument: str = ...,
         clientToken: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateTransformerResponseTypeDef:
         """
         Creates a transformer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/b2bi.html#B2BI.Client.create_transformer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_b2bi/client/#create_transformer)
         """
@@ -335,15 +335,15 @@
 
     async def start_transformer_job(
         self,
         *,
         inputFile: S3LocationTypeDef,
         outputLocation: S3LocationTypeDef,
         transformerId: str,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> StartTransformerJobResponseTypeDef:
         """
         Runs a job, using a transformer, to parse input EDI (electronic data
         interchange) file into the output structures used by Amazon Web Services B2BI
         Data
         Interchange.
 
@@ -397,15 +397,15 @@
 
     async def update_capability(
         self,
         *,
         capabilityId: str,
         name: str = ...,
         configuration: CapabilityConfigurationTypeDef = ...,
-        instructionsDocuments: Sequence[S3LocationTypeDef] = ...
+        instructionsDocuments: Sequence[S3LocationTypeDef] = ...,
     ) -> UpdateCapabilityResponseTypeDef:
         """
         Updates some of the parameters for a capability, based on the specified
         parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/b2bi.html#B2BI.Client.update_capability)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_b2bi/client/#update_capability)
@@ -425,15 +425,15 @@
     async def update_profile(
         self,
         *,
         profileId: str,
         name: str = ...,
         email: str = ...,
         phone: str = ...,
-        businessName: str = ...
+        businessName: str = ...,
     ) -> UpdateProfileResponseTypeDef:
         """
         Updates the specified parameters for a profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/b2bi.html#B2BI.Client.update_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_b2bi/client/#update_profile)
         """
@@ -443,15 +443,15 @@
         *,
         transformerId: str,
         name: str = ...,
         fileFormat: FileFormatType = ...,
         mappingTemplate: str = ...,
         status: TransformerStatusType = ...,
         ediType: EdiTypeTypeDef = ...,
-        sampleDocument: str = ...
+        sampleDocument: str = ...,
     ) -> UpdateTransformerResponseTypeDef:
         """
         Updates the specified parameters for a transformer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/b2bi.html#B2BI.Client.update_transformer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_b2bi/client/#update_transformer)
         """
```

### Comparing `types-aiobotocore-b2bi-2.9.0/types_aiobotocore_b2bi/literals.py` & `types-aiobotocore-b2bi-2.9.1/types_aiobotocore_b2bi/literals.py`

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
     "CapabilityTypeType",
     "FileFormatType",
     "ListCapabilitiesPaginatorName",
     "ListPartnershipsPaginatorName",
     "ListProfilesPaginatorName",
     "ListTransformersPaginatorName",
@@ -34,15 +33,14 @@
     "X12VersionType",
     "B2BIServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 CapabilityTypeType = Literal["edi"]
 FileFormatType = Literal["JSON", "XML"]
 ListCapabilitiesPaginatorName = Literal["list_capabilities"]
 ListPartnershipsPaginatorName = Literal["list_partnerships"]
 ListProfilesPaginatorName = Literal["list_profiles"]
 ListTransformersPaginatorName = Literal["list_transformers"]
 LoggingType = Literal["DISABLED", "ENABLED"]
```

### Comparing `types-aiobotocore-b2bi-2.9.0/types_aiobotocore_b2bi/literals.pyi` & `types-aiobotocore-b2bi-2.9.1/types_aiobotocore_b2bi/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-b2bi-2.9.0/types_aiobotocore_b2bi/paginator.py` & `types-aiobotocore-b2bi-2.9.1/types_aiobotocore_b2bi/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 __all__ = (
     "ListCapabilitiesPaginator",
     "ListPartnershipsPaginator",
     "ListProfilesPaginator",
     "ListTransformersPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
```

### Comparing `types-aiobotocore-b2bi-2.9.0/types_aiobotocore_b2bi/paginator.pyi` & `types-aiobotocore-b2bi-2.9.1/types_aiobotocore_b2bi/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-b2bi-2.9.0/types_aiobotocore_b2bi/type_defs.py` & `types-aiobotocore-b2bi-2.9.1/types_aiobotocore_b2bi/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CapabilitySummaryTypeDef",
     "S3LocationTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteCapabilityRequestRequestTypeDef",
     "DeletePartnershipRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-b2bi-2.9.0/types_aiobotocore_b2bi/type_defs.pyi` & `types-aiobotocore-b2bi-2.9.1/types_aiobotocore_b2bi/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-b2bi-2.9.0/types_aiobotocore_b2bi.egg-info/PKG-INFO` & `types-aiobotocore-b2bi-2.9.1/types_aiobotocore_b2bi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-b2bi
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.B2BI 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.B2BI 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_b2bi/
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
 
 <a id="types-aiobotocore-b2bi"></a>
 
 # types-aiobotocore-b2bi
 
 [![PyPI - types-aiobotocore-b2bi](https://img.shields.io/pypi/v/types-aiobotocore-b2bi.svg?color=blue)](https://pypi.org/project/types-aiobotocore-b2bi)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-b2bi.svg?color=blue)](https://pypi.org/project/types-aiobotocore-b2bi)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_b2bi/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-b2bi)](https://pepy.tech/project/types-aiobotocore-b2bi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.B2BI 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/b2bi.html#B2BI)
+[aiobotocore.B2BI 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/b2bi.html#B2BI)
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
 [types-aiobotocore-b2bi docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_b2bi/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-b2bi-2.9.0/types_aiobotocore_b2bi.egg-info/SOURCES.txt` & `types-aiobotocore-b2bi-2.9.1/types_aiobotocore_b2bi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

