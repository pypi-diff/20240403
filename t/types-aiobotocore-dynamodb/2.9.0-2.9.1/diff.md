# Comparing `tmp/types-aiobotocore-dynamodb-2.9.0.tar.gz` & `tmp/types-aiobotocore-dynamodb-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-dynamodb-2.9.0.tar", last modified: Wed Dec 13 19:59:09 2023, max compression
+gzip compressed data, was "types-aiobotocore-dynamodb-2.9.1.tar", last modified: Thu Jan 18 01:20:34 2024, max compression
```

## Comparing `types-aiobotocore-dynamodb-2.9.0.tar` & `types-aiobotocore-dynamodb-2.9.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:09.461810 types-aiobotocore-dynamodb-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:44:32.000000 types-aiobotocore-dynamodb-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16253 2023-12-13 19:59:09.461810 types-aiobotocore-dynamodb-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14686 2023-12-13 19:44:32.000000 types-aiobotocore-dynamodb-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:09.461810 types-aiobotocore-dynamodb-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2023-12-13 19:44:31.000000 types-aiobotocore-dynamodb-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:09.457810 types-aiobotocore-dynamodb-2.9.0/types_aiobotocore_dynamodb/
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2023-12-13 19:44:32.000000 types-aiobotocore-dynamodb-2.9.0/types_aiobotocore_dynamodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2023-12-13 19:44:32.000000 types-aiobotocore-dynamodb-2.9.0/types_aiobotocore_dynamodb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      936 2023-12-13 19:44:32.000000 types-aiobotocore-dynamodb-2.9.0/types_aiobotocore_dynamodb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    50810 2023-12-13 19:44:32.000000 types-aiobotocore-dynamodb-2.9.0/types_aiobotocore_dynamodb/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    50806 2023-12-13 19:44:32.000000 types-aiobotocore-dynamodb-2.9.0/types_aiobotocore_dynamodb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13628 2023-12-13 19:44:32.000000 types-aiobotocore-dynamodb-2.9.0/types_aiobotocore_dynamodb/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    13626 2023-12-13 19:44:32.000000 types-aiobotocore-dynamodb-2.9.0/types_aiobotocore_dynamodb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7823 2023-12-13 19:44:32.000000 types-aiobotocore-dynamodb-2.9.0/types_aiobotocore_dynamodb/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7816 2023-12-13 19:44:32.000000 types-aiobotocore-dynamodb-2.9.0/types_aiobotocore_dynamodb/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:44:32.000000 types-aiobotocore-dynamodb-2.9.0/types_aiobotocore_dynamodb/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    24484 2023-12-13 19:44:32.000000 types-aiobotocore-dynamodb-2.9.0/types_aiobotocore_dynamodb/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    24478 2023-12-13 19:44:32.000000 types-aiobotocore-dynamodb-2.9.0/types_aiobotocore_dynamodb/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    97932 2023-12-13 19:44:35.000000 types-aiobotocore-dynamodb-2.9.0/types_aiobotocore_dynamodb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    97931 2023-12-13 19:44:33.000000 types-aiobotocore-dynamodb-2.9.0/types_aiobotocore_dynamodb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:44:32.000000 types-aiobotocore-dynamodb-2.9.0/types_aiobotocore_dynamodb/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2023-12-13 19:44:32.000000 types-aiobotocore-dynamodb-2.9.0/types_aiobotocore_dynamodb/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2023-12-13 19:44:32.000000 types-aiobotocore-dynamodb-2.9.0/types_aiobotocore_dynamodb/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:09.461810 types-aiobotocore-dynamodb-2.9.0/types_aiobotocore_dynamodb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16253 2023-12-13 19:59:09.000000 types-aiobotocore-dynamodb-2.9.0/types_aiobotocore_dynamodb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2023-12-13 19:59:09.000000 types-aiobotocore-dynamodb-2.9.0/types_aiobotocore_dynamodb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:09.000000 types-aiobotocore-dynamodb-2.9.0/types_aiobotocore_dynamodb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:09.000000 types-aiobotocore-dynamodb-2.9.0/types_aiobotocore_dynamodb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:09.000000 types-aiobotocore-dynamodb-2.9.0/types_aiobotocore_dynamodb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-13 19:59:09.000000 types-aiobotocore-dynamodb-2.9.0/types_aiobotocore_dynamodb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:34.649371 types-aiobotocore-dynamodb-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:06:25.000000 types-aiobotocore-dynamodb-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16273 2024-01-18 01:20:34.649371 types-aiobotocore-dynamodb-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14686 2024-01-18 01:06:25.000000 types-aiobotocore-dynamodb-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:34.649371 types-aiobotocore-dynamodb-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-01-18 01:06:25.000000 types-aiobotocore-dynamodb-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:34.649371 types-aiobotocore-dynamodb-2.9.1/types_aiobotocore_dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-01-18 01:06:25.000000 types-aiobotocore-dynamodb-2.9.1/types_aiobotocore_dynamodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-01-18 01:06:25.000000 types-aiobotocore-dynamodb-2.9.1/types_aiobotocore_dynamodb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-01-18 01:06:25.000000 types-aiobotocore-dynamodb-2.9.1/types_aiobotocore_dynamodb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50833 2024-01-18 01:06:27.000000 types-aiobotocore-dynamodb-2.9.1/types_aiobotocore_dynamodb/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50830 2024-01-18 01:06:27.000000 types-aiobotocore-dynamodb-2.9.1/types_aiobotocore_dynamodb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13626 2024-01-18 01:06:27.000000 types-aiobotocore-dynamodb-2.9.1/types_aiobotocore_dynamodb/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13626 2024-01-18 01:06:27.000000 types-aiobotocore-dynamodb-2.9.1/types_aiobotocore_dynamodb/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7825 2024-01-18 01:06:27.000000 types-aiobotocore-dynamodb-2.9.1/types_aiobotocore_dynamodb/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7819 2024-01-18 01:06:27.000000 types-aiobotocore-dynamodb-2.9.1/types_aiobotocore_dynamodb/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:06:25.000000 types-aiobotocore-dynamodb-2.9.1/types_aiobotocore_dynamodb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    24541 2024-01-18 01:06:27.000000 types-aiobotocore-dynamodb-2.9.1/types_aiobotocore_dynamodb/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24536 2024-01-18 01:06:27.000000 types-aiobotocore-dynamodb-2.9.1/types_aiobotocore_dynamodb/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    97931 2024-01-18 01:06:29.000000 types-aiobotocore-dynamodb-2.9.1/types_aiobotocore_dynamodb/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    97931 2024-01-18 01:06:29.000000 types-aiobotocore-dynamodb-2.9.1/types_aiobotocore_dynamodb/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:06:25.000000 types-aiobotocore-dynamodb-2.9.1/types_aiobotocore_dynamodb/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-01-18 01:06:27.000000 types-aiobotocore-dynamodb-2.9.1/types_aiobotocore_dynamodb/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-01-18 01:06:27.000000 types-aiobotocore-dynamodb-2.9.1/types_aiobotocore_dynamodb/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:34.649371 types-aiobotocore-dynamodb-2.9.1/types_aiobotocore_dynamodb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16273 2024-01-18 01:20:34.000000 types-aiobotocore-dynamodb-2.9.1/types_aiobotocore_dynamodb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-01-18 01:20:34.000000 types-aiobotocore-dynamodb-2.9.1/types_aiobotocore_dynamodb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:34.000000 types-aiobotocore-dynamodb-2.9.1/types_aiobotocore_dynamodb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:34.000000 types-aiobotocore-dynamodb-2.9.1/types_aiobotocore_dynamodb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:34.000000 types-aiobotocore-dynamodb-2.9.1/types_aiobotocore_dynamodb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-18 01:20:34.000000 types-aiobotocore-dynamodb-2.9.1/types_aiobotocore_dynamodb.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-dynamodb-2.9.0/LICENSE` & `types-aiobotocore-dynamodb-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-dynamodb-2.9.0/PKG-INFO` & `types-aiobotocore-dynamodb-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-dynamodb
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.DynamoDB 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.DynamoDB 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/
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
 
 <a id="types-aiobotocore-dynamodb"></a>
 
 # types-aiobotocore-dynamodb
 
 [![PyPI - types-aiobotocore-dynamodb](https://img.shields.io/pypi/v/types-aiobotocore-dynamodb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dynamodb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dynamodb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dynamodb)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-dynamodb)](https://pepy.tech/project/types-aiobotocore-dynamodb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DynamoDB 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
+[aiobotocore.DynamoDB 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
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
 [types-aiobotocore-dynamodb docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-dynamodb-2.9.0/README.md` & `types-aiobotocore-dynamodb-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dynamodb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dynamodb)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-dynamodb)](https://pepy.tech/project/types-aiobotocore-dynamodb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DynamoDB 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
+[aiobotocore.DynamoDB 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
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
 [types-aiobotocore-dynamodb docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-dynamodb-2.9.0/setup.py` & `types-aiobotocore-dynamodb-2.9.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-dynamodb",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_dynamodb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.DynamoDB 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.DynamoDB 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore dynamodb type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_dynamodb": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-dynamodb-2.9.0/types_aiobotocore_dynamodb/__init__.py` & `types-aiobotocore-dynamodb-2.9.1/types_aiobotocore_dynamodb/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,18 +45,16 @@
     ScanPaginator,
 )
 from .service_resource import DynamoDBServiceResource
 from .waiter import TableExistsWaiter, TableNotExistsWaiter
 
 Client = DynamoDBClient
 
-
 ServiceResource = DynamoDBServiceResource
 
-
 __all__ = (
     "Client",
     "DynamoDBClient",
     "DynamoDBServiceResource",
     "ListBackupsPaginator",
     "ListTablesPaginator",
     "ListTagsOfResourcePaginator",
```

### Comparing `types-aiobotocore-dynamodb-2.9.0/types_aiobotocore_dynamodb/__init__.pyi` & `types-aiobotocore-dynamodb-2.9.1/types_aiobotocore_dynamodb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.9.0/types_aiobotocore_dynamodb/__main__.py` & `types-aiobotocore-dynamodb-2.9.1/types_aiobotocore_dynamodb/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.DynamoDB 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.DynamoDB 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB\nOther"
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

### Comparing `types-aiobotocore-dynamodb-2.9.0/types_aiobotocore_dynamodb/client.py` & `types-aiobotocore-dynamodb-2.9.1/types_aiobotocore_dynamodb/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,14 @@
 from .waiter import TableExistsWaiter, TableNotExistsWaiter
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("DynamoDBClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -203,30 +202,30 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#exceptions)
         """
 
     async def batch_execute_statement(
         self,
         *,
         Statements: Sequence[BatchStatementRequestTypeDef],
-        ReturnConsumedCapacity: ReturnConsumedCapacityType = ...
+        ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
     ) -> BatchExecuteStatementOutputTypeDef:
         """
         This operation allows you to perform batch reads or writes on data stored in
         DynamoDB, using
         PartiQL.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.batch_execute_statement)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#batch_execute_statement)
         """
 
     async def batch_get_item(
         self,
         *,
         RequestItems: Mapping[str, KeysAndAttributesTypeDef],
-        ReturnConsumedCapacity: ReturnConsumedCapacityType = ...
+        ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
     ) -> BatchGetItemOutputTypeDef:
         """
         The `BatchGetItem` operation returns the attributes of one or more items from
         one or more
         tables.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.batch_get_item)
@@ -234,15 +233,15 @@
         """
 
     async def batch_write_item(
         self,
         *,
         RequestItems: Mapping[str, Sequence[WriteRequestTypeDef]],
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
-        ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...
+        ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
     ) -> BatchWriteItemOutputTypeDef:
         """
         The `BatchWriteItem` operation puts or deletes multiple items in one or more
         tables.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.batch_write_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#batch_write_item)
@@ -292,15 +291,15 @@
         GlobalSecondaryIndexes: Sequence[GlobalSecondaryIndexTypeDef] = ...,
         BillingMode: BillingModeType = ...,
         ProvisionedThroughput: ProvisionedThroughputTypeDef = ...,
         StreamSpecification: StreamSpecificationTypeDef = ...,
         SSESpecification: SSESpecificationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         TableClass: TableClassType = ...,
-        DeletionProtectionEnabled: bool = ...
+        DeletionProtectionEnabled: bool = ...,
     ) -> CreateTableOutputTypeDef:
         """
         The `CreateTable` operation adds a new table to your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.create_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#create_table)
         """
@@ -322,15 +321,15 @@
         ConditionalOperator: ConditionalOperatorType = ...,
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         ConditionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
         ExpressionAttributeValues: Mapping[str, UniversalAttributeValueTypeDef] = ...,
-        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
+        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...,
     ) -> DeleteItemOutputTypeDef:
         """
         Deletes a single item in a table by primary key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.delete_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#delete_item)
         """
@@ -495,15 +494,15 @@
         *,
         Statement: str,
         Parameters: Sequence[UniversalAttributeValueTypeDef] = ...,
         ConsistentRead: bool = ...,
         NextToken: str = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         Limit: int = ...,
-        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
+        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...,
     ) -> ExecuteStatementOutputTypeDef:
         """
         This operation allows you to perform reads and singleton writes on data stored
         in DynamoDB, using
         PartiQL.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.execute_statement)
@@ -511,15 +510,15 @@
         """
 
     async def execute_transaction(
         self,
         *,
         TransactStatements: Sequence[ParameterizedStatementTypeDef],
         ClientRequestToken: str = ...,
-        ReturnConsumedCapacity: ReturnConsumedCapacityType = ...
+        ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
     ) -> ExecuteTransactionOutputTypeDef:
         """
         This operation allows you to perform transactional reads or writes on data
         stored in DynamoDB, using
         PartiQL.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.execute_transaction)
@@ -535,15 +534,15 @@
         ClientToken: str = ...,
         S3BucketOwner: str = ...,
         S3Prefix: str = ...,
         S3SseAlgorithm: S3SseAlgorithmType = ...,
         S3SseKmsKeyId: str = ...,
         ExportFormat: ExportFormatType = ...,
         ExportType: ExportTypeType = ...,
-        IncrementalExportSpecification: IncrementalExportSpecificationTypeDef = ...
+        IncrementalExportSpecification: IncrementalExportSpecificationTypeDef = ...,
     ) -> ExportTableToPointInTimeOutputTypeDef:
         """
         Exports table data to an S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.export_table_to_point_in_time)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#export_table_to_point_in_time)
         """
@@ -567,15 +566,15 @@
         *,
         TableName: str,
         Key: Mapping[str, UniversalAttributeValueTypeDef],
         AttributesToGet: Sequence[str] = ...,
         ConsistentRead: bool = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ProjectionExpression: str = ...,
-        ExpressionAttributeNames: Mapping[str, str] = ...
+        ExpressionAttributeNames: Mapping[str, str] = ...,
     ) -> GetItemOutputTypeDef:
         """
         The `GetItem` operation returns a set of attributes for the item with the given
         primary
         key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.get_item)
