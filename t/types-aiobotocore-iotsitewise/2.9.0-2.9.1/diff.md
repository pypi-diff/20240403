# Comparing `tmp/types-aiobotocore-iotsitewise-2.9.0.tar.gz` & `tmp/types-aiobotocore-iotsitewise-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iotsitewise-2.9.0.tar", last modified: Wed Dec 13 19:59:34 2023, max compression
+gzip compressed data, was "types-aiobotocore-iotsitewise-2.9.1.tar", last modified: Thu Jan 18 01:20:58 2024, max compression
```

## Comparing `types-aiobotocore-iotsitewise-2.9.0.tar` & `types-aiobotocore-iotsitewise-2.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:34.741617 types-aiobotocore-iotsitewise-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:48:03.000000 types-aiobotocore-iotsitewise-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    17669 2023-12-13 19:59:34.741617 types-aiobotocore-iotsitewise-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16090 2023-12-13 19:48:03.000000 types-aiobotocore-iotsitewise-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:34.741617 types-aiobotocore-iotsitewise-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2023-12-13 19:48:03.000000 types-aiobotocore-iotsitewise-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:34.741617 types-aiobotocore-iotsitewise-2.9.0/types_aiobotocore_iotsitewise/
--rw-r--r--   0 runner    (1001) docker     (127)     6235 2023-12-13 19:48:03.000000 types-aiobotocore-iotsitewise-2.9.0/types_aiobotocore_iotsitewise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6234 2023-12-13 19:48:03.000000 types-aiobotocore-iotsitewise-2.9.0/types_aiobotocore_iotsitewise/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      948 2023-12-13 19:48:03.000000 types-aiobotocore-iotsitewise-2.9.0/types_aiobotocore_iotsitewise/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    77117 2023-12-13 19:48:04.000000 types-aiobotocore-iotsitewise-2.9.0/types_aiobotocore_iotsitewise/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    77113 2023-12-13 19:48:03.000000 types-aiobotocore-iotsitewise-2.9.0/types_aiobotocore_iotsitewise/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    16863 2023-12-13 19:48:04.000000 types-aiobotocore-iotsitewise-2.9.0/types_aiobotocore_iotsitewise/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    16861 2023-12-13 19:48:04.000000 types-aiobotocore-iotsitewise-2.9.0/types_aiobotocore_iotsitewise/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    27650 2023-12-13 19:48:04.000000 types-aiobotocore-iotsitewise-2.9.0/types_aiobotocore_iotsitewise/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    27626 2023-12-13 19:48:04.000000 types-aiobotocore-iotsitewise-2.9.0/types_aiobotocore_iotsitewise/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:48:03.000000 types-aiobotocore-iotsitewise-2.9.0/types_aiobotocore_iotsitewise/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    95610 2023-12-13 19:48:07.000000 types-aiobotocore-iotsitewise-2.9.0/types_aiobotocore_iotsitewise/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    95609 2023-12-13 19:48:05.000000 types-aiobotocore-iotsitewise-2.9.0/types_aiobotocore_iotsitewise/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:48:03.000000 types-aiobotocore-iotsitewise-2.9.0/types_aiobotocore_iotsitewise/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6731 2023-12-13 19:48:04.000000 types-aiobotocore-iotsitewise-2.9.0/types_aiobotocore_iotsitewise/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6725 2023-12-13 19:48:04.000000 types-aiobotocore-iotsitewise-2.9.0/types_aiobotocore_iotsitewise/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:34.741617 types-aiobotocore-iotsitewise-2.9.0/types_aiobotocore_iotsitewise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17669 2023-12-13 19:59:34.000000 types-aiobotocore-iotsitewise-2.9.0/types_aiobotocore_iotsitewise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      970 2023-12-13 19:59:34.000000 types-aiobotocore-iotsitewise-2.9.0/types_aiobotocore_iotsitewise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:34.000000 types-aiobotocore-iotsitewise-2.9.0/types_aiobotocore_iotsitewise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:34.000000 types-aiobotocore-iotsitewise-2.9.0/types_aiobotocore_iotsitewise.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:34.000000 types-aiobotocore-iotsitewise-2.9.0/types_aiobotocore_iotsitewise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-13 19:59:34.000000 types-aiobotocore-iotsitewise-2.9.0/types_aiobotocore_iotsitewise.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:58.081262 types-aiobotocore-iotsitewise-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:09:52.000000 types-aiobotocore-iotsitewise-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17689 2024-01-18 01:20:58.081262 types-aiobotocore-iotsitewise-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16090 2024-01-18 01:09:52.000000 types-aiobotocore-iotsitewise-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:58.081262 types-aiobotocore-iotsitewise-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-01-18 01:09:52.000000 types-aiobotocore-iotsitewise-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:58.077262 types-aiobotocore-iotsitewise-2.9.1/types_aiobotocore_iotsitewise/
+-rw-r--r--   0 runner    (1001) docker     (127)     6234 2024-01-18 01:09:52.000000 types-aiobotocore-iotsitewise-2.9.1/types_aiobotocore_iotsitewise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6234 2024-01-18 01:09:52.000000 types-aiobotocore-iotsitewise-2.9.1/types_aiobotocore_iotsitewise/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-01-18 01:09:52.000000 types-aiobotocore-iotsitewise-2.9.1/types_aiobotocore_iotsitewise/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77150 2024-01-18 01:09:53.000000 types-aiobotocore-iotsitewise-2.9.1/types_aiobotocore_iotsitewise/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77147 2024-01-18 01:09:52.000000 types-aiobotocore-iotsitewise-2.9.1/types_aiobotocore_iotsitewise/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    16861 2024-01-18 01:09:53.000000 types-aiobotocore-iotsitewise-2.9.1/types_aiobotocore_iotsitewise/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16861 2024-01-18 01:09:53.000000 types-aiobotocore-iotsitewise-2.9.1/types_aiobotocore_iotsitewise/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    27661 2024-01-18 01:09:53.000000 types-aiobotocore-iotsitewise-2.9.1/types_aiobotocore_iotsitewise/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27639 2024-01-18 01:09:53.000000 types-aiobotocore-iotsitewise-2.9.1/types_aiobotocore_iotsitewise/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:09:52.000000 types-aiobotocore-iotsitewise-2.9.1/types_aiobotocore_iotsitewise/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    95609 2024-01-18 01:09:57.000000 types-aiobotocore-iotsitewise-2.9.1/types_aiobotocore_iotsitewise/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    95609 2024-01-18 01:09:56.000000 types-aiobotocore-iotsitewise-2.9.1/types_aiobotocore_iotsitewise/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:09:52.000000 types-aiobotocore-iotsitewise-2.9.1/types_aiobotocore_iotsitewise/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6735 2024-01-18 01:09:53.000000 types-aiobotocore-iotsitewise-2.9.1/types_aiobotocore_iotsitewise/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6729 2024-01-18 01:09:53.000000 types-aiobotocore-iotsitewise-2.9.1/types_aiobotocore_iotsitewise/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:58.081262 types-aiobotocore-iotsitewise-2.9.1/types_aiobotocore_iotsitewise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17689 2024-01-18 01:20:58.000000 types-aiobotocore-iotsitewise-2.9.1/types_aiobotocore_iotsitewise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-01-18 01:20:58.000000 types-aiobotocore-iotsitewise-2.9.1/types_aiobotocore_iotsitewise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:58.000000 types-aiobotocore-iotsitewise-2.9.1/types_aiobotocore_iotsitewise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:58.000000 types-aiobotocore-iotsitewise-2.9.1/types_aiobotocore_iotsitewise.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:58.000000 types-aiobotocore-iotsitewise-2.9.1/types_aiobotocore_iotsitewise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-01-18 01:20:58.000000 types-aiobotocore-iotsitewise-2.9.1/types_aiobotocore_iotsitewise.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iotsitewise-2.9.0/LICENSE` & `types-aiobotocore-iotsitewise-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-iotsitewise-2.9.0/PKG-INFO` & `types-aiobotocore-iotsitewise-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotsitewise
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.IoTSiteWise 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.IoTSiteWise 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/
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
 
 <a id="types-aiobotocore-iotsitewise"></a>
 
 # types-aiobotocore-iotsitewise
 
 [![PyPI - types-aiobotocore-iotsitewise](https://img.shields.io/pypi/v/types-aiobotocore-iotsitewise.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotsitewise)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotsitewise.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotsitewise)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotsitewise)](https://pepy.tech/project/types-aiobotocore-iotsitewise)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTSiteWise 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise)
+[aiobotocore.IoTSiteWise 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise)
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
 [types-aiobotocore-iotsitewise docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-iotsitewise-2.9.0/README.md` & `types-aiobotocore-iotsitewise-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotsitewise.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotsitewise)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotsitewise)](https://pepy.tech/project/types-aiobotocore-iotsitewise)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTSiteWise 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise)
+[aiobotocore.IoTSiteWise 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise)
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
 [types-aiobotocore-iotsitewise docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-iotsitewise-2.9.0/setup.py` & `types-aiobotocore-iotsitewise-2.9.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iotsitewise",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_iotsitewise"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.IoTSiteWise 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.IoTSiteWise 2.9.1 service generated with"
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
     keywords="aiobotocore iotsitewise type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_iotsitewise": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-iotsitewise-2.9.0/types_aiobotocore_iotsitewise/__init__.py` & `types-aiobotocore-iotsitewise-2.9.1/types_aiobotocore_iotsitewise/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,14 @@
     AssetNotExistsWaiter,
     PortalActiveWaiter,
     PortalNotExistsWaiter,
 )
 
 Client = IoTSiteWiseClient
 
-
 __all__ = (
     "AssetActiveWaiter",
     "AssetModelActiveWaiter",
     "AssetModelNotExistsWaiter",
     "AssetNotExistsWaiter",
     "Client",
     "ExecuteQueryPaginator",
```

### Comparing `types-aiobotocore-iotsitewise-2.9.0/types_aiobotocore_iotsitewise/__init__.pyi` & `types-aiobotocore-iotsitewise-2.9.1/types_aiobotocore_iotsitewise/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotsitewise-2.9.0/types_aiobotocore_iotsitewise/__main__.py` & `types-aiobotocore-iotsitewise-2.9.1/types_aiobotocore_iotsitewise/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IoTSiteWise 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.IoTSiteWise 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise\nOther"
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

### Comparing `types-aiobotocore-iotsitewise-2.9.0/types_aiobotocore_iotsitewise/client.py` & `types-aiobotocore-iotsitewise-2.9.1/types_aiobotocore_iotsitewise/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,15 +171,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("IoTSiteWiseClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -264,15 +263,15 @@
         """
 
     async def batch_get_asset_property_aggregates(
         self,
         *,
         entries: Sequence[BatchGetAssetPropertyAggregatesEntryTypeDef],
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> BatchGetAssetPropertyAggregatesResponseTypeDef:
         """
         Gets aggregated values (for example, average, minimum, and maximum) for one or
         more asset
         properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.batch_get_asset_property_aggregates)
@@ -290,15 +289,15 @@
         """
 
     async def batch_get_asset_property_value_history(
         self,
         *,
         entries: Sequence[BatchGetAssetPropertyValueHistoryEntryTypeDef],
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> BatchGetAssetPropertyValueHistoryResponseTypeDef:
         """
         Gets the historical values for one or more asset properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.batch_get_asset_property_value_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#batch_get_asset_property_value_history)
         """
@@ -332,15 +331,15 @@
     async def create_access_policy(
         self,
         *,
         accessPolicyIdentity: IdentityTypeDef,
         accessPolicyResource: ResourceTypeDef,
         accessPolicyPermission: PermissionType,
         clientToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateAccessPolicyResponseTypeDef:
         """
         Creates an access policy that grants the specified identity (IAM Identity
         Center user, IAM Identity Center group, or IAM user) access to the specified
         IoT SiteWise Monitor portal or project
         resource.
 
@@ -353,15 +352,15 @@
         *,
         assetName: str,
         assetModelId: str,
         clientToken: str = ...,
         tags: Mapping[str, str] = ...,
         assetDescription: str = ...,
         assetId: str = ...,
-        assetExternalId: str = ...
+        assetExternalId: str = ...,
     ) -> CreateAssetResponseTypeDef:
         """
         Creates an asset from an existing asset model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.create_asset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#create_asset)
         """
