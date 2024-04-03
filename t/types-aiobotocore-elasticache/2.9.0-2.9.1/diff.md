# Comparing `tmp/types-aiobotocore-elasticache-2.9.0.tar.gz` & `tmp/types-aiobotocore-elasticache-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-elasticache-2.9.0.tar", last modified: Wed Dec 13 19:59:14 2023, max compression
+gzip compressed data, was "types-aiobotocore-elasticache-2.9.1.tar", last modified: Thu Jan 18 01:20:39 2024, max compression
```

## Comparing `types-aiobotocore-elasticache-2.9.0.tar` & `types-aiobotocore-elasticache-2.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:14.165772 types-aiobotocore-elasticache-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:45:39.000000 types-aiobotocore-elasticache-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    17753 2023-12-13 19:59:14.165772 types-aiobotocore-elasticache-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16174 2023-12-13 19:45:39.000000 types-aiobotocore-elasticache-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:14.165772 types-aiobotocore-elasticache-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2023-12-13 19:45:39.000000 types-aiobotocore-elasticache-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:14.165772 types-aiobotocore-elasticache-2.9.0/types_aiobotocore_elasticache/
--rw-r--r--   0 runner    (1001) docker     (127)     6253 2023-12-13 19:45:39.000000 types-aiobotocore-elasticache-2.9.0/types_aiobotocore_elasticache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6252 2023-12-13 19:45:39.000000 types-aiobotocore-elasticache-2.9.0/types_aiobotocore_elasticache/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      948 2023-12-13 19:45:39.000000 types-aiobotocore-elasticache-2.9.0/types_aiobotocore_elasticache/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    80392 2023-12-13 19:45:39.000000 types-aiobotocore-elasticache-2.9.0/types_aiobotocore_elasticache/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    80388 2023-12-13 19:45:39.000000 types-aiobotocore-elasticache-2.9.0/types_aiobotocore_elasticache/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    15236 2023-12-13 19:45:40.000000 types-aiobotocore-elasticache-2.9.0/types_aiobotocore_elasticache/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    15234 2023-12-13 19:45:39.000000 types-aiobotocore-elasticache-2.9.0/types_aiobotocore_elasticache/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    26198 2023-12-13 19:45:39.000000 types-aiobotocore-elasticache-2.9.0/types_aiobotocore_elasticache/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    26177 2023-12-13 19:45:39.000000 types-aiobotocore-elasticache-2.9.0/types_aiobotocore_elasticache/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:45:39.000000 types-aiobotocore-elasticache-2.9.0/types_aiobotocore_elasticache/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    91665 2023-12-13 19:45:42.000000 types-aiobotocore-elasticache-2.9.0/types_aiobotocore_elasticache/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    91664 2023-12-13 19:45:42.000000 types-aiobotocore-elasticache-2.9.0/types_aiobotocore_elasticache/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:45:39.000000 types-aiobotocore-elasticache-2.9.0/types_aiobotocore_elasticache/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5425 2023-12-13 19:45:39.000000 types-aiobotocore-elasticache-2.9.0/types_aiobotocore_elasticache/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5421 2023-12-13 19:45:39.000000 types-aiobotocore-elasticache-2.9.0/types_aiobotocore_elasticache/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:14.165772 types-aiobotocore-elasticache-2.9.0/types_aiobotocore_elasticache.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17753 2023-12-13 19:59:14.000000 types-aiobotocore-elasticache-2.9.0/types_aiobotocore_elasticache.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      970 2023-12-13 19:59:14.000000 types-aiobotocore-elasticache-2.9.0/types_aiobotocore_elasticache.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:14.000000 types-aiobotocore-elasticache-2.9.0/types_aiobotocore_elasticache.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:14.000000 types-aiobotocore-elasticache-2.9.0/types_aiobotocore_elasticache.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:14.000000 types-aiobotocore-elasticache-2.9.0/types_aiobotocore_elasticache.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-13 19:59:14.000000 types-aiobotocore-elasticache-2.9.0/types_aiobotocore_elasticache.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:39.045350 types-aiobotocore-elasticache-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:07:34.000000 types-aiobotocore-elasticache-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17773 2024-01-18 01:20:39.045350 types-aiobotocore-elasticache-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16174 2024-01-18 01:07:34.000000 types-aiobotocore-elasticache-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:39.045350 types-aiobotocore-elasticache-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-01-18 01:07:34.000000 types-aiobotocore-elasticache-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:39.045350 types-aiobotocore-elasticache-2.9.1/types_aiobotocore_elasticache/
+-rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-01-18 01:07:34.000000 types-aiobotocore-elasticache-2.9.1/types_aiobotocore_elasticache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-01-18 01:07:34.000000 types-aiobotocore-elasticache-2.9.1/types_aiobotocore_elasticache/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-01-18 01:07:34.000000 types-aiobotocore-elasticache-2.9.1/types_aiobotocore_elasticache/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80437 2024-01-18 01:07:36.000000 types-aiobotocore-elasticache-2.9.1/types_aiobotocore_elasticache/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80434 2024-01-18 01:07:34.000000 types-aiobotocore-elasticache-2.9.1/types_aiobotocore_elasticache/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    15234 2024-01-18 01:07:36.000000 types-aiobotocore-elasticache-2.9.1/types_aiobotocore_elasticache/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15234 2024-01-18 01:07:36.000000 types-aiobotocore-elasticache-2.9.1/types_aiobotocore_elasticache/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    26209 2024-01-18 01:07:36.000000 types-aiobotocore-elasticache-2.9.1/types_aiobotocore_elasticache/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26189 2024-01-18 01:07:36.000000 types-aiobotocore-elasticache-2.9.1/types_aiobotocore_elasticache/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:07:34.000000 types-aiobotocore-elasticache-2.9.1/types_aiobotocore_elasticache/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    91664 2024-01-18 01:07:38.000000 types-aiobotocore-elasticache-2.9.1/types_aiobotocore_elasticache/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91664 2024-01-18 01:07:37.000000 types-aiobotocore-elasticache-2.9.1/types_aiobotocore_elasticache/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:07:34.000000 types-aiobotocore-elasticache-2.9.1/types_aiobotocore_elasticache/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-01-18 01:07:36.000000 types-aiobotocore-elasticache-2.9.1/types_aiobotocore_elasticache/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-01-18 01:07:36.000000 types-aiobotocore-elasticache-2.9.1/types_aiobotocore_elasticache/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:39.045350 types-aiobotocore-elasticache-2.9.1/types_aiobotocore_elasticache.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17773 2024-01-18 01:20:39.000000 types-aiobotocore-elasticache-2.9.1/types_aiobotocore_elasticache.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-01-18 01:20:39.000000 types-aiobotocore-elasticache-2.9.1/types_aiobotocore_elasticache.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:39.000000 types-aiobotocore-elasticache-2.9.1/types_aiobotocore_elasticache.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:39.000000 types-aiobotocore-elasticache-2.9.1/types_aiobotocore_elasticache.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:39.000000 types-aiobotocore-elasticache-2.9.1/types_aiobotocore_elasticache.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-01-18 01:20:39.000000 types-aiobotocore-elasticache-2.9.1/types_aiobotocore_elasticache.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-elasticache-2.9.0/LICENSE` & `types-aiobotocore-elasticache-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-elasticache-2.9.0/PKG-INFO` & `types-aiobotocore-elasticache-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-elasticache
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ElastiCache 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ElastiCache 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/
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
 
 <a id="types-aiobotocore-elasticache"></a>
 
 # types-aiobotocore-elasticache
 
 [![PyPI - types-aiobotocore-elasticache](https://img.shields.io/pypi/v/types-aiobotocore-elasticache.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elasticache)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-elasticache.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elasticache)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-elasticache)](https://pepy.tech/project/types-aiobotocore-elasticache)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ElastiCache 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache)
+[aiobotocore.ElastiCache 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache)
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
 [types-aiobotocore-elasticache docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-elasticache-2.9.0/README.md` & `types-aiobotocore-elasticache-2.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-elasticache.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elasticache)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-elasticache)](https://pepy.tech/project/types-aiobotocore-elasticache)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ElastiCache 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache)
+[aiobotocore.ElastiCache 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache)
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
 [types-aiobotocore-elasticache docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-elasticache-2.9.0/setup.py` & `types-aiobotocore-elasticache-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-elasticache",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_elasticache"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ElastiCache 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.ElastiCache 2.9.1 service generated with"
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
     keywords="aiobotocore elasticache type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_elasticache": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-elasticache-2.9.0/types_aiobotocore_elasticache/__init__.py` & `types-aiobotocore-elasticache-2.9.1/types_aiobotocore_elasticache/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,14 @@
     CacheClusterDeletedWaiter,
     ReplicationGroupAvailableWaiter,
     ReplicationGroupDeletedWaiter,
 )
 
 Client = ElastiCacheClient
 
-
 __all__ = (
     "CacheClusterAvailableWaiter",
     "CacheClusterDeletedWaiter",
     "Client",
     "DescribeCacheClustersPaginator",
     "DescribeCacheEngineVersionsPaginator",
     "DescribeCacheParameterGroupsPaginator",
```

### Comparing `types-aiobotocore-elasticache-2.9.0/types_aiobotocore_elasticache/__init__.pyi` & `types-aiobotocore-elasticache-2.9.1/types_aiobotocore_elasticache/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elasticache-2.9.0/types_aiobotocore_elasticache/__main__.py` & `types-aiobotocore-elasticache-2.9.1/types_aiobotocore_elasticache/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ElastiCache 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.ElastiCache 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache\nOther"
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

### Comparing `types-aiobotocore-elasticache-2.9.0/types_aiobotocore_elasticache/client.py` & `types-aiobotocore-elasticache-2.9.1/types_aiobotocore_elasticache/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ElastiCacheClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -266,43 +265,43 @@
         """
 
     async def authorize_cache_security_group_ingress(
         self,
         *,
         CacheSecurityGroupName: str,
         EC2SecurityGroupName: str,
-        EC2SecurityGroupOwnerId: str
+        EC2SecurityGroupOwnerId: str,
     ) -> AuthorizeCacheSecurityGroupIngressResultTypeDef:
         """
         Allows network ingress to a cache security group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.authorize_cache_security_group_ingress)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#authorize_cache_security_group_ingress)
         """
 
     async def batch_apply_update_action(
         self,
         *,
         ServiceUpdateName: str,
         ReplicationGroupIds: Sequence[str] = ...,
-        CacheClusterIds: Sequence[str] = ...
+        CacheClusterIds: Sequence[str] = ...,
     ) -> UpdateActionResultsMessageTypeDef:
         """
         Apply the service update.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.batch_apply_update_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#batch_apply_update_action)
         """
 
     async def batch_stop_update_action(
         self,
         *,
         ServiceUpdateName: str,
         ReplicationGroupIds: Sequence[str] = ...,
-        CacheClusterIds: Sequence[str] = ...
+        CacheClusterIds: Sequence[str] = ...,
     ) -> UpdateActionResultsMessageTypeDef:
         """
         Stop the service update.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.batch_stop_update_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#batch_stop_update_action)
         """
@@ -335,15 +334,15 @@
 
     async def copy_serverless_cache_snapshot(
         self,
         *,
         SourceServerlessCacheSnapshotName: str,
         TargetServerlessCacheSnapshotName: str,
         KmsKeyId: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CopyServerlessCacheSnapshotResponseTypeDef:
         """
         Creates a copy of an existing serverless cache’s snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.copy_serverless_cache_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#copy_serverless_cache_snapshot)
         """
@@ -351,15 +350,15 @@
     async def copy_snapshot(
         self,
         *,
         SourceSnapshotName: str,
         TargetSnapshotName: str,
         TargetBucket: str = ...,
         KmsKeyId: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CopySnapshotResultTypeDef:
         """
         Makes a copy of an existing snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.copy_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#copy_snapshot)
         """
@@ -392,30 +391,30 @@
         AuthToken: str = ...,
         OutpostMode: OutpostModeType = ...,
         PreferredOutpostArn: str = ...,
         PreferredOutpostArns: Sequence[str] = ...,
         LogDeliveryConfigurations: Sequence[LogDeliveryConfigurationRequestTypeDef] = ...,
         TransitEncryptionEnabled: bool = ...,
         NetworkType: NetworkTypeType = ...,
-        IpDiscovery: IpDiscoveryType = ...
+        IpDiscovery: IpDiscoveryType = ...,
     ) -> CreateCacheClusterResultTypeDef:
         """
         Creates a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.create_cache_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#create_cache_cluster)
         """
 
     async def create_cache_parameter_group(
         self,
         *,
         CacheParameterGroupName: str,
         CacheParameterGroupFamily: str,
         Description: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateCacheParameterGroupResultTypeDef:
         """
         Creates a new Amazon ElastiCache cache parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.create_cache_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#create_cache_parameter_group)
         """
@@ -432,29 +431,29 @@
 
     async def create_cache_subnet_group(
         self,
         *,
         CacheSubnetGroupName: str,
         CacheSubnetGroupDescription: str,
         SubnetIds: Sequence[str],
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateCacheSubnetGroupResultTypeDef:
         """
         Creates a new cache subnet group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.create_cache_subnet_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#create_cache_subnet_group)
         """
 
     async def create_global_replication_group(
         self,
         *,
         GlobalReplicationGroupIdSuffix: str,
         PrimaryReplicationGroupId: str,
-        GlobalReplicationGroupDescription: str = ...
+        GlobalReplicationGroupDescription: str = ...,
     ) -> CreateGlobalReplicationGroupResultTypeDef:
         """
         Global Datastore for Redis offers fully managed, fast, reliable and secure
         cross-region
         replication.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.create_global_replication_group)
