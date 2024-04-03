# Comparing `tmp/types-aiobotocore-storagegateway-2.9.0.tar.gz` & `tmp/types-aiobotocore-storagegateway-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-storagegateway-2.9.0.tar", last modified: Wed Dec 13 20:00:38 2023, max compression
+gzip compressed data, was "types-aiobotocore-storagegateway-2.9.1.tar", last modified: Thu Jan 18 01:21:55 2024, max compression
```

## Comparing `types-aiobotocore-storagegateway-2.9.0.tar` & `types-aiobotocore-storagegateway-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:38.161072 types-aiobotocore-storagegateway-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:57:05.000000 types-aiobotocore-storagegateway-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14816 2023-12-13 20:00:38.161072 types-aiobotocore-storagegateway-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13225 2023-12-13 19:57:05.000000 types-aiobotocore-storagegateway-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:38.161072 types-aiobotocore-storagegateway-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2023-12-13 19:57:05.000000 types-aiobotocore-storagegateway-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:38.157072 types-aiobotocore-storagegateway-2.9.0/types_aiobotocore_storagegateway/
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2023-12-13 19:57:05.000000 types-aiobotocore-storagegateway-2.9.0/types_aiobotocore_storagegateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2023-12-13 19:57:05.000000 types-aiobotocore-storagegateway-2.9.0/types_aiobotocore_storagegateway/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      960 2023-12-13 19:57:05.000000 types-aiobotocore-storagegateway-2.9.0/types_aiobotocore_storagegateway/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    71921 2023-12-13 19:57:06.000000 types-aiobotocore-storagegateway-2.9.0/types_aiobotocore_storagegateway/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    71917 2023-12-13 19:57:05.000000 types-aiobotocore-storagegateway-2.9.0/types_aiobotocore_storagegateway/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11402 2023-12-13 19:57:06.000000 types-aiobotocore-storagegateway-2.9.0/types_aiobotocore_storagegateway/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11400 2023-12-13 19:57:06.000000 types-aiobotocore-storagegateway-2.9.0/types_aiobotocore_storagegateway/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13762 2023-12-13 19:57:06.000000 types-aiobotocore-storagegateway-2.9.0/types_aiobotocore_storagegateway/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    13749 2023-12-13 19:57:06.000000 types-aiobotocore-storagegateway-2.9.0/types_aiobotocore_storagegateway/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:57:05.000000 types-aiobotocore-storagegateway-2.9.0/types_aiobotocore_storagegateway/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    68209 2023-12-13 19:57:10.000000 types-aiobotocore-storagegateway-2.9.0/types_aiobotocore_storagegateway/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    68208 2023-12-13 19:57:06.000000 types-aiobotocore-storagegateway-2.9.0/types_aiobotocore_storagegateway/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:57:05.000000 types-aiobotocore-storagegateway-2.9.0/types_aiobotocore_storagegateway/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:38.161072 types-aiobotocore-storagegateway-2.9.0/types_aiobotocore_storagegateway.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14816 2023-12-13 20:00:38.000000 types-aiobotocore-storagegateway-2.9.0/types_aiobotocore_storagegateway.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      946 2023-12-13 20:00:38.000000 types-aiobotocore-storagegateway-2.9.0/types_aiobotocore_storagegateway.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:38.000000 types-aiobotocore-storagegateway-2.9.0/types_aiobotocore_storagegateway.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:38.000000 types-aiobotocore-storagegateway-2.9.0/types_aiobotocore_storagegateway.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:38.000000 types-aiobotocore-storagegateway-2.9.0/types_aiobotocore_storagegateway.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-13 20:00:38.000000 types-aiobotocore-storagegateway-2.9.0/types_aiobotocore_storagegateway.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:55.817003 types-aiobotocore-storagegateway-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:18:36.000000 types-aiobotocore-storagegateway-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14836 2024-01-18 01:21:55.817003 types-aiobotocore-storagegateway-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13225 2024-01-18 01:18:36.000000 types-aiobotocore-storagegateway-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:55.817003 types-aiobotocore-storagegateway-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-01-18 01:18:36.000000 types-aiobotocore-storagegateway-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:55.817003 types-aiobotocore-storagegateway-2.9.1/types_aiobotocore_storagegateway/
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-01-18 01:18:36.000000 types-aiobotocore-storagegateway-2.9.1/types_aiobotocore_storagegateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-01-18 01:18:36.000000 types-aiobotocore-storagegateway-2.9.1/types_aiobotocore_storagegateway/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-01-18 01:18:36.000000 types-aiobotocore-storagegateway-2.9.1/types_aiobotocore_storagegateway/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71942 2024-01-18 01:18:37.000000 types-aiobotocore-storagegateway-2.9.1/types_aiobotocore_storagegateway/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71939 2024-01-18 01:18:36.000000 types-aiobotocore-storagegateway-2.9.1/types_aiobotocore_storagegateway/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11400 2024-01-18 01:18:37.000000 types-aiobotocore-storagegateway-2.9.1/types_aiobotocore_storagegateway/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11400 2024-01-18 01:18:37.000000 types-aiobotocore-storagegateway-2.9.1/types_aiobotocore_storagegateway/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13763 2024-01-18 01:18:37.000000 types-aiobotocore-storagegateway-2.9.1/types_aiobotocore_storagegateway/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13751 2024-01-18 01:18:37.000000 types-aiobotocore-storagegateway-2.9.1/types_aiobotocore_storagegateway/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:18:36.000000 types-aiobotocore-storagegateway-2.9.1/types_aiobotocore_storagegateway/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    68208 2024-01-18 01:18:38.000000 types-aiobotocore-storagegateway-2.9.1/types_aiobotocore_storagegateway/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68208 2024-01-18 01:18:38.000000 types-aiobotocore-storagegateway-2.9.1/types_aiobotocore_storagegateway/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:18:36.000000 types-aiobotocore-storagegateway-2.9.1/types_aiobotocore_storagegateway/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:55.817003 types-aiobotocore-storagegateway-2.9.1/types_aiobotocore_storagegateway.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14836 2024-01-18 01:21:55.000000 types-aiobotocore-storagegateway-2.9.1/types_aiobotocore_storagegateway.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-01-18 01:21:55.000000 types-aiobotocore-storagegateway-2.9.1/types_aiobotocore_storagegateway.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:55.000000 types-aiobotocore-storagegateway-2.9.1/types_aiobotocore_storagegateway.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:55.000000 types-aiobotocore-storagegateway-2.9.1/types_aiobotocore_storagegateway.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:55.000000 types-aiobotocore-storagegateway-2.9.1/types_aiobotocore_storagegateway.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-18 01:21:55.000000 types-aiobotocore-storagegateway-2.9.1/types_aiobotocore_storagegateway.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-storagegateway-2.9.0/LICENSE` & `types-aiobotocore-storagegateway-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-storagegateway-2.9.0/PKG-INFO` & `types-aiobotocore-storagegateway-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-storagegateway
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.StorageGateway 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.StorageGateway 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/
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
 
 <a id="types-aiobotocore-storagegateway"></a>
 
 # types-aiobotocore-storagegateway
 
 [![PyPI - types-aiobotocore-storagegateway](https://img.shields.io/pypi/v/types-aiobotocore-storagegateway.svg?color=blue)](https://pypi.org/project/types-aiobotocore-storagegateway)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-storagegateway.svg?color=blue)](https://pypi.org/project/types-aiobotocore-storagegateway)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-storagegateway)](https://pepy.tech/project/types-aiobotocore-storagegateway)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.StorageGateway 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway)
+[aiobotocore.StorageGateway 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway)
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
 [types-aiobotocore-storagegateway docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-storagegateway-2.9.0/README.md` & `types-aiobotocore-storagegateway-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-storagegateway.svg?color=blue)](https://pypi.org/project/types-aiobotocore-storagegateway)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-storagegateway)](https://pepy.tech/project/types-aiobotocore-storagegateway)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.StorageGateway 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway)
+[aiobotocore.StorageGateway 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway)
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
 [types-aiobotocore-storagegateway docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-storagegateway-2.9.0/setup.py` & `types-aiobotocore-storagegateway-2.9.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-storagegateway",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_storagegateway"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.StorageGateway 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.StorageGateway 2.9.1 service generated with"
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
     keywords="aiobotocore storagegateway type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_storagegateway": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-storagegateway-2.9.0/types_aiobotocore_storagegateway/__init__.py` & `types-aiobotocore-storagegateway-2.9.1/types_aiobotocore_storagegateway/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,14 @@
     ListTapePoolsPaginator,
     ListTapesPaginator,
     ListVolumesPaginator,
 )
 
 Client = StorageGatewayClient
 
-
 __all__ = (
     "Client",
     "DescribeTapeArchivesPaginator",
     "DescribeTapeRecoveryPointsPaginator",
     "DescribeTapesPaginator",
     "DescribeVTLDevicesPaginator",
     "ListFileSharesPaginator",
```

### Comparing `types-aiobotocore-storagegateway-2.9.0/types_aiobotocore_storagegateway/__init__.pyi` & `types-aiobotocore-storagegateway-2.9.1/types_aiobotocore_storagegateway/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-storagegateway-2.9.0/types_aiobotocore_storagegateway/__main__.py` & `types-aiobotocore-storagegateway-2.9.1/types_aiobotocore_storagegateway/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.StorageGateway 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.StorageGateway 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway\nOther"
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

### Comparing `types-aiobotocore-storagegateway-2.9.0/types_aiobotocore_storagegateway/client.py` & `types-aiobotocore-storagegateway-2.9.1/types_aiobotocore_storagegateway/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("StorageGatewayClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -189,15 +188,15 @@
         ActivationKey: str,
         GatewayName: str,
         GatewayTimezone: str,
         GatewayRegion: str,
         GatewayType: str = ...,
         TapeDriveType: str = ...,
         MediumChangerType: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> ActivateGatewayOutputTypeDef:
         """
         Activates the gateway you previously deployed on your host.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.activate_gateway)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#activate_gateway)
         """
@@ -258,15 +257,15 @@
         Password: str,
         ClientToken: str,
         GatewayARN: str,
         LocationARN: str,
         Tags: Sequence[TagTypeDef] = ...,
         AuditDestinationARN: str = ...,
         CacheAttributes: CacheAttributesTypeDef = ...,
-        EndpointNetworkConfiguration: EndpointNetworkConfigurationTypeDef = ...
+        EndpointNetworkConfiguration: EndpointNetworkConfigurationTypeDef = ...,
     ) -> AssociateFileSystemOutputTypeDef:
         """
         Associate an Amazon FSx file system with the FSx File Gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.associate_file_system)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#associate_file_system)
         """
@@ -274,15 +273,15 @@
     async def attach_volume(
         self,
         *,
         GatewayARN: str,
         VolumeARN: str,
         NetworkInterfaceId: str,
         TargetName: str = ...,
-        DiskId: str = ...
+        DiskId: str = ...,
     ) -> AttachVolumeOutputTypeDef:
         """
         Connects a volume to an iSCSI connection and then attaches the volume to the
         specified
         gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.attach_volume)
@@ -337,15 +336,15 @@
         TargetName: str,
         NetworkInterfaceId: str,
         ClientToken: str,
         SnapshotId: str = ...,
         SourceVolumeARN: str = ...,
         KMSEncrypted: bool = ...,
         KMSKey: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateCachediSCSIVolumeOutputTypeDef:
         """
         Creates a cached volume on a specified cached volume gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.create_cached_iscsi_volume)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#create_cached_iscsi_volume)
         """
@@ -369,15 +368,15 @@
         RequesterPays: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
         FileShareName: str = ...,
         CacheAttributes: CacheAttributesTypeDef = ...,
         NotificationPolicy: str = ...,
         VPCEndpointDNSName: str = ...,
         BucketRegion: str = ...,
-        AuditDestinationARN: str = ...
+        AuditDestinationARN: str = ...,
     ) -> CreateNFSFileShareOutputTypeDef:
         """
         Creates a Network File System (NFS) file share on an existing S3 File Gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.create_nfs_file_share)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#create_nfs_file_share)
         """
@@ -406,15 +405,15 @@
         CaseSensitivity: CaseSensitivityType = ...,
         Tags: Sequence[TagTypeDef] = ...,
         FileShareName: str = ...,
         CacheAttributes: CacheAttributesTypeDef = ...,
         NotificationPolicy: str = ...,
         VPCEndpointDNSName: str = ...,
         BucketRegion: str = ...,
-        OplocksEnabled: bool = ...
+        OplocksEnabled: bool = ...,
     ) -> CreateSMBFileShareOutputTypeDef:
         """
         Creates a Server Message Block (SMB) file share on an existing S3 File Gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.create_smb_file_share)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#create_smb_file_share)
         """
@@ -446,15 +445,15 @@
         DiskId: str,
         PreserveExistingData: bool,
         TargetName: str,
         NetworkInterfaceId: str,
         SnapshotId: str = ...,
         KMSEncrypted: bool = ...,
         KMSKey: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateStorediSCSIVolumeOutputTypeDef:
         """
         Creates a volume on a specified gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.create_stored_iscsi_volume)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#create_stored_iscsi_volume)
         """
@@ -462,15 +461,15 @@
     async def create_tape_pool(
         self,
         *,
         PoolName: str,
         StorageClass: TapeStorageClassType,
         RetentionLockType: RetentionLockTypeType = ...,
         RetentionLockTimeInDays: int = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateTapePoolOutputTypeDef:
         """
         Creates a new custom tape pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.create_tape_pool)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#create_tape_pool)
         """
@@ -481,15 +480,15 @@
         GatewayARN: str,
         TapeSizeInBytes: int,
         TapeBarcode: str,
         KMSEncrypted: bool = ...,
         KMSKey: str = ...,
         PoolId: str = ...,
         Worm: bool = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateTapeWithBarcodeOutputTypeDef:
         """
         Creates a virtual tape by using your own barcode.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.create_tape_with_barcode)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#create_tape_with_barcode)
         """
@@ -502,15 +501,15 @@
         ClientToken: str,
         NumTapesToCreate: int,
         TapeBarcodePrefix: str,
         KMSEncrypted: bool = ...,
         KMSKey: str = ...,
         PoolId: str = ...,
         Worm: bool = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateTapesOutputTypeDef:
         """
         Creates one or more virtual tapes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.create_tapes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#create_tapes)
         """
@@ -808,15 +807,15 @@
 
     async def describe_vtl_devices(
         self,
         *,
         GatewayARN: str,
         VTLDeviceARNs: Sequence[str] = ...,
         Marker: str = ...,
-        Limit: int = ...
+        Limit: int = ...,
     ) -> DescribeVTLDevicesOutputTypeDef:
         """
         Returns a description of virtual tape library (VTL) devices for the specified
         tape
         gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.describe_vtl_devices)
