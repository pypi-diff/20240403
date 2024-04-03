# Comparing `tmp/types-aiobotocore-appstream-2.9.0.tar.gz` & `tmp/types-aiobotocore-appstream-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-appstream-2.9.0.tar", last modified: Wed Dec 13 19:58:36 2023, max compression
+gzip compressed data, was "types-aiobotocore-appstream-2.9.1.tar", last modified: Thu Jan 18 01:20:04 2024, max compression
```

## Comparing `types-aiobotocore-appstream-2.9.0.tar` & `types-aiobotocore-appstream-2.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:36.834077 types-aiobotocore-appstream-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:41:14.000000 types-aiobotocore-appstream-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15278 2023-12-13 19:58:36.834077 types-aiobotocore-appstream-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13707 2023-12-13 19:41:14.000000 types-aiobotocore-appstream-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:36.834077 types-aiobotocore-appstream-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2023-12-13 19:41:14.000000 types-aiobotocore-appstream-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:36.834077 types-aiobotocore-appstream-2.9.0/types_aiobotocore_appstream/
--rw-r--r--   0 runner    (1001) docker     (127)     3012 2023-12-13 19:41:14.000000 types-aiobotocore-appstream-2.9.0/types_aiobotocore_appstream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2023-12-13 19:41:14.000000 types-aiobotocore-appstream-2.9.0/types_aiobotocore_appstream/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      940 2023-12-13 19:41:14.000000 types-aiobotocore-appstream-2.9.0/types_aiobotocore_appstream/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    61167 2023-12-13 19:41:15.000000 types-aiobotocore-appstream-2.9.0/types_aiobotocore_appstream/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    61163 2023-12-13 19:41:14.000000 types-aiobotocore-appstream-2.9.0/types_aiobotocore_appstream/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    15492 2023-12-13 19:41:15.000000 types-aiobotocore-appstream-2.9.0/types_aiobotocore_appstream/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    15490 2023-12-13 19:41:15.000000 types-aiobotocore-appstream-2.9.0/types_aiobotocore_appstream/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12957 2023-12-13 19:41:15.000000 types-aiobotocore-appstream-2.9.0/types_aiobotocore_appstream/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12945 2023-12-13 19:41:15.000000 types-aiobotocore-appstream-2.9.0/types_aiobotocore_appstream/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:41:14.000000 types-aiobotocore-appstream-2.9.0/types_aiobotocore_appstream/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    64352 2023-12-13 19:41:16.000000 types-aiobotocore-appstream-2.9.0/types_aiobotocore_appstream/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    64351 2023-12-13 19:41:16.000000 types-aiobotocore-appstream-2.9.0/types_aiobotocore_appstream/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:41:14.000000 types-aiobotocore-appstream-2.9.0/types_aiobotocore_appstream/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2023-12-13 19:41:15.000000 types-aiobotocore-appstream-2.9.0/types_aiobotocore_appstream/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2023-12-13 19:41:15.000000 types-aiobotocore-appstream-2.9.0/types_aiobotocore_appstream/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:36.834077 types-aiobotocore-appstream-2.9.0/types_aiobotocore_appstream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15278 2023-12-13 19:58:36.000000 types-aiobotocore-appstream-2.9.0/types_aiobotocore_appstream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      928 2023-12-13 19:58:36.000000 types-aiobotocore-appstream-2.9.0/types_aiobotocore_appstream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:36.000000 types-aiobotocore-appstream-2.9.0/types_aiobotocore_appstream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:36.000000 types-aiobotocore-appstream-2.9.0/types_aiobotocore_appstream.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:36.000000 types-aiobotocore-appstream-2.9.0/types_aiobotocore_appstream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-12-13 19:58:36.000000 types-aiobotocore-appstream-2.9.0/types_aiobotocore_appstream.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:04.745507 types-aiobotocore-appstream-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:03:12.000000 types-aiobotocore-appstream-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15298 2024-01-18 01:20:04.745507 types-aiobotocore-appstream-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13707 2024-01-18 01:03:12.000000 types-aiobotocore-appstream-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:04.745507 types-aiobotocore-appstream-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-01-18 01:03:12.000000 types-aiobotocore-appstream-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:04.741507 types-aiobotocore-appstream-2.9.1/types_aiobotocore_appstream/
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-01-18 01:03:13.000000 types-aiobotocore-appstream-2.9.1/types_aiobotocore_appstream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-01-18 01:03:12.000000 types-aiobotocore-appstream-2.9.1/types_aiobotocore_appstream/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-01-18 01:03:13.000000 types-aiobotocore-appstream-2.9.1/types_aiobotocore_appstream/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61191 2024-01-18 01:03:14.000000 types-aiobotocore-appstream-2.9.1/types_aiobotocore_appstream/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61188 2024-01-18 01:03:13.000000 types-aiobotocore-appstream-2.9.1/types_aiobotocore_appstream/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    15490 2024-01-18 01:03:14.000000 types-aiobotocore-appstream-2.9.1/types_aiobotocore_appstream/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15490 2024-01-18 01:03:14.000000 types-aiobotocore-appstream-2.9.1/types_aiobotocore_appstream/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12960 2024-01-18 01:03:14.000000 types-aiobotocore-appstream-2.9.1/types_aiobotocore_appstream/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12949 2024-01-18 01:03:14.000000 types-aiobotocore-appstream-2.9.1/types_aiobotocore_appstream/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:03:13.000000 types-aiobotocore-appstream-2.9.1/types_aiobotocore_appstream/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    64351 2024-01-18 01:03:16.000000 types-aiobotocore-appstream-2.9.1/types_aiobotocore_appstream/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64351 2024-01-18 01:03:15.000000 types-aiobotocore-appstream-2.9.1/types_aiobotocore_appstream/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:03:12.000000 types-aiobotocore-appstream-2.9.1/types_aiobotocore_appstream/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-01-18 01:03:14.000000 types-aiobotocore-appstream-2.9.1/types_aiobotocore_appstream/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-01-18 01:03:14.000000 types-aiobotocore-appstream-2.9.1/types_aiobotocore_appstream/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:04.745507 types-aiobotocore-appstream-2.9.1/types_aiobotocore_appstream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15298 2024-01-18 01:20:04.000000 types-aiobotocore-appstream-2.9.1/types_aiobotocore_appstream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-01-18 01:20:04.000000 types-aiobotocore-appstream-2.9.1/types_aiobotocore_appstream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:04.000000 types-aiobotocore-appstream-2.9.1/types_aiobotocore_appstream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:04.000000 types-aiobotocore-appstream-2.9.1/types_aiobotocore_appstream.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:04.000000 types-aiobotocore-appstream-2.9.1/types_aiobotocore_appstream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-18 01:20:04.000000 types-aiobotocore-appstream-2.9.1/types_aiobotocore_appstream.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-appstream-2.9.0/LICENSE` & `types-aiobotocore-appstream-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-appstream-2.9.0/PKG-INFO` & `types-aiobotocore-appstream-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-appstream
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.AppStream 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.AppStream 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/
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
 
 <a id="types-aiobotocore-appstream"></a>
 
 # types-aiobotocore-appstream
 
 [![PyPI - types-aiobotocore-appstream](https://img.shields.io/pypi/v/types-aiobotocore-appstream.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appstream)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appstream.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appstream)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appstream)](https://pepy.tech/project/types-aiobotocore-appstream)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AppStream 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream)
+[aiobotocore.AppStream 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream)
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
 [types-aiobotocore-appstream docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-appstream-2.9.0/README.md` & `types-aiobotocore-appstream-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appstream.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appstream)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appstream)](https://pepy.tech/project/types-aiobotocore-appstream)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AppStream 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream)
+[aiobotocore.AppStream 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream)
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
 [types-aiobotocore-appstream docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-appstream-2.9.0/setup.py` & `types-aiobotocore-appstream-2.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-appstream",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_appstream"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.AppStream 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.AppStream 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore appstream type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_appstream": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-appstream-2.9.0/types_aiobotocore_appstream/__init__.py` & `types-aiobotocore-appstream-2.9.1/types_aiobotocore_appstream/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,14 @@
     ListAssociatedFleetsPaginator,
     ListAssociatedStacksPaginator,
 )
 from .waiter import FleetStartedWaiter, FleetStoppedWaiter
 
 Client = AppStreamClient
 
-
 __all__ = (
     "AppStreamClient",
     "Client",
     "DescribeDirectoryConfigsPaginator",
     "DescribeFleetsPaginator",
     "DescribeImageBuildersPaginator",
     "DescribeImagesPaginator",
```

### Comparing `types-aiobotocore-appstream-2.9.0/types_aiobotocore_appstream/__init__.pyi` & `types-aiobotocore-appstream-2.9.1/types_aiobotocore_appstream/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appstream-2.9.0/types_aiobotocore_appstream/__main__.py` & `types-aiobotocore-appstream-2.9.1/types_aiobotocore_appstream/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.AppStream 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.AppStream 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream\nOther"
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

### Comparing `types-aiobotocore-appstream-2.9.0/types_aiobotocore_appstream/client.py` & `types-aiobotocore-appstream-2.9.1/types_aiobotocore_appstream/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,14 @@
 from .waiter import FleetStartedWaiter, FleetStoppedWaiter
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("AppStreamClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -244,15 +243,15 @@
 
     async def copy_image(
         self,
         *,
         SourceImageName: str,
         DestinationImageName: str,
         DestinationRegion: str,
-        DestinationImageDescription: str = ...
+        DestinationImageDescription: str = ...,
     ) -> CopyImageResponseTypeDef:
         """
         Copies the image within the same region or to a new region within the same AWS
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.copy_image)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#copy_image)
@@ -264,15 +263,15 @@
         Name: str,
         SourceS3Location: S3LocationTypeDef,
         Description: str = ...,
         DisplayName: str = ...,
         SetupScriptDetails: ScriptDetailsTypeDef = ...,
         Tags: Mapping[str, str] = ...,
         PostSetupScriptDetails: ScriptDetailsTypeDef = ...,
-        PackagingType: PackagingTypeType = ...
+        PackagingType: PackagingTypeType = ...,
     ) -> CreateAppBlockResultTypeDef:
         """
         Creates an app block.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.create_app_block)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#create_app_block)
         """
@@ -285,15 +284,15 @@
         InstanceType: str,
         VpcConfig: VpcConfigTypeDef,
         Description: str = ...,
         DisplayName: str = ...,
         Tags: Mapping[str, str] = ...,
         EnableDefaultInternetAccess: bool = ...,
         IamRoleArn: str = ...,
-        AccessEndpoints: Sequence[AccessEndpointTypeDef] = ...
+        AccessEndpoints: Sequence[AccessEndpointTypeDef] = ...,
     ) -> CreateAppBlockBuilderResultTypeDef:
         """
         Creates an app block builder.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.create_app_block_builder)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#create_app_block_builder)
         """
@@ -317,30 +316,30 @@
         Platforms: Sequence[PlatformTypeType],
         InstanceFamilies: Sequence[str],
         AppBlockArn: str,
         DisplayName: str = ...,
         Description: str = ...,
         WorkingDirectory: str = ...,
         LaunchParameters: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateApplicationResultTypeDef:
         """
         Creates an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.create_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#create_application)
         """
 
     async def create_directory_config(
         self,
         *,
         DirectoryName: str,
         OrganizationalUnitDistinguishedNames: Sequence[str],
         ServiceAccountCredentials: ServiceAccountCredentialsTypeDef = ...,
-        CertificateBasedAuthProperties: CertificateBasedAuthPropertiesTypeDef = ...
+        CertificateBasedAuthProperties: CertificateBasedAuthPropertiesTypeDef = ...,
     ) -> CreateDirectoryConfigResultTypeDef:
         """
         Creates a Directory Config object in AppStream 2.0.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.create_directory_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#create_directory_config)
         """
@@ -348,15 +347,15 @@
     async def create_entitlement(
         self,
         *,
         Name: str,
         StackName: str,
         AppVisibility: AppVisibilityType,
         Attributes: Sequence[EntitlementAttributeTypeDef],
-        Description: str = ...
+        Description: str = ...,
     ) -> CreateEntitlementResultTypeDef:
         """
         Creates a new entitlement.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.create_entitlement)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#create_entitlement)
         """
@@ -381,15 +380,15 @@
         IdleDisconnectTimeoutInSeconds: int = ...,
         IamRoleArn: str = ...,
         StreamView: StreamViewType = ...,
         Platform: PlatformTypeType = ...,
         MaxConcurrentSessions: int = ...,
         UsbDeviceFilterStrings: Sequence[str] = ...,
         SessionScriptS3Location: S3LocationTypeDef = ...,
-        MaxSessionsPerInstance: int = ...
+        MaxSessionsPerInstance: int = ...,
     ) -> CreateFleetResultTypeDef:
         """
         Creates a fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.create_fleet)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#create_fleet)
         """
@@ -405,15 +404,15 @@
         DisplayName: str = ...,
         VpcConfig: VpcConfigTypeDef = ...,
         IamRoleArn: str = ...,
         EnableDefaultInternetAccess: bool = ...,
         DomainJoinInfo: DomainJoinInfoTypeDef = ...,
         AppstreamAgentVersion: str = ...,
         Tags: Mapping[str, str] = ...,
-        AccessEndpoints: Sequence[AccessEndpointTypeDef] = ...
+        AccessEndpoints: Sequence[AccessEndpointTypeDef] = ...,
     ) -> CreateImageBuilderResultTypeDef:
         """
         Creates an image builder.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.create_image_builder)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#create_image_builder)
         """
@@ -438,15 +437,15 @@
         RedirectURL: str = ...,
         FeedbackURL: str = ...,
         UserSettings: Sequence[UserSettingTypeDef] = ...,
         ApplicationSettings: ApplicationSettingsTypeDef = ...,
         Tags: Mapping[str, str] = ...,
         AccessEndpoints: Sequence[AccessEndpointTypeDef] = ...,
         EmbedHostDomains: Sequence[str] = ...,
-        StreamingExperienceSettings: StreamingExperienceSettingsTypeDef = ...
+        StreamingExperienceSettings: StreamingExperienceSettingsTypeDef = ...,
     ) -> CreateStackResultTypeDef:
         """
         Creates a stack to start streaming applications to users.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.create_stack)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#create_stack)
         """
@@ -455,15 +454,15 @@
         self,
         *,
         StackName: str,
         FleetName: str,
         UserId: str,
         ApplicationId: str = ...,
         Validity: int = ...,
-        SessionContext: str = ...
+        SessionContext: str = ...,
     ) -> CreateStreamingURLResultTypeDef:
         """
         Creates a temporary URL to start an AppStream 2.0 streaming session for the
         specified
         user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.create_streaming_url)