@@ -374,15 +373,15 @@
         assetModelProperties: Sequence[AssetModelPropertyDefinitionTypeDef] = ...,
         assetModelHierarchies: Sequence[AssetModelHierarchyDefinitionTypeDef] = ...,
         assetModelCompositeModels: Sequence[AssetModelCompositeModelDefinitionTypeDef] = ...,
         clientToken: str = ...,
         tags: Mapping[str, str] = ...,
         assetModelId: str = ...,
         assetModelExternalId: str = ...,
-        assetModelType: AssetModelTypeType = ...
+        assetModelType: AssetModelTypeType = ...,
     ) -> CreateAssetModelResponseTypeDef:
         """
         Creates an asset model from specified property and hierarchy definitions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.create_asset_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#create_asset_model)
         """
@@ -395,15 +394,15 @@
         assetModelCompositeModelType: str,
         parentAssetModelCompositeModelId: str = ...,
         assetModelCompositeModelExternalId: str = ...,
         assetModelCompositeModelId: str = ...,
         assetModelCompositeModelDescription: str = ...,
         clientToken: str = ...,
         composedAssetModelId: str = ...,
-        assetModelCompositeModelProperties: Sequence[AssetModelPropertyDefinitionTypeDef] = ...
+        assetModelCompositeModelProperties: Sequence[AssetModelPropertyDefinitionTypeDef] = ...,
     ) -> CreateAssetModelCompositeModelResponseTypeDef:
         """
         Creates a custom composite model from specified property and hierarchy
         definitions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.create_asset_model_composite_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#create_asset_model_composite_model)
@@ -414,15 +413,15 @@
         *,
         jobName: str,
         jobRoleArn: str,
         files: Sequence[FileTypeDef],
         errorReportLocation: ErrorReportLocationTypeDef,
         jobConfiguration: JobConfigurationTypeDef,
         adaptiveIngestion: bool = ...,
-        deleteFilesAfterImport: bool = ...
+        deleteFilesAfterImport: bool = ...,
     ) -> CreateBulkImportJobResponseTypeDef:
         """
         Defines a job to ingest data to IoT SiteWise from Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.create_bulk_import_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#create_bulk_import_job)
         """
@@ -431,29 +430,29 @@
         self,
         *,
         projectId: str,
         dashboardName: str,
         dashboardDefinition: str,
         dashboardDescription: str = ...,
         clientToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateDashboardResponseTypeDef:
         """
         Creates a dashboard in an IoT SiteWise Monitor project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.create_dashboard)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#create_dashboard)
         """
 
     async def create_gateway(
         self,
         *,
         gatewayName: str,
         gatewayPlatform: GatewayPlatformTypeDef,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateGatewayResponseTypeDef:
         """
         Creates a gateway, which is a virtual or edge device that delivers industrial
         data streams from local servers to IoT
         SiteWise.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.create_gateway)