@@ -882,15 +881,15 @@
         *,
         GatewayARN: str,
         DomainName: str,
         UserName: str,
         Password: str,
         OrganizationalUnit: str = ...,
         DomainControllers: Sequence[str] = ...,
-        TimeoutInSeconds: int = ...
+        TimeoutInSeconds: int = ...,
     ) -> JoinDomainOutputTypeDef:
         """
         Adds a file gateway to an Active Directory domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.join_domain)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#join_domain)
         """
@@ -1116,57 +1115,57 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#start_gateway)
         """
 
     async def update_automatic_tape_creation_policy(
         self,
         *,
         AutomaticTapeCreationRules: Sequence[AutomaticTapeCreationRuleTypeDef],
-        GatewayARN: str
+        GatewayARN: str,
     ) -> UpdateAutomaticTapeCreationPolicyOutputTypeDef:
         """
         Updates the automatic tape creation policy of a gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_automatic_tape_creation_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#update_automatic_tape_creation_policy)
         """
 
     async def update_bandwidth_rate_limit(
         self,
         *,
         GatewayARN: str,
         AverageUploadRateLimitInBitsPerSec: int = ...,
-        AverageDownloadRateLimitInBitsPerSec: int = ...
+        AverageDownloadRateLimitInBitsPerSec: int = ...,
     ) -> UpdateBandwidthRateLimitOutputTypeDef:
         """
         Updates the bandwidth rate limits of a gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_bandwidth_rate_limit)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#update_bandwidth_rate_limit)
         """
 
     async def update_bandwidth_rate_limit_schedule(
         self,
         *,
         GatewayARN: str,
-        BandwidthRateLimitIntervals: Sequence[BandwidthRateLimitIntervalTypeDef]
+        BandwidthRateLimitIntervals: Sequence[BandwidthRateLimitIntervalTypeDef],
     ) -> UpdateBandwidthRateLimitScheduleOutputTypeDef:
         """
         Updates the bandwidth rate limit schedule for a specified gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_bandwidth_rate_limit_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#update_bandwidth_rate_limit_schedule)
         """
 
     async def update_chap_credentials(
         self,
         *,
         TargetARN: str,
         SecretToAuthenticateInitiator: str,
         InitiatorName: str,
-        SecretToAuthenticateTarget: str = ...
+        SecretToAuthenticateTarget: str = ...,
     ) -> UpdateChapCredentialsOutputTypeDef:
         """
         Updates the Challenge-Handshake Authentication Protocol (CHAP) credentials for
         a specified iSCSI
         target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_chap_credentials)