@@ -474,15 +473,15 @@
         self,
         *,
         existingImageName: str,
         newImageName: str,
         newImageDescription: str = ...,
         newImageDisplayName: str = ...,
         newImageTags: Mapping[str, str] = ...,
-        dryRun: bool = ...
+        dryRun: bool = ...,
     ) -> CreateUpdatedImageResultTypeDef:
         """
         Creates a new image with the latest Windows operating system updates, driver
         updates, and AppStream 2.0 agent
         software.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.create_updated_image)
@@ -500,15 +499,15 @@
     async def create_user(
         self,
         *,
         UserName: str,
         AuthenticationType: AuthenticationTypeType,
         MessageAction: MessageActionType = ...,
         FirstName: str = ...,
-        LastName: str = ...
+        LastName: str = ...,
     ) -> Dict[str, Any]:
         """
         Creates a new user in the user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.create_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#create_user)
         """
@@ -613,15 +612,15 @@
 
     async def describe_app_block_builder_app_block_associations(
         self,
         *,
         AppBlockArn: str = ...,
         AppBlockBuilderName: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef:
         """
         Retrieves a list that describes one or more app block builder associations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.describe_app_block_builder_app_block_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#describe_app_block_builder_app_block_associations)
         """
@@ -648,15 +647,15 @@
 
     async def describe_application_fleet_associations(
         self,
         *,
         FleetName: str = ...,
         ApplicationArn: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeApplicationFleetAssociationsResultTypeDef:
         """
         Retrieves a list that describes one or more application fleet associations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.describe_application_fleet_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#describe_application_fleet_associations)
         """
@@ -719,15 +718,15 @@
 
     async def describe_image_permissions(
         self,
         *,
         Name: str,
         MaxResults: int = ...,
         SharedAwsAccountIds: Sequence[str] = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeImagePermissionsResultTypeDef:
         """
         Retrieves a list that describes the permissions for shared AWS account IDs on a
         private image that you
         own.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.describe_image_permissions)