@@ -498,15 +497,15 @@
         UserGroupIds: Sequence[str] = ...,
         LogDeliveryConfigurations: Sequence[LogDeliveryConfigurationRequestTypeDef] = ...,
         DataTieringEnabled: bool = ...,
         NetworkType: NetworkTypeType = ...,
         IpDiscovery: IpDiscoveryType = ...,
         TransitEncryptionMode: TransitEncryptionModeType = ...,
         ClusterMode: ClusterModeType = ...,
-        ServerlessCacheSnapshotName: str = ...
+        ServerlessCacheSnapshotName: str = ...,
     ) -> CreateReplicationGroupResultTypeDef:
         """
         Creates a Redis (cluster mode disabled) or a Redis (cluster mode enabled)
         replication
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.create_replication_group)
@@ -524,30 +523,30 @@
         KmsKeyId: str = ...,
         SecurityGroupIds: Sequence[str] = ...,
         SnapshotArnsToRestore: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         UserGroupId: str = ...,
         SubnetIds: Sequence[str] = ...,
         SnapshotRetentionLimit: int = ...,
-        DailySnapshotTime: str = ...
+        DailySnapshotTime: str = ...,
     ) -> CreateServerlessCacheResponseTypeDef:
         """
         Creates a serverless cache.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.create_serverless_cache)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#create_serverless_cache)
         """
 
     async def create_serverless_cache_snapshot(
         self,
         *,
         ServerlessCacheSnapshotName: str,
         ServerlessCacheName: str,
         KmsKeyId: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateServerlessCacheSnapshotResponseTypeDef:
         """
         This API creates a copy of an entire ServerlessCache at a specific moment in
         time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.create_serverless_cache_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#create_serverless_cache_snapshot)
@@ -556,15 +555,15 @@
     async def create_snapshot(
         self,
         *,
         SnapshotName: str,
         ReplicationGroupId: str = ...,
         CacheClusterId: str = ...,
         KmsKeyId: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateSnapshotResultTypeDef:
         """
         Creates a copy of an entire cluster or replication group at a specific moment
         in
         time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.create_snapshot)
@@ -577,30 +576,30 @@
         UserId: str,
         UserName: str,
         Engine: str,
         AccessString: str,
         Passwords: Sequence[str] = ...,
         NoPasswordRequired: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        AuthenticationMode: AuthenticationModeTypeDef = ...
+        AuthenticationMode: AuthenticationModeTypeDef = ...,
     ) -> UserResponseTypeDef:
         """
         For Redis engine version 6.0 onwards: Creates a Redis user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.create_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#create_user)
         """
 
     async def create_user_group(
         self,
         *,
         UserGroupId: str,
         Engine: str,
         UserIds: Sequence[str] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> UserGroupResponseTypeDef:
         """
         For Redis engine version 6.0 onwards: Creates a Redis user group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.create_user_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#create_user_group)
         """
@@ -608,15 +607,15 @@
     async def decrease_node_groups_in_global_replication_group(
         self,
         *,
         GlobalReplicationGroupId: str,
         NodeGroupCount: int,
         ApplyImmediately: bool,
         GlobalNodeGroupsToRemove: Sequence[str] = ...,
-        GlobalNodeGroupsToRetain: Sequence[str] = ...
+        GlobalNodeGroupsToRetain: Sequence[str] = ...,
     ) -> DecreaseNodeGroupsInGlobalReplicationGroupResultTypeDef:
         """
         Decreases the number of node groups in a Global datastore See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/elasticache-2015-02-02/DecreaseNodeGroupsInGlobalReplicationGroup).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.decrease_node_groups_in_global_replication_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#decrease_node_groups_in_global_replication_group)