@@ -468,15 +467,15 @@
         roleArn: str,
         portalDescription: str = ...,
         clientToken: str = ...,
         portalLogoImageFile: ImageFileTypeDef = ...,
         tags: Mapping[str, str] = ...,
         portalAuthMode: AuthModeType = ...,
         notificationSenderEmail: str = ...,
-        alarms: AlarmsTypeDef = ...
+        alarms: AlarmsTypeDef = ...,
     ) -> CreatePortalResponseTypeDef:
         """
         Creates a portal, which can contain projects and dashboards.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.create_portal)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#create_portal)
         """
@@ -484,15 +483,15 @@
     async def create_project(
         self,
         *,
         portalId: str,
         projectName: str,
         projectDescription: str = ...,
         clientToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateProjectResponseTypeDef:
         """
         Creates a project in the specified portal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.create_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#create_project)
         """
@@ -768,15 +767,15 @@
 
     async def execute_action(
         self,
         *,
         targetResource: TargetResourceTypeDef,
         actionDefinitionId: str,
         actionPayload: ActionPayloadTypeDef,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> ExecuteActionResponseTypeDef:
         """
         Executes an action on a target resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.execute_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#execute_action)
         """
@@ -816,15 +815,15 @@
         endDate: TimestampTypeDef,
         assetId: str = ...,
         propertyId: str = ...,
         propertyAlias: str = ...,
         qualities: Sequence[QualityType] = ...,
         timeOrdering: TimeOrderingType = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> GetAssetPropertyAggregatesResponseTypeDef:
         """
         Gets aggregated values for an asset property.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.get_asset_property_aggregates)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#get_asset_property_aggregates)
         """
@@ -846,15 +845,15 @@
         propertyId: str = ...,
         propertyAlias: str = ...,
         startDate: TimestampTypeDef = ...,
         endDate: TimestampTypeDef = ...,
         qualities: Sequence[QualityType] = ...,
         timeOrdering: TimeOrderingType = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> GetAssetPropertyValueHistoryResponseTypeDef:
         """
         Gets the history of an asset property's values.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.get_asset_property_value_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#get_asset_property_value_history)
         """
@@ -870,15 +869,15 @@
         assetId: str = ...,
         propertyId: str = ...,
         propertyAlias: str = ...,
         startTimeOffsetInNanos: int = ...,
         endTimeOffsetInNanos: int = ...,
         nextToken: str = ...,
         maxResults: int = ...,
-        intervalWindowInSeconds: int = ...
+        intervalWindowInSeconds: int = ...,
     ) -> GetInterpolatedAssetPropertyValuesResponseTypeDef:
         """
         Get interpolated values for an asset property for a specified time interval,
         during a period of
         time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.get_interpolated_asset_property_values)
@@ -890,15 +889,15 @@
         *,
         identityType: IdentityTypeType = ...,
         identityId: str = ...,
         resourceType: ResourceTypeType = ...,
         resourceId: str = ...,
         iamArn: str = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListAccessPoliciesResponseTypeDef:
         """
         Retrieves a paginated list of access policies for an identity (an IAM Identity
         Center user, an IAM Identity Center group, or an IAM user) or an IoT SiteWise
         Monitor resource (a portal or
         project).
 
@@ -908,15 +907,15 @@
 
     async def list_actions(
         self,
         *,
         targetResourceType: Literal["ASSET"],
         targetResourceId: str,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListActionsResponseTypeDef:
         """
         Retrieves a paginated list of actions for a specific target resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.list_actions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#list_actions)
         """
@@ -935,74 +934,74 @@
 
     async def list_asset_model_properties(
         self,
         *,
         assetModelId: str,
         nextToken: str = ...,
         maxResults: int = ...,
-        filter: ListAssetModelPropertiesFilterType = ...
+        filter: ListAssetModelPropertiesFilterType = ...,
     ) -> ListAssetModelPropertiesResponseTypeDef:
         """
         Retrieves a paginated list of properties associated with an asset model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.list_asset_model_properties)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#list_asset_model_properties)
         """
 
     async def list_asset_models(
         self,
         *,
         nextToken: str = ...,
         maxResults: int = ...,
-        assetModelTypes: Sequence[AssetModelTypeType] = ...
+        assetModelTypes: Sequence[AssetModelTypeType] = ...,
     ) -> ListAssetModelsResponseTypeDef:
         """
         Retrieves a paginated list of summaries of all asset models.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.list_asset_models)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#list_asset_models)
         """
 
     async def list_asset_properties(
         self,
         *,
         assetId: str,
         nextToken: str = ...,
         maxResults: int = ...,
-        filter: ListAssetPropertiesFilterType = ...
+        filter: ListAssetPropertiesFilterType = ...,
     ) -> ListAssetPropertiesResponseTypeDef:
         """
         Retrieves a paginated list of properties associated with an asset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.list_asset_properties)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#list_asset_properties)
         """
 
     async def list_asset_relationships(
         self,
         *,
         assetId: str,
         traversalType: Literal["PATH_TO_ROOT"],
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListAssetRelationshipsResponseTypeDef:
         """
         Retrieves a paginated list of asset relationships for an asset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.list_asset_relationships)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#list_asset_relationships)
         """
 
     async def list_assets(
         self,
         *,
         nextToken: str = ...,
         maxResults: int = ...,
         assetModelId: str = ...,
-        filter: ListAssetsFilterType = ...
+        filter: ListAssetsFilterType = ...,
     ) -> ListAssetsResponseTypeDef:
         """
         Retrieves a paginated list of asset summaries.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.list_assets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#list_assets)
         """
@@ -1010,29 +1009,29 @@
     async def list_associated_assets(
         self,
         *,
         assetId: str,
         hierarchyId: str = ...,
         traversalDirection: TraversalDirectionType = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListAssociatedAssetsResponseTypeDef:
         """
         Retrieves a paginated list of associated assets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.list_associated_assets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#list_associated_assets)
         """
 
     async def list_bulk_import_jobs(
         self,
         *,
         nextToken: str = ...,
         maxResults: int = ...,
-        filter: ListBulkImportJobsFilterType = ...
+        filter: ListBulkImportJobsFilterType = ...,
     ) -> ListBulkImportJobsResponseTypeDef:
         """
         Retrieves a paginated list of bulk import job requests.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.list_bulk_import_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#list_bulk_import_jobs)
         """
@@ -1113,15 +1112,15 @@
     async def list_time_series(
         self,
         *,
         nextToken: str = ...,
         maxResults: int = ...,
         assetId: str = ...,
         aliasPrefix: str = ...,
-        timeSeriesType: ListTimeSeriesTypeType = ...
+        timeSeriesType: ListTimeSeriesTypeType = ...,
     ) -> ListTimeSeriesResponseTypeDef:
         """
         Retrieves a paginated list of time series (data streams).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.list_time_series)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#list_time_series)
         """
@@ -1148,15 +1147,15 @@
         self,
         *,
         storageType: StorageTypeType,
         multiLayerStorage: MultiLayerStorageTypeDef = ...,
         disassociatedDataStorage: DisassociatedDataStorageStateType = ...,
         retentionPeriod: RetentionPeriodTypeDef = ...,
         warmTier: WarmTierStateType = ...,
-        warmTierRetentionPeriod: WarmTierRetentionPeriodTypeDef = ...
+        warmTierRetentionPeriod: WarmTierRetentionPeriodTypeDef = ...,
     ) -> PutStorageConfigurationResponseTypeDef:
         """
         Configures storage settings for IoT SiteWise.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.put_storage_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#put_storage_configuration)
         """
@@ -1180,15 +1179,15 @@
     async def update_access_policy(
         self,
         *,
         accessPolicyId: str,
         accessPolicyIdentity: IdentityTypeDef,
         accessPolicyResource: ResourceTypeDef,
         accessPolicyPermission: PermissionType,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates an existing access policy that specifies an identity's access to an IoT
         SiteWise Monitor portal or project
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.update_access_policy)
@@ -1198,15 +1197,15 @@
     async def update_asset(
         self,
         *,
         assetId: str,
         assetName: str,
         clientToken: str = ...,
         assetDescription: str = ...,
-        assetExternalId: str = ...
+        assetExternalId: str = ...,
     ) -> UpdateAssetResponseTypeDef:
         """
         Updates an asset's name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.update_asset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#update_asset)
         """
@@ -1217,15 +1216,15 @@
         assetModelId: str,
         assetModelName: str,
         assetModelDescription: str = ...,
         assetModelProperties: Sequence[AssetModelPropertyTypeDef] = ...,
         assetModelHierarchies: Sequence[AssetModelHierarchyTypeDef] = ...,
         assetModelCompositeModels: Sequence[AssetModelCompositeModelTypeDef] = ...,
         clientToken: str = ...,
-        assetModelExternalId: str = ...
+        assetModelExternalId: str = ...,
     ) -> UpdateAssetModelResponseTypeDef:
         """
         Updates an asset model and all of the assets that were created from the model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.update_asset_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#update_asset_model)
         """
@@ -1235,15 +1234,15 @@
         *,
         assetModelId: str,
         assetModelCompositeModelId: str,
         assetModelCompositeModelName: str,
         assetModelCompositeModelExternalId: str = ...,
         assetModelCompositeModelDescription: str = ...,
         clientToken: str = ...,
-        assetModelCompositeModelProperties: Sequence[AssetModelPropertyTypeDef] = ...
+        assetModelCompositeModelProperties: Sequence[AssetModelPropertyTypeDef] = ...,
     ) -> UpdateAssetModelCompositeModelResponseTypeDef:
         """
         Updates a composite model and all of the assets that were created from the
         model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.update_asset_model_composite_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#update_asset_model_composite_model)
@@ -1253,15 +1252,15 @@
         self,
         *,
         assetId: str,
         propertyId: str,
         propertyAlias: str = ...,
         propertyNotificationState: PropertyNotificationStateType = ...,
         clientToken: str = ...,
-        propertyUnit: str = ...
+        propertyUnit: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates an asset property's alias and notification state.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.update_asset_property)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#update_asset_property)
         """
@@ -1269,15 +1268,15 @@
     async def update_dashboard(
         self,
         *,
         dashboardId: str,
         dashboardName: str,
         dashboardDefinition: str,
         dashboardDescription: str = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates an IoT SiteWise Monitor dashboard.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.update_dashboard)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#update_dashboard)
         """
@@ -1310,30 +1309,30 @@
         portalName: str,
         portalContactEmail: str,
         roleArn: str,
         portalDescription: str = ...,
         portalLogoImage: ImageTypeDef = ...,
         clientToken: str = ...,
         notificationSenderEmail: str = ...,
-        alarms: AlarmsTypeDef = ...
+        alarms: AlarmsTypeDef = ...,
     ) -> UpdatePortalResponseTypeDef:
         """
         Updates an IoT SiteWise Monitor portal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.update_portal)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#update_portal)
         """
 
     async def update_project(
         self,
         *,
         projectId: str,
         projectName: str,
         projectDescription: str = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates an IoT SiteWise Monitor project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.update_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#update_project)
         """