@@ -737,15 +736,15 @@
     async def describe_images(
         self,
         *,
         Names: Sequence[str] = ...,
         Arns: Sequence[str] = ...,
         Type: VisibilityTypeType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeImagesResultTypeDef:
         """
         Retrieves a list that describes one or more specified images, if the image
         names or image ARNs are
         provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.describe_images)
@@ -757,15 +756,15 @@
         *,
         StackName: str,
         FleetName: str,
         UserId: str = ...,
         NextToken: str = ...,
         Limit: int = ...,
         AuthenticationType: AuthenticationTypeType = ...,
-        InstanceId: str = ...
+        InstanceId: str = ...,
     ) -> DescribeSessionsResultTypeDef:
         """
         Retrieves a list that describes the streaming sessions for a specified stack
         and
         fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.describe_sessions)
@@ -797,29 +796,29 @@
     async def describe_user_stack_associations(
         self,
         *,
         StackName: str = ...,
         UserName: str = ...,
         AuthenticationType: AuthenticationTypeType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeUserStackAssociationsResultTypeDef:
         """
         Retrieves a list that describes the UserStackAssociation objects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.describe_user_stack_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#describe_user_stack_associations)
         """
 
     async def describe_users(
         self,
         *,
         AuthenticationType: AuthenticationTypeType,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeUsersResultTypeDef:
         """
         Retrieves a list that describes one or more specified users in the user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.describe_users)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#describe_users)
         """
@@ -1019,15 +1018,15 @@
         DisplayName: str = ...,
         Platform: PlatformTypeType = ...,
         InstanceType: str = ...,
         VpcConfig: VpcConfigTypeDef = ...,
         EnableDefaultInternetAccess: bool = ...,
         IamRoleArn: str = ...,
         AccessEndpoints: Sequence[AccessEndpointTypeDef] = ...,
-        AttributesToDelete: Sequence[AppBlockBuilderAttributeType] = ...
+        AttributesToDelete: Sequence[AppBlockBuilderAttributeType] = ...,
     ) -> UpdateAppBlockBuilderResultTypeDef:
         """
         Updates an app block builder.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.update_app_block_builder)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#update_app_block_builder)
         """
@@ -1039,30 +1038,30 @@
         DisplayName: str = ...,
         Description: str = ...,
         IconS3Location: S3LocationTypeDef = ...,
         LaunchPath: str = ...,
         WorkingDirectory: str = ...,
         LaunchParameters: str = ...,
         AppBlockArn: str = ...,
-        AttributesToDelete: Sequence[ApplicationAttributeType] = ...
+        AttributesToDelete: Sequence[ApplicationAttributeType] = ...,
     ) -> UpdateApplicationResultTypeDef:
         """
         Updates the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.update_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#update_application)
         """
 
     async def update_directory_config(
         self,
         *,
         DirectoryName: str,
         OrganizationalUnitDistinguishedNames: Sequence[str] = ...,
         ServiceAccountCredentials: ServiceAccountCredentialsTypeDef = ...,
-        CertificateBasedAuthProperties: CertificateBasedAuthPropertiesTypeDef = ...
+        CertificateBasedAuthProperties: CertificateBasedAuthPropertiesTypeDef = ...,
     ) -> UpdateDirectoryConfigResultTypeDef:
         """
         Updates the specified Directory Config object in AppStream 2.0.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.update_directory_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#update_directory_config)
         """