@@ -625,15 +624,15 @@
     async def decrease_replica_count(
         self,
         *,
         ReplicationGroupId: str,
         ApplyImmediately: bool,
         NewReplicaCount: int = ...,
         ReplicaConfiguration: Sequence[ConfigureShardTypeDef] = ...,
-        ReplicasToRemove: Sequence[str] = ...
+        ReplicasToRemove: Sequence[str] = ...,
     ) -> DecreaseReplicaCountResultTypeDef:
         """
         Dynamically decreases the number of replicas in a Redis (cluster mode disabled)
         replication group or the number of replica nodes in one or more node groups
         (shards) of a Redis (cluster mode enabled) replication
         group.
 
@@ -695,15 +694,15 @@
         """
 
     async def delete_replication_group(
         self,
         *,
         ReplicationGroupId: str,
         RetainPrimaryCluster: bool = ...,
-        FinalSnapshotIdentifier: str = ...
+        FinalSnapshotIdentifier: str = ...,
     ) -> DeleteReplicationGroupResultTypeDef:
         """
         Deletes an existing replication group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.delete_replication_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#delete_replication_group)
         """
@@ -755,15 +754,15 @@
     async def describe_cache_clusters(
         self,
         *,
         CacheClusterId: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         ShowCacheNodeInfo: bool = ...,
-        ShowCacheClustersNotInReplicationGroups: bool = ...
+        ShowCacheClustersNotInReplicationGroups: bool = ...,
     ) -> CacheClusterMessageTypeDef:
         """
         Returns information about all provisioned clusters if no cluster identifier is
         specified, or about a specific cache cluster if a cluster identifier is
         supplied.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.describe_cache_clusters)
@@ -774,15 +773,15 @@
         self,
         *,
         Engine: str = ...,
         EngineVersion: str = ...,
         CacheParameterGroupFamily: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
-        DefaultOnly: bool = ...
+        DefaultOnly: bool = ...,
     ) -> CacheEngineVersionMessageTypeDef:
         """
         Returns a list of the available cache engines and their versions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.describe_cache_engine_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#describe_cache_engine_versions)
         """
@@ -799,15 +798,15 @@
 
     async def describe_cache_parameters(
         self,
         *,
         CacheParameterGroupName: str,
         Source: str = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> CacheParameterGroupDetailsTypeDef:
         """
         Returns the detailed parameter list for a particular cache parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.describe_cache_parameters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#describe_cache_parameters)
         """
@@ -849,15 +848,15 @@
         *,
         SourceIdentifier: str = ...,
         SourceType: SourceTypeType = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         Duration: int = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> EventsMessageTypeDef:
         """
         Returns events related to clusters, cache security groups, and cache parameter
         groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.describe_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#describe_events)
@@ -865,15 +864,15 @@
 
     async def describe_global_replication_groups(
         self,
         *,
         GlobalReplicationGroupId: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
-        ShowMemberInfo: bool = ...
+        ShowMemberInfo: bool = ...,
     ) -> DescribeGlobalReplicationGroupsResultTypeDef:
         """
         Returns information about a particular global replication group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.describe_global_replication_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#describe_global_replication_groups)
         """
@@ -894,15 +893,15 @@
         ReservedCacheNodeId: str = ...,
         ReservedCacheNodesOfferingId: str = ...,
         CacheNodeType: str = ...,
         Duration: str = ...,
         ProductDescription: str = ...,
         OfferingType: str = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> ReservedCacheNodeMessageTypeDef:
         """
         Returns information about reserved cache nodes for this account, or about a
         specified reserved cache
         node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.describe_reserved_cache_nodes)
@@ -914,15 +913,15 @@
         *,
         ReservedCacheNodesOfferingId: str = ...,
         CacheNodeType: str = ...,
         Duration: str = ...,
         ProductDescription: str = ...,
         OfferingType: str = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> ReservedCacheNodesOfferingMessageTypeDef:
         """
         Lists available reserved cache node offerings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.describe_reserved_cache_nodes_offerings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#describe_reserved_cache_nodes_offerings)
         """
@@ -930,15 +929,15 @@
     async def describe_serverless_cache_snapshots(
         self,
         *,
         ServerlessCacheName: str = ...,
         ServerlessCacheSnapshotName: str = ...,
         SnapshotType: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeServerlessCacheSnapshotsResponseTypeDef:
         """
         Returns information about serverless cache snapshots.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.describe_serverless_cache_snapshots)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#describe_serverless_cache_snapshots)
         """
@@ -955,15 +954,15 @@
 
     async def describe_service_updates(
         self,
         *,
         ServiceUpdateName: str = ...,
         ServiceUpdateStatus: Sequence[ServiceUpdateStatusType] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> ServiceUpdatesMessageTypeDef:
         """
         Returns details of the service updates See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/elasticache-2015-02-02/DescribeServiceUpdates).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.describe_service_updates)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#describe_service_updates)
@@ -974,15 +973,15 @@
         *,
         ReplicationGroupId: str = ...,
         CacheClusterId: str = ...,
         SnapshotName: str = ...,
         SnapshotSource: str = ...,
         Marker: str = ...,
         MaxRecords: int = ...,
-        ShowNodeGroupConfig: bool = ...
+        ShowNodeGroupConfig: bool = ...,
     ) -> DescribeSnapshotsListMessageTypeDef:
         """
         Returns information about cluster or replication group snapshots.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.describe_snapshots)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#describe_snapshots)
         """
@@ -995,15 +994,15 @@
         CacheClusterIds: Sequence[str] = ...,
         Engine: str = ...,
         ServiceUpdateStatus: Sequence[ServiceUpdateStatusType] = ...,
         ServiceUpdateTimeRange: TimeRangeFilterTypeDef = ...,
         UpdateActionStatus: Sequence[UpdateActionStatusType] = ...,
         ShowNodeLevelUpdateStatus: bool = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> UpdateActionsMessageTypeDef:
         """
         Returns details of the update actions See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/elasticache-2015-02-02/DescribeUpdateActions).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.describe_update_actions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#describe_update_actions)
@@ -1022,15 +1021,15 @@
     async def describe_users(
         self,
         *,
         Engine: str = ...,
         UserId: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DescribeUsersResultTypeDef:
         """
         Returns a list of users.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.describe_users)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#describe_users)
         """
@@ -1084,15 +1083,15 @@
 
     async def increase_node_groups_in_global_replication_group(
         self,
         *,
         GlobalReplicationGroupId: str,
         NodeGroupCount: int,
         ApplyImmediately: bool,
-        RegionalConfigurations: Sequence[RegionalConfigurationTypeDef] = ...
+        RegionalConfigurations: Sequence[RegionalConfigurationTypeDef] = ...,
     ) -> IncreaseNodeGroupsInGlobalReplicationGroupResultTypeDef:
         """
         Increase the number of node groups in the Global datastore See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/elasticache-2015-02-02/IncreaseNodeGroupsInGlobalReplicationGroup).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.increase_node_groups_in_global_replication_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#increase_node_groups_in_global_replication_group)