```

### Comparing `types-aiobotocore-iotsitewise-2.9.0/types_aiobotocore_iotsitewise/client.pyi` & `types-aiobotocore-iotsitewise-2.9.1/types_aiobotocore_iotsitewise/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -260,15 +260,15 @@
         """
 
     async def batch_get_asset_property_aggregates(
         self,
         *,
         entries: Sequence[BatchGetAssetPropertyAggregatesEntryTypeDef],
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> BatchGetAssetPropertyAggregatesResponseTypeDef:
         """
         Gets aggregated values (for example, average, minimum, and maximum) for one or
         more asset
         properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.batch_get_asset_property_aggregates)
@@ -286,15 +286,15 @@
         """
 
     async def batch_get_asset_property_value_history(
         self,
         *,
         entries: Sequence[BatchGetAssetPropertyValueHistoryEntryTypeDef],
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> BatchGetAssetPropertyValueHistoryResponseTypeDef:
         """
         Gets the historical values for one or more asset properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.batch_get_asset_property_value_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#batch_get_asset_property_value_history)
         """
@@ -328,15 +328,15 @@
     async def create_access_policy(
         self,
         *,
         accessPolicyIdentity: IdentityTypeDef,
         accessPolicyResource: ResourceTypeDef,
         accessPolicyPermission: PermissionType,
         clientToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateAccessPolicyResponseTypeDef:
         """
         Creates an access policy that grants the specified identity (IAM Identity
         Center user, IAM Identity Center group, or IAM user) access to the specified
         IoT SiteWise Monitor portal or project
         resource.
 
@@ -349,15 +349,15 @@
         *,
         assetName: str,
         assetModelId: str,
         clientToken: str = ...,
         tags: Mapping[str, str] = ...,
         assetDescription: str = ...,
         assetId: str = ...,
-        assetExternalId: str = ...
+        assetExternalId: str = ...,
     ) -> CreateAssetResponseTypeDef:
         """
         Creates an asset from an existing asset model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.create_asset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#create_asset)
         """
@@ -370,15 +370,15 @@
         assetModelProperties: Sequence[AssetModelPropertyDefinitionTypeDef] = ...,
         assetModelHierarchies: Sequence[AssetModelHierarchyDefinitionTypeDef] = ...,
         assetModelCompositeModels: Sequence[AssetModelCompositeModelDefinitionTypeDef] = ...,
         clientToken: str = ...,
         tags: Mapping[str, str] = ...,
         assetModelId: str = ...,
         assetModelExternalId: str = ...,
