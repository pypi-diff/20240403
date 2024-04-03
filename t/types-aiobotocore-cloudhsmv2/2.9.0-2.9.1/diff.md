# Comparing `tmp/types-aiobotocore-cloudhsmv2-2.9.0.tar.gz` & `tmp/types-aiobotocore-cloudhsmv2-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cloudhsmv2-2.9.0.tar", last modified: Wed Dec 13 19:58:50 2023, max compression
+gzip compressed data, was "types-aiobotocore-cloudhsmv2-2.9.1.tar", last modified: Thu Jan 18 01:20:17 2024, max compression
```

## Comparing `types-aiobotocore-cloudhsmv2-2.9.0.tar` & `types-aiobotocore-cloudhsmv2-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:50.361967 types-aiobotocore-cloudhsmv2-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:42:30.000000 types-aiobotocore-cloudhsmv2-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13390 2023-12-13 19:58:50.361967 types-aiobotocore-cloudhsmv2-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11815 2023-12-13 19:42:30.000000 types-aiobotocore-cloudhsmv2-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:50.361967 types-aiobotocore-cloudhsmv2-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2023-12-13 19:42:30.000000 types-aiobotocore-cloudhsmv2-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:50.361967 types-aiobotocore-cloudhsmv2-2.9.0/types_aiobotocore_cloudhsmv2/
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2023-12-13 19:42:30.000000 types-aiobotocore-cloudhsmv2-2.9.0/types_aiobotocore_cloudhsmv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2023-12-13 19:42:30.000000 types-aiobotocore-cloudhsmv2-2.9.0/types_aiobotocore_cloudhsmv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      944 2023-12-13 19:42:30.000000 types-aiobotocore-cloudhsmv2-2.9.0/types_aiobotocore_cloudhsmv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14713 2023-12-13 19:42:30.000000 types-aiobotocore-cloudhsmv2-2.9.0/types_aiobotocore_cloudhsmv2/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14709 2023-12-13 19:42:30.000000 types-aiobotocore-cloudhsmv2-2.9.0/types_aiobotocore_cloudhsmv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9598 2023-12-13 19:42:31.000000 types-aiobotocore-cloudhsmv2-2.9.0/types_aiobotocore_cloudhsmv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9596 2023-12-13 19:42:30.000000 types-aiobotocore-cloudhsmv2-2.9.0/types_aiobotocore_cloudhsmv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2023-12-13 19:42:30.000000 types-aiobotocore-cloudhsmv2-2.9.0/types_aiobotocore_cloudhsmv2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4341 2023-12-13 19:42:30.000000 types-aiobotocore-cloudhsmv2-2.9.0/types_aiobotocore_cloudhsmv2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:42:30.000000 types-aiobotocore-cloudhsmv2-2.9.0/types_aiobotocore_cloudhsmv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    11663 2023-12-13 19:42:31.000000 types-aiobotocore-cloudhsmv2-2.9.0/types_aiobotocore_cloudhsmv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11662 2023-12-13 19:42:31.000000 types-aiobotocore-cloudhsmv2-2.9.0/types_aiobotocore_cloudhsmv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:42:30.000000 types-aiobotocore-cloudhsmv2-2.9.0/types_aiobotocore_cloudhsmv2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:50.361967 types-aiobotocore-cloudhsmv2-2.9.0/types_aiobotocore_cloudhsmv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13390 2023-12-13 19:58:50.000000 types-aiobotocore-cloudhsmv2-2.9.0/types_aiobotocore_cloudhsmv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      870 2023-12-13 19:58:50.000000 types-aiobotocore-cloudhsmv2-2.9.0/types_aiobotocore_cloudhsmv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:50.000000 types-aiobotocore-cloudhsmv2-2.9.0/types_aiobotocore_cloudhsmv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:50.000000 types-aiobotocore-cloudhsmv2-2.9.0/types_aiobotocore_cloudhsmv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:50.000000 types-aiobotocore-cloudhsmv2-2.9.0/types_aiobotocore_cloudhsmv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-13 19:58:50.000000 types-aiobotocore-cloudhsmv2-2.9.0/types_aiobotocore_cloudhsmv2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:17.045458 types-aiobotocore-cloudhsmv2-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:04:27.000000 types-aiobotocore-cloudhsmv2-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13410 2024-01-18 01:20:17.041458 types-aiobotocore-cloudhsmv2-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11815 2024-01-18 01:04:27.000000 types-aiobotocore-cloudhsmv2-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:17.045458 types-aiobotocore-cloudhsmv2-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-01-18 01:04:27.000000 types-aiobotocore-cloudhsmv2-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:17.041458 types-aiobotocore-cloudhsmv2-2.9.1/types_aiobotocore_cloudhsmv2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-01-18 01:04:27.000000 types-aiobotocore-cloudhsmv2-2.9.1/types_aiobotocore_cloudhsmv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-01-18 01:04:27.000000 types-aiobotocore-cloudhsmv2-2.9.1/types_aiobotocore_cloudhsmv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-01-18 01:04:27.000000 types-aiobotocore-cloudhsmv2-2.9.1/types_aiobotocore_cloudhsmv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14715 2024-01-18 01:04:27.000000 types-aiobotocore-cloudhsmv2-2.9.1/types_aiobotocore_cloudhsmv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14712 2024-01-18 01:04:27.000000 types-aiobotocore-cloudhsmv2-2.9.1/types_aiobotocore_cloudhsmv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9596 2024-01-18 01:04:28.000000 types-aiobotocore-cloudhsmv2-2.9.1/types_aiobotocore_cloudhsmv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9596 2024-01-18 01:04:28.000000 types-aiobotocore-cloudhsmv2-2.9.1/types_aiobotocore_cloudhsmv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-01-18 01:04:27.000000 types-aiobotocore-cloudhsmv2-2.9.1/types_aiobotocore_cloudhsmv2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-01-18 01:04:27.000000 types-aiobotocore-cloudhsmv2-2.9.1/types_aiobotocore_cloudhsmv2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:04:27.000000 types-aiobotocore-cloudhsmv2-2.9.1/types_aiobotocore_cloudhsmv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    11662 2024-01-18 01:04:28.000000 types-aiobotocore-cloudhsmv2-2.9.1/types_aiobotocore_cloudhsmv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11662 2024-01-18 01:04:28.000000 types-aiobotocore-cloudhsmv2-2.9.1/types_aiobotocore_cloudhsmv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:04:27.000000 types-aiobotocore-cloudhsmv2-2.9.1/types_aiobotocore_cloudhsmv2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:17.041458 types-aiobotocore-cloudhsmv2-2.9.1/types_aiobotocore_cloudhsmv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13410 2024-01-18 01:20:17.000000 types-aiobotocore-cloudhsmv2-2.9.1/types_aiobotocore_cloudhsmv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-01-18 01:20:17.000000 types-aiobotocore-cloudhsmv2-2.9.1/types_aiobotocore_cloudhsmv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:17.000000 types-aiobotocore-cloudhsmv2-2.9.1/types_aiobotocore_cloudhsmv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:17.000000 types-aiobotocore-cloudhsmv2-2.9.1/types_aiobotocore_cloudhsmv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:17.000000 types-aiobotocore-cloudhsmv2-2.9.1/types_aiobotocore_cloudhsmv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-01-18 01:20:17.000000 types-aiobotocore-cloudhsmv2-2.9.1/types_aiobotocore_cloudhsmv2.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cloudhsmv2-2.9.0/LICENSE` & `types-aiobotocore-cloudhsmv2-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-cloudhsmv2-2.9.0/PKG-INFO` & `types-aiobotocore-cloudhsmv2-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudhsmv2
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CloudHSMV2 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CloudHSMV2 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/
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
 
 <a id="types-aiobotocore-cloudhsmv2"></a>
 
 # types-aiobotocore-cloudhsmv2
 
 [![PyPI - types-aiobotocore-cloudhsmv2](https://img.shields.io/pypi/v/types-aiobotocore-cloudhsmv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudhsmv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudhsmv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudhsmv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudhsmv2)](https://pepy.tech/project/types-aiobotocore-cloudhsmv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudHSMV2 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2)
+[aiobotocore.CloudHSMV2 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2)
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
 [types-aiobotocore-cloudhsmv2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-cloudhsmv2-2.9.0/README.md` & `types-aiobotocore-cloudhsmv2-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudhsmv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudhsmv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudhsmv2)](https://pepy.tech/project/types-aiobotocore-cloudhsmv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudHSMV2 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2)
+[aiobotocore.CloudHSMV2 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2)
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
 [types-aiobotocore-cloudhsmv2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-cloudhsmv2-2.9.0/setup.py` & `types-aiobotocore-cloudhsmv2-2.9.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cloudhsmv2",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_cloudhsmv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CloudHSMV2 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.CloudHSMV2 2.9.1 service generated with"
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
     keywords="aiobotocore cloudhsmv2 type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_cloudhsmv2": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-cloudhsmv2-2.9.0/types_aiobotocore_cloudhsmv2/__init__.py` & `types-aiobotocore-cloudhsmv2-2.9.1/types_aiobotocore_cloudhsmv2/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 """
 
 from .client import CloudHSMV2Client
 from .paginator import DescribeBackupsPaginator, DescribeClustersPaginator, ListTagsPaginator
 
 Client = CloudHSMV2Client
 
-
 __all__ = (
     "Client",
     "CloudHSMV2Client",
     "DescribeBackupsPaginator",
     "DescribeClustersPaginator",
     "ListTagsPaginator",
 )
```

### Comparing `types-aiobotocore-cloudhsmv2-2.9.0/types_aiobotocore_cloudhsmv2/__init__.pyi` & `types-aiobotocore-cloudhsmv2-2.9.1/types_aiobotocore_cloudhsmv2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsmv2-2.9.0/types_aiobotocore_cloudhsmv2/__main__.py` & `types-aiobotocore-cloudhsmv2-2.9.1/types_aiobotocore_cloudhsmv2/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CloudHSMV2 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.CloudHSMV2 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2\nOther"
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

### Comparing `types-aiobotocore-cloudhsmv2-2.9.0/types_aiobotocore_cloudhsmv2/client.py` & `types-aiobotocore-cloudhsmv2-2.9.1/types_aiobotocore_cloudhsmv2/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("CloudHSMV2Client",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -113,15 +112,15 @@
     async def create_cluster(
         self,
         *,
         HsmType: str,
         SubnetIds: Sequence[str],
         BackupRetentionPolicy: BackupRetentionPolicyTypeDef = ...,
         SourceBackupId: str = ...,
-        TagList: Sequence[TagTypeDef] = ...
+        TagList: Sequence[TagTypeDef] = ...,
     ) -> CreateClusterResponseTypeDef:
         """
         Creates a new AWS CloudHSM cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Client.create_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/client/#create_cluster)
         """
@@ -165,29 +164,29 @@
 
     async def describe_backups(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         Filters: Mapping[str, Sequence[str]] = ...,
-        SortAscending: bool = ...
+        SortAscending: bool = ...,
     ) -> DescribeBackupsResponseTypeDef:
         """
         Gets information about backups of AWS CloudHSM clusters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Client.describe_backups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/client/#describe_backups)
         """
 
     async def describe_clusters(
         self,
         *,
         Filters: Mapping[str, Sequence[str]] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeClustersResponseTypeDef:
         """
         Gets information about AWS CloudHSM clusters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Client.describe_clusters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/client/#describe_clusters)
         """
```

### Comparing `types-aiobotocore-cloudhsmv2-2.9.0/types_aiobotocore_cloudhsmv2/client.pyi` & `types-aiobotocore-cloudhsmv2-2.9.1/types_aiobotocore_cloudhsmv2/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
     async def create_cluster(
         self,
         *,
         HsmType: str,
         SubnetIds: Sequence[str],
         BackupRetentionPolicy: BackupRetentionPolicyTypeDef = ...,
         SourceBackupId: str = ...,
-        TagList: Sequence[TagTypeDef] = ...
+        TagList: Sequence[TagTypeDef] = ...,
     ) -> CreateClusterResponseTypeDef:
         """
         Creates a new AWS CloudHSM cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Client.create_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/client/#create_cluster)
         """
@@ -161,29 +161,29 @@
 
     async def describe_backups(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         Filters: Mapping[str, Sequence[str]] = ...,
-        SortAscending: bool = ...
+        SortAscending: bool = ...,
     ) -> DescribeBackupsResponseTypeDef:
         """
         Gets information about backups of AWS CloudHSM clusters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Client.describe_backups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/client/#describe_backups)
         """
 
     async def describe_clusters(
         self,
         *,
         Filters: Mapping[str, Sequence[str]] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeClustersResponseTypeDef:
         """
         Gets information about AWS CloudHSM clusters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Client.describe_clusters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/client/#describe_clusters)
         """
```

### Comparing `types-aiobotocore-cloudhsmv2-2.9.0/types_aiobotocore_cloudhsmv2/literals.py` & `types-aiobotocore-cloudhsmv2-2.9.1/types_aiobotocore_cloudhsmv2/literals.py`

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
     "BackupPolicyType",
     "BackupRetentionTypeType",
     "BackupStateType",
     "ClusterStateType",
     "DescribeBackupsPaginatorName",
     "DescribeClustersPaginatorName",
@@ -32,15 +31,14 @@
     "CloudHSMV2ServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 BackupPolicyType = Literal["DEFAULT"]
 BackupRetentionTypeType = Literal["DAYS"]
 BackupStateType = Literal["CREATE_IN_PROGRESS", "DELETED", "PENDING_DELETION", "READY"]
 ClusterStateType = Literal[
     "ACTIVE",
     "CREATE_IN_PROGRESS",
     "DEGRADED",
```

### Comparing `types-aiobotocore-cloudhsmv2-2.9.0/types_aiobotocore_cloudhsmv2/literals.pyi` & `types-aiobotocore-cloudhsmv2-2.9.1/types_aiobotocore_cloudhsmv2/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsmv2-2.9.0/types_aiobotocore_cloudhsmv2/paginator.py` & `types-aiobotocore-cloudhsmv2-2.9.1/types_aiobotocore_cloudhsmv2/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,14 @@
     DescribeClustersResponseTypeDef,
     ListTagsResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("DescribeBackupsPaginator", "DescribeClustersPaginator", "ListTagsPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -57,15 +56,15 @@
     """
 
     def paginate(
         self,
         *,
         Filters: Mapping[str, Sequence[str]] = ...,
         SortAscending: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeBackupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Paginator.DescribeBackups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/paginators/#describebackupspaginator)
         """
 
 
@@ -75,15 +74,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/paginators/#describeclusterspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Mapping[str, Sequence[str]] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeClustersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Paginator.DescribeClusters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/paginators/#describeclusterspaginator)
         """
```

### Comparing `types-aiobotocore-cloudhsmv2-2.9.0/types_aiobotocore_cloudhsmv2/paginator.pyi` & `types-aiobotocore-cloudhsmv2-2.9.1/types_aiobotocore_cloudhsmv2/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     """
 
     def paginate(
         self,
         *,
         Filters: Mapping[str, Sequence[str]] = ...,
         SortAscending: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeBackupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Paginator.DescribeBackups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/paginators/#describebackupspaginator)
         """
 
 class DescribeClustersPaginator(AioPaginator):
@@ -71,15 +71,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/paginators/#describeclusterspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Mapping[str, Sequence[str]] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeClustersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Paginator.DescribeClusters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/paginators/#describeclusterspaginator)
         """
 
 class ListTagsPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-cloudhsmv2-2.9.0/types_aiobotocore_cloudhsmv2/type_defs.py` & `types-aiobotocore-cloudhsmv2-2.9.1/types_aiobotocore_cloudhsmv2/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "BackupRetentionPolicyTypeDef",
     "TagTypeDef",
     "CertificatesTypeDef",
     "HsmTypeDef",
     "DestinationBackupTypeDef",
     "ResponseMetadataTypeDef",
```

### Comparing `types-aiobotocore-cloudhsmv2-2.9.0/types_aiobotocore_cloudhsmv2/type_defs.pyi` & `types-aiobotocore-cloudhsmv2-2.9.1/types_aiobotocore_cloudhsmv2/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsmv2-2.9.0/types_aiobotocore_cloudhsmv2.egg-info/PKG-INFO` & `types-aiobotocore-cloudhsmv2-2.9.1/types_aiobotocore_cloudhsmv2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudhsmv2
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CloudHSMV2 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CloudHSMV2 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/
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
 
 <a id="types-aiobotocore-cloudhsmv2"></a>
 
 # types-aiobotocore-cloudhsmv2
 
 [![PyPI - types-aiobotocore-cloudhsmv2](https://img.shields.io/pypi/v/types-aiobotocore-cloudhsmv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudhsmv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudhsmv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudhsmv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudhsmv2)](https://pepy.tech/project/types-aiobotocore-cloudhsmv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudHSMV2 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2)
+[aiobotocore.CloudHSMV2 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2)
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
 [types-aiobotocore-cloudhsmv2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-cloudhsmv2-2.9.0/types_aiobotocore_cloudhsmv2.egg-info/SOURCES.txt` & `types-aiobotocore-cloudhsmv2-2.9.1/types_aiobotocore_cloudhsmv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