@@ -1070,15 +1069,15 @@
     async def update_entitlement(
         self,
         *,
         Name: str,
         StackName: str,
         Description: str = ...,
         AppVisibility: AppVisibilityType = ...,
-        Attributes: Sequence[EntitlementAttributeTypeDef] = ...
+        Attributes: Sequence[EntitlementAttributeTypeDef] = ...,
     ) -> UpdateEntitlementResultTypeDef:
         """
         Updates the specified entitlement.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.update_entitlement)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#update_entitlement)
         """
@@ -1103,15 +1102,15 @@
         AttributesToDelete: Sequence[FleetAttributeType] = ...,
         IamRoleArn: str = ...,
         StreamView: StreamViewType = ...,
         Platform: PlatformTypeType = ...,
         MaxConcurrentSessions: int = ...,
         UsbDeviceFilterStrings: Sequence[str] = ...,
         SessionScriptS3Location: S3LocationTypeDef = ...,
-        MaxSessionsPerInstance: int = ...
+        MaxSessionsPerInstance: int = ...,
     ) -> UpdateFleetResultTypeDef:
         """
         Updates the specified fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.update_fleet)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#update_fleet)
         """
@@ -1137,15 +1136,15 @@
         RedirectURL: str = ...,
         FeedbackURL: str = ...,
         AttributesToDelete: Sequence[StackAttributeType] = ...,
         UserSettings: Sequence[UserSettingTypeDef] = ...,
         ApplicationSettings: ApplicationSettingsTypeDef = ...,
         AccessEndpoints: Sequence[AccessEndpointTypeDef] = ...,
         EmbedHostDomains: Sequence[str] = ...,
