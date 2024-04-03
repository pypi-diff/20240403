# Comparing `tmp/types-aiobotocore-iotfleetwise-2.9.0.tar.gz` & `tmp/types-aiobotocore-iotfleetwise-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iotfleetwise-2.9.0.tar", last modified: Wed Dec 13 19:59:34 2023, max compression
+gzip compressed data, was "types-aiobotocore-iotfleetwise-2.9.1.tar", last modified: Thu Jan 18 01:20:57 2024, max compression
```

## Comparing `types-aiobotocore-iotfleetwise-2.9.0.tar` & `types-aiobotocore-iotfleetwise-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:34.001631 types-aiobotocore-iotfleetwise-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:47:58.000000 types-aiobotocore-iotfleetwise-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15220 2023-12-13 19:59:34.001631 types-aiobotocore-iotfleetwise-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13637 2023-12-13 19:47:58.000000 types-aiobotocore-iotfleetwise-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:34.001631 types-aiobotocore-iotfleetwise-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2023-12-13 19:47:58.000000 types-aiobotocore-iotfleetwise-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:34.001631 types-aiobotocore-iotfleetwise-2.9.0/types_aiobotocore_iotfleetwise/
--rw-r--r--   0 runner    (1001) docker     (127)     3446 2023-12-13 19:47:58.000000 types-aiobotocore-iotfleetwise-2.9.0/types_aiobotocore_iotfleetwise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3445 2023-12-13 19:47:58.000000 types-aiobotocore-iotfleetwise-2.9.0/types_aiobotocore_iotfleetwise/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      952 2023-12-13 19:47:58.000000 types-aiobotocore-iotfleetwise-2.9.0/types_aiobotocore_iotfleetwise/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44671 2023-12-13 19:47:59.000000 types-aiobotocore-iotfleetwise-2.9.0/types_aiobotocore_iotfleetwise/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    44667 2023-12-13 19:47:59.000000 types-aiobotocore-iotfleetwise-2.9.0/types_aiobotocore_iotfleetwise/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12959 2023-12-13 19:47:59.000000 types-aiobotocore-iotfleetwise-2.9.0/types_aiobotocore_iotfleetwise/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    12957 2023-12-13 19:47:59.000000 types-aiobotocore-iotfleetwise-2.9.0/types_aiobotocore_iotfleetwise/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    16248 2023-12-13 19:47:59.000000 types-aiobotocore-iotfleetwise-2.9.0/types_aiobotocore_iotfleetwise/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    16233 2023-12-13 19:47:59.000000 types-aiobotocore-iotfleetwise-2.9.0/types_aiobotocore_iotfleetwise/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:47:58.000000 types-aiobotocore-iotfleetwise-2.9.0/types_aiobotocore_iotfleetwise/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    53108 2023-12-13 19:48:00.000000 types-aiobotocore-iotfleetwise-2.9.0/types_aiobotocore_iotfleetwise/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    53107 2023-12-13 19:47:59.000000 types-aiobotocore-iotfleetwise-2.9.0/types_aiobotocore_iotfleetwise/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:47:58.000000 types-aiobotocore-iotfleetwise-2.9.0/types_aiobotocore_iotfleetwise/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:34.001631 types-aiobotocore-iotfleetwise-2.9.0/types_aiobotocore_iotfleetwise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15220 2023-12-13 19:59:33.000000 types-aiobotocore-iotfleetwise-2.9.0/types_aiobotocore_iotfleetwise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      908 2023-12-13 19:59:33.000000 types-aiobotocore-iotfleetwise-2.9.0/types_aiobotocore_iotfleetwise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:33.000000 types-aiobotocore-iotfleetwise-2.9.0/types_aiobotocore_iotfleetwise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:33.000000 types-aiobotocore-iotfleetwise-2.9.0/types_aiobotocore_iotfleetwise.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:33.000000 types-aiobotocore-iotfleetwise-2.9.0/types_aiobotocore_iotfleetwise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-13 19:59:33.000000 types-aiobotocore-iotfleetwise-2.9.0/types_aiobotocore_iotfleetwise.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:57.401265 types-aiobotocore-iotfleetwise-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:09:47.000000 types-aiobotocore-iotfleetwise-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15240 2024-01-18 01:20:57.401265 types-aiobotocore-iotfleetwise-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13637 2024-01-18 01:09:47.000000 types-aiobotocore-iotfleetwise-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:57.401265 types-aiobotocore-iotfleetwise-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-01-18 01:09:47.000000 types-aiobotocore-iotfleetwise-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:57.397266 types-aiobotocore-iotfleetwise-2.9.1/types_aiobotocore_iotfleetwise/
+-rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-01-18 01:09:47.000000 types-aiobotocore-iotfleetwise-2.9.1/types_aiobotocore_iotfleetwise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-01-18 01:09:47.000000 types-aiobotocore-iotfleetwise-2.9.1/types_aiobotocore_iotfleetwise/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-01-18 01:09:47.000000 types-aiobotocore-iotfleetwise-2.9.1/types_aiobotocore_iotfleetwise/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44683 2024-01-18 01:09:50.000000 types-aiobotocore-iotfleetwise-2.9.1/types_aiobotocore_iotfleetwise/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44680 2024-01-18 01:09:49.000000 types-aiobotocore-iotfleetwise-2.9.1/types_aiobotocore_iotfleetwise/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12957 2024-01-18 01:09:50.000000 types-aiobotocore-iotfleetwise-2.9.1/types_aiobotocore_iotfleetwise/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12957 2024-01-18 01:09:50.000000 types-aiobotocore-iotfleetwise-2.9.1/types_aiobotocore_iotfleetwise/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    16247 2024-01-18 01:09:50.000000 types-aiobotocore-iotfleetwise-2.9.1/types_aiobotocore_iotfleetwise/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16233 2024-01-18 01:09:50.000000 types-aiobotocore-iotfleetwise-2.9.1/types_aiobotocore_iotfleetwise/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:09:47.000000 types-aiobotocore-iotfleetwise-2.9.1/types_aiobotocore_iotfleetwise/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    53107 2024-01-18 01:09:51.000000 types-aiobotocore-iotfleetwise-2.9.1/types_aiobotocore_iotfleetwise/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53107 2024-01-18 01:09:50.000000 types-aiobotocore-iotfleetwise-2.9.1/types_aiobotocore_iotfleetwise/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:09:47.000000 types-aiobotocore-iotfleetwise-2.9.1/types_aiobotocore_iotfleetwise/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:57.397266 types-aiobotocore-iotfleetwise-2.9.1/types_aiobotocore_iotfleetwise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15240 2024-01-18 01:20:57.000000 types-aiobotocore-iotfleetwise-2.9.1/types_aiobotocore_iotfleetwise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-01-18 01:20:57.000000 types-aiobotocore-iotfleetwise-2.9.1/types_aiobotocore_iotfleetwise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:57.000000 types-aiobotocore-iotfleetwise-2.9.1/types_aiobotocore_iotfleetwise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:57.000000 types-aiobotocore-iotfleetwise-2.9.1/types_aiobotocore_iotfleetwise.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:57.000000 types-aiobotocore-iotfleetwise-2.9.1/types_aiobotocore_iotfleetwise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-01-18 01:20:57.000000 types-aiobotocore-iotfleetwise-2.9.1/types_aiobotocore_iotfleetwise.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iotfleetwise-2.9.0/LICENSE` & `types-aiobotocore-iotfleetwise-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-iotfleetwise-2.9.0/PKG-INFO` & `types-aiobotocore-iotfleetwise-2.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotfleetwise
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.IoTFleetWise 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.IoTFleetWise 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/
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
 
 <a id="types-aiobotocore-iotfleetwise"></a>
 
 # types-aiobotocore-iotfleetwise
 
 [![PyPI - types-aiobotocore-iotfleetwise](https://img.shields.io/pypi/v/types-aiobotocore-iotfleetwise.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotfleetwise)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotfleetwise.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotfleetwise)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotfleetwise)](https://pepy.tech/project/types-aiobotocore-iotfleetwise)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTFleetWise 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise)
+[aiobotocore.IoTFleetWise 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise)
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
 [types-aiobotocore-iotfleetwise docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-iotfleetwise-2.9.0/README.md` & `types-aiobotocore-iotfleetwise-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotfleetwise.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotfleetwise)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotfleetwise)](https://pepy.tech/project/types-aiobotocore-iotfleetwise)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTFleetWise 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise)
+[aiobotocore.IoTFleetWise 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise)
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
 [types-aiobotocore-iotfleetwise docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-iotfleetwise-2.9.0/setup.py` & `types-aiobotocore-iotfleetwise-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iotfleetwise",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_iotfleetwise"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.IoTFleetWise 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.IoTFleetWise 2.9.1 service generated with"
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
     keywords="aiobotocore iotfleetwise type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_iotfleetwise": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-iotfleetwise-2.9.0/types_aiobotocore_iotfleetwise/__init__.py` & `types-aiobotocore-iotfleetwise-2.9.1/types_aiobotocore_iotfleetwise/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,14 @@
     ListSignalCatalogsPaginator,
     ListVehiclesInFleetPaginator,
     ListVehiclesPaginator,
 )
 
 Client = IoTFleetWiseClient
 
-
 __all__ = (
     "Client",
     "GetVehicleStatusPaginator",
     "IoTFleetWiseClient",
     "ListCampaignsPaginator",
     "ListDecoderManifestNetworkInterfacesPaginator",
     "ListDecoderManifestSignalsPaginator",
```

### Comparing `types-aiobotocore-iotfleetwise-2.9.0/types_aiobotocore_iotfleetwise/__init__.pyi` & `types-aiobotocore-iotfleetwise-2.9.1/types_aiobotocore_iotfleetwise/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotfleetwise-2.9.0/types_aiobotocore_iotfleetwise/__main__.py` & `types-aiobotocore-iotfleetwise-2.9.1/types_aiobotocore_iotfleetwise/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IoTFleetWise 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.IoTFleetWise 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise\nOther"
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

### Comparing `types-aiobotocore-iotfleetwise-2.9.0/types_aiobotocore_iotfleetwise/client.py` & `types-aiobotocore-iotfleetwise-2.9.1/types_aiobotocore_iotfleetwise/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("IoTFleetWiseClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -217,15 +216,15 @@
         diagnosticsMode: DiagnosticsModeType = ...,
         spoolingMode: SpoolingModeType = ...,
         compression: CompressionType = ...,
         priority: int = ...,
         signalsToCollect: Sequence[SignalInformationTypeDef] = ...,
         dataExtraDimensions: Sequence[str] = ...,
         tags: Sequence[TagTypeDef] = ...,
-        dataDestinationConfigs: Sequence[DataDestinationConfigTypeDef] = ...
+        dataDestinationConfigs: Sequence[DataDestinationConfigTypeDef] = ...,
     ) -> CreateCampaignResponseTypeDef:
         """
         Creates an orchestration of data collection rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Client.create_campaign)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/client/#create_campaign)
         """
@@ -234,30 +233,30 @@
         self,
         *,
         name: str,
         modelManifestArn: str,
         description: str = ...,
         signalDecoders: Sequence[SignalDecoderTypeDef] = ...,
         networkInterfaces: Sequence[NetworkInterfaceTypeDef] = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDecoderManifestResponseTypeDef:
         """
         Creates the decoder manifest associated with a model manifest.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Client.create_decoder_manifest)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/client/#create_decoder_manifest)
         """
 
     async def create_fleet(
         self,
         *,
         fleetId: str,
         signalCatalogArn: str,
         description: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateFleetResponseTypeDef:
         """
         Creates a fleet that represents a group of vehicles.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Client.create_fleet)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/client/#create_fleet)
         """
@@ -265,15 +264,15 @@
     async def create_model_manifest(
         self,
         *,
         name: str,
         nodes: Sequence[str],
         signalCatalogArn: str,
         description: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateModelManifestResponseTypeDef:
         """
         Creates a vehicle model (model manifest) that specifies signals (attributes,
         branches, sensors, and
         actuators).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Client.create_model_manifest)
@@ -282,15 +281,15 @@
 
     async def create_signal_catalog(
         self,
         *,
         name: str,
         description: str = ...,
         nodes: Sequence[NodeTypeDef] = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateSignalCatalogResponseTypeDef:
         """
         Creates a collection of standardized signals that can be reused to create
         vehicle
         models.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Client.create_signal_catalog)
@@ -301,15 +300,15 @@
         self,
         *,
         vehicleName: str,
         modelManifestArn: str,
         decoderManifestArn: str,
         attributes: Mapping[str, str] = ...,
         associationBehavior: VehicleAssociationBehaviorType = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateVehicleResponseTypeDef:
         """
         Creates a vehicle, which is an instance of a vehicle model (model manifest).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Client.create_vehicle)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/client/#create_vehicle)
         """
@@ -485,15 +484,15 @@
 
     async def import_signal_catalog(
         self,
         *,
         name: str,
         description: str = ...,
         vss: FormattedVssTypeDef = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> ImportSignalCatalogResponseTypeDef:
         """
         Creates a signal catalog using your existing VSS formatted content from your
         local
         device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Client.import_signal_catalog)
@@ -650,15 +649,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/client/#put_logging_options)
         """
 
     async def register_account(
         self,
         *,
         timestreamResources: TimestreamResourcesTypeDef = ...,
-        iamResources: IamResourcesTypeDef = ...
+        iamResources: IamResourcesTypeDef = ...,
     ) -> RegisterAccountResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Client.register_account)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/client/#register_account)
         """
@@ -681,15 +680,15 @@
 
     async def update_campaign(
         self,
         *,
         name: str,
         action: UpdateCampaignActionType,
         description: str = ...,
-        dataExtraDimensions: Sequence[str] = ...
+        dataExtraDimensions: Sequence[str] = ...,
     ) -> UpdateCampaignResponseTypeDef:
         """
         Updates a campaign.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Client.update_campaign)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/client/#update_campaign)
         """
@@ -701,15 +700,15 @@
         description: str = ...,
         signalDecodersToAdd: Sequence[SignalDecoderTypeDef] = ...,
         signalDecodersToUpdate: Sequence[SignalDecoderTypeDef] = ...,
         signalDecodersToRemove: Sequence[str] = ...,
         networkInterfacesToAdd: Sequence[NetworkInterfaceTypeDef] = ...,
         networkInterfacesToUpdate: Sequence[NetworkInterfaceTypeDef] = ...,
         networkInterfacesToRemove: Sequence[str] = ...,
-        status: ManifestStatusType = ...
+        status: ManifestStatusType = ...,
     ) -> UpdateDecoderManifestResponseTypeDef:
         """
         Updates a decoder manifest.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Client.update_decoder_manifest)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/client/#update_decoder_manifest)
         """
@@ -727,15 +726,15 @@
     async def update_model_manifest(
         self,
         *,
         name: str,
         description: str = ...,
         nodesToAdd: Sequence[str] = ...,
         nodesToRemove: Sequence[str] = ...,
-        status: ManifestStatusType = ...
+        status: ManifestStatusType = ...,
     ) -> UpdateModelManifestResponseTypeDef:
         """
         Updates a vehicle model (model manifest).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Client.update_model_manifest)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/client/#update_model_manifest)
         """
@@ -743,15 +742,15 @@
     async def update_signal_catalog(
         self,
         *,
         name: str,
         description: str = ...,
         nodesToAdd: Sequence[NodeTypeDef] = ...,
         nodesToUpdate: Sequence[NodeTypeDef] = ...,
-        nodesToRemove: Sequence[str] = ...
+        nodesToRemove: Sequence[str] = ...,
     ) -> UpdateSignalCatalogResponseTypeDef:
         """
         Updates a signal catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Client.update_signal_catalog)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/client/#update_signal_catalog)
         """
@@ -759,15 +758,15 @@
     async def update_vehicle(
         self,
         *,
         vehicleName: str,
         modelManifestArn: str = ...,
         decoderManifestArn: str = ...,
         attributes: Mapping[str, str] = ...,
-        attributeUpdateMode: UpdateModeType = ...
+        attributeUpdateMode: UpdateModeType = ...,
     ) -> UpdateVehicleResponseTypeDef:
         """
         Updates a vehicle.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Client.update_vehicle)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/client/#update_vehicle)
         """
```

### Comparing `types-aiobotocore-iotfleetwise-2.9.0/types_aiobotocore_iotfleetwise/client.pyi` & `types-aiobotocore-iotfleetwise-2.9.1/types_aiobotocore_iotfleetwise/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -213,15 +213,15 @@
         diagnosticsMode: DiagnosticsModeType = ...,
         spoolingMode: SpoolingModeType = ...,
         compression: CompressionType = ...,
         priority: int = ...,
         signalsToCollect: Sequence[SignalInformationTypeDef] = ...,
         dataExtraDimensions: Sequence[str] = ...,
         tags: Sequence[TagTypeDef] = ...,
-        dataDestinationConfigs: Sequence[DataDestinationConfigTypeDef] = ...
+        dataDestinationConfigs: Sequence[DataDestinationConfigTypeDef] = ...,
     ) -> CreateCampaignResponseTypeDef:
         """
         Creates an orchestration of data collection rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Client.create_campaign)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/client/#create_campaign)
         """
@@ -230,30 +230,30 @@
         self,
         *,
         name: str,
         modelManifestArn: str,
         description: str = ...,
         signalDecoders: Sequence[SignalDecoderTypeDef] = ...,
         networkInterfaces: Sequence[NetworkInterfaceTypeDef] = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDecoderManifestResponseTypeDef:
         """
         Creates the decoder manifest associated with a model manifest.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Client.create_decoder_manifest)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/client/#create_decoder_manifest)
         """
 
     async def create_fleet(
         self,
         *,
         fleetId: str,
         signalCatalogArn: str,
         description: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateFleetResponseTypeDef:
         """
         Creates a fleet that represents a group of vehicles.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Client.create_fleet)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/client/#create_fleet)
         """
@@ -261,15 +261,15 @@
     async def create_model_manifest(
         self,
         *,
         name: str,
         nodes: Sequence[str],
         signalCatalogArn: str,
         description: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateModelManifestResponseTypeDef:
         """
         Creates a vehicle model (model manifest) that specifies signals (attributes,
         branches, sensors, and
         actuators).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Client.create_model_manifest)