-        assetModelType: AssetModelTypeType = ...
+        assetModelType: AssetModelTypeType = ...,
     ) -> CreateAssetModelResponseTypeDef:
         """
         Creates an asset model from specified property and hierarchy definitions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.create_asset_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#create_asset_model)
         """
@@ -391,15 +391,15 @@
         assetModelCompositeModelType: str,
         parentAssetModelCompositeModelId: str = ...,
         assetModelCompositeModelExternalId: str = ...,
         assetModelCompositeModelId: str = ...,
         assetModelCompositeModelDescription: str = ...,
         clientToken: str = ...,
         composedAssetModelId: str = ...,
-        assetModelCompositeModelProperties: Sequence[AssetModelPropertyDefinitionTypeDef] = ...
+        assetModelCompositeModelProperties: Sequence[AssetModelPropertyDefinitionTypeDef] = ...,
     ) -> CreateAssetModelCompositeModelResponseTypeDef:
         """
         Creates a custom composite model from specified property and hierarchy
         definitions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.create_asset_model_composite_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#create_asset_model_composite_model)
@@ -410,15 +410,15 @@
         *,
         jobName: str,
         jobRoleArn: str,
         files: Sequence[FileTypeDef],
         errorReportLocation: ErrorReportLocationTypeDef,
         jobConfiguration: JobConfigurationTypeDef,
         adaptiveIngestion: bool = ...,
-        deleteFilesAfterImport: bool = ...
+        deleteFilesAfterImport: bool = ...,
     ) -> CreateBulkImportJobResponseTypeDef:
         """
         Defines a job to ingest data to IoT SiteWise from Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.create_bulk_import_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#create_bulk_import_job)
         """
@@ -427,29 +427,29 @@
         self,
         *,
         projectId: str,
         dashboardName: str,
         dashboardDefinition: str,
         dashboardDescription: str = ...,
         clientToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateDashboardResponseTypeDef:
         """
         Creates a dashboard in an IoT SiteWise Monitor project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.create_dashboard)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#create_dashboard)
         """
 
     async def create_gateway(
         self,
         *,
         gatewayName: str,
         gatewayPlatform: GatewayPlatformTypeDef,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateGatewayResponseTypeDef:
         """
         Creates a gateway, which is a virtual or edge device that delivers industrial
         data streams from local servers to IoT
         SiteWise.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.create_gateway)
@@ -464,15 +464,15 @@
         roleArn: str,
         portalDescription: str = ...,
         clientToken: str = ...,
         portalLogoImageFile: ImageFileTypeDef = ...,
         tags: Mapping[str, str] = ...,
         portalAuthMode: AuthModeType = ...,
         notificationSenderEmail: str = ...,
-        alarms: AlarmsTypeDef = ...
+        alarms: AlarmsTypeDef = ...,
     ) -> CreatePortalResponseTypeDef:
         """
         Creates a portal, which can contain projects and dashboards.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.create_portal)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#create_portal)
         """
