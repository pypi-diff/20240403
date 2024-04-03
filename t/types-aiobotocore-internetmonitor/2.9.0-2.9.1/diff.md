# Comparing `tmp/types-aiobotocore-internetmonitor-2.9.0.tar.gz` & `tmp/types-aiobotocore-internetmonitor-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-internetmonitor-2.9.0.tar", last modified: Wed Dec 13 19:59:29 2023, max compression
+gzip compressed data, was "types-aiobotocore-internetmonitor-2.9.1.tar", last modified: Thu Jan 18 01:20:53 2024, max compression
```

## Comparing `types-aiobotocore-internetmonitor-2.9.0.tar` & `types-aiobotocore-internetmonitor-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:29.553676 types-aiobotocore-internetmonitor-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:47:34.000000 types-aiobotocore-internetmonitor-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13705 2023-12-13 19:59:29.553676 types-aiobotocore-internetmonitor-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12100 2023-12-13 19:47:34.000000 types-aiobotocore-internetmonitor-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:29.553676 types-aiobotocore-internetmonitor-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2023-12-13 19:47:34.000000 types-aiobotocore-internetmonitor-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:29.549677 types-aiobotocore-internetmonitor-2.9.0/types_aiobotocore_internetmonitor/
--rw-r--r--   0 runner    (1001) docker     (127)      965 2023-12-13 19:47:34.000000 types-aiobotocore-internetmonitor-2.9.0/types_aiobotocore_internetmonitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2023-12-13 19:47:34.000000 types-aiobotocore-internetmonitor-2.9.0/types_aiobotocore_internetmonitor/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      984 2023-12-13 19:47:34.000000 types-aiobotocore-internetmonitor-2.9.0/types_aiobotocore_internetmonitor/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15470 2023-12-13 19:47:34.000000 types-aiobotocore-internetmonitor-2.9.0/types_aiobotocore_internetmonitor/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    15466 2023-12-13 19:47:34.000000 types-aiobotocore-internetmonitor-2.9.0/types_aiobotocore_internetmonitor/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10122 2023-12-13 19:47:35.000000 types-aiobotocore-internetmonitor-2.9.0/types_aiobotocore_internetmonitor/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10120 2023-12-13 19:47:34.000000 types-aiobotocore-internetmonitor-2.9.0/types_aiobotocore_internetmonitor/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3520 2023-12-13 19:47:34.000000 types-aiobotocore-internetmonitor-2.9.0/types_aiobotocore_internetmonitor/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3516 2023-12-13 19:47:34.000000 types-aiobotocore-internetmonitor-2.9.0/types_aiobotocore_internetmonitor/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:47:34.000000 types-aiobotocore-internetmonitor-2.9.0/types_aiobotocore_internetmonitor/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    14116 2023-12-13 19:47:35.000000 types-aiobotocore-internetmonitor-2.9.0/types_aiobotocore_internetmonitor/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    14115 2023-12-13 19:47:35.000000 types-aiobotocore-internetmonitor-2.9.0/types_aiobotocore_internetmonitor/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:47:34.000000 types-aiobotocore-internetmonitor-2.9.0/types_aiobotocore_internetmonitor/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:29.553676 types-aiobotocore-internetmonitor-2.9.0/types_aiobotocore_internetmonitor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13705 2023-12-13 19:59:29.000000 types-aiobotocore-internetmonitor-2.9.0/types_aiobotocore_internetmonitor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      965 2023-12-13 19:59:29.000000 types-aiobotocore-internetmonitor-2.9.0/types_aiobotocore_internetmonitor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:29.000000 types-aiobotocore-internetmonitor-2.9.0/types_aiobotocore_internetmonitor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:29.000000 types-aiobotocore-internetmonitor-2.9.0/types_aiobotocore_internetmonitor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:29.000000 types-aiobotocore-internetmonitor-2.9.0/types_aiobotocore_internetmonitor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-12-13 19:59:29.000000 types-aiobotocore-internetmonitor-2.9.0/types_aiobotocore_internetmonitor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:53.261284 types-aiobotocore-internetmonitor-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:09:26.000000 types-aiobotocore-internetmonitor-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13725 2024-01-18 01:20:53.261284 types-aiobotocore-internetmonitor-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12100 2024-01-18 01:09:26.000000 types-aiobotocore-internetmonitor-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:53.261284 types-aiobotocore-internetmonitor-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-01-18 01:09:26.000000 types-aiobotocore-internetmonitor-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:53.261284 types-aiobotocore-internetmonitor-2.9.1/types_aiobotocore_internetmonitor/
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-01-18 01:09:26.000000 types-aiobotocore-internetmonitor-2.9.1/types_aiobotocore_internetmonitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-01-18 01:09:26.000000 types-aiobotocore-internetmonitor-2.9.1/types_aiobotocore_internetmonitor/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-01-18 01:09:26.000000 types-aiobotocore-internetmonitor-2.9.1/types_aiobotocore_internetmonitor/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15473 2024-01-18 01:09:26.000000 types-aiobotocore-internetmonitor-2.9.1/types_aiobotocore_internetmonitor/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15470 2024-01-18 01:09:26.000000 types-aiobotocore-internetmonitor-2.9.1/types_aiobotocore_internetmonitor/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10120 2024-01-18 01:09:26.000000 types-aiobotocore-internetmonitor-2.9.1/types_aiobotocore_internetmonitor/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10120 2024-01-18 01:09:26.000000 types-aiobotocore-internetmonitor-2.9.1/types_aiobotocore_internetmonitor/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-01-18 01:09:26.000000 types-aiobotocore-internetmonitor-2.9.1/types_aiobotocore_internetmonitor/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-01-18 01:09:26.000000 types-aiobotocore-internetmonitor-2.9.1/types_aiobotocore_internetmonitor/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:09:26.000000 types-aiobotocore-internetmonitor-2.9.1/types_aiobotocore_internetmonitor/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    14115 2024-01-18 01:09:26.000000 types-aiobotocore-internetmonitor-2.9.1/types_aiobotocore_internetmonitor/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14115 2024-01-18 01:09:26.000000 types-aiobotocore-internetmonitor-2.9.1/types_aiobotocore_internetmonitor/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:09:26.000000 types-aiobotocore-internetmonitor-2.9.1/types_aiobotocore_internetmonitor/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:53.261284 types-aiobotocore-internetmonitor-2.9.1/types_aiobotocore_internetmonitor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13725 2024-01-18 01:20:53.000000 types-aiobotocore-internetmonitor-2.9.1/types_aiobotocore_internetmonitor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-01-18 01:20:53.000000 types-aiobotocore-internetmonitor-2.9.1/types_aiobotocore_internetmonitor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:53.000000 types-aiobotocore-internetmonitor-2.9.1/types_aiobotocore_internetmonitor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:53.000000 types-aiobotocore-internetmonitor-2.9.1/types_aiobotocore_internetmonitor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:53.000000 types-aiobotocore-internetmonitor-2.9.1/types_aiobotocore_internetmonitor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-01-18 01:20:53.000000 types-aiobotocore-internetmonitor-2.9.1/types_aiobotocore_internetmonitor.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-internetmonitor-2.9.0/LICENSE` & `types-aiobotocore-internetmonitor-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-internetmonitor-2.9.0/PKG-INFO` & `types-aiobotocore-internetmonitor-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-internetmonitor
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CloudWatchInternetMonitor 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CloudWatchInternetMonitor 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/
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
 
 <a id="types-aiobotocore-internetmonitor"></a>
 
 # types-aiobotocore-internetmonitor
 
 [![PyPI - types-aiobotocore-internetmonitor](https://img.shields.io/pypi/v/types-aiobotocore-internetmonitor.svg?color=blue)](https://pypi.org/project/types-aiobotocore-internetmonitor)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-internetmonitor.svg?color=blue)](https://pypi.org/project/types-aiobotocore-internetmonitor)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-internetmonitor)](https://pepy.tech/project/types-aiobotocore-internetmonitor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudWatchInternetMonitor 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor)
+[aiobotocore.CloudWatchInternetMonitor 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor)
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
 [types-aiobotocore-internetmonitor docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-internetmonitor-2.9.0/README.md` & `types-aiobotocore-internetmonitor-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-internetmonitor.svg?color=blue)](https://pypi.org/project/types-aiobotocore-internetmonitor)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-internetmonitor)](https://pepy.tech/project/types-aiobotocore-internetmonitor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudWatchInternetMonitor 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor)
+[aiobotocore.CloudWatchInternetMonitor 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor)
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
 [types-aiobotocore-internetmonitor docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-internetmonitor-2.9.0/setup.py` & `types-aiobotocore-internetmonitor-2.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-internetmonitor",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_internetmonitor"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CloudWatchInternetMonitor 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.CloudWatchInternetMonitor 2.9.1 service generated with"
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
     keywords="aiobotocore internetmonitor type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_internetmonitor": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-internetmonitor-2.9.0/types_aiobotocore_internetmonitor/__init__.py` & `types-aiobotocore-internetmonitor-2.9.1/types_aiobotocore_internetmonitor/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,13 @@
 """
 
 from .client import CloudWatchInternetMonitorClient
 from .paginator import ListHealthEventsPaginator, ListMonitorsPaginator
 
 Client = CloudWatchInternetMonitorClient
 
-
 __all__ = (
     "Client",
     "CloudWatchInternetMonitorClient",
     "ListHealthEventsPaginator",
     "ListMonitorsPaginator",
 )
```

### Comparing `types-aiobotocore-internetmonitor-2.9.0/types_aiobotocore_internetmonitor/__init__.pyi` & `types-aiobotocore-internetmonitor-2.9.1/types_aiobotocore_internetmonitor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-internetmonitor-2.9.0/types_aiobotocore_internetmonitor/__main__.py` & `types-aiobotocore-internetmonitor-2.9.1/types_aiobotocore_internetmonitor/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CloudWatchInternetMonitor 2.9.0\nVersion:        "
-        " 2.9.0\nBuilder version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.CloudWatchInternetMonitor 2.9.1\nVersion:        "
+        " 2.9.1\nBuilder version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor\nOther"
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

### Comparing `types-aiobotocore-internetmonitor-2.9.0/types_aiobotocore_internetmonitor/client.py` & `types-aiobotocore-internetmonitor-2.9.1/types_aiobotocore_internetmonitor/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("CloudWatchInternetMonitorClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -111,15 +110,15 @@
         MonitorName: str,
         Resources: Sequence[str] = ...,
         ClientToken: str = ...,
         Tags: Mapping[str, str] = ...,
         MaxCityNetworksToMonitor: int = ...,
         InternetMeasurementsLogDelivery: InternetMeasurementsLogDeliveryTypeDef = ...,
         TrafficPercentageToMonitor: int = ...,
-        HealthEventsConfig: HealthEventsConfigTypeDef = ...
+        HealthEventsConfig: HealthEventsConfigTypeDef = ...,
     ) -> CreateMonitorOutputTypeDef:
         """
         Creates a monitor in Amazon CloudWatch Internet Monitor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.create_monitor)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/client/#create_monitor)
         """
@@ -195,15 +194,15 @@
         self,
         *,
         MonitorName: str,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        EventStatus: HealthEventStatusType = ...
+        EventStatus: HealthEventStatusType = ...,
     ) -> ListHealthEventsOutputTypeDef:
         """
         Lists all health events for a monitor in Amazon CloudWatch Internet Monitor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.list_health_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/client/#list_health_events)
         """
@@ -231,15 +230,15 @@
     async def start_query(
         self,
         *,
         MonitorName: str,
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
         QueryType: QueryTypeType,
-        FilterParameters: Sequence[FilterParameterTypeDef] = ...
+        FilterParameters: Sequence[FilterParameterTypeDef] = ...,
     ) -> StartQueryOutputTypeDef:
         """
         Start a query to return data for a specific query type for the Amazon
         CloudWatch Internet Monitor query
         interface.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.start_query)
@@ -277,15 +276,15 @@
         ResourcesToAdd: Sequence[str] = ...,
         ResourcesToRemove: Sequence[str] = ...,
         Status: MonitorConfigStateType = ...,
         ClientToken: str = ...,
         MaxCityNetworksToMonitor: int = ...,
         InternetMeasurementsLogDelivery: InternetMeasurementsLogDeliveryTypeDef = ...,
         TrafficPercentageToMonitor: int = ...,
-        HealthEventsConfig: HealthEventsConfigTypeDef = ...
+        HealthEventsConfig: HealthEventsConfigTypeDef = ...,
     ) -> UpdateMonitorOutputTypeDef:
         """
         Updates a monitor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.update_monitor)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/client/#update_monitor)
         """