@@ -586,15 +585,15 @@
         self,
         *,
         S3BucketSource: S3BucketSourceTypeDef,
         InputFormat: InputFormatType,
         TableCreationParameters: TableCreationParametersTypeDef,
         ClientToken: str = ...,
         InputFormatOptions: InputFormatOptionsTypeDef = ...,
-        InputCompressionType: InputCompressionTypeType = ...
+        InputCompressionType: InputCompressionTypeType = ...,
     ) -> ImportTableOutputTypeDef:
         """
         Imports table data from an S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.import_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#import_table)
         """
@@ -603,15 +602,15 @@
         self,
         *,
         TableName: str = ...,
         Limit: int = ...,
         TimeRangeLowerBound: TimestampTypeDef = ...,
         TimeRangeUpperBound: TimestampTypeDef = ...,
         ExclusiveStartBackupArn: str = ...,
-        BackupType: BackupTypeFilterType = ...
+        BackupType: BackupTypeFilterType = ...,
     ) -> ListBackupsOutputTypeDef:
         """
         List DynamoDB backups that are associated with an Amazon Web Services account
         and weren't made with Amazon Web Services
         Backup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.list_backups)
@@ -690,15 +689,15 @@
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ConditionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
         ExpressionAttributeValues: Mapping[str, UniversalAttributeValueTypeDef] = ...,
-        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
+        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...,
     ) -> PutItemOutputTypeDef:
         """
         Creates a new item, or replaces an old item with a new item.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.put_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#put_item)
         """
@@ -718,15 +717,15 @@
         ScanIndexForward: bool = ...,
         ExclusiveStartKey: Mapping[str, UniversalAttributeValueTypeDef] = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ProjectionExpression: str = ...,
         FilterExpression: str = ...,
         KeyConditionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[str, UniversalAttributeValueTypeDef] = ...
+        ExpressionAttributeValues: Mapping[str, UniversalAttributeValueTypeDef] = ...,
     ) -> QueryOutputTypeDef:
         """
         You must provide the name of the partition key attribute and a single value for
         that
         attribute.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.query)