@@ -480,15 +480,15 @@
     async def create_project(
         self,
         *,
         portalId: str,
         projectName: str,
         projectDescription: str = ...,
         clientToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateProjectResponseTypeDef:
         """
         Creates a project in the specified portal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.create_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#create_project)
         """
@@ -764,15 +764,15 @@
 
     async def execute_action(
         self,
         *,
         targetResource: TargetResourceTypeDef,
         actionDefinitionId: str,
         actionPayload: ActionPayloadTypeDef,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> ExecuteActionResponseTypeDef:
         """
         Executes an action on a target resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.execute_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#execute_action)
         """
@@ -812,15 +812,15 @@
         endDate: TimestampTypeDef,
         assetId: str = ...,
         propertyId: str = ...,
         propertyAlias: str = ...,
         qualities: Sequence[QualityType] = ...,
         timeOrdering: TimeOrderingType = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> GetAssetPropertyAggregatesResponseTypeDef:
         """
         Gets aggregated values for an asset property.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.get_asset_property_aggregates)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#get_asset_property_aggregates)
         """
@@ -842,15 +842,15 @@
         propertyId: str = ...,
         propertyAlias: str = ...,
         startDate: TimestampTypeDef = ...,
         endDate: TimestampTypeDef = ...,
         qualities: Sequence[QualityType] = ...,
         timeOrdering: TimeOrderingType = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> GetAssetPropertyValueHistoryResponseTypeDef:
         """
         Gets the history of an asset property's values.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.get_asset_property_value_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#get_asset_property_value_history)
         """
@@ -866,15 +866,15 @@
         assetId: str = ...,
         propertyId: str = ...,
         propertyAlias: str = ...,
         startTimeOffsetInNanos: int = ...,
         endTimeOffsetInNanos: int = ...,
         nextToken: str = ...,
         maxResults: int = ...,
-        intervalWindowInSeconds: int = ...
+        intervalWindowInSeconds: int = ...,
     ) -> GetInterpolatedAssetPropertyValuesResponseTypeDef:
         """
         Get interpolated values for an asset property for a specified time interval,
         during a period of
         time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.get_interpolated_asset_property_values)
@@ -886,15 +886,15 @@
         *,
         identityType: IdentityTypeType = ...,
         identityId: str = ...,
         resourceType: ResourceTypeType = ...,
         resourceId: str = ...,
         iamArn: str = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListAccessPoliciesResponseTypeDef:
         """
         Retrieves a paginated list of access policies for an identity (an IAM Identity
         Center user, an IAM Identity Center group, or an IAM user) or an IoT SiteWise
         Monitor resource (a portal or
         project).
 
@@ -904,15 +904,15 @@
 
     async def list_actions(
         self,
         *,
         targetResourceType: Literal["ASSET"],
         targetResourceId: str,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListActionsResponseTypeDef:
         """
         Retrieves a paginated list of actions for a specific target resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.list_actions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#list_actions)
         """
@@ -931,74 +931,74 @@
 
     async def list_asset_model_properties(
         self,
         *,
         assetModelId: str,
         nextToken: str = ...,
         maxResults: int = ...,
-        filter: ListAssetModelPropertiesFilterType = ...
+        filter: ListAssetModelPropertiesFilterType = ...,
     ) -> ListAssetModelPropertiesResponseTypeDef:
         """
         Retrieves a paginated list of properties associated with an asset model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.list_asset_model_properties)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#list_asset_model_properties)
         """
 
     async def list_asset_models(
         self,
         *,
         nextToken: str = ...,
         maxResults: int = ...,
-        assetModelTypes: Sequence[AssetModelTypeType] = ...
+        assetModelTypes: Sequence[AssetModelTypeType] = ...,
     ) -> ListAssetModelsResponseTypeDef:
         """
         Retrieves a paginated list of summaries of all asset models.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.list_asset_models)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#list_asset_models)
         """
 
     async def list_asset_properties(
         self,
         *,
         assetId: str,
         nextToken: str = ...,
         maxResults: int = ...,
-        filter: ListAssetPropertiesFilterType = ...
+        filter: ListAssetPropertiesFilterType = ...,
     ) -> ListAssetPropertiesResponseTypeDef:
         """
         Retrieves a paginated list of properties associated with an asset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.list_asset_properties)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#list_asset_properties)
         """
 
     async def list_asset_relationships(
         self,
         *,
         assetId: str,
         traversalType: Literal["PATH_TO_ROOT"],
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListAssetRelationshipsResponseTypeDef:
         """
         Retrieves a paginated list of asset relationships for an asset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.list_asset_relationships)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#list_asset_relationships)
         """
 
     async def list_assets(
         self,
         *,
         nextToken: str = ...,
         maxResults: int = ...,
         assetModelId: str = ...,
-        filter: ListAssetsFilterType = ...
+        filter: ListAssetsFilterType = ...,
     ) -> ListAssetsResponseTypeDef:
         """
         Retrieves a paginated list of asset summaries.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.list_assets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#list_assets)
         """
@@ -1006,29 +1006,29 @@
     async def list_associated_assets(
         self,
         *,
         assetId: str,
         hierarchyId: str = ...,
         traversalDirection: TraversalDirectionType = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListAssociatedAssetsResponseTypeDef:
         """
         Retrieves a paginated list of associated assets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.list_associated_assets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#list_associated_assets)
         """
 
     async def list_bulk_import_jobs(
         self,
         *,
         nextToken: str = ...,
         maxResults: int = ...,
-        filter: ListBulkImportJobsFilterType = ...
+        filter: ListBulkImportJobsFilterType = ...,
     ) -> ListBulkImportJobsResponseTypeDef:
         """
         Retrieves a paginated list of bulk import job requests.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.list_bulk_import_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#list_bulk_import_jobs)
         """
@@ -1109,15 +1109,15 @@
     async def list_time_series(
         self,
         *,
         nextToken: str = ...,
         maxResults: int = ...,
         assetId: str = ...,
         aliasPrefix: str = ...,
-        timeSeriesType: ListTimeSeriesTypeType = ...
+        timeSeriesType: ListTimeSeriesTypeType = ...,
     ) -> ListTimeSeriesResponseTypeDef:
         """
         Retrieves a paginated list of time series (data streams).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.list_time_series)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#list_time_series)
         """
@@ -1144,15 +1144,15 @@
         self,
         *,
         storageType: StorageTypeType,
         multiLayerStorage: MultiLayerStorageTypeDef = ...,
         disassociatedDataStorage: DisassociatedDataStorageStateType = ...,
         retentionPeriod: RetentionPeriodTypeDef = ...,
         warmTier: WarmTierStateType = ...,
-        warmTierRetentionPeriod: WarmTierRetentionPeriodTypeDef = ...
+        warmTierRetentionPeriod: WarmTierRetentionPeriodTypeDef = ...,
     ) -> PutStorageConfigurationResponseTypeDef:
         """
         Configures storage settings for IoT SiteWise.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.put_storage_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#put_storage_configuration)
         """
@@ -1176,15 +1176,15 @@
     async def update_access_policy(
         self,
         *,
         accessPolicyId: str,
         accessPolicyIdentity: IdentityTypeDef,
         accessPolicyResource: ResourceTypeDef,
         accessPolicyPermission: PermissionType,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates an existing access policy that specifies an identity's access to an IoT
         SiteWise Monitor portal or project
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.update_access_policy)
@@ -1194,15 +1194,15 @@
     async def update_asset(
         self,
         *,
         assetId: str,
         assetName: str,
         clientToken: str = ...,
         assetDescription: str = ...,
-        assetExternalId: str = ...
+        assetExternalId: str = ...,
     ) -> UpdateAssetResponseTypeDef:
         """
         Updates an asset's name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.update_asset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#update_asset)
         """
@@ -1213,15 +1213,15 @@
         assetModelId: str,
         assetModelName: str,
         assetModelDescription: str = ...,
         assetModelProperties: Sequence[AssetModelPropertyTypeDef] = ...,
         assetModelHierarchies: Sequence[AssetModelHierarchyTypeDef] = ...,
         assetModelCompositeModels: Sequence[AssetModelCompositeModelTypeDef] = ...,
         clientToken: str = ...,
-        assetModelExternalId: str = ...
+        assetModelExternalId: str = ...,
     ) -> UpdateAssetModelResponseTypeDef:
         """
         Updates an asset model and all of the assets that were created from the model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.update_asset_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#update_asset_model)
         """
@@ -1231,15 +1231,15 @@
         *,
         assetModelId: str,
         assetModelCompositeModelId: str,
         assetModelCompositeModelName: str,
         assetModelCompositeModelExternalId: str = ...,
         assetModelCompositeModelDescription: str = ...,
         clientToken: str = ...,
-        assetModelCompositeModelProperties: Sequence[AssetModelPropertyTypeDef] = ...
+        assetModelCompositeModelProperties: Sequence[AssetModelPropertyTypeDef] = ...,
     ) -> UpdateAssetModelCompositeModelResponseTypeDef:
         """
         Updates a composite model and all of the assets that were created from the
         model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.update_asset_model_composite_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#update_asset_model_composite_model)
@@ -1249,15 +1249,15 @@
         self,
         *,
         assetId: str,
         propertyId: str,
         propertyAlias: str = ...,
         propertyNotificationState: PropertyNotificationStateType = ...,
         clientToken: str = ...,
-        propertyUnit: str = ...
+        propertyUnit: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates an asset property's alias and notification state.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.update_asset_property)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#update_asset_property)
         """
@@ -1265,15 +1265,15 @@
     async def update_dashboard(
         self,
         *,
         dashboardId: str,
         dashboardName: str,
         dashboardDefinition: str,
         dashboardDescription: str = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates an IoT SiteWise Monitor dashboard.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.update_dashboard)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#update_dashboard)
         """
@@ -1306,30 +1306,30 @@
         portalName: str,
         portalContactEmail: str,
         roleArn: str,
         portalDescription: str = ...,
         portalLogoImage: ImageTypeDef = ...,
         clientToken: str = ...,
         notificationSenderEmail: str = ...,
-        alarms: AlarmsTypeDef = ...
+        alarms: AlarmsTypeDef = ...,
     ) -> UpdatePortalResponseTypeDef:
         """
         Updates an IoT SiteWise Monitor portal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.update_portal)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#update_portal)
         """
 
     async def update_project(
         self,
         *,
         projectId: str,
         projectName: str,
         projectDescription: str = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates an IoT SiteWise Monitor project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.update_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#update_project)
         """
```

### Comparing `types-aiobotocore-iotsitewise-2.9.0/types_aiobotocore_iotsitewise/literals.py` & `types-aiobotocore-iotsitewise-2.9.1/types_aiobotocore_iotsitewise/literals.py`

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
     "AggregateTypeType",
     "AssetActiveWaiterName",
     "AssetErrorCodeType",
     "AssetModelActiveWaiterName",
     "AssetModelNotExistsWaiterName",
     "AssetModelStateType",
@@ -96,15 +95,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 AggregateTypeType = Literal["AVERAGE", "COUNT", "MAXIMUM", "MINIMUM", "STANDARD_DEVIATION", "SUM"]
 AssetActiveWaiterName = Literal["asset_active"]
 AssetErrorCodeType = Literal["INTERNAL_FAILURE"]
 AssetModelActiveWaiterName = Literal["asset_model_active"]
 AssetModelNotExistsWaiterName = Literal["asset_model_not_exists"]
 AssetModelStateType = Literal["ACTIVE", "CREATING", "DELETING", "FAILED", "PROPAGATING", "UPDATING"]
 AssetModelTypeType = Literal["ASSET_MODEL", "COMPONENT_MODEL"]
```