@@ -278,15 +278,15 @@
 
     async def create_signal_catalog(
         self,
         *,
         name: str,
         description: str = ...,
         nodes: Sequence[NodeTypeDef] = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateSignalCatalogResponseTypeDef:
         """
         Creates a collection of standardized signals that can be reused to create
         vehicle
         models.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Client.create_signal_catalog)
@@ -297,15 +297,15 @@
         self,
         *,
         vehicleName: str,
         modelManifestArn: str,
         decoderManifestArn: str,
         attributes: Mapping[str, str] = ...,
         associationBehavior: VehicleAssociationBehaviorType = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateVehicleResponseTypeDef:
         """
         Creates a vehicle, which is an instance of a vehicle model (model manifest).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Client.create_vehicle)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/client/#create_vehicle)
         """
@@ -481,15 +481,15 @@
 
     async def import_signal_catalog(
         self,
         *,
         name: str,
         description: str = ...,
         vss: FormattedVssTypeDef = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> ImportSignalCatalogResponseTypeDef:
         """
         Creates a signal catalog using your existing VSS formatted content from your
         local
         device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Client.import_signal_catalog)
@@ -646,15 +646,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/client/#put_logging_options)
         """
 
     async def register_account(
         self,
         *,
         timestreamResources: TimestreamResourcesTypeDef = ...,
-        iamResources: IamResourcesTypeDef = ...
+        iamResources: IamResourcesTypeDef = ...,
     ) -> RegisterAccountResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Client.register_account)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/client/#register_account)
         """