@@ -738,15 +737,15 @@
         *,
         TargetTableName: str,
         BackupArn: str,
         BillingModeOverride: BillingModeType = ...,
         GlobalSecondaryIndexOverride: Sequence[GlobalSecondaryIndexTypeDef] = ...,
         LocalSecondaryIndexOverride: Sequence[LocalSecondaryIndexTypeDef] = ...,
         ProvisionedThroughputOverride: ProvisionedThroughputTypeDef = ...,
-        SSESpecificationOverride: SSESpecificationTypeDef = ...
+        SSESpecificationOverride: SSESpecificationTypeDef = ...,
     ) -> RestoreTableFromBackupOutputTypeDef:
         """
         Creates a new table from an existing backup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.restore_table_from_backup)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#restore_table_from_backup)
         """
@@ -759,15 +758,15 @@
         SourceTableName: str = ...,
         UseLatestRestorableTime: bool = ...,
         RestoreDateTime: TimestampTypeDef = ...,
         BillingModeOverride: BillingModeType = ...,
         GlobalSecondaryIndexOverride: Sequence[GlobalSecondaryIndexTypeDef] = ...,
         LocalSecondaryIndexOverride: Sequence[LocalSecondaryIndexTypeDef] = ...,
         ProvisionedThroughputOverride: ProvisionedThroughputTypeDef = ...,
-        SSESpecificationOverride: SSESpecificationTypeDef = ...
+        SSESpecificationOverride: SSESpecificationTypeDef = ...,
     ) -> RestoreTableToPointInTimeOutputTypeDef:
         """
         Restores the specified table to the specified point in time within
         `EarliestRestorableDateTime` and
         `LatestRestorableDateTime`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.restore_table_to_point_in_time)
@@ -788,15 +787,15 @@
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         TotalSegments: int = ...,
         Segment: int = ...,
         ProjectionExpression: str = ...,
         FilterExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
         ExpressionAttributeValues: Mapping[str, UniversalAttributeValueTypeDef] = ...,
-        ConsistentRead: bool = ...
+        ConsistentRead: bool = ...,
     ) -> ScanOutputTypeDef:
         """
         The `Scan` operation returns one or more items and item attributes by accessing
         every item in a table or a secondary
         index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.scan)
@@ -813,15 +812,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#tag_resource)
         """
 
     async def transact_get_items(
         self,
         *,
         TransactItems: Sequence[TransactGetItemTypeDef],
-        ReturnConsumedCapacity: ReturnConsumedCapacityType = ...
+        ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
     ) -> TransactGetItemsOutputTypeDef:
         """
         `TransactGetItems` is a synchronous operation that atomically retrieves
         multiple items from one or more tables (but not from indexes) in a single
         account and
         Region.
 
@@ -831,15 +830,15 @@
 
     async def transact_write_items(
         self,
         *,
         TransactItems: Sequence[TransactWriteItemTypeDef],
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
     ) -> TransactWriteItemsOutputTypeDef:
         """
         `TransactWriteItems` is a synchronous write operation that groups up to 100
         action
         requests.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.transact_write_items)
@@ -856,15 +855,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#untag_resource)
         """
 
     async def update_continuous_backups(
         self,
         *,
         TableName: str,
-        PointInTimeRecoverySpecification: PointInTimeRecoverySpecificationTypeDef
+        PointInTimeRecoverySpecification: PointInTimeRecoverySpecificationTypeDef,
     ) -> UpdateContinuousBackupsOutputTypeDef:
         """
         `UpdateContinuousBackups` enables or disables point in time recovery for the
         specified
         table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.update_continuous_backups)
@@ -872,15 +871,15 @@
         """
 
     async def update_contributor_insights(
         self,
         *,
         TableName: str,
         ContributorInsightsAction: ContributorInsightsActionType,
-        IndexName: str = ...
+        IndexName: str = ...,
     ) -> UpdateContributorInsightsOutputTypeDef:
         """
         Updates the status for contributor insights for a specific table or index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.update_contributor_insights)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#update_contributor_insights)
         """