@@ -1100,15 +1099,15 @@
 
     async def increase_replica_count(
         self,
         *,
         ReplicationGroupId: str,
         ApplyImmediately: bool,
         NewReplicaCount: int = ...,
-        ReplicaConfiguration: Sequence[ConfigureShardTypeDef] = ...
+        ReplicaConfiguration: Sequence[ConfigureShardTypeDef] = ...,
     ) -> IncreaseReplicaCountResultTypeDef:
         """
         Dynamically increases the number of replicas in a Redis (cluster mode disabled)
         replication group or the number of replica nodes in one or more node groups
         (shards) of a Redis (cluster mode enabled) replication
         group.
 
@@ -1155,42 +1154,42 @@
         AutoMinorVersionUpgrade: bool = ...,
         SnapshotRetentionLimit: int = ...,
         SnapshotWindow: str = ...,
         CacheNodeType: str = ...,
         AuthToken: str = ...,
         AuthTokenUpdateStrategy: AuthTokenUpdateStrategyTypeType = ...,
         LogDeliveryConfigurations: Sequence[LogDeliveryConfigurationRequestTypeDef] = ...,
-        IpDiscovery: IpDiscoveryType = ...
+        IpDiscovery: IpDiscoveryType = ...,
     ) -> ModifyCacheClusterResultTypeDef:
         """
         Modifies the settings for a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.modify_cache_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#modify_cache_cluster)
         """
 
     async def modify_cache_parameter_group(
         self,
         *,
         CacheParameterGroupName: str,
-        ParameterNameValues: Sequence[ParameterNameValueTypeDef]
+        ParameterNameValues: Sequence[ParameterNameValueTypeDef],
     ) -> CacheParameterGroupNameMessageTypeDef:
         """
         Modifies the parameters of a cache parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.modify_cache_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#modify_cache_parameter_group)
         """
 
     async def modify_cache_subnet_group(
         self,
         *,
         CacheSubnetGroupName: str,
         CacheSubnetGroupDescription: str = ...,
-        SubnetIds: Sequence[str] = ...
+        SubnetIds: Sequence[str] = ...,
     ) -> ModifyCacheSubnetGroupResultTypeDef:
         """
         Modifies an existing cache subnet group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.modify_cache_subnet_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#modify_cache_subnet_group)
         """
@@ -1200,15 +1199,15 @@
         *,
         GlobalReplicationGroupId: str,
         ApplyImmediately: bool,
         CacheNodeType: str = ...,
         EngineVersion: str = ...,
         CacheParameterGroupName: str = ...,
         GlobalReplicationGroupDescription: str = ...,
-        AutomaticFailoverEnabled: bool = ...
+        AutomaticFailoverEnabled: bool = ...,
     ) -> ModifyGlobalReplicationGroupResultTypeDef:
         """
         Modifies the settings for a Global datastore.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.modify_global_replication_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#modify_global_replication_group)
         """
@@ -1240,15 +1239,15 @@
         UserGroupIdsToAdd: Sequence[str] = ...,
         UserGroupIdsToRemove: Sequence[str] = ...,
         RemoveUserGroups: bool = ...,
         LogDeliveryConfigurations: Sequence[LogDeliveryConfigurationRequestTypeDef] = ...,
         IpDiscovery: IpDiscoveryType = ...,
         TransitEncryptionEnabled: bool = ...,
         TransitEncryptionMode: TransitEncryptionModeType = ...,
-        ClusterMode: ClusterModeType = ...
+        ClusterMode: ClusterModeType = ...,
     ) -> ModifyReplicationGroupResultTypeDef:
         """
         Modifies the settings for a replication group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.modify_replication_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#modify_replication_group)
         """
@@ -1257,15 +1256,15 @@
         self,
         *,
         ReplicationGroupId: str,
         NodeGroupCount: int,
         ApplyImmediately: bool,
         ReshardingConfiguration: Sequence[ReshardingConfigurationTypeDef] = ...,
         NodeGroupsToRemove: Sequence[str] = ...,
-        NodeGroupsToRetain: Sequence[str] = ...
+        NodeGroupsToRetain: Sequence[str] = ...,
     ) -> ModifyReplicationGroupShardConfigurationResultTypeDef:
         """
         Modifies a replication group's shards (node groups) by allowing you to add
         shards, remove shards, or rebalance the keyspaces among existing
         shards.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.modify_replication_group_shard_configuration)
@@ -1278,15 +1277,15 @@
         ServerlessCacheName: str,
         Description: str = ...,
         CacheUsageLimits: CacheUsageLimitsTypeDef = ...,
         RemoveUserGroup: bool = ...,
         UserGroupId: str = ...,
         SecurityGroupIds: Sequence[str] = ...,
         SnapshotRetentionLimit: int = ...,
-        DailySnapshotTime: str = ...
+        DailySnapshotTime: str = ...,
     ) -> ModifyServerlessCacheResponseTypeDef:
         """
         This API modifies the attributes of a serverless cache.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.modify_serverless_cache)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#modify_serverless_cache)
         """
@@ -1295,44 +1294,44 @@
         self,
         *,
         UserId: str,
         AccessString: str = ...,
         AppendAccessString: str = ...,
         Passwords: Sequence[str] = ...,
         NoPasswordRequired: bool = ...,
-        AuthenticationMode: AuthenticationModeTypeDef = ...
+        AuthenticationMode: AuthenticationModeTypeDef = ...,
     ) -> UserResponseTypeDef:
         """
         Changes user password(s) and/or access string.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.modify_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#modify_user)
         """
 
     async def modify_user_group(
         self,
         *,
         UserGroupId: str,
         UserIdsToAdd: Sequence[str] = ...,
-        UserIdsToRemove: Sequence[str] = ...
+        UserIdsToRemove: Sequence[str] = ...,
     ) -> UserGroupResponseTypeDef:
         """
         Changes the list of users that belong to the user group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.modify_user_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#modify_user_group)
         """
 
     async def purchase_reserved_cache_nodes_offering(
         self,
         *,
         ReservedCacheNodesOfferingId: str,
         ReservedCacheNodeId: str = ...,
         CacheNodeCount: int = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> PurchaseReservedCacheNodesOfferingResultTypeDef:
         """
         Allows you to purchase a reserved cache node offering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.purchase_reserved_cache_nodes_offering)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#purchase_reserved_cache_nodes_offering)
         """
@@ -1369,15 +1368,15 @@
         """
 
     async def reset_cache_parameter_group(
         self,
         *,
         CacheParameterGroupName: str,
         ResetAllParameters: bool = ...,
-        ParameterNameValues: Sequence[ParameterNameValueTypeDef] = ...
+        ParameterNameValues: Sequence[ParameterNameValueTypeDef] = ...,
     ) -> CacheParameterGroupNameMessageTypeDef:
         """
         Modifies the parameters of a cache parameter group to the engine or system
         default
         value.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.reset_cache_parameter_group)
@@ -1385,28 +1384,28 @@
         """
 
     async def revoke_cache_security_group_ingress(
         self,
         *,
         CacheSecurityGroupName: str,
         EC2SecurityGroupName: str,
-        EC2SecurityGroupOwnerId: str
+        EC2SecurityGroupOwnerId: str,
     ) -> RevokeCacheSecurityGroupIngressResultTypeDef:
         """
         Revokes ingress from a cache security group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.revoke_cache_security_group_ingress)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#revoke_cache_security_group_ingress)
         """
 
     async def start_migration(
         self,
         *,
         ReplicationGroupId: str,
-        CustomerNodeEndpointList: Sequence[CustomerNodeEndpointTypeDef]
+        CustomerNodeEndpointList: Sequence[CustomerNodeEndpointTypeDef],
     ) -> StartMigrationResponseTypeDef:
         """
         Start the migration of data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.start_migration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#start_migration)
         """
@@ -1424,15 +1423,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#test_failover)
         """
 
     async def test_migration(
         self,
         *,
         ReplicationGroupId: str,
-        CustomerNodeEndpointList: Sequence[CustomerNodeEndpointTypeDef]
+        CustomerNodeEndpointList: Sequence[CustomerNodeEndpointTypeDef],
     ) -> TestMigrationResponseTypeDef:
         """
         Async API to test connection between source and target replication group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.test_migration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#test_migration)
         """
```

### Comparing `types-aiobotocore-elasticache-2.9.0/types_aiobotocore_elasticache/client.pyi` & `types-aiobotocore-elasticache-2.9.1/types_aiobotocore_elasticache/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -262,43 +262,43 @@
         """
 
     async def authorize_cache_security_group_ingress(
         self,
         *,
         CacheSecurityGroupName: str,
         EC2SecurityGroupName: str,
-        EC2SecurityGroupOwnerId: str
+        EC2SecurityGroupOwnerId: str,
     ) -> AuthorizeCacheSecurityGroupIngressResultTypeDef:
         """
         Allows network ingress to a cache security group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.authorize_cache_security_group_ingress)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#authorize_cache_security_group_ingress)
         """
 
     async def batch_apply_update_action(
         self,
         *,
         ServiceUpdateName: str,
         ReplicationGroupIds: Sequence[str] = ...,
-        CacheClusterIds: Sequence[str] = ...
+        CacheClusterIds: Sequence[str] = ...,
     ) -> UpdateActionResultsMessageTypeDef:
         """
         Apply the service update.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.batch_apply_update_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#batch_apply_update_action)
         """
 
     async def batch_stop_update_action(
         self,
         *,
         ServiceUpdateName: str,
         ReplicationGroupIds: Sequence[str] = ...,
-        CacheClusterIds: Sequence[str] = ...
+        CacheClusterIds: Sequence[str] = ...,
     ) -> UpdateActionResultsMessageTypeDef:
         """
         Stop the service update.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.batch_stop_update_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#batch_stop_update_action)
         """
@@ -331,15 +331,15 @@
 
     async def copy_serverless_cache_snapshot(
         self,
         *,
         SourceServerlessCacheSnapshotName: str,
         TargetServerlessCacheSnapshotName: str,
         KmsKeyId: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CopyServerlessCacheSnapshotResponseTypeDef:
         """
         Creates a copy of an existing serverless cache’s snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.copy_serverless_cache_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#copy_serverless_cache_snapshot)
         """
@@ -347,15 +347,15 @@
     async def copy_snapshot(
         self,
         *,
         SourceSnapshotName: str,
         TargetSnapshotName: str,
         TargetBucket: str = ...,
         KmsKeyId: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CopySnapshotResultTypeDef:
         """
         Makes a copy of an existing snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.copy_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#copy_snapshot)
         """
@@ -388,30 +388,30 @@
         AuthToken: str = ...,
         OutpostMode: OutpostModeType = ...,
         PreferredOutpostArn: str = ...,
         PreferredOutpostArns: Sequence[str] = ...,
         LogDeliveryConfigurations: Sequence[LogDeliveryConfigurationRequestTypeDef] = ...,
         TransitEncryptionEnabled: bool = ...,
         NetworkType: NetworkTypeType = ...,
-        IpDiscovery: IpDiscoveryType = ...
+        IpDiscovery: IpDiscoveryType = ...,
     ) -> CreateCacheClusterResultTypeDef:
         """
         Creates a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.create_cache_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#create_cache_cluster)
         """
 
     async def create_cache_parameter_group(
         self,
         *,
         CacheParameterGroupName: str,
         CacheParameterGroupFamily: str,
         Description: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateCacheParameterGroupResultTypeDef:
         """
         Creates a new Amazon ElastiCache cache parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.create_cache_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#create_cache_parameter_group)
         """
@@ -428,29 +428,29 @@
 
     async def create_cache_subnet_group(
         self,
         *,
         CacheSubnetGroupName: str,
         CacheSubnetGroupDescription: str,
         SubnetIds: Sequence[str],
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateCacheSubnetGroupResultTypeDef:
         """
         Creates a new cache subnet group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.create_cache_subnet_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#create_cache_subnet_group)
         """
 
     async def create_global_replication_group(
         self,
         *,
         GlobalReplicationGroupIdSuffix: str,
         PrimaryReplicationGroupId: str,
-        GlobalReplicationGroupDescription: str = ...
+        GlobalReplicationGroupDescription: str = ...,
     ) -> CreateGlobalReplicationGroupResultTypeDef:
         """
         Global Datastore for Redis offers fully managed, fast, reliable and secure
         cross-region
         replication.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.create_global_replication_group)
