# Comparing `tmp/types-aiobotocore-iotfleethub-2.9.0.tar.gz` & `tmp/types-aiobotocore-iotfleethub-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iotfleethub-2.9.0.tar", last modified: Wed Dec 13 19:59:33 2023, max compression
+gzip compressed data, was "types-aiobotocore-iotfleethub-2.9.1.tar", last modified: Thu Jan 18 01:20:57 2024, max compression
```

## Comparing `types-aiobotocore-iotfleethub-2.9.0.tar` & `types-aiobotocore-iotfleethub-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:33.633637 types-aiobotocore-iotfleethub-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:47:58.000000 types-aiobotocore-iotfleethub-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13210 2023-12-13 19:59:33.633637 types-aiobotocore-iotfleethub-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11631 2023-12-13 19:47:58.000000 types-aiobotocore-iotfleethub-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:33.633637 types-aiobotocore-iotfleethub-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2023-12-13 19:47:58.000000 types-aiobotocore-iotfleethub-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:33.633637 types-aiobotocore-iotfleethub-2.9.0/types_aiobotocore_iotfleethub/
--rw-r--r--   0 runner    (1001) docker     (127)      692 2023-12-13 19:47:58.000000 types-aiobotocore-iotfleethub-2.9.0/types_aiobotocore_iotfleethub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2023-12-13 19:47:58.000000 types-aiobotocore-iotfleethub-2.9.0/types_aiobotocore_iotfleethub/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      948 2023-12-13 19:47:58.000000 types-aiobotocore-iotfleethub-2.9.0/types_aiobotocore_iotfleethub/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9575 2023-12-13 19:47:58.000000 types-aiobotocore-iotfleethub-2.9.0/types_aiobotocore_iotfleethub/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     9571 2023-12-13 19:47:58.000000 types-aiobotocore-iotfleethub-2.9.0/types_aiobotocore_iotfleethub/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8697 2023-12-13 19:47:58.000000 types-aiobotocore-iotfleethub-2.9.0/types_aiobotocore_iotfleethub/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8695 2023-12-13 19:47:58.000000 types-aiobotocore-iotfleethub-2.9.0/types_aiobotocore_iotfleethub/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2023-12-13 19:47:58.000000 types-aiobotocore-iotfleethub-2.9.0/types_aiobotocore_iotfleethub/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2023-12-13 19:47:58.000000 types-aiobotocore-iotfleethub-2.9.0/types_aiobotocore_iotfleethub/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:47:58.000000 types-aiobotocore-iotfleethub-2.9.0/types_aiobotocore_iotfleethub/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5181 2023-12-13 19:47:58.000000 types-aiobotocore-iotfleethub-2.9.0/types_aiobotocore_iotfleethub/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5180 2023-12-13 19:47:58.000000 types-aiobotocore-iotfleethub-2.9.0/types_aiobotocore_iotfleethub/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:47:58.000000 types-aiobotocore-iotfleethub-2.9.0/types_aiobotocore_iotfleethub/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:33.633637 types-aiobotocore-iotfleethub-2.9.0/types_aiobotocore_iotfleethub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13210 2023-12-13 19:59:33.000000 types-aiobotocore-iotfleethub-2.9.0/types_aiobotocore_iotfleethub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      889 2023-12-13 19:59:33.000000 types-aiobotocore-iotfleethub-2.9.0/types_aiobotocore_iotfleethub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:33.000000 types-aiobotocore-iotfleethub-2.9.0/types_aiobotocore_iotfleethub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:33.000000 types-aiobotocore-iotfleethub-2.9.0/types_aiobotocore_iotfleethub.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:33.000000 types-aiobotocore-iotfleethub-2.9.0/types_aiobotocore_iotfleethub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-13 19:59:33.000000 types-aiobotocore-iotfleethub-2.9.0/types_aiobotocore_iotfleethub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:57.053267 types-aiobotocore-iotfleethub-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:09:47.000000 types-aiobotocore-iotfleethub-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13230 2024-01-18 01:20:57.053267 types-aiobotocore-iotfleethub-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11631 2024-01-18 01:09:47.000000 types-aiobotocore-iotfleethub-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:57.053267 types-aiobotocore-iotfleethub-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-01-18 01:09:47.000000 types-aiobotocore-iotfleethub-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:57.053267 types-aiobotocore-iotfleethub-2.9.1/types_aiobotocore_iotfleethub/
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-01-18 01:09:47.000000 types-aiobotocore-iotfleethub-2.9.1/types_aiobotocore_iotfleethub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-01-18 01:09:47.000000 types-aiobotocore-iotfleethub-2.9.1/types_aiobotocore_iotfleethub/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-01-18 01:09:47.000000 types-aiobotocore-iotfleethub-2.9.1/types_aiobotocore_iotfleethub/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9576 2024-01-18 01:09:47.000000 types-aiobotocore-iotfleethub-2.9.1/types_aiobotocore_iotfleethub/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9573 2024-01-18 01:09:47.000000 types-aiobotocore-iotfleethub-2.9.1/types_aiobotocore_iotfleethub/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8695 2024-01-18 01:09:47.000000 types-aiobotocore-iotfleethub-2.9.1/types_aiobotocore_iotfleethub/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8695 2024-01-18 01:09:47.000000 types-aiobotocore-iotfleethub-2.9.1/types_aiobotocore_iotfleethub/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-01-18 01:09:47.000000 types-aiobotocore-iotfleethub-2.9.1/types_aiobotocore_iotfleethub/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-01-18 01:09:47.000000 types-aiobotocore-iotfleethub-2.9.1/types_aiobotocore_iotfleethub/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:09:47.000000 types-aiobotocore-iotfleethub-2.9.1/types_aiobotocore_iotfleethub/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-01-18 01:09:47.000000 types-aiobotocore-iotfleethub-2.9.1/types_aiobotocore_iotfleethub/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-01-18 01:09:47.000000 types-aiobotocore-iotfleethub-2.9.1/types_aiobotocore_iotfleethub/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:09:47.000000 types-aiobotocore-iotfleethub-2.9.1/types_aiobotocore_iotfleethub/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:57.053267 types-aiobotocore-iotfleethub-2.9.1/types_aiobotocore_iotfleethub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13230 2024-01-18 01:20:57.000000 types-aiobotocore-iotfleethub-2.9.1/types_aiobotocore_iotfleethub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-01-18 01:20:57.000000 types-aiobotocore-iotfleethub-2.9.1/types_aiobotocore_iotfleethub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:57.000000 types-aiobotocore-iotfleethub-2.9.1/types_aiobotocore_iotfleethub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:57.000000 types-aiobotocore-iotfleethub-2.9.1/types_aiobotocore_iotfleethub.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:57.000000 types-aiobotocore-iotfleethub-2.9.1/types_aiobotocore_iotfleethub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-01-18 01:20:57.000000 types-aiobotocore-iotfleethub-2.9.1/types_aiobotocore_iotfleethub.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iotfleethub-2.9.0/LICENSE` & `types-aiobotocore-iotfleethub-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-iotfleethub-2.9.0/PKG-INFO` & `types-aiobotocore-iotfleethub-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotfleethub
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.IoTFleetHub 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.IoTFleetHub 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleethub/
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
 
 <a id="types-aiobotocore-iotfleethub"></a>
 
 # types-aiobotocore-iotfleethub
 
 [![PyPI - types-aiobotocore-iotfleethub](https://img.shields.io/pypi/v/types-aiobotocore-iotfleethub.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotfleethub)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotfleethub.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotfleethub)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleethub/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotfleethub)](https://pepy.tech/project/types-aiobotocore-iotfleethub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTFleetHub 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub)
+[aiobotocore.IoTFleetHub 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub)
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
 [types-aiobotocore-iotfleethub docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleethub/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-iotfleethub-2.9.0/README.md` & `types-aiobotocore-iotfleethub-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotfleethub.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotfleethub)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleethub/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotfleethub)](https://pepy.tech/project/types-aiobotocore-iotfleethub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTFleetHub 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub)
+[aiobotocore.IoTFleetHub 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub)
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
 [types-aiobotocore-iotfleethub docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleethub/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-iotfleethub-2.9.0/setup.py` & `types-aiobotocore-iotfleethub-2.9.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iotfleethub",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_iotfleethub"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.IoTFleetHub 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.IoTFleetHub 2.9.1 service generated with"
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
     keywords="aiobotocore iotfleethub type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_iotfleethub": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleethub/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-iotfleethub-2.9.0/types_aiobotocore_iotfleethub/__init__.py` & `types-aiobotocore-iotfleethub-2.9.1/types_aiobotocore_iotfleethub/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,9 +22,8 @@
 """
 
 from .client import IoTFleetHubClient
 from .paginator import ListApplicationsPaginator
 
 Client = IoTFleetHubClient
 
-
 __all__ = ("Client", "IoTFleetHubClient", "ListApplicationsPaginator")
```

### Comparing `types-aiobotocore-iotfleethub-2.9.0/types_aiobotocore_iotfleethub/__init__.pyi` & `types-aiobotocore-iotfleethub-2.9.1/types_aiobotocore_iotfleethub/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotfleethub-2.9.0/types_aiobotocore_iotfleethub/__main__.py` & `types-aiobotocore-iotfleethub-2.9.1/types_aiobotocore_iotfleethub/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IoTFleetHub 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.IoTFleetHub 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleethub//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub\nOther"
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

### Comparing `types-aiobotocore-iotfleethub-2.9.0/types_aiobotocore_iotfleethub/client.py` & `types-aiobotocore-iotfleethub-2.9.1/types_aiobotocore_iotfleethub/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("IoTFleetHubClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -92,15 +91,15 @@
     async def create_application(
         self,
         *,
         applicationName: str,
         roleArn: str,
         applicationDescription: str = ...,
         clientToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateApplicationResponseTypeDef:
         """
         Creates a Fleet Hub for AWS IoT Device Management web application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub.Client.create_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleethub/client/#create_application)
         """
@@ -178,15 +177,15 @@
 
     async def update_application(
         self,
         *,
         applicationId: str,
         applicationName: str = ...,
         applicationDescription: str = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates information about a Fleet Hub for a AWS IoT Device Management web
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub.Client.update_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleethub/client/#update_application)
```

### Comparing `types-aiobotocore-iotfleethub-2.9.0/types_aiobotocore_iotfleethub/client.pyi` & `types-aiobotocore-iotfleethub-2.9.1/types_aiobotocore_iotfleethub/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     async def create_application(
         self,
         *,
         applicationName: str,
         roleArn: str,
         applicationDescription: str = ...,
         clientToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateApplicationResponseTypeDef:
         """
         Creates a Fleet Hub for AWS IoT Device Management web application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub.Client.create_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleethub/client/#create_application)
         """
@@ -174,15 +174,15 @@
 
     async def update_application(
         self,
         *,
         applicationId: str,
         applicationName: str = ...,
         applicationDescription: str = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates information about a Fleet Hub for a AWS IoT Device Management web
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub.Client.update_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleethub/client/#update_application)
```

### Comparing `types-aiobotocore-iotfleethub-2.9.0/types_aiobotocore_iotfleethub/literals.py` & `types-aiobotocore-iotfleethub-2.9.1/types_aiobotocore_iotfleethub/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,26 +15,24 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ApplicationStateType",
     "ListApplicationsPaginatorName",
     "IoTFleetHubServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ApplicationStateType = Literal["ACTIVE", "CREATE_FAILED", "CREATING", "DELETE_FAILED", "DELETING"]
 ListApplicationsPaginatorName = Literal["list_applications"]
 IoTFleetHubServiceName = Literal["iotfleethub"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
```

### Comparing `types-aiobotocore-iotfleethub-2.9.0/types_aiobotocore_iotfleethub/literals.pyi` & `types-aiobotocore-iotfleethub-2.9.1/types_aiobotocore_iotfleethub/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotfleethub-2.9.0/types_aiobotocore_iotfleethub/paginator.py` & `types-aiobotocore-iotfleethub-2.9.1/types_aiobotocore_iotfleethub/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .type_defs import ListApplicationsResponseTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListApplicationsPaginator",)
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
```

### Comparing `types-aiobotocore-iotfleethub-2.9.0/types_aiobotocore_iotfleethub/paginator.pyi` & `types-aiobotocore-iotfleethub-2.9.1/types_aiobotocore_iotfleethub/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotfleethub-2.9.0/types_aiobotocore_iotfleethub/type_defs.py` & `types-aiobotocore-iotfleethub-2.9.1/types_aiobotocore_iotfleethub/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ApplicationSummaryTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DescribeApplicationRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
```

### Comparing `types-aiobotocore-iotfleethub-2.9.0/types_aiobotocore_iotfleethub/type_defs.pyi` & `types-aiobotocore-iotfleethub-2.9.1/types_aiobotocore_iotfleethub/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotfleethub-2.9.0/types_aiobotocore_iotfleethub.egg-info/PKG-INFO` & `types-aiobotocore-iotfleethub-2.9.1/types_aiobotocore_iotfleethub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotfleethub
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.IoTFleetHub 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.IoTFleetHub 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleethub/
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
 
 <a id="types-aiobotocore-iotfleethub"></a>
 
 # types-aiobotocore-iotfleethub
 
 [![PyPI - types-aiobotocore-iotfleethub](https://img.shields.io/pypi/v/types-aiobotocore-iotfleethub.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotfleethub)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotfleethub.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotfleethub)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleethub/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotfleethub)](https://pepy.tech/project/types-aiobotocore-iotfleethub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTFleetHub 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub)
+[aiobotocore.IoTFleetHub 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub)
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
 [types-aiobotocore-iotfleethub docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleethub/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-iotfleethub-2.9.0/types_aiobotocore_iotfleethub.egg-info/SOURCES.txt` & `types-aiobotocore-iotfleethub-2.9.1/types_aiobotocore_iotfleethub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