@@ -1176,15 +1175,15 @@
     async def update_file_system_association(
         self,
         *,
         FileSystemAssociationARN: str,
         UserName: str = ...,
         Password: str = ...,
         AuditDestinationARN: str = ...,
-        CacheAttributes: CacheAttributesTypeDef = ...
+        CacheAttributes: CacheAttributesTypeDef = ...,
     ) -> UpdateFileSystemAssociationOutputTypeDef:
         """
         Updates a file system association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_file_system_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#update_file_system_association)
         """
@@ -1192,15 +1191,15 @@
     async def update_gateway_information(
         self,
         *,
         GatewayARN: str,
         GatewayName: str = ...,
         GatewayTimezone: str = ...,
         CloudWatchLogGroupARN: str = ...,
-        GatewayCapacity: GatewayCapacityType = ...
+        GatewayCapacity: GatewayCapacityType = ...,
     ) -> UpdateGatewayInformationOutputTypeDef:
         """
         Updates a gateway's metadata, which includes the gateway's name and time zone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_gateway_information)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#update_gateway_information)
         """
@@ -1218,15 +1217,15 @@
     async def update_maintenance_start_time(
         self,
         *,
         GatewayARN: str,
         HourOfDay: int,
         MinuteOfHour: int,
         DayOfWeek: int = ...,
-        DayOfMonth: int = ...
+        DayOfMonth: int = ...,
     ) -> UpdateMaintenanceStartTimeOutputTypeDef:
         """
         Updates a gateway's weekly maintenance start time information, including day
         and time of the
         week.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_maintenance_start_time)
@@ -1246,15 +1245,15 @@
         Squash: str = ...,
         ReadOnly: bool = ...,
         GuessMIMETypeEnabled: bool = ...,
         RequesterPays: bool = ...,
         FileShareName: str = ...,
         CacheAttributes: CacheAttributesTypeDef = ...,
         NotificationPolicy: str = ...,
-        AuditDestinationARN: str = ...
+        AuditDestinationARN: str = ...,
     ) -> UpdateNFSFileShareOutputTypeDef:
         """
         Updates a Network File System (NFS) file share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_nfs_file_share)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#update_nfs_file_share)
         """
@@ -1276,15 +1275,15 @@
         ValidUserList: Sequence[str] = ...,
         InvalidUserList: Sequence[str] = ...,
         AuditDestinationARN: str = ...,
         CaseSensitivity: CaseSensitivityType = ...,
         FileShareName: str = ...,
         CacheAttributes: CacheAttributesTypeDef = ...,
         NotificationPolicy: str = ...,
-        OplocksEnabled: bool = ...
+        OplocksEnabled: bool = ...,
     ) -> UpdateSMBFileShareOutputTypeDef:
         """
         Updates a Server Message Block (SMB) file share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_smb_file_share)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#update_smb_file_share)
         """
@@ -1326,15 +1325,15 @@
     async def update_snapshot_schedule(
         self,
         *,
         VolumeARN: str,
         StartAt: int,
         RecurrenceInHours: int,
         Description: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> UpdateSnapshotScheduleOutputTypeDef:
         """
         Updates a snapshot schedule configured for a gateway volume.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_snapshot_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#update_snapshot_schedule)
         """
```

### Comparing `types-aiobotocore-storagegateway-2.9.0/types_aiobotocore_storagegateway/client.pyi` & `types-aiobotocore-storagegateway-2.9.1/types_aiobotocore_storagegateway/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,15 @@
         ActivationKey: str,
         GatewayName: str,
         GatewayTimezone: str,
         GatewayRegion: str,
         GatewayType: str = ...,
         TapeDriveType: str = ...,
         MediumChangerType: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> ActivateGatewayOutputTypeDef:
         """
         Activates the gateway you previously deployed on your host.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.activate_gateway)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#activate_gateway)
         """
@@ -254,15 +254,15 @@
         Password: str,
         ClientToken: str,
         GatewayARN: str,
         LocationARN: str,
         Tags: Sequence[TagTypeDef] = ...,
         AuditDestinationARN: str = ...,
         CacheAttributes: CacheAttributesTypeDef = ...,
-        EndpointNetworkConfiguration: EndpointNetworkConfigurationTypeDef = ...
+        EndpointNetworkConfiguration: EndpointNetworkConfigurationTypeDef = ...,
     ) -> AssociateFileSystemOutputTypeDef:
         """
         Associate an Amazon FSx file system with the FSx File Gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.associate_file_system)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#associate_file_system)
         """
@@ -270,15 +270,15 @@
     async def attach_volume(
         self,
         *,
         GatewayARN: str,
         VolumeARN: str,
         NetworkInterfaceId: str,
         TargetName: str = ...,
-        DiskId: str = ...
+        DiskId: str = ...,
     ) -> AttachVolumeOutputTypeDef:
         """
         Connects a volume to an iSCSI connection and then attaches the volume to the
         specified
         gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.attach_volume)