@@ -901,15 +900,15 @@
         GlobalTableName: str,
         GlobalTableBillingMode: BillingModeType = ...,
         GlobalTableProvisionedWriteCapacityUnits: int = ...,
         GlobalTableProvisionedWriteCapacityAutoScalingSettingsUpdate: AutoScalingSettingsUpdateTypeDef = ...,
         GlobalTableGlobalSecondaryIndexSettingsUpdate: Sequence[
             GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef
         ] = ...,
-        ReplicaSettingsUpdate: Sequence[ReplicaSettingsUpdateTypeDef] = ...
+        ReplicaSettingsUpdate: Sequence[ReplicaSettingsUpdateTypeDef] = ...,
     ) -> UpdateGlobalTableSettingsOutputTypeDef:
         """
         Updates settings for a global table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.update_global_table_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#update_global_table_settings)
         """
@@ -925,15 +924,15 @@
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         UpdateExpression: str = ...,
         ConditionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
         ExpressionAttributeValues: Mapping[str, UniversalAttributeValueTypeDef] = ...,
-        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
+        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...,
     ) -> UpdateItemOutputTypeDef:
         """
         Edits an existing item's attributes, or adds a new item to the table if it does
         not already
         exist.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.update_item)
@@ -948,15 +947,15 @@
         BillingMode: BillingModeType = ...,
         ProvisionedThroughput: ProvisionedThroughputTypeDef = ...,
         GlobalSecondaryIndexUpdates: Sequence[GlobalSecondaryIndexUpdateTypeDef] = ...,
         StreamSpecification: StreamSpecificationTypeDef = ...,
         SSESpecification: SSESpecificationTypeDef = ...,
         ReplicaUpdates: Sequence[ReplicationGroupUpdateTypeDef] = ...,
         TableClass: TableClassType = ...,
-        DeletionProtectionEnabled: bool = ...
+        DeletionProtectionEnabled: bool = ...,
     ) -> UpdateTableOutputTypeDef:
         """
         Modifies the provisioned throughput settings, global secondary indexes, or
         DynamoDB Streams settings for a given
         table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.update_table)
@@ -965,15 +964,15 @@
 
     async def update_table_replica_auto_scaling(
         self,
         *,
         TableName: str,
         GlobalSecondaryIndexUpdates: Sequence[GlobalSecondaryIndexAutoScalingUpdateTypeDef] = ...,
         ProvisionedWriteCapacityAutoScalingUpdate: AutoScalingSettingsUpdateTypeDef = ...,
-        ReplicaUpdates: Sequence[ReplicaAutoScalingUpdateTypeDef] = ...
+        ReplicaUpdates: Sequence[ReplicaAutoScalingUpdateTypeDef] = ...,
     ) -> UpdateTableReplicaAutoScalingOutputTypeDef:
         """
         Updates auto scaling settings on your global tables at once.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.update_table_replica_auto_scaling)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#update_table_replica_auto_scaling)
         """
```

### Comparing `types-aiobotocore-dynamodb-2.9.0/types_aiobotocore_dynamodb/client.pyi` & `types-aiobotocore-dynamodb-2.9.1/types_aiobotocore_dynamodb/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -199,30 +199,30 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#exceptions)
         """
 
     async def batch_execute_statement(
         self,
         *,
         Statements: Sequence[BatchStatementRequestTypeDef],
-        ReturnConsumedCapacity: ReturnConsumedCapacityType = ...
+        ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
     ) -> BatchExecuteStatementOutputTypeDef:
         """
         This operation allows you to perform batch reads or writes on data stored in
         DynamoDB, using
         PartiQL.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.batch_execute_statement)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#batch_execute_statement)
         """
 
     async def batch_get_item(
         self,
         *,
         RequestItems: Mapping[str, KeysAndAttributesTypeDef],
-        ReturnConsumedCapacity: ReturnConsumedCapacityType = ...
+        ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
     ) -> BatchGetItemOutputTypeDef:
         """
         The `BatchGetItem` operation returns the attributes of one or more items from
         one or more
         tables.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.batch_get_item)
@@ -230,15 +230,15 @@
         """
 
     async def batch_write_item(
         self,
         *,
         RequestItems: Mapping[str, Sequence[WriteRequestTypeDef]],
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
-        ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...
+        ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
     ) -> BatchWriteItemOutputTypeDef:
         """
         The `BatchWriteItem` operation puts or deletes multiple items in one or more
         tables.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.batch_write_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#batch_write_item)
@@ -288,15 +288,15 @@
         GlobalSecondaryIndexes: Sequence[GlobalSecondaryIndexTypeDef] = ...,
         BillingMode: BillingModeType = ...,
         ProvisionedThroughput: ProvisionedThroughputTypeDef = ...,
         StreamSpecification: StreamSpecificationTypeDef = ...,
         SSESpecification: SSESpecificationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         TableClass: TableClassType = ...,
-        DeletionProtectionEnabled: bool = ...
+        DeletionProtectionEnabled: bool = ...,
     ) -> CreateTableOutputTypeDef:
         """
         The `CreateTable` operation adds a new table to your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.create_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#create_table)
         """
@@ -318,15 +318,15 @@
         ConditionalOperator: ConditionalOperatorType = ...,
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         ConditionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
         ExpressionAttributeValues: Mapping[str, UniversalAttributeValueTypeDef] = ...,
-        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
+        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...,
     ) -> DeleteItemOutputTypeDef:
         """
         Deletes a single item in a table by primary key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.delete_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#delete_item)
         """
@@ -491,15 +491,15 @@
         *,
         Statement: str,
         Parameters: Sequence[UniversalAttributeValueTypeDef] = ...,
         ConsistentRead: bool = ...,
         NextToken: str = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         Limit: int = ...,
-        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
+        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...,
     ) -> ExecuteStatementOutputTypeDef:
         """
         This operation allows you to perform reads and singleton writes on data stored
         in DynamoDB, using
         PartiQL.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.execute_statement)
@@ -507,15 +507,15 @@
         """
 
     async def execute_transaction(
         self,
         *,
         TransactStatements: Sequence[ParameterizedStatementTypeDef],
         ClientRequestToken: str = ...,
-        ReturnConsumedCapacity: ReturnConsumedCapacityType = ...
+        ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
     ) -> ExecuteTransactionOutputTypeDef:
         """
         This operation allows you to perform transactional reads or writes on data
         stored in DynamoDB, using
         PartiQL.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.execute_transaction)
@@ -531,15 +531,15 @@
         ClientToken: str = ...,
         S3BucketOwner: str = ...,
         S3Prefix: str = ...,
         S3SseAlgorithm: S3SseAlgorithmType = ...,
         S3SseKmsKeyId: str = ...,
         ExportFormat: ExportFormatType = ...,
         ExportType: ExportTypeType = ...,
-        IncrementalExportSpecification: IncrementalExportSpecificationTypeDef = ...
+        IncrementalExportSpecification: IncrementalExportSpecificationTypeDef = ...,
     ) -> ExportTableToPointInTimeOutputTypeDef:
         """
         Exports table data to an S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.export_table_to_point_in_time)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#export_table_to_point_in_time)
         """
@@ -563,15 +563,15 @@
         *,
         TableName: str,
         Key: Mapping[str, UniversalAttributeValueTypeDef],
         AttributesToGet: Sequence[str] = ...,
         ConsistentRead: bool = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ProjectionExpression: str = ...,
-        ExpressionAttributeNames: Mapping[str, str] = ...
+        ExpressionAttributeNames: Mapping[str, str] = ...,
     ) -> GetItemOutputTypeDef:
         """
         The `GetItem` operation returns a set of attributes for the item with the given
         primary
         key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.get_item)