```

### Comparing `types-aiobotocore-internetmonitor-2.9.0/types_aiobotocore_internetmonitor/client.pyi` & `types-aiobotocore-internetmonitor-2.9.1/types_aiobotocore_internetmonitor/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         MonitorName: str,
         Resources: Sequence[str] = ...,
         ClientToken: str = ...,
         Tags: Mapping[str, str] = ...,
         MaxCityNetworksToMonitor: int = ...,
         InternetMeasurementsLogDelivery: InternetMeasurementsLogDeliveryTypeDef = ...,
         TrafficPercentageToMonitor: int = ...,
-        HealthEventsConfig: HealthEventsConfigTypeDef = ...
+        HealthEventsConfig: HealthEventsConfigTypeDef = ...,
     ) -> CreateMonitorOutputTypeDef:
         """
         Creates a monitor in Amazon CloudWatch Internet Monitor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.create_monitor)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/client/#create_monitor)
         """
@@ -191,15 +191,15 @@
         self,
         *,
         MonitorName: str,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        EventStatus: HealthEventStatusType = ...
+        EventStatus: HealthEventStatusType = ...,
     ) -> ListHealthEventsOutputTypeDef:
         """
         Lists all health events for a monitor in Amazon CloudWatch Internet Monitor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.list_health_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/client/#list_health_events)
         """