@@ -333,15 +333,15 @@
         TargetName: str,
         NetworkInterfaceId: str,
         ClientToken: str,
         SnapshotId: str = ...,
         SourceVolumeARN: str = ...,
         KMSEncrypted: bool = ...,
         KMSKey: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateCachediSCSIVolumeOutputTypeDef:
         """
         Creates a cached volume on a specified cached volume gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.create_cached_iscsi_volume)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#create_cached_iscsi_volume)
         """
@@ -365,15 +365,15 @@
         RequesterPays: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
         FileShareName: str = ...,
         CacheAttributes: CacheAttributesTypeDef = ...,
         NotificationPolicy: str = ...,
         VPCEndpointDNSName: str = ...,
         BucketRegion: str = ...,
-        AuditDestinationARN: str = ...
+        AuditDestinationARN: str = ...,
     ) -> CreateNFSFileShareOutputTypeDef:
         """
         Creates a Network File System (NFS) file share on an existing S3 File Gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.create_nfs_file_share)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#create_nfs_file_share)
         """
@@ -402,15 +402,15 @@
         CaseSensitivity: CaseSensitivityType = ...,
         Tags: Sequence[TagTypeDef] = ...,
         FileShareName: str = ...,
         CacheAttributes: CacheAttributesTypeDef = ...,
         NotificationPolicy: str = ...,
         VPCEndpointDNSName: str = ...,
         BucketRegion: str = ...,