@@ -582,15 +582,15 @@
         self,
         *,
         S3BucketSource: S3BucketSourceTypeDef,
         InputFormat: InputFormatType,
         TableCreationParameters: TableCreationParametersTypeDef,
         ClientToken: str = ...,
         InputFormatOptions: InputFormatOptionsTypeDef = ...,
-        InputCompressionType: InputCompressionTypeType = ...
+        InputCompressionType: InputCompressionTypeType = ...,
     ) -> ImportTableOutputTypeDef:
         """
         Imports table data from an S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.import_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#import_table)
         """
@@ -599,15 +599,15 @@
         self,
         *,
         TableName: str = ...,
         Limit: int = ...,
         TimeRangeLowerBound: TimestampTypeDef = ...,
         TimeRangeUpperBound: TimestampTypeDef = ...,
         ExclusiveStartBackupArn: str = ...,
-        BackupType: BackupTypeFilterType = ...
+        BackupType: BackupTypeFilterType = ...,
     ) -> ListBackupsOutputTypeDef:
         """
         List DynamoDB backups that are associated with an Amazon Web Services account
         and weren't made with Amazon Web Services
         Backup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.list_backups)
@@ -686,15 +686,15 @@
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ConditionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
         ExpressionAttributeValues: Mapping[str, UniversalAttributeValueTypeDef] = ...,
-        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
+        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...,
     ) -> PutItemOutputTypeDef:
         """
         Creates a new item, or replaces an old item with a new item.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.put_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#put_item)
         """
@@ -714,15 +714,15 @@
         ScanIndexForward: bool = ...,
         ExclusiveStartKey: Mapping[str, UniversalAttributeValueTypeDef] = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ProjectionExpression: str = ...,
         FilterExpression: str = ...,
         KeyConditionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[str, UniversalAttributeValueTypeDef] = ...
+        ExpressionAttributeValues: Mapping[str, UniversalAttributeValueTypeDef] = ...,
     ) -> QueryOutputTypeDef:
         """
         You must provide the name of the partition key attribute and a single value for
         that
         attribute.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.query)
@@ -734,15 +734,15 @@
         *,
         TargetTableName: str,
         BackupArn: str,
         BillingModeOverride: BillingModeType = ...,
         GlobalSecondaryIndexOverride: Sequence[GlobalSecondaryIndexTypeDef] = ...,
         LocalSecondaryIndexOverride: Sequence[LocalSecondaryIndexTypeDef] = ...,
         ProvisionedThroughputOverride: ProvisionedThroughputTypeDef = ...,
-        SSESpecificationOverride: SSESpecificationTypeDef = ...
+        SSESpecificationOverride: SSESpecificationTypeDef = ...,
     ) -> RestoreTableFromBackupOutputTypeDef:
         """
         Creates a new table from an existing backup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.restore_table_from_backup)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#restore_table_from_backup)
         """
@@ -755,15 +755,15 @@
         SourceTableName: str = ...,
         UseLatestRestorableTime: bool = ...,
         RestoreDateTime: TimestampTypeDef = ...,
         BillingModeOverride: BillingModeType = ...,
         GlobalSecondaryIndexOverride: Sequence[GlobalSecondaryIndexTypeDef] = ...,
         LocalSecondaryIndexOverride: Sequence[LocalSecondaryIndexTypeDef] = ...,
         ProvisionedThroughputOverride: ProvisionedThroughputTypeDef = ...,
-        SSESpecificationOverride: SSESpecificationTypeDef = ...
+        SSESpecificationOverride: SSESpecificationTypeDef = ...,
     ) -> RestoreTableToPointInTimeOutputTypeDef:
         """
         Restores the specified table to the specified point in time within
         `EarliestRestorableDateTime` and
         `LatestRestorableDateTime`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.restore_table_to_point_in_time)
@@ -784,15 +784,15 @@
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         TotalSegments: int = ...,
         Segment: int = ...,
         ProjectionExpression: str = ...,
         FilterExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
         ExpressionAttributeValues: Mapping[str, UniversalAttributeValueTypeDef] = ...,
-        ConsistentRead: bool = ...
+        ConsistentRead: bool = ...,
     ) -> ScanOutputTypeDef:
         """
         The `Scan` operation returns one or more items and item attributes by accessing
         every item in a table or a secondary
         index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.scan)
@@ -809,15 +809,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#tag_resource)
         """
 
     async def transact_get_items(
         self,
         *,
         TransactItems: Sequence[TransactGetItemTypeDef],
-        ReturnConsumedCapacity: ReturnConsumedCapacityType = ...
+        ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
     ) -> TransactGetItemsOutputTypeDef:
         """
         `TransactGetItems` is a synchronous operation that atomically retrieves
         multiple items from one or more tables (but not from indexes) in a single
         account and
         Region.
 
@@ -827,15 +827,15 @@
 
     async def transact_write_items(
         self,
         *,
         TransactItems: Sequence[TransactWriteItemTypeDef],
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
     ) -> TransactWriteItemsOutputTypeDef:
         """
         `TransactWriteItems` is a synchronous write operation that groups up to 100
         action
         requests.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.transact_write_items)
@@ -852,15 +852,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#untag_resource)
         """
 
     async def update_continuous_backups(
         self,
         *,
         TableName: str,
-        PointInTimeRecoverySpecification: PointInTimeRecoverySpecificationTypeDef
+        PointInTimeRecoverySpecification: PointInTimeRecoverySpecificationTypeDef,
     ) -> UpdateContinuousBackupsOutputTypeDef:
         """
         `UpdateContinuousBackups` enables or disables point in time recovery for the
         specified
         table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.update_continuous_backups)
@@ -868,15 +868,15 @@
         """
 
     async def update_contributor_insights(
         self,
         *,
         TableName: str,
         ContributorInsightsAction: ContributorInsightsActionType,
-        IndexName: str = ...
+        IndexName: str = ...,
     ) -> UpdateContributorInsightsOutputTypeDef:
         """
         Updates the status for contributor insights for a specific table or index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.update_contributor_insights)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#update_contributor_insights)
         """
@@ -897,15 +897,15 @@
         GlobalTableName: str,
         GlobalTableBillingMode: BillingModeType = ...,
         GlobalTableProvisionedWriteCapacityUnits: int = ...,
         GlobalTableProvisionedWriteCapacityAutoScalingSettingsUpdate: AutoScalingSettingsUpdateTypeDef = ...,
         GlobalTableGlobalSecondaryIndexSettingsUpdate: Sequence[
             GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef
         ] = ...,