### Comparing `types-aiobotocore-iotsitewise-2.9.0/types_aiobotocore_iotsitewise/literals.pyi` & `types-aiobotocore-iotsitewise-2.9.1/types_aiobotocore_iotsitewise/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotsitewise-2.9.0/types_aiobotocore_iotsitewise/paginator.py` & `types-aiobotocore-iotsitewise-2.9.1/types_aiobotocore_iotsitewise/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ExecuteQueryPaginator",
     "GetAssetPropertyAggregatesPaginator",
     "GetAssetPropertyValueHistoryPaginator",
     "GetInterpolatedAssetPropertyValuesPaginator",
     "ListAccessPoliciesPaginator",
     "ListActionsPaginator",
@@ -133,15 +132,14 @@
     "ListGatewaysPaginator",
     "ListPortalsPaginator",
     "ListProjectAssetsPaginator",
     "ListProjectsPaginator",
     "ListTimeSeriesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -177,15 +175,15 @@
         startDate: TimestampTypeDef,
         endDate: TimestampTypeDef,
         assetId: str = ...,
         propertyId: str = ...,
         propertyAlias: str = ...,
         qualities: Sequence[QualityType] = ...,
         timeOrdering: TimeOrderingType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetAssetPropertyAggregatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.GetAssetPropertyAggregates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/paginators/#getassetpropertyaggregatespaginator)
         """
 
 
@@ -201,15 +199,15 @@
         assetId: str = ...,
         propertyId: str = ...,
         propertyAlias: str = ...,
         startDate: TimestampTypeDef = ...,
         endDate: TimestampTypeDef = ...,
         qualities: Sequence[QualityType] = ...,
         timeOrdering: TimeOrderingType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetAssetPropertyValueHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.GetAssetPropertyValueHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/paginators/#getassetpropertyvaluehistorypaginator)
         """
 
 
@@ -229,15 +227,15 @@
         type: str,
         assetId: str = ...,
         propertyId: str = ...,
         propertyAlias: str = ...,
         startTimeOffsetInNanos: int = ...,
         endTimeOffsetInNanos: int = ...,
         intervalWindowInSeconds: int = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetInterpolatedAssetPropertyValuesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.GetInterpolatedAssetPropertyValues.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/paginators/#getinterpolatedassetpropertyvaluespaginator)
         """
 
 
@@ -251,15 +249,15 @@
         self,
         *,
         identityType: IdentityTypeType = ...,
         identityId: str = ...,
         resourceType: ResourceTypeType = ...,
         resourceId: str = ...,
         iamArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAccessPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAccessPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/paginators/#listaccesspoliciespaginator)
         """
 
 
@@ -270,15 +268,15 @@
     """
 
     def paginate(
         self,
         *,
         targetResourceType: Literal["ASSET"],
         targetResourceId: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListActionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListActions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/paginators/#listactionspaginator)
         """
 
 
@@ -304,15 +302,15 @@
     """
 
     def paginate(
         self,
         *,
         assetModelId: str,
         filter: ListAssetModelPropertiesFilterType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAssetModelPropertiesResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssetModelProperties.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/paginators/#listassetmodelpropertiespaginator)
         """
 
 
@@ -322,15 +320,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/paginators/#listassetmodelspaginator)
     """
 
     def paginate(
         self,
         *,
         assetModelTypes: Sequence[AssetModelTypeType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAssetModelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssetModels.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/paginators/#listassetmodelspaginator)
         """
 
 
@@ -341,15 +339,15 @@
     """
 
     def paginate(
         self,
         *,
         assetId: str,
         filter: ListAssetPropertiesFilterType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAssetPropertiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssetProperties.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/paginators/#listassetpropertiespaginator)
         """
 
 
@@ -360,15 +358,15 @@
     """
 
     def paginate(
         self,
         *,
         assetId: str,
         traversalType: Literal["PATH_TO_ROOT"],
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAssetRelationshipsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssetRelationships.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/paginators/#listassetrelationshipspaginator)
         """
 
 
@@ -379,15 +377,15 @@
     """
 
     def paginate(
         self,
         *,
         assetModelId: str = ...,
         filter: ListAssetsFilterType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAssetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/paginators/#listassetspaginator)
         """
 
 