@@ -677,15 +677,15 @@
 
     async def update_campaign(
         self,
         *,
         name: str,
         action: UpdateCampaignActionType,
         description: str = ...,
-        dataExtraDimensions: Sequence[str] = ...
+        dataExtraDimensions: Sequence[str] = ...,
     ) -> UpdateCampaignResponseTypeDef:
         """
         Updates a campaign.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Client.update_campaign)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/client/#update_campaign)
         """
@@ -697,15 +697,15 @@
         description: str = ...,
         signalDecodersToAdd: Sequence[SignalDecoderTypeDef] = ...,
         signalDecodersToUpdate: Sequence[SignalDecoderTypeDef] = ...,
         signalDecodersToRemove: Sequence[str] = ...,
         networkInterfacesToAdd: Sequence[NetworkInterfaceTypeDef] = ...,
         networkInterfacesToUpdate: Sequence[NetworkInterfaceTypeDef] = ...,
         networkInterfacesToRemove: Sequence[str] = ...,
-        status: ManifestStatusType = ...
+        status: ManifestStatusType = ...,
     ) -> UpdateDecoderManifestResponseTypeDef:
         """
         Updates a decoder manifest.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Client.update_decoder_manifest)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/client/#update_decoder_manifest)
         """
@@ -723,15 +723,15 @@
     async def update_model_manifest(
         self,
         *,
         name: str,
         description: str = ...,
         nodesToAdd: Sequence[str] = ...,
         nodesToRemove: Sequence[str] = ...,
-        status: ManifestStatusType = ...
+        status: ManifestStatusType = ...,
     ) -> UpdateModelManifestResponseTypeDef:
         """
         Updates a vehicle model (model manifest).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Client.update_model_manifest)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/client/#update_model_manifest)
         """