-        ReplicaSettingsUpdate: Sequence[ReplicaSettingsUpdateTypeDef] = ...
+        ReplicaSettingsUpdate: Sequence[ReplicaSettingsUpdateTypeDef] = ...,
     ) -> UpdateGlobalTableSettingsOutputTypeDef:
         """
         Updates settings for a global table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.update_global_table_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#update_global_table_settings)
         """
@@ -921,15 +921,15 @@
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         UpdateExpression: str = ...,
         ConditionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
         ExpressionAttributeValues: Mapping[str, UniversalAttributeValueTypeDef] = ...,
-        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
+        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...,
     ) -> UpdateItemOutputTypeDef:
         """
         Edits an existing item's attributes, or adds a new item to the table if it does
         not already
         exist.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.update_item)
@@ -944,15 +944,15 @@
         BillingMode: BillingModeType = ...,
         ProvisionedThroughput: ProvisionedThroughputTypeDef = ...,
         GlobalSecondaryIndexUpdates: Sequence[GlobalSecondaryIndexUpdateTypeDef] = ...,
         StreamSpecification: StreamSpecificationTypeDef = ...,
         SSESpecification: SSESpecificationTypeDef = ...,
         ReplicaUpdates: Sequence[ReplicationGroupUpdateTypeDef] = ...,
         TableClass: TableClassType = ...,
-        DeletionProtectionEnabled: bool = ...
+        DeletionProtectionEnabled: bool = ...,
     ) -> UpdateTableOutputTypeDef:
         """
         Modifies the provisioned throughput settings, global secondary indexes, or
         DynamoDB Streams settings for a given
         table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.update_table)
@@ -961,15 +961,15 @@
 
     async def update_table_replica_auto_scaling(
         self,
         *,
         TableName: str,
         GlobalSecondaryIndexUpdates: Sequence[GlobalSecondaryIndexAutoScalingUpdateTypeDef] = ...,
         ProvisionedWriteCapacityAutoScalingUpdate: AutoScalingSettingsUpdateTypeDef = ...,
-        ReplicaUpdates: Sequence[ReplicaAutoScalingUpdateTypeDef] = ...
+        ReplicaUpdates: Sequence[ReplicaAutoScalingUpdateTypeDef] = ...,
     ) -> UpdateTableReplicaAutoScalingOutputTypeDef:
         """
         Updates auto scaling settings on your global tables at once.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.update_table_replica_auto_scaling)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#update_table_replica_auto_scaling)
         """
```

### Comparing `types-aiobotocore-dynamodb-2.9.0/types_aiobotocore_dynamodb/literals.py` & `types-aiobotocore-dynamodb-2.9.1/types_aiobotocore_dynamodb/literals.py`

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
     "AttributeActionType",
     "BackupStatusType",
     "BackupTypeFilterType",
     "BackupTypeType",
     "BatchStatementErrorCodeEnumType",
     "BillingModeType",
@@ -70,15 +69,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 AttributeActionType = Literal["ADD", "DELETE", "PUT"]
 BackupStatusType = Literal["AVAILABLE", "CREATING", "DELETED"]
 BackupTypeFilterType = Literal["ALL", "AWS_BACKUP", "SYSTEM", "USER"]
 BackupTypeType = Literal["AWS_BACKUP", "SYSTEM", "USER"]
 BatchStatementErrorCodeEnumType = Literal[
     "AccessDenied",
     "ConditionalCheckFailed",
```

### Comparing `types-aiobotocore-dynamodb-2.9.0/types_aiobotocore_dynamodb/literals.pyi` & `types-aiobotocore-dynamodb-2.9.1/types_aiobotocore_dynamodb/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.9.0/types_aiobotocore_dynamodb/paginator.py` & `types-aiobotocore-dynamodb-2.9.1/types_aiobotocore_dynamodb/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,14 @@
     "ListBackupsPaginator",
     "ListTablesPaginator",
     "ListTagsOfResourcePaginator",
     "QueryPaginator",
     "ScanPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -80,15 +79,15 @@
     def paginate(
         self,
         *,
         TableName: str = ...,
         TimeRangeLowerBound: TimestampTypeDef = ...,
         TimeRangeUpperBound: TimestampTypeDef = ...,
         BackupType: BackupTypeFilterType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListBackupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListBackups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/paginators/#listbackupspaginator)
         """
 
 
@@ -142,15 +141,15 @@
         ScanIndexForward: bool = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ProjectionExpression: str = ...,
         FilterExpression: str = ...,
         KeyConditionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
         ExpressionAttributeValues: Mapping[str, UniversalAttributeValueTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[QueryOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.Query.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/paginators/#querypaginator)
         """
 
 
@@ -173,13 +172,13 @@
         TotalSegments: int = ...,
         Segment: int = ...,
         ProjectionExpression: str = ...,
         FilterExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
         ExpressionAttributeValues: Mapping[str, UniversalAttributeValueTypeDef] = ...,
         ConsistentRead: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ScanOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.Scan.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/paginators/#scanpaginator)
         """
```

### Comparing `types-aiobotocore-dynamodb-2.9.0/types_aiobotocore_dynamodb/paginator.pyi` & `types-aiobotocore-dynamodb-2.9.1/types_aiobotocore_dynamodb/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
     def paginate(
         self,
         *,
         TableName: str = ...,
         TimeRangeLowerBound: TimestampTypeDef = ...,
         TimeRangeUpperBound: TimestampTypeDef = ...,
         BackupType: BackupTypeFilterType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListBackupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListBackups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/paginators/#listbackupspaginator)
         """
 
 class ListTablesPaginator(AioPaginator):
@@ -136,15 +136,15 @@
         ScanIndexForward: bool = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ProjectionExpression: str = ...,
         FilterExpression: str = ...,
         KeyConditionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
         ExpressionAttributeValues: Mapping[str, UniversalAttributeValueTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[QueryOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.Query.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/paginators/#querypaginator)
         """
 
 class ScanPaginator(AioPaginator):
@@ -166,13 +166,13 @@
         TotalSegments: int = ...,
         Segment: int = ...,
         ProjectionExpression: str = ...,
         FilterExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
         ExpressionAttributeValues: Mapping[str, UniversalAttributeValueTypeDef] = ...,
         ConsistentRead: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ScanOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.Scan.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/paginators/#scanpaginator)
         """
```

### Comparing `types-aiobotocore-dynamodb-2.9.0/types_aiobotocore_dynamodb/service_resource.py` & `types-aiobotocore-dynamodb-2.9.1/types_aiobotocore_dynamodb/service_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,14 @@
 except ImportError:
     from builtins import object as AIOResourceCollection
 try:
     from boto3.resources.base import ResourceMeta
 except ImportError:
     from builtins import object as ResourceMeta
 
-
 __all__ = ("DynamoDBServiceResource", "Table", "ServiceResourceTablesCollection")
 
 
 class ServiceResourceTablesCollection(AIOResourceCollection):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.tables)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#serviceresourcetablescollection)
@@ -185,14 +184,15 @@
     replicas: Awaitable[List[ReplicaDescriptionTypeDef]]
     restore_summary: Awaitable[RestoreSummaryResponseTypeDef]
     sse_description: Awaitable[SSEDescriptionResponseTypeDef]
     archival_summary: Awaitable[ArchivalSummaryResponseTypeDef]
     table_class_summary: Awaitable[TableClassSummaryResponseTypeDef]
     deletion_protection_enabled: Awaitable[bool]
     name: str
+    meta: Awaitable["DynamoDBResourceMeta"]
 
     def batch_writer(
         self,
         overwrite_by_pkeys: Optional[List[str]] = ...,
         flush_amount: int = ...,
         on_exit_loop_sleep: int = ...,
     ) -> BatchWriter:
@@ -219,15 +219,15 @@
         ConditionalOperator: ConditionalOperatorType = ...,
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         ConditionExpression: ConditionBaseImportTypeDef = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
         ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...,
-        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
+        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...,
     ) -> DeleteItemOutputTableTypeDef:
         """
         Deletes a single item in a table by primary key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.delete_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tabledelete_item-method)
         """
@@ -244,15 +244,15 @@
         self,
         *,
         Key: Mapping[str, TableAttributeValueTypeDef],
         AttributesToGet: Sequence[str] = ...,
         ConsistentRead: bool = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ProjectionExpression: str = ...,
-        ExpressionAttributeNames: Mapping[str, str] = ...
+        ExpressionAttributeNames: Mapping[str, str] = ...,
     ) -> GetItemOutputTableTypeDef:
         """
         The `GetItem` operation returns a set of attributes for the item with the given
         primary
         key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.get_item)
@@ -277,15 +277,15 @@
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ConditionExpression: ConditionBaseImportTypeDef = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
         ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...,
-        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
+        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...,
     ) -> PutItemOutputTableTypeDef:
         """
         Creates a new item, or replaces an old item with a new item.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.put_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tableput_item-method)
         """
@@ -304,15 +304,15 @@
         ScanIndexForward: bool = ...,
         ExclusiveStartKey: Mapping[str, TableAttributeValueTypeDef] = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ProjectionExpression: str = ...,
         FilterExpression: ConditionBaseImportTypeDef = ...,
         KeyConditionExpression: ConditionBaseImportTypeDef = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...
+        ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...,
     ) -> QueryOutputTableTypeDef:
         """
         You must provide the name of the partition key attribute and a single value for
         that
         attribute.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.query)