@@ -227,15 +227,15 @@
     async def start_query(
         self,
         *,
         MonitorName: str,
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
         QueryType: QueryTypeType,
-        FilterParameters: Sequence[FilterParameterTypeDef] = ...
+        FilterParameters: Sequence[FilterParameterTypeDef] = ...,
     ) -> StartQueryOutputTypeDef:
         """
         Start a query to return data for a specific query type for the Amazon
         CloudWatch Internet Monitor query
         interface.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.start_query)
@@ -273,15 +273,15 @@
         ResourcesToAdd: Sequence[str] = ...,
         ResourcesToRemove: Sequence[str] = ...,
         Status: MonitorConfigStateType = ...,
         ClientToken: str = ...,
         MaxCityNetworksToMonitor: int = ...,
         InternetMeasurementsLogDelivery: InternetMeasurementsLogDeliveryTypeDef = ...,
         TrafficPercentageToMonitor: int = ...,
-        HealthEventsConfig: HealthEventsConfigTypeDef = ...
+        HealthEventsConfig: HealthEventsConfigTypeDef = ...,
     ) -> UpdateMonitorOutputTypeDef:
         """
         Updates a monitor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.update_monitor)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/client/#update_monitor)
         """
```

### Comparing `types-aiobotocore-internetmonitor-2.9.0/types_aiobotocore_internetmonitor/literals.py` & `types-aiobotocore-internetmonitor-2.9.1/types_aiobotocore_internetmonitor/literals.py`

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
     "HealthEventImpactTypeType",
     "HealthEventStatusType",
     "ListHealthEventsPaginatorName",
     "ListMonitorsPaginatorName",
     "LocalHealthEventsConfigStatusType",
     "LogDeliveryStatusType",
@@ -36,15 +35,14 @@
     "CloudWatchInternetMonitorServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 HealthEventImpactTypeType = Literal[
     "AVAILABILITY", "LOCAL_AVAILABILITY", "LOCAL_PERFORMANCE", "PERFORMANCE"
 ]
 HealthEventStatusType = Literal["ACTIVE", "RESOLVED"]
 ListHealthEventsPaginatorName = Literal["list_health_events"]
 ListMonitorsPaginatorName = Literal["list_monitors"]
 LocalHealthEventsConfigStatusType = Literal["DISABLED", "ENABLED"]
```

### Comparing `types-aiobotocore-internetmonitor-2.9.0/types_aiobotocore_internetmonitor/literals.pyi` & `types-aiobotocore-internetmonitor-2.9.1/types_aiobotocore_internetmonitor/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-internetmonitor-2.9.0/types_aiobotocore_internetmonitor/paginator.py` & `types-aiobotocore-internetmonitor-2.9.1/types_aiobotocore_internetmonitor/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,14 @@
     ListMonitorsOutputTypeDef,
     PaginatorConfigTypeDef,
     TimestampTypeDef,
 )
 
 __all__ = ("ListHealthEventsPaginator", "ListMonitorsPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -58,15 +57,15 @@
     def paginate(
         self,
         *,
         MonitorName: str,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         EventStatus: HealthEventStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListHealthEventsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Paginator.ListHealthEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/paginators/#listhealtheventspaginator)
         """