@@ -739,15 +739,15 @@
     async def update_signal_catalog(
         self,
         *,
         name: str,
         description: str = ...,
         nodesToAdd: Sequence[NodeTypeDef] = ...,
         nodesToUpdate: Sequence[NodeTypeDef] = ...,
-        nodesToRemove: Sequence[str] = ...
+        nodesToRemove: Sequence[str] = ...,
     ) -> UpdateSignalCatalogResponseTypeDef:
         """
         Updates a signal catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Client.update_signal_catalog)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/client/#update_signal_catalog)
         """
@@ -755,15 +755,15 @@
     async def update_vehicle(
         self,
         *,
         vehicleName: str,
         modelManifestArn: str = ...,
         decoderManifestArn: str = ...,
         attributes: Mapping[str, str] = ...,
-        attributeUpdateMode: UpdateModeType = ...
+        attributeUpdateMode: UpdateModeType = ...,
     ) -> UpdateVehicleResponseTypeDef:
         """
         Updates a vehicle.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Client.update_vehicle)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/client/#update_vehicle)
         """
```

### Comparing `types-aiobotocore-iotfleetwise-2.9.0/types_aiobotocore_iotfleetwise/literals.py` & `types-aiobotocore-iotfleetwise-2.9.1/types_aiobotocore_iotfleetwise/literals.py`

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
     "CampaignStatusType",
     "CompressionType",
     "DataFormatType",
     "DiagnosticsModeType",
     "EncryptionStatusType",
     "EncryptionTypeType",
@@ -60,15 +59,14 @@
     "IoTFleetWiseServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 CampaignStatusType = Literal["CREATING", "RUNNING", "SUSPENDED", "WAITING_FOR_APPROVAL"]
 CompressionType = Literal["OFF", "SNAPPY"]
 DataFormatType = Literal["JSON", "PARQUET"]
 DiagnosticsModeType = Literal["OFF", "SEND_ACTIVE_DTCS"]
 EncryptionStatusType = Literal["FAILURE", "PENDING", "SUCCESS"]
 EncryptionTypeType = Literal["FLEETWISE_DEFAULT_ENCRYPTION", "KMS_BASED_ENCRYPTION"]
 GetVehicleStatusPaginatorName = Literal["get_vehicle_status"]
```