@@ -399,15 +397,15 @@
 
     def paginate(
         self,
         *,
         assetId: str,
         hierarchyId: str = ...,
         traversalDirection: TraversalDirectionType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAssociatedAssetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssociatedAssets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/paginators/#listassociatedassetspaginator)
         """
 
 
@@ -417,15 +415,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/paginators/#listbulkimportjobspaginator)
     """
 
     def paginate(
         self,
         *,
         filter: ListBulkImportJobsFilterType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListBulkImportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListBulkImportJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/paginators/#listbulkimportjobspaginator)
         """
 
 
@@ -527,13 +525,13 @@
 
     def paginate(
         self,
         *,
         assetId: str = ...,
         aliasPrefix: str = ...,
         timeSeriesType: ListTimeSeriesTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTimeSeriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListTimeSeries.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/paginators/#listtimeseriespaginator)
         """
```

### Comparing `types-aiobotocore-iotsitewise-2.9.0/types_aiobotocore_iotsitewise/paginator.pyi` & `types-aiobotocore-iotsitewise-2.9.1/types_aiobotocore_iotsitewise/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,15 @@
         startDate: TimestampTypeDef,
         endDate: TimestampTypeDef,
         assetId: str = ...,
         propertyId: str = ...,
         propertyAlias: str = ...,
         qualities: Sequence[QualityType] = ...,
         timeOrdering: TimeOrderingType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetAssetPropertyAggregatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.GetAssetPropertyAggregates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/paginators/#getassetpropertyaggregatespaginator)
         """
 
 class GetAssetPropertyValueHistoryPaginator(AioPaginator):
@@ -195,15 +195,15 @@
         assetId: str = ...,
         propertyId: str = ...,
         propertyAlias: str = ...,
         startDate: TimestampTypeDef = ...,
         endDate: TimestampTypeDef = ...,
         qualities: Sequence[QualityType] = ...,
         timeOrdering: TimeOrderingType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetAssetPropertyValueHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.GetAssetPropertyValueHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/paginators/#getassetpropertyvaluehistorypaginator)
         """
 
 class GetInterpolatedAssetPropertyValuesPaginator(AioPaginator):
@@ -222,15 +222,15 @@
         type: str,
         assetId: str = ...,
         propertyId: str = ...,
         propertyAlias: str = ...,
         startTimeOffsetInNanos: int = ...,
         endTimeOffsetInNanos: int = ...,
         intervalWindowInSeconds: int = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetInterpolatedAssetPropertyValuesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.GetInterpolatedAssetPropertyValues.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/paginators/#getinterpolatedassetpropertyvaluespaginator)
         """
 
 class ListAccessPoliciesPaginator(AioPaginator):
@@ -243,15 +243,15 @@
         self,
         *,
         identityType: IdentityTypeType = ...,
         identityId: str = ...,
         resourceType: ResourceTypeType = ...,
         resourceId: str = ...,
         iamArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAccessPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAccessPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/paginators/#listaccesspoliciespaginator)
         """
 
 class ListActionsPaginator(AioPaginator):
@@ -261,15 +261,15 @@
     """
 
     def paginate(
         self,
         *,
         targetResourceType: Literal["ASSET"],
         targetResourceId: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListActionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListActions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/paginators/#listactionspaginator)
         """
 
 class ListAssetModelCompositeModelsPaginator(AioPaginator):
@@ -293,15 +293,15 @@
     """
 
     def paginate(
         self,
         *,
         assetModelId: str,
         filter: ListAssetModelPropertiesFilterType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAssetModelPropertiesResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssetModelProperties.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/paginators/#listassetmodelpropertiespaginator)
         """
 
 class ListAssetModelsPaginator(AioPaginator):
@@ -310,15 +310,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/paginators/#listassetmodelspaginator)
     """
 
     def paginate(
         self,
         *,
         assetModelTypes: Sequence[AssetModelTypeType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAssetModelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssetModels.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/paginators/#listassetmodelspaginator)
         """
 
 class ListAssetPropertiesPaginator(AioPaginator):
@@ -328,15 +328,15 @@
     """
 
     def paginate(
         self,
         *,
         assetId: str,
         filter: ListAssetPropertiesFilterType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAssetPropertiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssetProperties.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/paginators/#listassetpropertiespaginator)
         """
 
 class ListAssetRelationshipsPaginator(AioPaginator):
@@ -346,15 +346,15 @@
     """
 
     def paginate(
         self,
         *,
         assetId: str,
         traversalType: Literal["PATH_TO_ROOT"],
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAssetRelationshipsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssetRelationships.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/paginators/#listassetrelationshipspaginator)
         """
 
 class ListAssetsPaginator(AioPaginator):
@@ -364,15 +364,15 @@
     """
 
     def paginate(
         self,
         *,
         assetModelId: str = ...,
         filter: ListAssetsFilterType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAssetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/paginators/#listassetspaginator)
         """
 
 class ListAssociatedAssetsPaginator(AioPaginator):
@@ -383,15 +383,15 @@
 
     def paginate(
         self,
         *,
         assetId: str,
         hierarchyId: str = ...,
         traversalDirection: TraversalDirectionType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAssociatedAssetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssociatedAssets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/paginators/#listassociatedassetspaginator)
         """
 
 class ListBulkImportJobsPaginator(AioPaginator):
@@ -400,15 +400,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/paginators/#listbulkimportjobspaginator)
     """
 
     def paginate(
         self,
         *,
         filter: ListBulkImportJobsFilterType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListBulkImportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListBulkImportJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/paginators/#listbulkimportjobspaginator)
         """
 
 class ListCompositionRelationshipsPaginator(AioPaginator):
@@ -503,13 +503,13 @@
 
     def paginate(
         self,
         *,
         assetId: str = ...,
         aliasPrefix: str = ...,
         timeSeriesType: ListTimeSeriesTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTimeSeriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListTimeSeries.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/paginators/#listtimeseriespaginator)
         """
```

### Comparing `types-aiobotocore-iotsitewise-2.9.0/types_aiobotocore_iotsitewise/type_defs.py` & `types-aiobotocore-iotsitewise-2.9.1/types_aiobotocore_iotsitewise/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ActionDefinitionTypeDef",
     "ActionPayloadTypeDef",
     "TargetResourceTypeDef",
     "AggregatesTypeDef",
     "AlarmsTypeDef",
     "AssetCompositeModelPathSegmentTypeDef",
```

### Comparing `types-aiobotocore-iotsitewise-2.9.0/types_aiobotocore_iotsitewise/type_defs.pyi` & `types-aiobotocore-iotsitewise-2.9.1/types_aiobotocore_iotsitewise/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotsitewise-2.9.0/types_aiobotocore_iotsitewise/waiter.py` & `types-aiobotocore-iotsitewise-2.9.1/types_aiobotocore_iotsitewise/waiter.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     """
 
     async def wait(
         self,
         *,
         assetId: str,
         excludeProperties: bool = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Waiter.AssetActive.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/waiters/#assetactivewaiter)
         """
 
 
@@ -71,15 +71,15 @@
     """
 
     async def wait(
         self,
         *,
         assetModelId: str,
         excludeProperties: bool = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Waiter.AssetModelActive.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/waiters/#assetmodelactivewaiter)
         """
 
 
@@ -90,15 +90,15 @@
     """
 
     async def wait(
         self,
         *,
         assetModelId: str,
         excludeProperties: bool = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Waiter.AssetModelNotExists.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/waiters/#assetmodelnotexistswaiter)
         """
 
 
@@ -109,15 +109,15 @@
     """
 
     async def wait(
         self,
         *,
         assetId: str,
         excludeProperties: bool = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Waiter.AssetNotExists.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/waiters/#assetnotexistswaiter)
         """
```

### Comparing `types-aiobotocore-iotsitewise-2.9.0/types_aiobotocore_iotsitewise/waiter.pyi` & `types-aiobotocore-iotsitewise-2.9.1/types_aiobotocore_iotsitewise/waiter.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     """
 
     async def wait(
         self,
         *,
         assetId: str,
         excludeProperties: bool = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Waiter.AssetActive.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/waiters/#assetactivewaiter)
         """
 
 class AssetModelActiveWaiter(AIOWaiter):
@@ -69,15 +69,15 @@
     """
 
     async def wait(
         self,
         *,
         assetModelId: str,
         excludeProperties: bool = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Waiter.AssetModelActive.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/waiters/#assetmodelactivewaiter)
         """
 
 class AssetModelNotExistsWaiter(AIOWaiter):
@@ -87,15 +87,15 @@
     """
 
     async def wait(
         self,
         *,
         assetModelId: str,
         excludeProperties: bool = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Waiter.AssetModelNotExists.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/waiters/#assetmodelnotexistswaiter)
         """
 
 class AssetNotExistsWaiter(AIOWaiter):
@@ -105,15 +105,15 @@
     """
 
     async def wait(
         self,
         *,
         assetId: str,
         excludeProperties: bool = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Waiter.AssetNotExists.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/waiters/#assetnotexistswaiter)
         """
 
 class PortalActiveWaiter(AIOWaiter):
```

### Comparing `types-aiobotocore-iotsitewise-2.9.0/types_aiobotocore_iotsitewise.egg-info/PKG-INFO` & `types-aiobotocore-iotsitewise-2.9.1/types_aiobotocore_iotsitewise.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotsitewise
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.IoTSiteWise 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.IoTSiteWise 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/
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
 
 <a id="types-aiobotocore-iotsitewise"></a>
 
 # types-aiobotocore-iotsitewise
 
 [![PyPI - types-aiobotocore-iotsitewise](https://img.shields.io/pypi/v/types-aiobotocore-iotsitewise.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotsitewise)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotsitewise.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotsitewise)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotsitewise)](https://pepy.tech/project/types-aiobotocore-iotsitewise)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTSiteWise 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise)
+[aiobotocore.IoTSiteWise 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise)
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
 [types-aiobotocore-iotsitewise docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-iotsitewise-2.9.0/types_aiobotocore_iotsitewise.egg-info/SOURCES.txt` & `types-aiobotocore-iotsitewise-2.9.1/types_aiobotocore_iotsitewise.egg-info/SOURCES.txt`

 * *Files identical despite different names*