@@ -494,15 +494,15 @@
         UserGroupIds: Sequence[str] = ...,
         LogDeliveryConfigurations: Sequence[LogDeliveryConfigurationRequestTypeDef] = ...,
         DataTieringEnabled: bool = ...,
         NetworkType: NetworkTypeType = ...,
         IpDiscovery: IpDiscoveryType = ...,
         TransitEncryptionMode: TransitEncryptionModeType = ...,
         ClusterMode: ClusterModeType = ...,
-        ServerlessCacheSnapshotName: str = ...
+        ServerlessCacheSnapshotName: str = ...,
     ) -> CreateReplicationGroupResultTypeDef:
         """
         Creates a Redis (cluster mode disabled) or a Redis (cluster mode enabled)
         replication
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.create_replication_group)
@@ -520,30 +520,30 @@
         KmsKeyId: str = ...,
         SecurityGroupIds: Sequence[str] = ...,
         SnapshotArnsToRestore: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         UserGroupId: str = ...,
         SubnetIds: Sequence[str] = ...,
         SnapshotRetentionLimit: int = ...,
-        DailySnapshotTime: str = ...
+        DailySnapshotTime: str = ...,
     ) -> CreateServerlessCacheResponseTypeDef:
         """
         Creates a serverless cache.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.create_serverless_cache)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#create_serverless_cache)
         """
 
     async def create_serverless_cache_snapshot(
         self,
         *,
         ServerlessCacheSnapshotName: str,
         ServerlessCacheName: str,
         KmsKeyId: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateServerlessCacheSnapshotResponseTypeDef:
         """
         This API creates a copy of an entire ServerlessCache at a specific moment in
         time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.create_serverless_cache_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#create_serverless_cache_snapshot)
@@ -552,15 +552,15 @@
     async def create_snapshot(
         self,
         *,
         SnapshotName: str,
         ReplicationGroupId: str = ...,
         CacheClusterId: str = ...,
         KmsKeyId: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateSnapshotResultTypeDef:
         """
         Creates a copy of an entire cluster or replication group at a specific moment
         in
         time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.create_snapshot)
@@ -573,30 +573,30 @@
         UserId: str,
         UserName: str,
         Engine: str,
         AccessString: str,
         Passwords: Sequence[str] = ...,
         NoPasswordRequired: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        AuthenticationMode: AuthenticationModeTypeDef = ...
+        AuthenticationMode: AuthenticationModeTypeDef = ...,
     ) -> UserResponseTypeDef:
         """
         For Redis engine version 6.0 onwards: Creates a Redis user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.create_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#create_user)
         """
 
     async def create_user_group(
         self,
         *,
         UserGroupId: str,
         Engine: str,
         UserIds: Sequence[str] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> UserGroupResponseTypeDef:
         """
         For Redis engine version 6.0 onwards: Creates a Redis user group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.create_user_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#create_user_group)
         """
@@ -604,15 +604,15 @@
     async def decrease_node_groups_in_global_replication_group(
         self,
         *,
         GlobalReplicationGroupId: str,
         NodeGroupCount: int,
         ApplyImmediately: bool,
         GlobalNodeGroupsToRemove: Sequence[str] = ...,
-        GlobalNodeGroupsToRetain: Sequence[str] = ...
+        GlobalNodeGroupsToRetain: Sequence[str] = ...,
     ) -> DecreaseNodeGroupsInGlobalReplicationGroupResultTypeDef:
         """
         Decreases the number of node groups in a Global datastore See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/elasticache-2015-02-02/DecreaseNodeGroupsInGlobalReplicationGroup).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.decrease_node_groups_in_global_replication_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#decrease_node_groups_in_global_replication_group)
@@ -621,15 +621,15 @@
     async def decrease_replica_count(
         self,
         *,
         ReplicationGroupId: str,
         ApplyImmediately: bool,
         NewReplicaCount: int = ...,
         ReplicaConfiguration: Sequence[ConfigureShardTypeDef] = ...,
-        ReplicasToRemove: Sequence[str] = ...
+        ReplicasToRemove: Sequence[str] = ...,
     ) -> DecreaseReplicaCountResultTypeDef:
         """
         Dynamically decreases the number of replicas in a Redis (cluster mode disabled)
         replication group or the number of replica nodes in one or more node groups
         (shards) of a Redis (cluster mode enabled) replication
         group.
 
@@ -691,15 +691,15 @@
         """
 
     async def delete_replication_group(
         self,
         *,
         ReplicationGroupId: str,
         RetainPrimaryCluster: bool = ...,
-        FinalSnapshotIdentifier: str = ...
+        FinalSnapshotIdentifier: str = ...,
     ) -> DeleteReplicationGroupResultTypeDef:
         """
         Deletes an existing replication group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.delete_replication_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#delete_replication_group)
         """
@@ -751,15 +751,15 @@
     async def describe_cache_clusters(
         self,
         *,
         CacheClusterId: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         ShowCacheNodeInfo: bool = ...,
-        ShowCacheClustersNotInReplicationGroups: bool = ...
+        ShowCacheClustersNotInReplicationGroups: bool = ...,
     ) -> CacheClusterMessageTypeDef:
         """
         Returns information about all provisioned clusters if no cluster identifier is
         specified, or about a specific cache cluster if a cluster identifier is
         supplied.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.describe_cache_clusters)
@@ -770,15 +770,15 @@
         self,
         *,
         Engine: str = ...,
         EngineVersion: str = ...,
         CacheParameterGroupFamily: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
-        DefaultOnly: bool = ...
+        DefaultOnly: bool = ...,
     ) -> CacheEngineVersionMessageTypeDef:
         """
         Returns a list of the available cache engines and their versions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.describe_cache_engine_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#describe_cache_engine_versions)
         """
@@ -795,15 +795,15 @@
 
     async def describe_cache_parameters(
         self,
         *,
         CacheParameterGroupName: str,
         Source: str = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> CacheParameterGroupDetailsTypeDef:
         """
         Returns the detailed parameter list for a particular cache parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.describe_cache_parameters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#describe_cache_parameters)
         """
@@ -845,15 +845,15 @@
         *,
         SourceIdentifier: str = ...,
         SourceType: SourceTypeType = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         Duration: int = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> EventsMessageTypeDef:
         """
         Returns events related to clusters, cache security groups, and cache parameter
         groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.describe_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#describe_events)
@@ -861,15 +861,15 @@
 
     async def describe_global_replication_groups(
         self,
         *,
         GlobalReplicationGroupId: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
-        ShowMemberInfo: bool = ...
+        ShowMemberInfo: bool = ...,
     ) -> DescribeGlobalReplicationGroupsResultTypeDef:
         """
         Returns information about a particular global replication group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.describe_global_replication_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#describe_global_replication_groups)
         """