### Comparing `types-aiobotocore-iotfleetwise-2.9.0/types_aiobotocore_iotfleetwise/literals.pyi` & `types-aiobotocore-iotfleetwise-2.9.1/types_aiobotocore_iotfleetwise/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotfleetwise-2.9.0/types_aiobotocore_iotfleetwise/paginator.py` & `types-aiobotocore-iotfleetwise-2.9.1/types_aiobotocore_iotfleetwise/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,14 @@
     "ListModelManifestsPaginator",
     "ListSignalCatalogNodesPaginator",
     "ListSignalCatalogsPaginator",
     "ListVehiclesPaginator",
     "ListVehiclesInFleetPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
```

### Comparing `types-aiobotocore-iotfleetwise-2.9.0/types_aiobotocore_iotfleetwise/paginator.pyi` & `types-aiobotocore-iotfleetwise-2.9.1/types_aiobotocore_iotfleetwise/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotfleetwise-2.9.0/types_aiobotocore_iotfleetwise/type_defs.py` & `types-aiobotocore-iotfleetwise-2.9.1/types_aiobotocore_iotfleetwise/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ActuatorPaginatorTypeDef",
     "ActuatorTypeDef",
     "AssociateVehicleFleetRequestRequestTypeDef",
     "AttributePaginatorTypeDef",
     "AttributeTypeDef",
     "CreateVehicleErrorTypeDef",