-        StreamingExperienceSettings: StreamingExperienceSettingsTypeDef = ...
+        StreamingExperienceSettings: StreamingExperienceSettingsTypeDef = ...,
     ) -> UpdateStackResultTypeDef:
         """
         Updates the specified fields for the specified stack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.update_stack)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#update_stack)
         """
```

### Comparing `types-aiobotocore-appstream-2.9.0/types_aiobotocore_appstream/client.pyi` & `types-aiobotocore-appstream-2.9.1/types_aiobotocore_appstream/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -240,15 +240,15 @@
 
     async def copy_image(
         self,
         *,
         SourceImageName: str,
         DestinationImageName: str,
         DestinationRegion: str,
-        DestinationImageDescription: str = ...
+        DestinationImageDescription: str = ...,
     ) -> CopyImageResponseTypeDef:
         """
         Copies the image within the same region or to a new region within the same AWS
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.copy_image)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#copy_image)
@@ -260,15 +260,15 @@
         Name: str,
         SourceS3Location: S3LocationTypeDef,
         Description: str = ...,
         DisplayName: str = ...,
         SetupScriptDetails: ScriptDetailsTypeDef = ...,
         Tags: Mapping[str, str] = ...,
         PostSetupScriptDetails: ScriptDetailsTypeDef = ...,
-        PackagingType: PackagingTypeType = ...
+        PackagingType: PackagingTypeType = ...,
     ) -> CreateAppBlockResultTypeDef:
         """
         Creates an app block.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.create_app_block)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#create_app_block)
         """
@@ -281,15 +281,15 @@
         InstanceType: str,
         VpcConfig: VpcConfigTypeDef,
         Description: str = ...,
         DisplayName: str = ...,
         Tags: Mapping[str, str] = ...,
         EnableDefaultInternetAccess: bool = ...,
         IamRoleArn: str = ...,
-        AccessEndpoints: Sequence[AccessEndpointTypeDef] = ...
+        AccessEndpoints: Sequence[AccessEndpointTypeDef] = ...,
     ) -> CreateAppBlockBuilderResultTypeDef:
         """
         Creates an app block builder.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.create_app_block_builder)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#create_app_block_builder)
         """
@@ -313,30 +313,30 @@
         Platforms: Sequence[PlatformTypeType],
         InstanceFamilies: Sequence[str],
         AppBlockArn: str,
         DisplayName: str = ...,
         Description: str = ...,
         WorkingDirectory: str = ...,
         LaunchParameters: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateApplicationResultTypeDef:
         """
         Creates an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.create_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#create_application)
         """
 
     async def create_directory_config(
         self,
         *,
         DirectoryName: str,
         OrganizationalUnitDistinguishedNames: Sequence[str],
         ServiceAccountCredentials: ServiceAccountCredentialsTypeDef = ...,
-        CertificateBasedAuthProperties: CertificateBasedAuthPropertiesTypeDef = ...
+        CertificateBasedAuthProperties: CertificateBasedAuthPropertiesTypeDef = ...,
     ) -> CreateDirectoryConfigResultTypeDef:
         """
         Creates a Directory Config object in AppStream 2.0.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.create_directory_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#create_directory_config)
         """
@@ -344,15 +344,15 @@
     async def create_entitlement(
         self,
         *,
         Name: str,
         StackName: str,
         AppVisibility: AppVisibilityType,
         Attributes: Sequence[EntitlementAttributeTypeDef],
-        Description: str = ...
+        Description: str = ...,
     ) -> CreateEntitlementResultTypeDef:
         """
         Creates a new entitlement.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.create_entitlement)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#create_entitlement)
         """
@@ -377,15 +377,15 @@
         IdleDisconnectTimeoutInSeconds: int = ...,
         IamRoleArn: str = ...,
         StreamView: StreamViewType = ...,
         Platform: PlatformTypeType = ...,
         MaxConcurrentSessions: int = ...,
         UsbDeviceFilterStrings: Sequence[str] = ...,
         SessionScriptS3Location: S3LocationTypeDef = ...,
-        MaxSessionsPerInstance: int = ...
+        MaxSessionsPerInstance: int = ...,
     ) -> CreateFleetResultTypeDef:
         """
         Creates a fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.create_fleet)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#create_fleet)
         """
@@ -401,15 +401,15 @@
         DisplayName: str = ...,
         VpcConfig: VpcConfigTypeDef = ...,
         IamRoleArn: str = ...,
         EnableDefaultInternetAccess: bool = ...,
         DomainJoinInfo: DomainJoinInfoTypeDef = ...,
         AppstreamAgentVersion: str = ...,
         Tags: Mapping[str, str] = ...,
-        AccessEndpoints: Sequence[AccessEndpointTypeDef] = ...
+        AccessEndpoints: Sequence[AccessEndpointTypeDef] = ...,
     ) -> CreateImageBuilderResultTypeDef:
         """
         Creates an image builder.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.create_image_builder)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#create_image_builder)
         """
@@ -434,15 +434,15 @@
         RedirectURL: str = ...,
         FeedbackURL: str = ...,
         UserSettings: Sequence[UserSettingTypeDef] = ...,
         ApplicationSettings: ApplicationSettingsTypeDef = ...,
         Tags: Mapping[str, str] = ...,
         AccessEndpoints: Sequence[AccessEndpointTypeDef] = ...,
         EmbedHostDomains: Sequence[str] = ...,
-        StreamingExperienceSettings: StreamingExperienceSettingsTypeDef = ...
+        StreamingExperienceSettings: StreamingExperienceSettingsTypeDef = ...,
     ) -> CreateStackResultTypeDef:
         """
         Creates a stack to start streaming applications to users.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.create_stack)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#create_stack)
         """
@@ -451,15 +451,15 @@
         self,
         *,
         StackName: str,
         FleetName: str,
         UserId: str,
         ApplicationId: str = ...,
         Validity: int = ...,
-        SessionContext: str = ...
+        SessionContext: str = ...,
     ) -> CreateStreamingURLResultTypeDef:
         """
         Creates a temporary URL to start an AppStream 2.0 streaming session for the
         specified
         user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.create_streaming_url)