@@ -890,15 +890,15 @@
         ReservedCacheNodeId: str = ...,
         ReservedCacheNodesOfferingId: str = ...,
         CacheNodeType: str = ...,
         Duration: str = ...,
         ProductDescription: str = ...,
         OfferingType: str = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> ReservedCacheNodeMessageTypeDef:
         """
         Returns information about reserved cache nodes for this account, or about a
         specified reserved cache
         node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.describe_reserved_cache_nodes)
@@ -910,15 +910,15 @@
         *,
         ReservedCacheNodesOfferingId: str = ...,
         CacheNodeType: str = ...,
         Duration: str = ...,
         ProductDescription: str = ...,
         OfferingType: str = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> ReservedCacheNodesOfferingMessageTypeDef:
         """
         Lists available reserved cache node offerings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.describe_reserved_cache_nodes_offerings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#describe_reserved_cache_nodes_offerings)
         """
@@ -926,15 +926,15 @@
     async def describe_serverless_cache_snapshots(
         self,
         *,
         ServerlessCacheName: str = ...,
         ServerlessCacheSnapshotName: str = ...,
         SnapshotType: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeServerlessCacheSnapshotsResponseTypeDef:
         """
         Returns information about serverless cache snapshots.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.describe_serverless_cache_snapshots)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#describe_serverless_cache_snapshots)
         """
@@ -951,15 +951,15 @@
 
     async def describe_service_updates(
         self,
         *,
         ServiceUpdateName: str = ...,
         ServiceUpdateStatus: Sequence[ServiceUpdateStatusType] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> ServiceUpdatesMessageTypeDef:
         """
         Returns details of the service updates See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/elasticache-2015-02-02/DescribeServiceUpdates).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.describe_service_updates)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#describe_service_updates)
@@ -970,15 +970,15 @@
         *,
         ReplicationGroupId: str = ...,
         CacheClusterId: str = ...,
         SnapshotName: str = ...,
         SnapshotSource: str = ...,
         Marker: str = ...,
         MaxRecords: int = ...,
-        ShowNodeGroupConfig: bool = ...
+        ShowNodeGroupConfig: bool = ...,
     ) -> DescribeSnapshotsListMessageTypeDef:
         """
         Returns information about cluster or replication group snapshots.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.describe_snapshots)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#describe_snapshots)
         """
@@ -991,15 +991,15 @@
         CacheClusterIds: Sequence[str] = ...,
         Engine: str = ...,
         ServiceUpdateStatus: Sequence[ServiceUpdateStatusType] = ...,
         ServiceUpdateTimeRange: TimeRangeFilterTypeDef = ...,
         UpdateActionStatus: Sequence[UpdateActionStatusType] = ...,
         ShowNodeLevelUpdateStatus: bool = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> UpdateActionsMessageTypeDef:
         """
         Returns details of the update actions See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/elasticache-2015-02-02/DescribeUpdateActions).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.describe_update_actions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#describe_update_actions)
@@ -1018,15 +1018,15 @@
     async def describe_users(
         self,
         *,
         Engine: str = ...,
         UserId: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DescribeUsersResultTypeDef:
         """
         Returns a list of users.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.describe_users)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#describe_users)
         """
@@ -1080,15 +1080,15 @@
 
     async def increase_node_groups_in_global_replication_group(
         self,
         *,
         GlobalReplicationGroupId: str,
         NodeGroupCount: int,
         ApplyImmediately: bool,
-        RegionalConfigurations: Sequence[RegionalConfigurationTypeDef] = ...
+        RegionalConfigurations: Sequence[RegionalConfigurationTypeDef] = ...,
     ) -> IncreaseNodeGroupsInGlobalReplicationGroupResultTypeDef:
         """
         Increase the number of node groups in the Global datastore See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/elasticache-2015-02-02/IncreaseNodeGroupsInGlobalReplicationGroup).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.increase_node_groups_in_global_replication_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#increase_node_groups_in_global_replication_group)
@@ -1096,15 +1096,15 @@
 
     async def increase_replica_count(
         self,
         *,
         ReplicationGroupId: str,
         ApplyImmediately: bool,
         NewReplicaCount: int = ...,
-        ReplicaConfiguration: Sequence[ConfigureShardTypeDef] = ...
+        ReplicaConfiguration: Sequence[ConfigureShardTypeDef] = ...,
     ) -> IncreaseReplicaCountResultTypeDef:
         """
         Dynamically increases the number of replicas in a Redis (cluster mode disabled)
         replication group or the number of replica nodes in one or more node groups
         (shards) of a Redis (cluster mode enabled) replication
         group.
 
@@ -1151,42 +1151,42 @@
         AutoMinorVersionUpgrade: bool = ...,
         SnapshotRetentionLimit: int = ...,
         SnapshotWindow: str = ...,
         CacheNodeType: str = ...,
         AuthToken: str = ...,
         AuthTokenUpdateStrategy: AuthTokenUpdateStrategyTypeType = ...,
         LogDeliveryConfigurations: Sequence[LogDeliveryConfigurationRequestTypeDef] = ...,
-        IpDiscovery: IpDiscoveryType = ...
+        IpDiscovery: IpDiscoveryType = ...,
     ) -> ModifyCacheClusterResultTypeDef:
         """
         Modifies the settings for a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.modify_cache_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#modify_cache_cluster)
         """
 
     async def modify_cache_parameter_group(
         self,
         *,
         CacheParameterGroupName: str,
-        ParameterNameValues: Sequence[ParameterNameValueTypeDef]
+        ParameterNameValues: Sequence[ParameterNameValueTypeDef],
     ) -> CacheParameterGroupNameMessageTypeDef:
         """
         Modifies the parameters of a cache parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.modify_cache_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#modify_cache_parameter_group)
         """
 
     async def modify_cache_subnet_group(
         self,
         *,
         CacheSubnetGroupName: str,
         CacheSubnetGroupDescription: str = ...,
-        SubnetIds: Sequence[str] = ...
+        SubnetIds: Sequence[str] = ...,
     ) -> ModifyCacheSubnetGroupResultTypeDef:
         """
         Modifies an existing cache subnet group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.modify_cache_subnet_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#modify_cache_subnet_group)
         """
@@ -1196,15 +1196,15 @@
         *,
         GlobalReplicationGroupId: str,
         ApplyImmediately: bool,
         CacheNodeType: str = ...,
         EngineVersion: str = ...,
         CacheParameterGroupName: str = ...,
         GlobalReplicationGroupDescription: str = ...,
-        AutomaticFailoverEnabled: bool = ...
+        AutomaticFailoverEnabled: bool = ...,
     ) -> ModifyGlobalReplicationGroupResultTypeDef:
         """
         Modifies the settings for a Global datastore.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.modify_global_replication_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#modify_global_replication_group)
         """
@@ -1236,15 +1236,15 @@
         UserGroupIdsToAdd: Sequence[str] = ...,
         UserGroupIdsToRemove: Sequence[str] = ...,
         RemoveUserGroups: bool = ...,
         LogDeliveryConfigurations: Sequence[LogDeliveryConfigurationRequestTypeDef] = ...,
         IpDiscovery: IpDiscoveryType = ...,
         TransitEncryptionEnabled: bool = ...,
         TransitEncryptionMode: TransitEncryptionModeType = ...,
-        ClusterMode: ClusterModeType = ...
+        ClusterMode: ClusterModeType = ...,
     ) -> ModifyReplicationGroupResultTypeDef:
         """
         Modifies the settings for a replication group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.modify_replication_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#modify_replication_group)
         """
@@ -1253,15 +1253,15 @@
         self,
         *,
         ReplicationGroupId: str,
         NodeGroupCount: int,
         ApplyImmediately: bool,
         ReshardingConfiguration: Sequence[ReshardingConfigurationTypeDef] = ...,
         NodeGroupsToRemove: Sequence[str] = ...,
-        NodeGroupsToRetain: Sequence[str] = ...
+        NodeGroupsToRetain: Sequence[str] = ...,
     ) -> ModifyReplicationGroupShardConfigurationResultTypeDef:
         """
         Modifies a replication group's shards (node groups) by allowing you to add
         shards, remove shards, or rebalance the keyspaces among existing
         shards.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.modify_replication_group_shard_configuration)
@@ -1274,15 +1274,15 @@
         ServerlessCacheName: str,
         Description: str = ...,
         CacheUsageLimits: CacheUsageLimitsTypeDef = ...,
         RemoveUserGroup: bool = ...,
         UserGroupId: str = ...,
         SecurityGroupIds: Sequence[str] = ...,
         SnapshotRetentionLimit: int = ...,
-        DailySnapshotTime: str = ...
+        DailySnapshotTime: str = ...,
     ) -> ModifyServerlessCacheResponseTypeDef:
         """
         This API modifies the attributes of a serverless cache.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.modify_serverless_cache)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#modify_serverless_cache)
         """
@@ -1291,44 +1291,44 @@
         self,
         *,
         UserId: str,
         AccessString: str = ...,
         AppendAccessString: str = ...,
         Passwords: Sequence[str] = ...,
         NoPasswordRequired: bool = ...,