```

### Comparing `types-aiobotocore-iotfleetwise-2.9.0/types_aiobotocore_iotfleetwise/type_defs.pyi` & `types-aiobotocore-iotfleetwise-2.9.1/types_aiobotocore_iotfleetwise/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotfleetwise-2.9.0/types_aiobotocore_iotfleetwise.egg-info/PKG-INFO` & `types-aiobotocore-iotfleetwise-2.9.1/types_aiobotocore_iotfleetwise.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotfleetwise
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.IoTFleetWise 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.IoTFleetWise 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/
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
 
 <a id="types-aiobotocore-iotfleetwise"></a>
 
 # types-aiobotocore-iotfleetwise
 
 [![PyPI - types-aiobotocore-iotfleetwise](https://img.shields.io/pypi/v/types-aiobotocore-iotfleetwise.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotfleetwise)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotfleetwise.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotfleetwise)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotfleetwise)](https://pepy.tech/project/types-aiobotocore-iotfleetwise)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTFleetWise 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise)
+[aiobotocore.IoTFleetWise 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise)
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
 [types-aiobotocore-iotfleetwise docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-iotfleetwise-2.9.0/types_aiobotocore_iotfleetwise.egg-info/SOURCES.txt` & `types-aiobotocore-iotfleetwise-2.9.1/types_aiobotocore_iotfleetwise.egg-info/SOURCES.txt`

 * *Files identical despite different names*