@@ -470,15 +470,15 @@
         self,
         *,
         existingImageName: str,
         newImageName: str,
         newImageDescription: str = ...,
         newImageDisplayName: str = ...,
         newImageTags: Mapping[str, str] = ...,
-        dryRun: bool = ...
+        dryRun: bool = ...,
     ) -> CreateUpdatedImageResultTypeDef:
         """
         Creates a new image with the latest Windows operating system updates, driver
         updates, and AppStream 2.0 agent
         software.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.create_updated_image)
@@ -496,15 +496,15 @@
     async def create_user(
         self,
         *,
         UserName: str,
         AuthenticationType: AuthenticationTypeType,
         MessageAction: MessageActionType = ...,
         FirstName: str = ...,
-        LastName: str = ...
+        LastName: str = ...,
     ) -> Dict[str, Any]:
         """
         Creates a new user in the user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.create_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#create_user)
         """
@@ -609,15 +609,15 @@
 
     async def describe_app_block_builder_app_block_associations(
         self,
         *,
         AppBlockArn: str = ...,
         AppBlockBuilderName: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef:
         """
         Retrieves a list that describes one or more app block builder associations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.describe_app_block_builder_app_block_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#describe_app_block_builder_app_block_associations)
         """
@@ -644,15 +644,15 @@
 
     async def describe_application_fleet_associations(
         self,
         *,
         FleetName: str = ...,
         ApplicationArn: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeApplicationFleetAssociationsResultTypeDef:
         """
         Retrieves a list that describes one or more application fleet associations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.describe_application_fleet_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#describe_application_fleet_associations)
         """
@@ -715,15 +715,15 @@
 
     async def describe_image_permissions(
         self,
         *,
         Name: str,
         MaxResults: int = ...,
         SharedAwsAccountIds: Sequence[str] = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeImagePermissionsResultTypeDef:
         """
         Retrieves a list that describes the permissions for shared AWS account IDs on a
         private image that you
         own.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.describe_image_permissions)
@@ -733,15 +733,15 @@
     async def describe_images(
         self,
         *,
         Names: Sequence[str] = ...,
         Arns: Sequence[str] = ...,
         Type: VisibilityTypeType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeImagesResultTypeDef:
         """
         Retrieves a list that describes one or more specified images, if the image
         names or image ARNs are
         provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.describe_images)
@@ -753,15 +753,15 @@
         *,
         StackName: str,
         FleetName: str,
         UserId: str = ...,
         NextToken: str = ...,
         Limit: int = ...,
         AuthenticationType: AuthenticationTypeType = ...,
-        InstanceId: str = ...
+        InstanceId: str = ...,
     ) -> DescribeSessionsResultTypeDef:
         """
         Retrieves a list that describes the streaming sessions for a specified stack
         and
         fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.describe_sessions)