-        OplocksEnabled: bool = ...
+        OplocksEnabled: bool = ...,
     ) -> CreateSMBFileShareOutputTypeDef:
         """
         Creates a Server Message Block (SMB) file share on an existing S3 File Gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.create_smb_file_share)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#create_smb_file_share)
         """
@@ -442,15 +442,15 @@
         DiskId: str,
         PreserveExistingData: bool,
         TargetName: str,
         NetworkInterfaceId: str,
         SnapshotId: str = ...,
         KMSEncrypted: bool = ...,
         KMSKey: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateStorediSCSIVolumeOutputTypeDef:
         """
         Creates a volume on a specified gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.create_stored_iscsi_volume)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#create_stored_iscsi_volume)
         """
@@ -458,15 +458,15 @@
     async def create_tape_pool(
         self,
         *,
         PoolName: str,
         StorageClass: TapeStorageClassType,
         RetentionLockType: RetentionLockTypeType = ...,
         RetentionLockTimeInDays: int = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateTapePoolOutputTypeDef:
         """
         Creates a new custom tape pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.create_tape_pool)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#create_tape_pool)
         """
@@ -477,15 +477,15 @@
         GatewayARN: str,
         TapeSizeInBytes: int,
         TapeBarcode: str,
         KMSEncrypted: bool = ...,
         KMSKey: str = ...,
         PoolId: str = ...,
         Worm: bool = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateTapeWithBarcodeOutputTypeDef:
         """
         Creates a virtual tape by using your own barcode.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.create_tape_with_barcode)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#create_tape_with_barcode)
         """
@@ -498,15 +498,15 @@
         ClientToken: str,
         NumTapesToCreate: int,
         TapeBarcodePrefix: str,
         KMSEncrypted: bool = ...,
         KMSKey: str = ...,
         PoolId: str = ...,
         Worm: bool = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateTapesOutputTypeDef:
         """
         Creates one or more virtual tapes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.create_tapes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#create_tapes)
         """
@@ -804,15 +804,15 @@
 
     async def describe_vtl_devices(
         self,
         *,
         GatewayARN: str,
         VTLDeviceARNs: Sequence[str] = ...,
         Marker: str = ...,
-        Limit: int = ...
+        Limit: int = ...,
     ) -> DescribeVTLDevicesOutputTypeDef:
         """
         Returns a description of virtual tape library (VTL) devices for the specified
         tape
         gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.describe_vtl_devices)
@@ -878,15 +878,15 @@
         *,
         GatewayARN: str,
         DomainName: str,
         UserName: str,
         Password: str,
         OrganizationalUnit: str = ...,
         DomainControllers: Sequence[str] = ...,
-        TimeoutInSeconds: int = ...
+        TimeoutInSeconds: int = ...,
     ) -> JoinDomainOutputTypeDef:
         """
         Adds a file gateway to an Active Directory domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.join_domain)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#join_domain)
         """
@@ -1112,57 +1112,57 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#start_gateway)
         """
 
     async def update_automatic_tape_creation_policy(
         self,
         *,
         AutomaticTapeCreationRules: Sequence[AutomaticTapeCreationRuleTypeDef],
-        GatewayARN: str
+        GatewayARN: str,
     ) -> UpdateAutomaticTapeCreationPolicyOutputTypeDef:
         """
         Updates the automatic tape creation policy of a gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_automatic_tape_creation_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#update_automatic_tape_creation_policy)
         """
 
     async def update_bandwidth_rate_limit(
         self,
         *,
         GatewayARN: str,
         AverageUploadRateLimitInBitsPerSec: int = ...,
-        AverageDownloadRateLimitInBitsPerSec: int = ...
+        AverageDownloadRateLimitInBitsPerSec: int = ...,
     ) -> UpdateBandwidthRateLimitOutputTypeDef:
         """
         Updates the bandwidth rate limits of a gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_bandwidth_rate_limit)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#update_bandwidth_rate_limit)
         """
 
     async def update_bandwidth_rate_limit_schedule(
         self,
         *,
         GatewayARN: str,
-        BandwidthRateLimitIntervals: Sequence[BandwidthRateLimitIntervalTypeDef]
+        BandwidthRateLimitIntervals: Sequence[BandwidthRateLimitIntervalTypeDef],
     ) -> UpdateBandwidthRateLimitScheduleOutputTypeDef:
         """
         Updates the bandwidth rate limit schedule for a specified gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_bandwidth_rate_limit_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#update_bandwidth_rate_limit_schedule)
         """
 
     async def update_chap_credentials(
         self,
         *,
         TargetARN: str,
         SecretToAuthenticateInitiator: str,
         InitiatorName: str,
-        SecretToAuthenticateTarget: str = ...
+        SecretToAuthenticateTarget: str = ...,
     ) -> UpdateChapCredentialsOutputTypeDef:
         """
         Updates the Challenge-Handshake Authentication Protocol (CHAP) credentials for
         a specified iSCSI
         target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_chap_credentials)
@@ -1172,15 +1172,15 @@
     async def update_file_system_association(
         self,
         *,
         FileSystemAssociationARN: str,
         UserName: str = ...,
         Password: str = ...,
         AuditDestinationARN: str = ...,
-        CacheAttributes: CacheAttributesTypeDef = ...
+        CacheAttributes: CacheAttributesTypeDef = ...,
     ) -> UpdateFileSystemAssociationOutputTypeDef:
         """
         Updates a file system association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_file_system_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#update_file_system_association)
         """
@@ -1188,15 +1188,15 @@
     async def update_gateway_information(
         self,
         *,
         GatewayARN: str,
         GatewayName: str = ...,
         GatewayTimezone: str = ...,
         CloudWatchLogGroupARN: str = ...,
-        GatewayCapacity: GatewayCapacityType = ...
+        GatewayCapacity: GatewayCapacityType = ...,
     ) -> UpdateGatewayInformationOutputTypeDef:
         """
         Updates a gateway's metadata, which includes the gateway's name and time zone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_gateway_information)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#update_gateway_information)
         """
@@ -1214,15 +1214,15 @@
     async def update_maintenance_start_time(
         self,
         *,
         GatewayARN: str,
         HourOfDay: int,
         MinuteOfHour: int,
         DayOfWeek: int = ...,
-        DayOfMonth: int = ...
+        DayOfMonth: int = ...,
     ) -> UpdateMaintenanceStartTimeOutputTypeDef:
         """
         Updates a gateway's weekly maintenance start time information, including day
         and time of the
         week.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_maintenance_start_time)
