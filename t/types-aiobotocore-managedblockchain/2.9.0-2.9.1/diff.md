# Comparing `tmp/types-aiobotocore-managedblockchain-2.9.0.tar.gz` & `tmp/types-aiobotocore-managedblockchain-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-managedblockchain-2.9.0.tar", last modified: Wed Dec 13 19:59:49 2023, max compression
+gzip compressed data, was "types-aiobotocore-managedblockchain-2.9.1.tar", last modified: Thu Jan 18 01:21:11 2024, max compression
```

## Comparing `types-aiobotocore-managedblockchain-2.9.0.tar` & `types-aiobotocore-managedblockchain-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:49.733494 types-aiobotocore-managedblockchain-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:49:40.000000 types-aiobotocore-managedblockchain-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13538 2023-12-13 19:59:49.733494 types-aiobotocore-managedblockchain-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11935 2023-12-13 19:49:40.000000 types-aiobotocore-managedblockchain-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:49.733494 types-aiobotocore-managedblockchain-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2023-12-13 19:49:40.000000 types-aiobotocore-managedblockchain-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:49.733494 types-aiobotocore-managedblockchain-2.9.0/types_aiobotocore_managedblockchain/
--rw-r--r--   0 runner    (1001) docker     (127)      722 2023-12-13 19:49:40.000000 types-aiobotocore-managedblockchain-2.9.0/types_aiobotocore_managedblockchain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2023-12-13 19:49:40.000000 types-aiobotocore-managedblockchain-2.9.0/types_aiobotocore_managedblockchain/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      972 2023-12-13 19:49:40.000000 types-aiobotocore-managedblockchain-2.9.0/types_aiobotocore_managedblockchain/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22569 2023-12-13 19:49:41.000000 types-aiobotocore-managedblockchain-2.9.0/types_aiobotocore_managedblockchain/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    22565 2023-12-13 19:49:40.000000 types-aiobotocore-managedblockchain-2.9.0/types_aiobotocore_managedblockchain/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9964 2023-12-13 19:49:41.000000 types-aiobotocore-managedblockchain-2.9.0/types_aiobotocore_managedblockchain/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9962 2023-12-13 19:49:41.000000 types-aiobotocore-managedblockchain-2.9.0/types_aiobotocore_managedblockchain/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2023-12-13 19:49:41.000000 types-aiobotocore-managedblockchain-2.9.0/types_aiobotocore_managedblockchain/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2023-12-13 19:49:41.000000 types-aiobotocore-managedblockchain-2.9.0/types_aiobotocore_managedblockchain/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:49:40.000000 types-aiobotocore-managedblockchain-2.9.0/types_aiobotocore_managedblockchain/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    24503 2023-12-13 19:49:41.000000 types-aiobotocore-managedblockchain-2.9.0/types_aiobotocore_managedblockchain/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    24502 2023-12-13 19:49:41.000000 types-aiobotocore-managedblockchain-2.9.0/types_aiobotocore_managedblockchain/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:49:40.000000 types-aiobotocore-managedblockchain-2.9.0/types_aiobotocore_managedblockchain/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:49.733494 types-aiobotocore-managedblockchain-2.9.0/types_aiobotocore_managedblockchain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13538 2023-12-13 19:59:49.000000 types-aiobotocore-managedblockchain-2.9.0/types_aiobotocore_managedblockchain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2023-12-13 19:59:49.000000 types-aiobotocore-managedblockchain-2.9.0/types_aiobotocore_managedblockchain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:49.000000 types-aiobotocore-managedblockchain-2.9.0/types_aiobotocore_managedblockchain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:49.000000 types-aiobotocore-managedblockchain-2.9.0/types_aiobotocore_managedblockchain.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:49.000000 types-aiobotocore-managedblockchain-2.9.0/types_aiobotocore_managedblockchain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-13 19:59:49.000000 types-aiobotocore-managedblockchain-2.9.0/types_aiobotocore_managedblockchain.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:11.909201 types-aiobotocore-managedblockchain-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:11:25.000000 types-aiobotocore-managedblockchain-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13558 2024-01-18 01:21:11.909201 types-aiobotocore-managedblockchain-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11935 2024-01-18 01:11:25.000000 types-aiobotocore-managedblockchain-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:11.909201 types-aiobotocore-managedblockchain-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-01-18 01:11:25.000000 types-aiobotocore-managedblockchain-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:11.909201 types-aiobotocore-managedblockchain-2.9.1/types_aiobotocore_managedblockchain/
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-01-18 01:11:25.000000 types-aiobotocore-managedblockchain-2.9.1/types_aiobotocore_managedblockchain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-01-18 01:11:25.000000 types-aiobotocore-managedblockchain-2.9.1/types_aiobotocore_managedblockchain/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-01-18 01:11:25.000000 types-aiobotocore-managedblockchain-2.9.1/types_aiobotocore_managedblockchain/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22579 2024-01-18 01:11:26.000000 types-aiobotocore-managedblockchain-2.9.1/types_aiobotocore_managedblockchain/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22576 2024-01-18 01:11:26.000000 types-aiobotocore-managedblockchain-2.9.1/types_aiobotocore_managedblockchain/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9962 2024-01-18 01:11:26.000000 types-aiobotocore-managedblockchain-2.9.1/types_aiobotocore_managedblockchain/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9962 2024-01-18 01:11:26.000000 types-aiobotocore-managedblockchain-2.9.1/types_aiobotocore_managedblockchain/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-01-18 01:11:26.000000 types-aiobotocore-managedblockchain-2.9.1/types_aiobotocore_managedblockchain/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-01-18 01:11:26.000000 types-aiobotocore-managedblockchain-2.9.1/types_aiobotocore_managedblockchain/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:11:25.000000 types-aiobotocore-managedblockchain-2.9.1/types_aiobotocore_managedblockchain/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    24502 2024-01-18 01:11:26.000000 types-aiobotocore-managedblockchain-2.9.1/types_aiobotocore_managedblockchain/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24502 2024-01-18 01:11:26.000000 types-aiobotocore-managedblockchain-2.9.1/types_aiobotocore_managedblockchain/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:11:25.000000 types-aiobotocore-managedblockchain-2.9.1/types_aiobotocore_managedblockchain/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:11.909201 types-aiobotocore-managedblockchain-2.9.1/types_aiobotocore_managedblockchain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13558 2024-01-18 01:21:11.000000 types-aiobotocore-managedblockchain-2.9.1/types_aiobotocore_managedblockchain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-01-18 01:21:11.000000 types-aiobotocore-managedblockchain-2.9.1/types_aiobotocore_managedblockchain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:11.000000 types-aiobotocore-managedblockchain-2.9.1/types_aiobotocore_managedblockchain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:11.000000 types-aiobotocore-managedblockchain-2.9.1/types_aiobotocore_managedblockchain.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:11.000000 types-aiobotocore-managedblockchain-2.9.1/types_aiobotocore_managedblockchain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-01-18 01:21:11.000000 types-aiobotocore-managedblockchain-2.9.1/types_aiobotocore_managedblockchain.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-managedblockchain-2.9.0/LICENSE` & `types-aiobotocore-managedblockchain-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-managedblockchain-2.9.0/PKG-INFO` & `types-aiobotocore-managedblockchain-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-managedblockchain
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ManagedBlockchain 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ManagedBlockchain 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/
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
 
 <a id="types-aiobotocore-managedblockchain"></a>
 
 # types-aiobotocore-managedblockchain
 
 [![PyPI - types-aiobotocore-managedblockchain](https://img.shields.io/pypi/v/types-aiobotocore-managedblockchain.svg?color=blue)](https://pypi.org/project/types-aiobotocore-managedblockchain)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-managedblockchain.svg?color=blue)](https://pypi.org/project/types-aiobotocore-managedblockchain)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-managedblockchain)](https://pepy.tech/project/types-aiobotocore-managedblockchain)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ManagedBlockchain 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
+[aiobotocore.ManagedBlockchain 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
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
 [types-aiobotocore-managedblockchain docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-managedblockchain-2.9.0/README.md` & `types-aiobotocore-managedblockchain-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-managedblockchain.svg?color=blue)](https://pypi.org/project/types-aiobotocore-managedblockchain)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-managedblockchain)](https://pepy.tech/project/types-aiobotocore-managedblockchain)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ManagedBlockchain 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
+[aiobotocore.ManagedBlockchain 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
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
 [types-aiobotocore-managedblockchain docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-managedblockchain-2.9.0/setup.py` & `types-aiobotocore-managedblockchain-2.9.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-managedblockchain",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_managedblockchain"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ManagedBlockchain 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.ManagedBlockchain 2.9.1 service generated with"
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
     keywords="aiobotocore managedblockchain type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_managedblockchain": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-managedblockchain-2.9.0/types_aiobotocore_managedblockchain/__init__.py` & `types-aiobotocore-managedblockchain-2.9.1/types_aiobotocore_managedblockchain/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,9 +22,8 @@
 """
 
 from .client import ManagedBlockchainClient
 from .paginator import ListAccessorsPaginator
 
 Client = ManagedBlockchainClient
 
-
 __all__ = ("Client", "ListAccessorsPaginator", "ManagedBlockchainClient")
```

### Comparing `types-aiobotocore-managedblockchain-2.9.0/types_aiobotocore_managedblockchain/__init__.pyi` & `types-aiobotocore-managedblockchain-2.9.1/types_aiobotocore_managedblockchain/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-managedblockchain-2.9.0/types_aiobotocore_managedblockchain/__main__.py` & `types-aiobotocore-managedblockchain-2.9.1/types_aiobotocore_managedblockchain/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ManagedBlockchain 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.ManagedBlockchain 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain\nOther"
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

### Comparing `types-aiobotocore-managedblockchain-2.9.0/types_aiobotocore_managedblockchain/client.py` & `types-aiobotocore-managedblockchain-2.9.1/types_aiobotocore_managedblockchain/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ManagedBlockchainClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -124,15 +123,15 @@
 
     async def create_accessor(
         self,
         *,
         ClientRequestToken: str,
         AccessorType: Literal["BILLING_TOKEN"],
         Tags: Mapping[str, str] = ...,
-        NetworkType: AccessorNetworkTypeType = ...
+        NetworkType: AccessorNetworkTypeType = ...,
     ) -> CreateAccessorOutputTypeDef:
         """
         Creates a new accessor for use with Amazon Managed Blockchain service that
         supports token based
         access.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.create_accessor)
@@ -141,15 +140,15 @@
 
     async def create_member(
         self,
         *,
         ClientRequestToken: str,
         InvitationId: str,
         NetworkId: str,
-        MemberConfiguration: MemberConfigurationTypeDef
+        MemberConfiguration: MemberConfigurationTypeDef,
     ) -> CreateMemberOutputTypeDef:
         """
         Creates a member within a Managed Blockchain network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.create_member)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/client/#create_member)
         """
@@ -161,15 +160,15 @@
         Name: str,
         Framework: FrameworkType,
         FrameworkVersion: str,
         VotingPolicy: VotingPolicyTypeDef,
         MemberConfiguration: MemberConfigurationTypeDef,
         Description: str = ...,
         FrameworkConfiguration: NetworkFrameworkConfigurationTypeDef = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateNetworkOutputTypeDef:
         """
         Creates a new blockchain network using Amazon Managed Blockchain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.create_network)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/client/#create_network)
         """
@@ -177,15 +176,15 @@
     async def create_node(
         self,
         *,
         ClientRequestToken: str,
         NetworkId: str,
         NodeConfiguration: NodeConfigurationTypeDef,
         MemberId: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateNodeOutputTypeDef:
         """
         Creates a node on the specified blockchain network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.create_node)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/client/#create_node)
         """
@@ -194,15 +193,15 @@
         self,
         *,
         ClientRequestToken: str,
         NetworkId: str,
         MemberId: str,
         Actions: ProposalActionsTypeDef,
         Description: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateProposalOutputTypeDef:
         """
         Creates a proposal for a change to the network that other members of the
         network can vote on, for example, a proposal to add a new member to the
         network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.create_proposal)
@@ -292,15 +291,15 @@
         """
 
     async def list_accessors(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
-        NetworkType: AccessorNetworkTypeType = ...
+        NetworkType: AccessorNetworkTypeType = ...,
     ) -> ListAccessorsOutputTypeDef:
         """
         Returns a list of the accessors and their properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.list_accessors)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/client/#list_accessors)
         """
@@ -319,15 +318,15 @@
         self,
         *,
         NetworkId: str,
         Name: str = ...,
         Status: MemberStatusType = ...,
         IsOwned: bool = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListMembersOutputTypeDef:
         """
         Returns a list of the members in a network and properties of their
         configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.list_members)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/client/#list_members)
@@ -336,15 +335,15 @@
     async def list_networks(
         self,
         *,
         Name: str = ...,
         Framework: FrameworkType = ...,
         Status: NetworkStatusType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListNetworksOutputTypeDef:
         """
         Returns information about the networks in which the current Amazon Web Services
         account
         participates.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.list_networks)
@@ -354,15 +353,15 @@
     async def list_nodes(
         self,
         *,
         NetworkId: str,
         MemberId: str = ...,
         Status: NodeStatusType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListNodesOutputTypeDef:
         """
         Returns information about the nodes within a network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.list_nodes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/client/#list_nodes)
         """
@@ -426,30 +425,30 @@
         """
 
     async def update_member(
         self,
         *,
         NetworkId: str,
         MemberId: str,
-        LogPublishingConfiguration: MemberLogPublishingConfigurationTypeDef = ...
+        LogPublishingConfiguration: MemberLogPublishingConfigurationTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates a member configuration with new parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.update_member)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/client/#update_member)
         """
 
     async def update_node(
         self,
         *,
         NetworkId: str,
         NodeId: str,
         MemberId: str = ...,
-        LogPublishingConfiguration: NodeLogPublishingConfigurationTypeDef = ...
+        LogPublishingConfiguration: NodeLogPublishingConfigurationTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates a node configuration with new parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.update_node)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/client/#update_node)
         """
```

### Comparing `types-aiobotocore-managedblockchain-2.9.0/types_aiobotocore_managedblockchain/client.pyi` & `types-aiobotocore-managedblockchain-2.9.1/types_aiobotocore_managedblockchain/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -120,15 +120,15 @@
 
     async def create_accessor(
         self,
         *,
         ClientRequestToken: str,
         AccessorType: Literal["BILLING_TOKEN"],
         Tags: Mapping[str, str] = ...,
-        NetworkType: AccessorNetworkTypeType = ...
+        NetworkType: AccessorNetworkTypeType = ...,
     ) -> CreateAccessorOutputTypeDef:
         """
         Creates a new accessor for use with Amazon Managed Blockchain service that
         supports token based
         access.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.create_accessor)
@@ -137,15 +137,15 @@
 
     async def create_member(
         self,
         *,
         ClientRequestToken: str,
         InvitationId: str,
         NetworkId: str,
-        MemberConfiguration: MemberConfigurationTypeDef
+        MemberConfiguration: MemberConfigurationTypeDef,
     ) -> CreateMemberOutputTypeDef:
         """
         Creates a member within a Managed Blockchain network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.create_member)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/client/#create_member)
         """
@@ -157,15 +157,15 @@
         Name: str,
         Framework: FrameworkType,
         FrameworkVersion: str,
         VotingPolicy: VotingPolicyTypeDef,
         MemberConfiguration: MemberConfigurationTypeDef,
         Description: str = ...,
         FrameworkConfiguration: NetworkFrameworkConfigurationTypeDef = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateNetworkOutputTypeDef:
         """
         Creates a new blockchain network using Amazon Managed Blockchain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.create_network)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/client/#create_network)
         """
@@ -173,15 +173,15 @@
     async def create_node(
         self,
         *,
         ClientRequestToken: str,
         NetworkId: str,
         NodeConfiguration: NodeConfigurationTypeDef,
         MemberId: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateNodeOutputTypeDef:
         """
         Creates a node on the specified blockchain network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.create_node)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/client/#create_node)
         """
@@ -190,15 +190,15 @@
         self,
         *,
         ClientRequestToken: str,
         NetworkId: str,
         MemberId: str,
         Actions: ProposalActionsTypeDef,
         Description: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateProposalOutputTypeDef:
         """
         Creates a proposal for a change to the network that other members of the
         network can vote on, for example, a proposal to add a new member to the
         network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.create_proposal)
@@ -288,15 +288,15 @@
         """
 
     async def list_accessors(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
-        NetworkType: AccessorNetworkTypeType = ...
+        NetworkType: AccessorNetworkTypeType = ...,
     ) -> ListAccessorsOutputTypeDef:
         """
         Returns a list of the accessors and their properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.list_accessors)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/client/#list_accessors)
         """
@@ -315,15 +315,15 @@
         self,
         *,
         NetworkId: str,
         Name: str = ...,
         Status: MemberStatusType = ...,
         IsOwned: bool = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListMembersOutputTypeDef:
         """
         Returns a list of the members in a network and properties of their
         configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.list_members)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/client/#list_members)
@@ -332,15 +332,15 @@
     async def list_networks(
         self,
         *,
         Name: str = ...,
         Framework: FrameworkType = ...,
         Status: NetworkStatusType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListNetworksOutputTypeDef:
         """
         Returns information about the networks in which the current Amazon Web Services
         account
         participates.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.list_networks)
@@ -350,15 +350,15 @@
     async def list_nodes(
         self,
         *,
         NetworkId: str,
         MemberId: str = ...,
         Status: NodeStatusType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListNodesOutputTypeDef:
         """
         Returns information about the nodes within a network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.list_nodes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/client/#list_nodes)
         """
@@ -422,30 +422,30 @@
         """
 
     async def update_member(
         self,
         *,
         NetworkId: str,
         MemberId: str,
-        LogPublishingConfiguration: MemberLogPublishingConfigurationTypeDef = ...
+        LogPublishingConfiguration: MemberLogPublishingConfigurationTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates a member configuration with new parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.update_member)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/client/#update_member)
         """
 
     async def update_node(
         self,
         *,
         NetworkId: str,
         NodeId: str,
         MemberId: str = ...,
-        LogPublishingConfiguration: NodeLogPublishingConfigurationTypeDef = ...
+        LogPublishingConfiguration: NodeLogPublishingConfigurationTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates a node configuration with new parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.update_node)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/client/#update_node)
         """
```

### Comparing `types-aiobotocore-managedblockchain-2.9.0/types_aiobotocore_managedblockchain/literals.py` & `types-aiobotocore-managedblockchain-2.9.1/types_aiobotocore_managedblockchain/literals.py`

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
     "AccessorNetworkTypeType",
     "AccessorStatusType",
     "AccessorTypeType",
     "EditionType",
     "FrameworkType",
     "InvitationStatusType",
@@ -38,15 +37,14 @@
     "ManagedBlockchainServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AccessorNetworkTypeType = Literal[
     "ETHEREUM_GOERLI",
     "ETHEREUM_MAINNET",
     "ETHEREUM_MAINNET_AND_GOERLI",
     "POLYGON_MAINNET",
     "POLYGON_MUMBAI",
 ]
```

### Comparing `types-aiobotocore-managedblockchain-2.9.0/types_aiobotocore_managedblockchain/literals.pyi` & `types-aiobotocore-managedblockchain-2.9.1/types_aiobotocore_managedblockchain/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-managedblockchain-2.9.0/types_aiobotocore_managedblockchain/paginator.py` & `types-aiobotocore-managedblockchain-2.9.1/types_aiobotocore_managedblockchain/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 from botocore.paginate import PageIterator
 
 from .literals import AccessorNetworkTypeType
 from .type_defs import ListAccessorsOutputTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListAccessorsPaginator",)
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -48,13 +47,13 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/paginators/#listaccessorspaginator)
     """
 
     def paginate(
         self,
         *,
         NetworkType: AccessorNetworkTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAccessorsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Paginator.ListAccessors.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/paginators/#listaccessorspaginator)
         """
```

### Comparing `types-aiobotocore-managedblockchain-2.9.0/types_aiobotocore_managedblockchain/paginator.pyi` & `types-aiobotocore-managedblockchain-2.9.1/types_aiobotocore_managedblockchain/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -45,13 +45,13 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/paginators/#listaccessorspaginator)
     """
 
     def paginate(
         self,
         *,
         NetworkType: AccessorNetworkTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAccessorsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Paginator.ListAccessors.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/paginators/#listaccessorspaginator)
         """
```

### Comparing `types-aiobotocore-managedblockchain-2.9.0/types_aiobotocore_managedblockchain/type_defs.py` & `types-aiobotocore-managedblockchain-2.9.1/types_aiobotocore_managedblockchain/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccessorSummaryTypeDef",
     "AccessorTypeDef",
     "ApprovalThresholdPolicyTypeDef",
     "CreateAccessorInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteAccessorInputRequestTypeDef",
```

### Comparing `types-aiobotocore-managedblockchain-2.9.0/types_aiobotocore_managedblockchain/type_defs.pyi` & `types-aiobotocore-managedblockchain-2.9.1/types_aiobotocore_managedblockchain/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-managedblockchain-2.9.0/types_aiobotocore_managedblockchain.egg-info/PKG-INFO` & `types-aiobotocore-managedblockchain-2.9.1/types_aiobotocore_managedblockchain.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-managedblockchain
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ManagedBlockchain 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ManagedBlockchain 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/
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
 
 <a id="types-aiobotocore-managedblockchain"></a>
 
 # types-aiobotocore-managedblockchain
 
 [![PyPI - types-aiobotocore-managedblockchain](https://img.shields.io/pypi/v/types-aiobotocore-managedblockchain.svg?color=blue)](https://pypi.org/project/types-aiobotocore-managedblockchain)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-managedblockchain.svg?color=blue)](https://pypi.org/project/types-aiobotocore-managedblockchain)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-managedblockchain)](https://pepy.tech/project/types-aiobotocore-managedblockchain)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ManagedBlockchain 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
+[aiobotocore.ManagedBlockchain 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
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
 [types-aiobotocore-managedblockchain docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-managedblockchain-2.9.0/types_aiobotocore_managedblockchain.egg-info/SOURCES.txt` & `types-aiobotocore-managedblockchain-2.9.1/types_aiobotocore_managedblockchain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