@@ -793,29 +793,29 @@
     async def describe_user_stack_associations(
         self,
         *,
         StackName: str = ...,
         UserName: str = ...,
         AuthenticationType: AuthenticationTypeType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeUserStackAssociationsResultTypeDef:
         """
         Retrieves a list that describes the UserStackAssociation objects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.describe_user_stack_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#describe_user_stack_associations)
         """
 
     async def describe_users(
         self,
         *,
         AuthenticationType: AuthenticationTypeType,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeUsersResultTypeDef:
         """
         Retrieves a list that describes one or more specified users in the user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.describe_users)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#describe_users)
         """
@@ -1015,15 +1015,15 @@
         DisplayName: str = ...,
         Platform: PlatformTypeType = ...,
         InstanceType: str = ...,
         VpcConfig: VpcConfigTypeDef = ...,
         EnableDefaultInternetAccess: bool = ...,
         IamRoleArn: str = ...,
         AccessEndpoints: Sequence[AccessEndpointTypeDef] = ...,
-        AttributesToDelete: Sequence[AppBlockBuilderAttributeType] = ...
+        AttributesToDelete: Sequence[AppBlockBuilderAttributeType] = ...,
     ) -> UpdateAppBlockBuilderResultTypeDef:
         """
         Updates an app block builder.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.update_app_block_builder)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#update_app_block_builder)
         """
@@ -1035,30 +1035,30 @@
         DisplayName: str = ...,
         Description: str = ...,
         IconS3Location: S3LocationTypeDef = ...,
         LaunchPath: str = ...,
         WorkingDirectory: str = ...,
         LaunchParameters: str = ...,
         AppBlockArn: str = ...,
-        AttributesToDelete: Sequence[ApplicationAttributeType] = ...
+        AttributesToDelete: Sequence[ApplicationAttributeType] = ...,
     ) -> UpdateApplicationResultTypeDef:
         """
         Updates the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.update_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#update_application)
         """
 
     async def update_directory_config(
         self,
         *,
         DirectoryName: str,
         OrganizationalUnitDistinguishedNames: Sequence[str] = ...,
         ServiceAccountCredentials: ServiceAccountCredentialsTypeDef = ...,
-        CertificateBasedAuthProperties: CertificateBasedAuthPropertiesTypeDef = ...
+        CertificateBasedAuthProperties: CertificateBasedAuthPropertiesTypeDef = ...,
     ) -> UpdateDirectoryConfigResultTypeDef:
         """
         Updates the specified Directory Config object in AppStream 2.0.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.update_directory_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#update_directory_config)
         """
@@ -1066,15 +1066,15 @@
     async def update_entitlement(
         self,
         *,
         Name: str,
         StackName: str,
         Description: str = ...,
         AppVisibility: AppVisibilityType = ...,
-        Attributes: Sequence[EntitlementAttributeTypeDef] = ...
+        Attributes: Sequence[EntitlementAttributeTypeDef] = ...,
     ) -> UpdateEntitlementResultTypeDef:
         """
         Updates the specified entitlement.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.update_entitlement)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#update_entitlement)
         """
@@ -1099,15 +1099,15 @@
         AttributesToDelete: Sequence[FleetAttributeType] = ...,
         IamRoleArn: str = ...,
         StreamView: StreamViewType = ...,
         Platform: PlatformTypeType = ...,
         MaxConcurrentSessions: int = ...,
         UsbDeviceFilterStrings: Sequence[str] = ...,
         SessionScriptS3Location: S3LocationTypeDef = ...,
-        MaxSessionsPerInstance: int = ...
+        MaxSessionsPerInstance: int = ...,
     ) -> UpdateFleetResultTypeDef:
         """
         Updates the specified fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.update_fleet)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#update_fleet)
         """
@@ -1133,15 +1133,15 @@
         RedirectURL: str = ...,
         FeedbackURL: str = ...,
         AttributesToDelete: Sequence[StackAttributeType] = ...,
         UserSettings: Sequence[UserSettingTypeDef] = ...,
         ApplicationSettings: ApplicationSettingsTypeDef = ...,
         AccessEndpoints: Sequence[AccessEndpointTypeDef] = ...,
         EmbedHostDomains: Sequence[str] = ...,
-        StreamingExperienceSettings: StreamingExperienceSettingsTypeDef = ...
+        StreamingExperienceSettings: StreamingExperienceSettingsTypeDef = ...,
     ) -> UpdateStackResultTypeDef:
         """
         Updates the specified fields for the specified stack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.update_stack)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#update_stack)
         """
```

### Comparing `types-aiobotocore-appstream-2.9.0/types_aiobotocore_appstream/literals.py` & `types-aiobotocore-appstream-2.9.1/types_aiobotocore_appstream/literals.py`

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
     "AccessEndpointTypeType",
     "ActionType",
     "AppBlockBuilderAttributeType",
     "AppBlockBuilderPlatformTypeType",
     "AppBlockBuilderStateChangeReasonCodeType",
     "AppBlockBuilderStateType",
@@ -71,15 +70,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 AccessEndpointTypeType = Literal["STREAMING"]
 ActionType = Literal[
     "CLIPBOARD_COPY_FROM_LOCAL_DEVICE",
     "CLIPBOARD_COPY_TO_LOCAL_DEVICE",
     "DOMAIN_PASSWORD_SIGNIN",
     "DOMAIN_SMART_CARD_SIGNIN",
     "FILE_DOWNLOAD",
```

