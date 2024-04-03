# Comparing `tmp/types-aiobotocore-managedblockchain-query-2.9.0.tar.gz` & `tmp/types-aiobotocore-managedblockchain-query-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-managedblockchain-query-2.9.0.tar", last modified: Wed Dec 13 19:59:50 2023, max compression
+gzip compressed data, was "types-aiobotocore-managedblockchain-query-2.9.1.tar", last modified: Thu Jan 18 01:21:12 2024, max compression
```

## Comparing `types-aiobotocore-managedblockchain-query-2.9.0.tar` & `types-aiobotocore-managedblockchain-query-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:50.105490 types-aiobotocore-managedblockchain-query-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:49:41.000000 types-aiobotocore-managedblockchain-query-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14384 2023-12-13 19:59:50.105490 types-aiobotocore-managedblockchain-query-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12758 2023-12-13 19:49:41.000000 types-aiobotocore-managedblockchain-query-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:50.105490 types-aiobotocore-managedblockchain-query-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2023-12-13 19:49:41.000000 types-aiobotocore-managedblockchain-query-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:50.105490 types-aiobotocore-managedblockchain-query-2.9.0/types_aiobotocore_managedblockchain_query/
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2023-12-13 19:49:41.000000 types-aiobotocore-managedblockchain-query-2.9.0/types_aiobotocore_managedblockchain_query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2023-12-13 19:49:41.000000 types-aiobotocore-managedblockchain-query-2.9.0/types_aiobotocore_managedblockchain_query/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      994 2023-12-13 19:49:41.000000 types-aiobotocore-managedblockchain-query-2.9.0/types_aiobotocore_managedblockchain_query/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13236 2023-12-13 19:49:42.000000 types-aiobotocore-managedblockchain-query-2.9.0/types_aiobotocore_managedblockchain_query/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13232 2023-12-13 19:49:41.000000 types-aiobotocore-managedblockchain-query-2.9.0/types_aiobotocore_managedblockchain_query/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9723 2023-12-13 19:49:42.000000 types-aiobotocore-managedblockchain-query-2.9.0/types_aiobotocore_managedblockchain_query/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9721 2023-12-13 19:49:42.000000 types-aiobotocore-managedblockchain-query-2.9.0/types_aiobotocore_managedblockchain_query/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6557 2023-12-13 19:49:42.000000 types-aiobotocore-managedblockchain-query-2.9.0/types_aiobotocore_managedblockchain_query/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6551 2023-12-13 19:49:42.000000 types-aiobotocore-managedblockchain-query-2.9.0/types_aiobotocore_managedblockchain_query/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:49:41.000000 types-aiobotocore-managedblockchain-query-2.9.0/types_aiobotocore_managedblockchain_query/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    14054 2023-12-13 19:49:44.000000 types-aiobotocore-managedblockchain-query-2.9.0/types_aiobotocore_managedblockchain_query/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    14053 2023-12-13 19:49:42.000000 types-aiobotocore-managedblockchain-query-2.9.0/types_aiobotocore_managedblockchain_query/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:49:41.000000 types-aiobotocore-managedblockchain-query-2.9.0/types_aiobotocore_managedblockchain_query/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:50.105490 types-aiobotocore-managedblockchain-query-2.9.0/types_aiobotocore_managedblockchain_query.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14384 2023-12-13 19:59:50.000000 types-aiobotocore-managedblockchain-query-2.9.0/types_aiobotocore_managedblockchain_query.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2023-12-13 19:59:50.000000 types-aiobotocore-managedblockchain-query-2.9.0/types_aiobotocore_managedblockchain_query.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:50.000000 types-aiobotocore-managedblockchain-query-2.9.0/types_aiobotocore_managedblockchain_query.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:50.000000 types-aiobotocore-managedblockchain-query-2.9.0/types_aiobotocore_managedblockchain_query.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:50.000000 types-aiobotocore-managedblockchain-query-2.9.0/types_aiobotocore_managedblockchain_query.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-12-13 19:59:50.000000 types-aiobotocore-managedblockchain-query-2.9.0/types_aiobotocore_managedblockchain_query.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:12.253199 types-aiobotocore-managedblockchain-query-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:11:26.000000 types-aiobotocore-managedblockchain-query-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14404 2024-01-18 01:21:12.253199 types-aiobotocore-managedblockchain-query-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12758 2024-01-18 01:11:26.000000 types-aiobotocore-managedblockchain-query-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:12.253199 types-aiobotocore-managedblockchain-query-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-01-18 01:11:26.000000 types-aiobotocore-managedblockchain-query-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:12.249199 types-aiobotocore-managedblockchain-query-2.9.1/types_aiobotocore_managedblockchain_query/
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-01-18 01:11:26.000000 types-aiobotocore-managedblockchain-query-2.9.1/types_aiobotocore_managedblockchain_query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-01-18 01:11:26.000000 types-aiobotocore-managedblockchain-query-2.9.1/types_aiobotocore_managedblockchain_query/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-01-18 01:11:26.000000 types-aiobotocore-managedblockchain-query-2.9.1/types_aiobotocore_managedblockchain_query/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-01-18 01:11:27.000000 types-aiobotocore-managedblockchain-query-2.9.1/types_aiobotocore_managedblockchain_query/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13236 2024-01-18 01:11:26.000000 types-aiobotocore-managedblockchain-query-2.9.1/types_aiobotocore_managedblockchain_query/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9721 2024-01-18 01:11:29.000000 types-aiobotocore-managedblockchain-query-2.9.1/types_aiobotocore_managedblockchain_query/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9721 2024-01-18 01:11:27.000000 types-aiobotocore-managedblockchain-query-2.9.1/types_aiobotocore_managedblockchain_query/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6560 2024-01-18 01:11:27.000000 types-aiobotocore-managedblockchain-query-2.9.1/types_aiobotocore_managedblockchain_query/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6555 2024-01-18 01:11:27.000000 types-aiobotocore-managedblockchain-query-2.9.1/types_aiobotocore_managedblockchain_query/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:11:26.000000 types-aiobotocore-managedblockchain-query-2.9.1/types_aiobotocore_managedblockchain_query/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    14053 2024-01-18 01:11:29.000000 types-aiobotocore-managedblockchain-query-2.9.1/types_aiobotocore_managedblockchain_query/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14053 2024-01-18 01:11:29.000000 types-aiobotocore-managedblockchain-query-2.9.1/types_aiobotocore_managedblockchain_query/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:11:26.000000 types-aiobotocore-managedblockchain-query-2.9.1/types_aiobotocore_managedblockchain_query/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:12.249199 types-aiobotocore-managedblockchain-query-2.9.1/types_aiobotocore_managedblockchain_query.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14404 2024-01-18 01:21:12.000000 types-aiobotocore-managedblockchain-query-2.9.1/types_aiobotocore_managedblockchain_query.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-01-18 01:21:12.000000 types-aiobotocore-managedblockchain-query-2.9.1/types_aiobotocore_managedblockchain_query.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:12.000000 types-aiobotocore-managedblockchain-query-2.9.1/types_aiobotocore_managedblockchain_query.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:12.000000 types-aiobotocore-managedblockchain-query-2.9.1/types_aiobotocore_managedblockchain_query.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:12.000000 types-aiobotocore-managedblockchain-query-2.9.1/types_aiobotocore_managedblockchain_query.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-01-18 01:21:12.000000 types-aiobotocore-managedblockchain-query-2.9.1/types_aiobotocore_managedblockchain_query.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-managedblockchain-query-2.9.0/LICENSE` & `types-aiobotocore-managedblockchain-query-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-managedblockchain-query-2.9.0/PKG-INFO` & `types-aiobotocore-managedblockchain-query-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-managedblockchain-query
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ManagedBlockchainQuery 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ManagedBlockchainQuery 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain_query/
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
 
 <a id="types-aiobotocore-managedblockchain-query"></a>
 
 # types-aiobotocore-managedblockchain-query
 
 [![PyPI - types-aiobotocore-managedblockchain-query](https://img.shields.io/pypi/v/types-aiobotocore-managedblockchain-query.svg?color=blue)](https://pypi.org/project/types-aiobotocore-managedblockchain-query)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-managedblockchain-query.svg?color=blue)](https://pypi.org/project/types-aiobotocore-managedblockchain-query)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain_query/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-managedblockchain-query)](https://pepy.tech/project/types-aiobotocore-managedblockchain-query)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ManagedBlockchainQuery 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery)
+[aiobotocore.ManagedBlockchainQuery 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery)
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
 [types-aiobotocore-managedblockchain-query docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain_query/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-managedblockchain-query-2.9.0/README.md` & `types-aiobotocore-managedblockchain-query-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-managedblockchain-query.svg?color=blue)](https://pypi.org/project/types-aiobotocore-managedblockchain-query)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain_query/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-managedblockchain-query)](https://pepy.tech/project/types-aiobotocore-managedblockchain-query)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ManagedBlockchainQuery 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery)
+[aiobotocore.ManagedBlockchainQuery 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery)
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
 [types-aiobotocore-managedblockchain-query docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain_query/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-managedblockchain-query-2.9.0/setup.py` & `types-aiobotocore-managedblockchain-query-2.9.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,50 +7,49 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-managedblockchain-query",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_managedblockchain_query"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ManagedBlockchainQuery 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.ManagedBlockchainQuery 2.9.1 service generated with"
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
         "aiobotocore managedblockchain-query type-annotations botocore mypy typeshed autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_managedblockchain_query": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain_query/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-managedblockchain-query-2.9.0/types_aiobotocore_managedblockchain_query/__init__.py` & `types-aiobotocore-managedblockchain-query-2.9.1/types_aiobotocore_managedblockchain_query/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     ListTokenBalancesPaginator,
     ListTransactionEventsPaginator,
     ListTransactionsPaginator,
 )
 
 Client = ManagedBlockchainQueryClient
 
-
 __all__ = (
     "Client",
     "ListAssetContractsPaginator",
     "ListTokenBalancesPaginator",
     "ListTransactionEventsPaginator",
     "ListTransactionsPaginator",
     "ManagedBlockchainQueryClient",
```

### Comparing `types-aiobotocore-managedblockchain-query-2.9.0/types_aiobotocore_managedblockchain_query/__init__.pyi` & `types-aiobotocore-managedblockchain-query-2.9.1/types_aiobotocore_managedblockchain_query/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-managedblockchain-query-2.9.0/types_aiobotocore_managedblockchain_query/__main__.py` & `types-aiobotocore-managedblockchain-query-2.9.1/types_aiobotocore_managedblockchain_query/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ManagedBlockchainQuery 2.9.0\nVersion:        "
-        " 2.9.0\nBuilder version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.ManagedBlockchainQuery 2.9.1\nVersion:        "
+        " 2.9.1\nBuilder version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain_query//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery\nOther"
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

### Comparing `types-aiobotocore-managedblockchain-query-2.9.0/types_aiobotocore_managedblockchain_query/client.py` & `types-aiobotocore-managedblockchain-query-2.9.1/types_aiobotocore_managedblockchain_query/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ManagedBlockchainQueryClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -145,15 +144,15 @@
         """
 
     async def get_token_balance(
         self,
         *,
         tokenIdentifier: TokenIdentifierTypeDef,
         ownerIdentifier: OwnerIdentifierTypeDef,
-        atBlockchainInstant: BlockchainInstantTypeDef = ...
+        atBlockchainInstant: BlockchainInstantTypeDef = ...,
     ) -> GetTokenBalanceOutputTypeDef:
         """
         Gets the balance of a specific token, including native tokens, for a given
         address (wallet or contract) on the
         blockchain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Client.get_token_balance)
@@ -184,15 +183,15 @@
 
     async def list_token_balances(
         self,
         *,
         tokenFilter: TokenFilterTypeDef,
         ownerFilter: OwnerFilterTypeDef = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListTokenBalancesOutputTypeDef:
         """
         This action returns the following for a given blockchain network: * Lists all
         token balances owned by an address (either a contract address or a wallet
         address).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Client.list_token_balances)
@@ -201,15 +200,15 @@
 
     async def list_transaction_events(
         self,
         *,
         transactionHash: str,
         network: QueryNetworkType,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListTransactionEventsOutputTypeDef:
         """
         An array of `TransactionEvent` objects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Client.list_transaction_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain_query/client/#list_transaction_events)
         """
@@ -219,15 +218,15 @@
         *,
         address: str,
         network: QueryNetworkType,
         fromBlockchainInstant: BlockchainInstantTypeDef = ...,
         toBlockchainInstant: BlockchainInstantTypeDef = ...,
         sort: ListTransactionsSortTypeDef = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListTransactionsOutputTypeDef:
         """
         Lists all of the transactions on a given wallet address or to a specific
         contract.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Client.list_transactions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain_query/client/#list_transactions)
```

### Comparing `types-aiobotocore-managedblockchain-query-2.9.0/types_aiobotocore_managedblockchain_query/client.pyi` & `types-aiobotocore-managedblockchain-query-2.9.1/types_aiobotocore_managedblockchain_query/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,15 @@
         """
 
     async def get_token_balance(
         self,
         *,
         tokenIdentifier: TokenIdentifierTypeDef,
         ownerIdentifier: OwnerIdentifierTypeDef,
-        atBlockchainInstant: BlockchainInstantTypeDef = ...
+        atBlockchainInstant: BlockchainInstantTypeDef = ...,
     ) -> GetTokenBalanceOutputTypeDef:
         """
         Gets the balance of a specific token, including native tokens, for a given
         address (wallet or contract) on the
         blockchain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Client.get_token_balance)
@@ -180,15 +180,15 @@
 
     async def list_token_balances(
         self,
         *,
         tokenFilter: TokenFilterTypeDef,
         ownerFilter: OwnerFilterTypeDef = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListTokenBalancesOutputTypeDef:
         """
         This action returns the following for a given blockchain network: * Lists all
         token balances owned by an address (either a contract address or a wallet
         address).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Client.list_token_balances)
@@ -197,15 +197,15 @@
 
     async def list_transaction_events(
         self,
         *,
         transactionHash: str,
         network: QueryNetworkType,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListTransactionEventsOutputTypeDef:
         """
         An array of `TransactionEvent` objects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Client.list_transaction_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain_query/client/#list_transaction_events)
         """
@@ -215,15 +215,15 @@
         *,
         address: str,
         network: QueryNetworkType,
         fromBlockchainInstant: BlockchainInstantTypeDef = ...,
         toBlockchainInstant: BlockchainInstantTypeDef = ...,
         sort: ListTransactionsSortTypeDef = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListTransactionsOutputTypeDef:
         """
         Lists all of the transactions on a given wallet address or to a specific
         contract.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Client.list_transactions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain_query/client/#list_transactions)
```

### Comparing `types-aiobotocore-managedblockchain-query-2.9.0/types_aiobotocore_managedblockchain_query/literals.py` & `types-aiobotocore-managedblockchain-query-2.9.1/types_aiobotocore_managedblockchain_query/literals.py`

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
     "ErrorTypeType",
     "ListAssetContractsPaginatorName",
     "ListTokenBalancesPaginatorName",
     "ListTransactionEventsPaginatorName",
     "ListTransactionsPaginatorName",
     "ListTransactionsSortByType",
@@ -35,15 +34,14 @@
     "ManagedBlockchainQueryServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ErrorTypeType = Literal["RESOURCE_NOT_FOUND_EXCEPTION", "VALIDATION_EXCEPTION"]
 ListAssetContractsPaginatorName = Literal["list_asset_contracts"]
 ListTokenBalancesPaginatorName = Literal["list_token_balances"]
 ListTransactionEventsPaginatorName = Literal["list_transaction_events"]
 ListTransactionsPaginatorName = Literal["list_transactions"]
 ListTransactionsSortByType = Literal["TRANSACTION_TIMESTAMP"]
 QueryNetworkType = Literal[
```

### Comparing `types-aiobotocore-managedblockchain-query-2.9.0/types_aiobotocore_managedblockchain_query/literals.pyi` & `types-aiobotocore-managedblockchain-query-2.9.1/types_aiobotocore_managedblockchain_query/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-managedblockchain-query-2.9.0/types_aiobotocore_managedblockchain_query/paginator.py` & `types-aiobotocore-managedblockchain-query-2.9.1/types_aiobotocore_managedblockchain_query/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,14 @@
 __all__ = (
     "ListAssetContractsPaginator",
     "ListTokenBalancesPaginator",
     "ListTransactionEventsPaginator",
     "ListTransactionsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -70,15 +69,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain_query/paginators/#listassetcontractspaginator)
     """
 
     def paginate(
         self,
         *,
         contractFilter: ContractFilterTypeDef,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAssetContractsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Paginator.ListAssetContracts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain_query/paginators/#listassetcontractspaginator)
         """
 
 
@@ -89,15 +88,15 @@
     """
 
     def paginate(
         self,
         *,
         tokenFilter: TokenFilterTypeDef,
         ownerFilter: OwnerFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTokenBalancesOutputPaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Paginator.ListTokenBalances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain_query/paginators/#listtokenbalancespaginator)
         """
 
 
@@ -108,15 +107,15 @@
     """
 
     def paginate(
         self,
         *,
         transactionHash: str,
         network: QueryNetworkType,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTransactionEventsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Paginator.ListTransactionEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain_query/paginators/#listtransactioneventspaginator)
         """
 
 
@@ -130,13 +129,13 @@
         self,
         *,
         address: str,
         network: QueryNetworkType,
         fromBlockchainInstant: BlockchainInstantPaginatorTypeDef = ...,
         toBlockchainInstant: BlockchainInstantPaginatorTypeDef = ...,
         sort: ListTransactionsSortTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTransactionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Paginator.ListTransactions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain_query/paginators/#listtransactionspaginator)
         """
```

### Comparing `types-aiobotocore-managedblockchain-query-2.9.0/types_aiobotocore_managedblockchain_query/paginator.pyi` & `types-aiobotocore-managedblockchain-query-2.9.1/types_aiobotocore_managedblockchain_query/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain_query/paginators/#listassetcontractspaginator)
     """
 
     def paginate(
         self,
         *,
         contractFilter: ContractFilterTypeDef,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAssetContractsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Paginator.ListAssetContracts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain_query/paginators/#listassetcontractspaginator)
         """
 
 class ListTokenBalancesPaginator(AioPaginator):
@@ -85,15 +85,15 @@
     """
 
     def paginate(
         self,
         *,
         tokenFilter: TokenFilterTypeDef,
         ownerFilter: OwnerFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTokenBalancesOutputPaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Paginator.ListTokenBalances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain_query/paginators/#listtokenbalancespaginator)
         """
 
 class ListTransactionEventsPaginator(AioPaginator):
@@ -103,15 +103,15 @@
     """
 
     def paginate(
         self,
         *,
         transactionHash: str,
         network: QueryNetworkType,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTransactionEventsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Paginator.ListTransactionEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain_query/paginators/#listtransactioneventspaginator)
         """
 
 class ListTransactionsPaginator(AioPaginator):
@@ -124,13 +124,13 @@
         self,
         *,
         address: str,
         network: QueryNetworkType,
         fromBlockchainInstant: BlockchainInstantPaginatorTypeDef = ...,
         toBlockchainInstant: BlockchainInstantPaginatorTypeDef = ...,
         sort: ListTransactionsSortTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTransactionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Paginator.ListTransactions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain_query/paginators/#listtransactionspaginator)
         """
```

### Comparing `types-aiobotocore-managedblockchain-query-2.9.0/types_aiobotocore_managedblockchain_query/type_defs.py` & `types-aiobotocore-managedblockchain-query-2.9.1/types_aiobotocore_managedblockchain_query/type_defs.py`

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
     "ContractIdentifierTypeDef",
     "OwnerIdentifierTypeDef",
     "TokenIdentifierTypeDef",
     "ResponseMetadataTypeDef",
     "BlockchainInstantPaginatorTypeDef",
     "TimestampTypeDef",
```

### Comparing `types-aiobotocore-managedblockchain-query-2.9.0/types_aiobotocore_managedblockchain_query/type_defs.pyi` & `types-aiobotocore-managedblockchain-query-2.9.1/types_aiobotocore_managedblockchain_query/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-managedblockchain-query-2.9.0/types_aiobotocore_managedblockchain_query.egg-info/PKG-INFO` & `types-aiobotocore-managedblockchain-query-2.9.1/types_aiobotocore_managedblockchain_query.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-managedblockchain-query
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ManagedBlockchainQuery 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ManagedBlockchainQuery 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain_query/
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
 
 <a id="types-aiobotocore-managedblockchain-query"></a>
 
 # types-aiobotocore-managedblockchain-query
 
 [![PyPI - types-aiobotocore-managedblockchain-query](https://img.shields.io/pypi/v/types-aiobotocore-managedblockchain-query.svg?color=blue)](https://pypi.org/project/types-aiobotocore-managedblockchain-query)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-managedblockchain-query.svg?color=blue)](https://pypi.org/project/types-aiobotocore-managedblockchain-query)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain_query/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-managedblockchain-query)](https://pepy.tech/project/types-aiobotocore-managedblockchain-query)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ManagedBlockchainQuery 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery)
+[aiobotocore.ManagedBlockchainQuery 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery)
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
 [types-aiobotocore-managedblockchain-query docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain_query/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-managedblockchain-query-2.9.0/types_aiobotocore_managedblockchain_query.egg-info/SOURCES.txt` & `types-aiobotocore-managedblockchain-query-2.9.1/types_aiobotocore_managedblockchain_query.egg-info/SOURCES.txt`

 * *Files identical despite different names*