@@ -342,15 +342,15 @@
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         TotalSegments: int = ...,
         Segment: int = ...,
         ProjectionExpression: str = ...,
         FilterExpression: ConditionBaseImportTypeDef = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
         ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...,
-        ConsistentRead: bool = ...
+        ConsistentRead: bool = ...,
     ) -> ScanOutputTableTypeDef:
         """
         The `Scan` operation returns one or more items and item attributes by accessing
         every item in a table or a secondary
         index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.scan)
@@ -364,15 +364,15 @@
         BillingMode: BillingModeType = ...,
         ProvisionedThroughput: ProvisionedThroughputTypeDef = ...,
         GlobalSecondaryIndexUpdates: Sequence[GlobalSecondaryIndexUpdateTableTypeDef] = ...,
         StreamSpecification: StreamSpecificationTypeDef = ...,
         SSESpecification: SSESpecificationTypeDef = ...,
         ReplicaUpdates: Sequence[ReplicationGroupUpdateTypeDef] = ...,
         TableClass: TableClassType = ...,
-        DeletionProtectionEnabled: bool = ...
+        DeletionProtectionEnabled: bool = ...,
     ) -> "_Table":
         """
         Modifies the provisioned throughput settings, global secondary indexes, or
         DynamoDB Streams settings for a given
         table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.update)
@@ -389,15 +389,15 @@
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         UpdateExpression: str = ...,
         ConditionExpression: ConditionBaseImportTypeDef = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
         ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...,
-        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
+        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...,
     ) -> UpdateItemOutputTableTypeDef:
         """
         Edits an existing item's attributes, or adds a new item to the table if it does
         not already
         exist.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.update_item)
@@ -433,27 +433,27 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/)
     """
 
     meta: "DynamoDBResourceMeta"
     tables: ServiceResourceTablesCollection
 
-    async def Table(self, name: str) -> _Table:
+    async def Table(self, name: str) -> "_Table":
         """
         Creates a Table resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.Table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#dynamodbserviceresourcetable-method)
         """
 
     async def batch_get_item(
         self,
         *,
         RequestItems: Mapping[str, KeysAndAttributesServiceResourceTypeDef],
-        ReturnConsumedCapacity: ReturnConsumedCapacityType = ...
+        ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
     ) -> BatchGetItemOutputServiceResourceTypeDef:
         """
         The `BatchGetItem` operation returns the attributes of one or more items from
         one or more
         tables.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.batch_get_item)
@@ -461,15 +461,15 @@
         """
 
     async def batch_write_item(
         self,
         *,
         RequestItems: Mapping[str, Sequence[WriteRequestServiceResourceTypeDef]],
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
-        ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...
+        ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
     ) -> BatchWriteItemOutputServiceResourceTypeDef:
         """
         The `BatchWriteItem` operation puts or deletes multiple items in one or more
         tables.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.batch_write_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#dynamodbserviceresourcebatch_write_item-method)
@@ -485,16 +485,16 @@
         GlobalSecondaryIndexes: Sequence[GlobalSecondaryIndexTypeDef] = ...,
         BillingMode: BillingModeType = ...,
         ProvisionedThroughput: ProvisionedThroughputTypeDef = ...,
         StreamSpecification: StreamSpecificationTypeDef = ...,
         SSESpecification: SSESpecificationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         TableClass: TableClassType = ...,
-        DeletionProtectionEnabled: bool = ...
-    ) -> _Table:
+        DeletionProtectionEnabled: bool = ...,
+    ) -> "_Table":
         """
         The `CreateTable` operation adds a new table to your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.create_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#dynamodbserviceresourcecreate_table-method)
         """
```

### Comparing `types-aiobotocore-dynamodb-2.9.0/types_aiobotocore_dynamodb/service_resource.pyi` & `types-aiobotocore-dynamodb-2.9.1/types_aiobotocore_dynamodb/service_resource.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -182,14 +182,15 @@
     replicas: Awaitable[List[ReplicaDescriptionTypeDef]]
     restore_summary: Awaitable[RestoreSummaryResponseTypeDef]
     sse_description: Awaitable[SSEDescriptionResponseTypeDef]
     archival_summary: Awaitable[ArchivalSummaryResponseTypeDef]
     table_class_summary: Awaitable[TableClassSummaryResponseTypeDef]
     deletion_protection_enabled: Awaitable[bool]
     name: str
+    meta: Awaitable["DynamoDBResourceMeta"]
 
     def batch_writer(
         self,
         overwrite_by_pkeys: Optional[List[str]] = ...,
         flush_amount: int = ...,
         on_exit_loop_sleep: int = ...,
     ) -> BatchWriter:
@@ -216,15 +217,15 @@
         ConditionalOperator: ConditionalOperatorType = ...,
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         ConditionExpression: ConditionBaseImportTypeDef = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
         ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...,
-        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
+        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...,
     ) -> DeleteItemOutputTableTypeDef:
         """
         Deletes a single item in a table by primary key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.delete_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tabledelete_item-method)
         """
@@ -241,15 +242,15 @@
         self,
         *,
         Key: Mapping[str, TableAttributeValueTypeDef],
         AttributesToGet: Sequence[str] = ...,
         ConsistentRead: bool = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ProjectionExpression: str = ...,
-        ExpressionAttributeNames: Mapping[str, str] = ...
+        ExpressionAttributeNames: Mapping[str, str] = ...,
     ) -> GetItemOutputTableTypeDef:
         """
         The `GetItem` operation returns a set of attributes for the item with the given
         primary
         key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.get_item)