-        AuthenticationMode: AuthenticationModeTypeDef = ...
+        AuthenticationMode: AuthenticationModeTypeDef = ...,
     ) -> UserResponseTypeDef:
         """
         Changes user password(s) and/or access string.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.modify_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#modify_user)
         """
 
     async def modify_user_group(
         self,
         *,
         UserGroupId: str,
         UserIdsToAdd: Sequence[str] = ...,
-        UserIdsToRemove: Sequence[str] = ...
+        UserIdsToRemove: Sequence[str] = ...,
     ) -> UserGroupResponseTypeDef:
         """
         Changes the list of users that belong to the user group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.modify_user_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#modify_user_group)
         """
 
     async def purchase_reserved_cache_nodes_offering(
         self,
         *,
         ReservedCacheNodesOfferingId: str,
         ReservedCacheNodeId: str = ...,
         CacheNodeCount: int = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> PurchaseReservedCacheNodesOfferingResultTypeDef:
         """
         Allows you to purchase a reserved cache node offering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.purchase_reserved_cache_nodes_offering)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#purchase_reserved_cache_nodes_offering)
         """
@@ -1365,15 +1365,15 @@
         """
 
     async def reset_cache_parameter_group(
         self,
         *,
         CacheParameterGroupName: str,
         ResetAllParameters: bool = ...,
-        ParameterNameValues: Sequence[ParameterNameValueTypeDef] = ...
+        ParameterNameValues: Sequence[ParameterNameValueTypeDef] = ...,
     ) -> CacheParameterGroupNameMessageTypeDef:
         """
         Modifies the parameters of a cache parameter group to the engine or system
         default
         value.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.reset_cache_parameter_group)
@@ -1381,28 +1381,28 @@
         """
 
     async def revoke_cache_security_group_ingress(
         self,
         *,
         CacheSecurityGroupName: str,
         EC2SecurityGroupName: str,
-        EC2SecurityGroupOwnerId: str
+        EC2SecurityGroupOwnerId: str,
     ) -> RevokeCacheSecurityGroupIngressResultTypeDef:
         """
         Revokes ingress from a cache security group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.revoke_cache_security_group_ingress)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#revoke_cache_security_group_ingress)
         """
 
     async def start_migration(
         self,
         *,
         ReplicationGroupId: str,
-        CustomerNodeEndpointList: Sequence[CustomerNodeEndpointTypeDef]
+        CustomerNodeEndpointList: Sequence[CustomerNodeEndpointTypeDef],
     ) -> StartMigrationResponseTypeDef:
         """
         Start the migration of data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.start_migration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#start_migration)
         """
@@ -1420,15 +1420,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#test_failover)
         """
 
     async def test_migration(
         self,
         *,
         ReplicationGroupId: str,
-        CustomerNodeEndpointList: Sequence[CustomerNodeEndpointTypeDef]
+        CustomerNodeEndpointList: Sequence[CustomerNodeEndpointTypeDef],
     ) -> TestMigrationResponseTypeDef:
         """
         Async API to test connection between source and target replication group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.test_migration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#test_migration)
         """
```

### Comparing `types-aiobotocore-elasticache-2.9.0/types_aiobotocore_elasticache/literals.py` & `types-aiobotocore-elasticache-2.9.1/types_aiobotocore_elasticache/literals.py`

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
     "AZModeType",
     "AuthTokenUpdateStatusType",
     "AuthTokenUpdateStrategyTypeType",
     "AuthenticationTypeType",
     "AutomaticFailoverStatusType",
     "CacheClusterAvailableWaiterName",
@@ -76,15 +75,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 AZModeType = Literal["cross-az", "single-az"]
 AuthTokenUpdateStatusType = Literal["ROTATING", "SETTING"]
 AuthTokenUpdateStrategyTypeType = Literal["DELETE", "ROTATE", "SET"]
 AuthenticationTypeType = Literal["iam", "no-password", "password"]
 AutomaticFailoverStatusType = Literal["disabled", "disabling", "enabled", "enabling"]
 CacheClusterAvailableWaiterName = Literal["cache_cluster_available"]
 CacheClusterDeletedWaiterName = Literal["cache_cluster_deleted"]
```

### Comparing `types-aiobotocore-elasticache-2.9.0/types_aiobotocore_elasticache/literals.pyi` & `types-aiobotocore-elasticache-2.9.1/types_aiobotocore_elasticache/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elasticache-2.9.0/types_aiobotocore_elasticache/paginator.py` & `types-aiobotocore-elasticache-2.9.1/types_aiobotocore_elasticache/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,14 @@
     "DescribeServiceUpdatesPaginator",
     "DescribeSnapshotsPaginator",
     "DescribeUpdateActionsPaginator",
     "DescribeUserGroupsPaginator",
     "DescribeUsersPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -130,15 +129,15 @@
 
     def paginate(
         self,
         *,
         CacheClusterId: str = ...,
         ShowCacheNodeInfo: bool = ...,
         ShowCacheClustersNotInReplicationGroups: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[CacheClusterMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheClusters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describecacheclusterspaginator)
         """
 
 
@@ -151,15 +150,15 @@
     def paginate(
         self,
         *,
         Engine: str = ...,
         EngineVersion: str = ...,
         CacheParameterGroupFamily: str = ...,
         DefaultOnly: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[CacheEngineVersionMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheEngineVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describecacheengineversionspaginator)
         """
 
 
@@ -185,15 +184,15 @@
     """
 
     def paginate(
         self,
         *,
         CacheParameterGroupName: str,
         Source: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[CacheParameterGroupDetailsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheParameters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describecacheparameterspaginator)
         """
 
 
@@ -252,15 +251,15 @@
         self,
         *,
         SourceIdentifier: str = ...,
         SourceType: SourceTypeType = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         Duration: int = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[EventsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describeeventspaginator)
         """
 
 
@@ -271,15 +270,15 @@
     """
 
     def paginate(
         self,
         *,
         GlobalReplicationGroupId: str = ...,
         ShowMemberInfo: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeGlobalReplicationGroupsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeGlobalReplicationGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describeglobalreplicationgroupspaginator)
         """
 
 
@@ -309,15 +308,15 @@
         *,
         ReservedCacheNodeId: str = ...,
         ReservedCacheNodesOfferingId: str = ...,
         CacheNodeType: str = ...,
         Duration: str = ...,
         ProductDescription: str = ...,
         OfferingType: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ReservedCacheNodeMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeReservedCacheNodes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describereservedcachenodespaginator)
         """
 
 
@@ -331,15 +330,15 @@
         self,
         *,
         ReservedCacheNodesOfferingId: str = ...,
         CacheNodeType: str = ...,
         Duration: str = ...,
         ProductDescription: str = ...,
         OfferingType: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ReservedCacheNodesOfferingMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeReservedCacheNodesOfferings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describereservedcachenodesofferingspaginator)
         """
 
 
@@ -351,15 +350,15 @@
 
     def paginate(
         self,
         *,
         ServerlessCacheName: str = ...,
         ServerlessCacheSnapshotName: str = ...,
         SnapshotType: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeServerlessCacheSnapshotsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeServerlessCacheSnapshots.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describeserverlesscachesnapshotspaginator)
         """
 
 
@@ -385,15 +384,15 @@
     """
 
     def paginate(
         self,
         *,
         ServiceUpdateName: str = ...,
         ServiceUpdateStatus: Sequence[ServiceUpdateStatusType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ServiceUpdatesMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeServiceUpdates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describeserviceupdatespaginator)
         """
 
 
@@ -407,15 +406,15 @@
         self,
         *,
         ReplicationGroupId: str = ...,
         CacheClusterId: str = ...,
         SnapshotName: str = ...,
         SnapshotSource: str = ...,
         ShowNodeGroupConfig: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeSnapshotsListMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeSnapshots.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describesnapshotspaginator)
         """
 
 
@@ -432,15 +431,15 @@
         ReplicationGroupIds: Sequence[str] = ...,
         CacheClusterIds: Sequence[str] = ...,
         Engine: str = ...,
         ServiceUpdateStatus: Sequence[ServiceUpdateStatusType] = ...,
         ServiceUpdateTimeRange: TimeRangeFilterTypeDef = ...,
         UpdateActionStatus: Sequence[UpdateActionStatusType] = ...,
         ShowNodeLevelUpdateStatus: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[UpdateActionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeUpdateActions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describeupdateactionspaginator)
         """
 
 
@@ -467,13 +466,13 @@
 
     def paginate(
         self,
         *,
         Engine: str = ...,
         UserId: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeUsersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeUsers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describeuserspaginator)
         """
```

### Comparing `types-aiobotocore-elasticache-2.9.0/types_aiobotocore_elasticache/paginator.pyi` & `types-aiobotocore-elasticache-2.9.1/types_aiobotocore_elasticache/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 
     def paginate(
         self,
         *,
         CacheClusterId: str = ...,
         ShowCacheNodeInfo: bool = ...,
         ShowCacheClustersNotInReplicationGroups: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[CacheClusterMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheClusters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describecacheclusterspaginator)
         """
 
 class DescribeCacheEngineVersionsPaginator(AioPaginator):