```

### Comparing `types-aiobotocore-internetmonitor-2.9.0/types_aiobotocore_internetmonitor/paginator.pyi` & `types-aiobotocore-internetmonitor-2.9.1/types_aiobotocore_internetmonitor/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     def paginate(
         self,
         *,
         MonitorName: str,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         EventStatus: HealthEventStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListHealthEventsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Paginator.ListHealthEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/paginators/#listhealtheventspaginator)
         """
 
 class ListMonitorsPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-internetmonitor-2.9.0/types_aiobotocore_internetmonitor/type_defs.py` & `types-aiobotocore-internetmonitor-2.9.1/types_aiobotocore_internetmonitor/type_defs.py`

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
     "AvailabilityMeasurementTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteMonitorInputRequestTypeDef",
     "FilterParameterTypeDef",
     "GetHealthEventInputRequestTypeDef",
     "GetMonitorInputRequestTypeDef",
```

### Comparing `types-aiobotocore-internetmonitor-2.9.0/types_aiobotocore_internetmonitor/type_defs.pyi` & `types-aiobotocore-internetmonitor-2.9.1/types_aiobotocore_internetmonitor/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-internetmonitor-2.9.0/types_aiobotocore_internetmonitor.egg-info/PKG-INFO` & `types-aiobotocore-internetmonitor-2.9.1/types_aiobotocore_internetmonitor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-internetmonitor
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CloudWatchInternetMonitor 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CloudWatchInternetMonitor 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/
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
 
 <a id="types-aiobotocore-internetmonitor"></a>
 
 # types-aiobotocore-internetmonitor
 
 [![PyPI - types-aiobotocore-internetmonitor](https://img.shields.io/pypi/v/types-aiobotocore-internetmonitor.svg?color=blue)](https://pypi.org/project/types-aiobotocore-internetmonitor)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-internetmonitor.svg?color=blue)](https://pypi.org/project/types-aiobotocore-internetmonitor)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-internetmonitor)](https://pepy.tech/project/types-aiobotocore-internetmonitor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudWatchInternetMonitor 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor)
+[aiobotocore.CloudWatchInternetMonitor 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor)
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
 [types-aiobotocore-internetmonitor docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-internetmonitor-2.9.0/types_aiobotocore_internetmonitor.egg-info/SOURCES.txt` & `types-aiobotocore-internetmonitor-2.9.1/types_aiobotocore_internetmonitor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