@@ -274,15 +275,15 @@
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ConditionExpression: ConditionBaseImportTypeDef = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
         ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...,
-        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
+        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...,
     ) -> PutItemOutputTableTypeDef:
         """
         Creates a new item, or replaces an old item with a new item.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.put_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tableput_item-method)
         """
@@ -301,15 +302,15 @@
         ScanIndexForward: bool = ...,
         ExclusiveStartKey: Mapping[str, TableAttributeValueTypeDef] = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ProjectionExpression: str = ...,
         FilterExpression: ConditionBaseImportTypeDef = ...,
         KeyConditionExpression: ConditionBaseImportTypeDef = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...
+        ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...,
     ) -> QueryOutputTableTypeDef:
         """
         You must provide the name of the partition key attribute and a single value for
         that
         attribute.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.query)
@@ -339,15 +340,15 @@
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         TotalSegments: int = ...,
         Segment: int = ...,
         ProjectionExpression: str = ...,
         FilterExpression: ConditionBaseImportTypeDef = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
         ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...,
-        ConsistentRead: bool = ...
+        ConsistentRead: bool = ...,
     ) -> ScanOutputTableTypeDef:
         """
         The `Scan` operation returns one or more items and item attributes by accessing
         every item in a table or a secondary
         index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.scan)
@@ -361,15 +362,15 @@
         BillingMode: BillingModeType = ...,
         ProvisionedThroughput: ProvisionedThroughputTypeDef = ...,
         GlobalSecondaryIndexUpdates: Sequence[GlobalSecondaryIndexUpdateTableTypeDef] = ...,
         StreamSpecification: StreamSpecificationTypeDef = ...,
         SSESpecification: SSESpecificationTypeDef = ...,
         ReplicaUpdates: Sequence[ReplicationGroupUpdateTypeDef] = ...,
         TableClass: TableClassType = ...,
-        DeletionProtectionEnabled: bool = ...
+        DeletionProtectionEnabled: bool = ...,
     ) -> "_Table":
         """
         Modifies the provisioned throughput settings, global secondary indexes, or
         DynamoDB Streams settings for a given
         table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.update)
@@ -386,15 +387,15 @@
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         UpdateExpression: str = ...,
         ConditionExpression: ConditionBaseImportTypeDef = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
         ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...,
-        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
+        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...,
     ) -> UpdateItemOutputTableTypeDef:
         """
         Edits an existing item's attributes, or adds a new item to the table if it does
         not already
         exist.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.update_item)
@@ -427,27 +428,27 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/)
     """
 
     meta: "DynamoDBResourceMeta"
     tables: ServiceResourceTablesCollection
 
-    async def Table(self, name: str) -> _Table:
+    async def Table(self, name: str) -> "_Table":
         """
         Creates a Table resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.Table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#dynamodbserviceresourcetable-method)
         """
 
     async def batch_get_item(
         self,
         *,
         RequestItems: Mapping[str, KeysAndAttributesServiceResourceTypeDef],
-        ReturnConsumedCapacity: ReturnConsumedCapacityType = ...
+        ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
     ) -> BatchGetItemOutputServiceResourceTypeDef:
         """
         The `BatchGetItem` operation returns the attributes of one or more items from
         one or more
         tables.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.batch_get_item)
@@ -455,15 +456,15 @@
         """
 
     async def batch_write_item(
         self,
         *,
         RequestItems: Mapping[str, Sequence[WriteRequestServiceResourceTypeDef]],
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
-        ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...
+        ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
     ) -> BatchWriteItemOutputServiceResourceTypeDef:
         """
         The `BatchWriteItem` operation puts or deletes multiple items in one or more
         tables.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.batch_write_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#dynamodbserviceresourcebatch_write_item-method)
@@ -479,16 +480,16 @@
         GlobalSecondaryIndexes: Sequence[GlobalSecondaryIndexTypeDef] = ...,
         BillingMode: BillingModeType = ...,
         ProvisionedThroughput: ProvisionedThroughputTypeDef = ...,
         StreamSpecification: StreamSpecificationTypeDef = ...,
         SSESpecification: SSESpecificationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         TableClass: TableClassType = ...,
-        DeletionProtectionEnabled: bool = ...
-    ) -> _Table:
+        DeletionProtectionEnabled: bool = ...,
+    ) -> "_Table":
         """
         The `CreateTable` operation adds a new table to your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.create_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#dynamodbserviceresourcecreate_table-method)
         """
```

### Comparing `types-aiobotocore-dynamodb-2.9.0/types_aiobotocore_dynamodb/type_defs.py` & `types-aiobotocore-dynamodb-2.9.1/types_aiobotocore_dynamodb/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,14 @@
 else:
     from typing_extensions import TypedDict
 try:
     from boto3.dynamodb.conditions import ConditionBase
 except ImportError:
     from builtins import object as ConditionBase
 
-
 __all__ = (
     "ResponseMetadataTypeDef",
     "ArchivalSummaryTypeDef",
     "AttributeDefinitionTypeDef",
     "AttributeValueTypeDef",
     "TableAttributeValueTypeDef",
     "AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef",
```

### Comparing `types-aiobotocore-dynamodb-2.9.0/types_aiobotocore_dynamodb/type_defs.pyi` & `types-aiobotocore-dynamodb-2.9.1/types_aiobotocore_dynamodb/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.9.0/types_aiobotocore_dynamodb/waiter.py` & `types-aiobotocore-dynamodb-2.9.1/types_aiobotocore_dynamodb/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.9.0/types_aiobotocore_dynamodb/waiter.pyi` & `types-aiobotocore-dynamodb-2.9.1/types_aiobotocore_dynamodb/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.9.0/types_aiobotocore_dynamodb.egg-info/PKG-INFO` & `types-aiobotocore-dynamodb-2.9.1/types_aiobotocore_dynamodb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-dynamodb
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.DynamoDB 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.DynamoDB 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/
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
 
 <a id="types-aiobotocore-dynamodb"></a>
 
 # types-aiobotocore-dynamodb
 
 [![PyPI - types-aiobotocore-dynamodb](https://img.shields.io/pypi/v/types-aiobotocore-dynamodb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dynamodb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dynamodb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dynamodb)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-dynamodb)](https://pepy.tech/project/types-aiobotocore-dynamodb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DynamoDB 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
+[aiobotocore.DynamoDB 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
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
 [types-aiobotocore-dynamodb docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-dynamodb-2.9.0/types_aiobotocore_dynamodb.egg-info/SOURCES.txt` & `types-aiobotocore-dynamodb-2.9.1/types_aiobotocore_dynamodb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