### Comparing `types-aiobotocore-appstream-2.9.0/types_aiobotocore_appstream/literals.pyi` & `types-aiobotocore-appstream-2.9.1/types_aiobotocore_appstream/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appstream-2.9.0/types_aiobotocore_appstream/paginator.py` & `types-aiobotocore-appstream-2.9.1/types_aiobotocore_appstream/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,14 @@
     "DescribeStacksPaginator",
     "DescribeUserStackAssociationsPaginator",
     "DescribeUsersPaginator",
     "ListAssociatedFleetsPaginator",
     "ListAssociatedStacksPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -136,15 +135,15 @@
 
     def paginate(
         self,
         *,
         Names: Sequence[str] = ...,
         Arns: Sequence[str] = ...,
         Type: VisibilityTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeImagesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeImages.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/paginators/#describeimagespaginator)
         """
 
 
@@ -158,15 +157,15 @@
         self,
         *,
         StackName: str,
         FleetName: str,
         UserId: str = ...,
         AuthenticationType: AuthenticationTypeType = ...,
         InstanceId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeSessionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeSessions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/paginators/#describesessionspaginator)
         """
 
 
@@ -193,15 +192,15 @@
 
     def paginate(
         self,
         *,
         StackName: str = ...,
         UserName: str = ...,
         AuthenticationType: AuthenticationTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeUserStackAssociationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeUserStackAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/paginators/#describeuserstackassociationspaginator)
         """
 
 
@@ -211,15 +210,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/paginators/#describeuserspaginator)
     """
 
     def paginate(
         self,
         *,
         AuthenticationType: AuthenticationTypeType,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeUsersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeUsers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/paginators/#describeuserspaginator)
         """
```

### Comparing `types-aiobotocore-appstream-2.9.0/types_aiobotocore_appstream/paginator.pyi` & `types-aiobotocore-appstream-2.9.1/types_aiobotocore_appstream/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -130,15 +130,15 @@
 
     def paginate(
         self,
         *,
         Names: Sequence[str] = ...,
         Arns: Sequence[str] = ...,
         Type: VisibilityTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeImagesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeImages.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/paginators/#describeimagespaginator)
         """
 
 class DescribeSessionsPaginator(AioPaginator):
@@ -151,15 +151,15 @@
         self,
         *,
         StackName: str,
         FleetName: str,
         UserId: str = ...,
         AuthenticationType: AuthenticationTypeType = ...,
         InstanceId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeSessionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeSessions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/paginators/#describesessionspaginator)
         """
 
 class DescribeStacksPaginator(AioPaginator):
@@ -184,15 +184,15 @@
 
     def paginate(
         self,
         *,
         StackName: str = ...,
         UserName: str = ...,
         AuthenticationType: AuthenticationTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeUserStackAssociationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeUserStackAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/paginators/#describeuserstackassociationspaginator)
         """
 
 class DescribeUsersPaginator(AioPaginator):
@@ -201,15 +201,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/paginators/#describeuserspaginator)
     """
 
     def paginate(
         self,
         *,
         AuthenticationType: AuthenticationTypeType,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeUsersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeUsers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/paginators/#describeuserspaginator)
         """
 
 class ListAssociatedFleetsPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-appstream-2.9.0/types_aiobotocore_appstream/type_defs.py` & `types-aiobotocore-appstream-2.9.1/types_aiobotocore_appstream/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccessEndpointTypeDef",
     "AppBlockBuilderAppBlockAssociationTypeDef",
     "AppBlockBuilderStateChangeReasonTypeDef",
     "ResourceErrorTypeDef",
     "VpcConfigTypeDef",
     "ErrorDetailsTypeDef",
```

### Comparing `types-aiobotocore-appstream-2.9.0/types_aiobotocore_appstream/type_defs.pyi` & `types-aiobotocore-appstream-2.9.1/types_aiobotocore_appstream/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appstream-2.9.0/types_aiobotocore_appstream/waiter.py` & `types-aiobotocore-appstream-2.9.1/types_aiobotocore_appstream/waiter.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     """
 
     async def wait(
         self,
         *,
         Names: Sequence[str] = ...,
         NextToken: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Waiter.FleetStarted.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/waiters/#fleetstartedwaiter)
         """
 
 
@@ -58,13 +58,13 @@
     """
 
     async def wait(
         self,
         *,
         Names: Sequence[str] = ...,
         NextToken: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Waiter.FleetStopped.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/waiters/#fleetstoppedwaiter)
         """
```

### Comparing `types-aiobotocore-appstream-2.9.0/types_aiobotocore_appstream/waiter.pyi` & `types-aiobotocore-appstream-2.9.1/types_aiobotocore_appstream/waiter.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     """
 
     async def wait(
         self,
         *,
         Names: Sequence[str] = ...,
         NextToken: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Waiter.FleetStarted.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/waiters/#fleetstartedwaiter)
         """
 
 class FleetStoppedWaiter(AIOWaiter):
@@ -56,13 +56,13 @@
     """
 
     async def wait(
         self,
         *,
         Names: Sequence[str] = ...,
         NextToken: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Waiter.FleetStopped.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/waiters/#fleetstoppedwaiter)
         """
```

### Comparing `types-aiobotocore-appstream-2.9.0/types_aiobotocore_appstream.egg-info/PKG-INFO` & `types-aiobotocore-appstream-2.9.1/types_aiobotocore_appstream.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-appstream
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.AppStream 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.AppStream 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/
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
 
 <a id="types-aiobotocore-appstream"></a>
 
 # types-aiobotocore-appstream
 
 [![PyPI - types-aiobotocore-appstream](https://img.shields.io/pypi/v/types-aiobotocore-appstream.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appstream)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appstream.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appstream)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appstream)](https://pepy.tech/project/types-aiobotocore-appstream)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AppStream 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream)
+[aiobotocore.AppStream 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream)
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
 [types-aiobotocore-appstream docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-appstream-2.9.0/types_aiobotocore_appstream.egg-info/SOURCES.txt` & `types-aiobotocore-appstream-2.9.1/types_aiobotocore_appstream.egg-info/SOURCES.txt`

 * *Files identical despite different names*