@@ -147,15 +147,15 @@
     def paginate(
         self,
         *,
         Engine: str = ...,
         EngineVersion: str = ...,
         CacheParameterGroupFamily: str = ...,
         DefaultOnly: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[CacheEngineVersionMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheEngineVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describecacheengineversionspaginator)
         """
 
 class DescribeCacheParameterGroupsPaginator(AioPaginator):
@@ -179,15 +179,15 @@
     """
 
     def paginate(
         self,
         *,
         CacheParameterGroupName: str,
         Source: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[CacheParameterGroupDetailsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheParameters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describecacheparameterspaginator)
         """
 
 class DescribeCacheSecurityGroupsPaginator(AioPaginator):
@@ -242,15 +242,15 @@
         self,
         *,
         SourceIdentifier: str = ...,
         SourceType: SourceTypeType = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         Duration: int = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[EventsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describeeventspaginator)
         """
 
 class DescribeGlobalReplicationGroupsPaginator(AioPaginator):
@@ -260,15 +260,15 @@
     """
 
     def paginate(
         self,
         *,
         GlobalReplicationGroupId: str = ...,
         ShowMemberInfo: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeGlobalReplicationGroupsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeGlobalReplicationGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describeglobalreplicationgroupspaginator)
         """
 
 class DescribeReplicationGroupsPaginator(AioPaginator):
@@ -296,15 +296,15 @@
         *,
         ReservedCacheNodeId: str = ...,
         ReservedCacheNodesOfferingId: str = ...,
         CacheNodeType: str = ...,
         Duration: str = ...,
         ProductDescription: str = ...,
         OfferingType: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ReservedCacheNodeMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeReservedCacheNodes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describereservedcachenodespaginator)
         """
 
 class DescribeReservedCacheNodesOfferingsPaginator(AioPaginator):
@@ -317,15 +317,15 @@
         self,
         *,
         ReservedCacheNodesOfferingId: str = ...,
         CacheNodeType: str = ...,
         Duration: str = ...,
         ProductDescription: str = ...,
         OfferingType: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ReservedCacheNodesOfferingMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeReservedCacheNodesOfferings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describereservedcachenodesofferingspaginator)
         """
 
 class DescribeServerlessCacheSnapshotsPaginator(AioPaginator):
@@ -336,15 +336,15 @@
 
     def paginate(
         self,
         *,
         ServerlessCacheName: str = ...,
         ServerlessCacheSnapshotName: str = ...,
         SnapshotType: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeServerlessCacheSnapshotsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeServerlessCacheSnapshots.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describeserverlesscachesnapshotspaginator)
         """
 
 class DescribeServerlessCachesPaginator(AioPaginator):
@@ -368,15 +368,15 @@
     """
 
     def paginate(
         self,
         *,
         ServiceUpdateName: str = ...,
         ServiceUpdateStatus: Sequence[ServiceUpdateStatusType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ServiceUpdatesMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeServiceUpdates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describeserviceupdatespaginator)
         """
 
 class DescribeSnapshotsPaginator(AioPaginator):
@@ -389,15 +389,15 @@
         self,
         *,
         ReplicationGroupId: str = ...,
         CacheClusterId: str = ...,
         SnapshotName: str = ...,
         SnapshotSource: str = ...,
         ShowNodeGroupConfig: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeSnapshotsListMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeSnapshots.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describesnapshotspaginator)
         """
 
 class DescribeUpdateActionsPaginator(AioPaginator):
@@ -413,15 +413,15 @@
         ReplicationGroupIds: Sequence[str] = ...,
         CacheClusterIds: Sequence[str] = ...,
         Engine: str = ...,
         ServiceUpdateStatus: Sequence[ServiceUpdateStatusType] = ...,
         ServiceUpdateTimeRange: TimeRangeFilterTypeDef = ...,
         UpdateActionStatus: Sequence[UpdateActionStatusType] = ...,
         ShowNodeLevelUpdateStatus: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[UpdateActionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeUpdateActions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describeupdateactionspaginator)
         """
 
 class DescribeUserGroupsPaginator(AioPaginator):
@@ -446,13 +446,13 @@
 
     def paginate(
         self,
         *,
         Engine: str = ...,
         UserId: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeUsersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeUsers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describeuserspaginator)
         """
```

### Comparing `types-aiobotocore-elasticache-2.9.0/types_aiobotocore_elasticache/type_defs.py` & `types-aiobotocore-elasticache-2.9.1/types_aiobotocore_elasticache/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "AuthenticationModeTypeDef",
     "AuthenticationTypeDef",
     "AuthorizeCacheSecurityGroupIngressMessageRequestTypeDef",
     "AvailabilityZoneTypeDef",
```

### Comparing `types-aiobotocore-elasticache-2.9.0/types_aiobotocore_elasticache/type_defs.pyi` & `types-aiobotocore-elasticache-2.9.1/types_aiobotocore_elasticache/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elasticache-2.9.0/types_aiobotocore_elasticache/waiter.py` & `types-aiobotocore-elasticache-2.9.1/types_aiobotocore_elasticache/waiter.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         self,
         *,
         CacheClusterId: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         ShowCacheNodeInfo: bool = ...,
         ShowCacheClustersNotInReplicationGroups: bool = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Waiter.CacheClusterAvailable.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/waiters/#cacheclusteravailablewaiter)
         """
 
 
@@ -71,15 +71,15 @@
         self,
         *,
         CacheClusterId: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         ShowCacheNodeInfo: bool = ...,
         ShowCacheClustersNotInReplicationGroups: bool = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Waiter.CacheClusterDeleted.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/waiters/#cacheclusterdeletedwaiter)
         """
 
 
@@ -91,15 +91,15 @@
 
     async def wait(
         self,
         *,
         ReplicationGroupId: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Waiter.ReplicationGroupAvailable.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/waiters/#replicationgroupavailablewaiter)
         """
 
 
@@ -111,13 +111,13 @@
 
     async def wait(
         self,
         *,
         ReplicationGroupId: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Waiter.ReplicationGroupDeleted.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/waiters/#replicationgroupdeletedwaiter)
         """
```

### Comparing `types-aiobotocore-elasticache-2.9.0/types_aiobotocore_elasticache/waiter.pyi` & `types-aiobotocore-elasticache-2.9.1/types_aiobotocore_elasticache/waiter.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         self,
         *,
         CacheClusterId: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         ShowCacheNodeInfo: bool = ...,
         ShowCacheClustersNotInReplicationGroups: bool = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Waiter.CacheClusterAvailable.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/waiters/#cacheclusteravailablewaiter)
         """
 
 class CacheClusterDeletedWaiter(AIOWaiter):
@@ -69,15 +69,15 @@
         self,
         *,
         CacheClusterId: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         ShowCacheNodeInfo: bool = ...,
         ShowCacheClustersNotInReplicationGroups: bool = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Waiter.CacheClusterDeleted.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/waiters/#cacheclusterdeletedwaiter)
         """
 
 class ReplicationGroupAvailableWaiter(AIOWaiter):
@@ -88,15 +88,15 @@
 
     async def wait(
         self,
         *,
         ReplicationGroupId: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Waiter.ReplicationGroupAvailable.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/waiters/#replicationgroupavailablewaiter)
         """
 
 class ReplicationGroupDeletedWaiter(AIOWaiter):
@@ -107,13 +107,13 @@
 
     async def wait(
         self,
         *,
         ReplicationGroupId: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Waiter.ReplicationGroupDeleted.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/waiters/#replicationgroupdeletedwaiter)
         """
```

### Comparing `types-aiobotocore-elasticache-2.9.0/types_aiobotocore_elasticache.egg-info/PKG-INFO` & `types-aiobotocore-elasticache-2.9.1/types_aiobotocore_elasticache.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-elasticache
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ElastiCache 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ElastiCache 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/
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
 
 <a id="types-aiobotocore-elasticache"></a>
 
 # types-aiobotocore-elasticache
 
 [![PyPI - types-aiobotocore-elasticache](https://img.shields.io/pypi/v/types-aiobotocore-elasticache.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elasticache)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-elasticache.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elasticache)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-elasticache)](https://pepy.tech/project/types-aiobotocore-elasticache)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ElastiCache 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache)
+[aiobotocore.ElastiCache 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache)
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
 [types-aiobotocore-elasticache docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-elasticache-2.9.0/types_aiobotocore_elasticache.egg-info/SOURCES.txt` & `types-aiobotocore-elasticache-2.9.1/types_aiobotocore_elasticache.egg-info/SOURCES.txt`

 * *Files identical despite different names*