@@ -1242,15 +1242,15 @@
         Squash: str = ...,
         ReadOnly: bool = ...,
         GuessMIMETypeEnabled: bool = ...,
         RequesterPays: bool = ...,
         FileShareName: str = ...,
         CacheAttributes: CacheAttributesTypeDef = ...,
         NotificationPolicy: str = ...,
-        AuditDestinationARN: str = ...
+        AuditDestinationARN: str = ...,
     ) -> UpdateNFSFileShareOutputTypeDef:
         """
         Updates a Network File System (NFS) file share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_nfs_file_share)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#update_nfs_file_share)
         """
@@ -1272,15 +1272,15 @@
         ValidUserList: Sequence[str] = ...,
         InvalidUserList: Sequence[str] = ...,
         AuditDestinationARN: str = ...,
         CaseSensitivity: CaseSensitivityType = ...,
         FileShareName: str = ...,
         CacheAttributes: CacheAttributesTypeDef = ...,
         NotificationPolicy: str = ...,
-        OplocksEnabled: bool = ...
+        OplocksEnabled: bool = ...,
     ) -> UpdateSMBFileShareOutputTypeDef:
         """
         Updates a Server Message Block (SMB) file share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_smb_file_share)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#update_smb_file_share)
         """
@@ -1322,15 +1322,15 @@
     async def update_snapshot_schedule(
         self,
         *,
         VolumeARN: str,
         StartAt: int,
         RecurrenceInHours: int,
         Description: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> UpdateSnapshotScheduleOutputTypeDef:
         """
         Updates a snapshot schedule configured for a gateway volume.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_snapshot_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#update_snapshot_schedule)
         """
```

### Comparing `types-aiobotocore-storagegateway-2.9.0/types_aiobotocore_storagegateway/literals.py` & `types-aiobotocore-storagegateway-2.9.1/types_aiobotocore_storagegateway/literals.py`

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
     "ActiveDirectoryStatusType",
     "AvailabilityMonitorTestStatusType",
     "CaseSensitivityType",
     "DescribeTapeArchivesPaginatorName",
     "DescribeTapeRecoveryPointsPaginatorName",
     "DescribeTapesPaginatorName",
@@ -46,15 +45,14 @@
     "StorageGatewayServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ActiveDirectoryStatusType = Literal[
     "ACCESS_DENIED", "DETACHED", "JOINED", "JOINING", "NETWORK_ERROR", "TIMEOUT", "UNKNOWN_ERROR"
 ]
 AvailabilityMonitorTestStatusType = Literal["COMPLETE", "FAILED", "PENDING"]
 CaseSensitivityType = Literal["CaseSensitive", "ClientSpecified"]
 DescribeTapeArchivesPaginatorName = Literal["describe_tape_archives"]
 DescribeTapeRecoveryPointsPaginatorName = Literal["describe_tape_recovery_points"]
```

### Comparing `types-aiobotocore-storagegateway-2.9.0/types_aiobotocore_storagegateway/literals.pyi` & `types-aiobotocore-storagegateway-2.9.1/types_aiobotocore_storagegateway/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-storagegateway-2.9.0/types_aiobotocore_storagegateway/paginator.py` & `types-aiobotocore-storagegateway-2.9.1/types_aiobotocore_storagegateway/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,14 @@
     "ListGatewaysPaginator",
     "ListTagsForResourcePaginator",
     "ListTapePoolsPaginator",
     "ListTapesPaginator",
     "ListVolumesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -123,15 +122,15 @@
     """
 
     def paginate(
         self,
         *,
         GatewayARN: str,
         TapeARNs: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeTapesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.DescribeTapes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/paginators/#describetapespaginator)
         """
 
 
@@ -142,15 +141,15 @@
     """
 
     def paginate(
         self,
         *,
         GatewayARN: str,
         VTLDeviceARNs: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeVTLDevicesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.DescribeVTLDevices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/paginators/#describevtldevicespaginator)
         """
```

### Comparing `types-aiobotocore-storagegateway-2.9.0/types_aiobotocore_storagegateway/paginator.pyi` & `types-aiobotocore-storagegateway-2.9.1/types_aiobotocore_storagegateway/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
     """
 
     def paginate(
         self,
         *,
         GatewayARN: str,
         TapeARNs: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeTapesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.DescribeTapes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/paginators/#describetapespaginator)
         """
 
 class DescribeVTLDevicesPaginator(AioPaginator):
@@ -136,15 +136,15 @@
     """
 
     def paginate(
         self,
         *,
         GatewayARN: str,
         VTLDeviceARNs: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeVTLDevicesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.DescribeVTLDevices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/paginators/#describevtldevicespaginator)
         """
 
 class ListFileSharesPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-storagegateway-2.9.0/types_aiobotocore_storagegateway/type_defs.py` & `types-aiobotocore-storagegateway-2.9.1/types_aiobotocore_storagegateway/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,14 @@
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
     "AddCacheInputRequestTypeDef",
     "AddUploadBufferInputRequestTypeDef",
     "AddWorkingStorageInputRequestTypeDef",
     "AssignTapePoolInputRequestTypeDef",
```

### Comparing `types-aiobotocore-storagegateway-2.9.0/types_aiobotocore_storagegateway/type_defs.pyi` & `types-aiobotocore-storagegateway-2.9.1/types_aiobotocore_storagegateway/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-storagegateway-2.9.0/types_aiobotocore_storagegateway.egg-info/PKG-INFO` & `types-aiobotocore-storagegateway-2.9.1/types_aiobotocore_storagegateway.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-storagegateway
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.StorageGateway 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.StorageGateway 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/
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
 
 <a id="types-aiobotocore-storagegateway"></a>
 
 # types-aiobotocore-storagegateway
 
 [![PyPI - types-aiobotocore-storagegateway](https://img.shields.io/pypi/v/types-aiobotocore-storagegateway.svg?color=blue)](https://pypi.org/project/types-aiobotocore-storagegateway)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-storagegateway.svg?color=blue)](https://pypi.org/project/types-aiobotocore-storagegateway)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-storagegateway)](https://pepy.tech/project/types-aiobotocore-storagegateway)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.StorageGateway 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway)
+[aiobotocore.StorageGateway 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway)
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
 [types-aiobotocore-storagegateway docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-storagegateway-2.9.0/types_aiobotocore_storagegateway.egg-info/SOURCES.txt` & `types-aiobotocore-storagegateway-2.9.1/types_aiobotocore_storagegateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

