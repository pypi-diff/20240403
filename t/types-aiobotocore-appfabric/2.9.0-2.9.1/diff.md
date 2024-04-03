# Comparing `tmp/types-aiobotocore-appfabric-2.9.0.tar.gz` & `tmp/types-aiobotocore-appfabric-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-appfabric-2.9.0.tar", last modified: Wed Dec 13 19:58:33 2023, max compression
+gzip compressed data, was "types-aiobotocore-appfabric-2.9.1.tar", last modified: Thu Jan 18 01:20:02 2024, max compression
```

## Comparing `types-aiobotocore-appfabric-2.9.0.tar` & `types-aiobotocore-appfabric-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:33.866102 types-aiobotocore-appfabric-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:40:59.000000 types-aiobotocore-appfabric-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13573 2023-12-13 19:58:33.866102 types-aiobotocore-appfabric-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12002 2023-12-13 19:40:59.000000 types-aiobotocore-appfabric-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:33.866102 types-aiobotocore-appfabric-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2023-12-13 19:40:59.000000 types-aiobotocore-appfabric-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:33.866102 types-aiobotocore-appfabric-2.9.0/types_aiobotocore_appfabric/
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2023-12-13 19:40:59.000000 types-aiobotocore-appfabric-2.9.0/types_aiobotocore_appfabric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2023-12-13 19:40:59.000000 types-aiobotocore-appfabric-2.9.0/types_aiobotocore_appfabric/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      940 2023-12-13 19:40:59.000000 types-aiobotocore-appfabric-2.9.0/types_aiobotocore_appfabric/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23023 2023-12-13 19:41:00.000000 types-aiobotocore-appfabric-2.9.0/types_aiobotocore_appfabric/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    23019 2023-12-13 19:41:00.000000 types-aiobotocore-appfabric-2.9.0/types_aiobotocore_appfabric/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9434 2023-12-13 19:41:00.000000 types-aiobotocore-appfabric-2.9.0/types_aiobotocore_appfabric/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9432 2023-12-13 19:41:00.000000 types-aiobotocore-appfabric-2.9.0/types_aiobotocore_appfabric/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5593 2023-12-13 19:41:00.000000 types-aiobotocore-appfabric-2.9.0/types_aiobotocore_appfabric/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5587 2023-12-13 19:41:00.000000 types-aiobotocore-appfabric-2.9.0/types_aiobotocore_appfabric/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:40:59.000000 types-aiobotocore-appfabric-2.9.0/types_aiobotocore_appfabric/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    20316 2023-12-13 19:41:00.000000 types-aiobotocore-appfabric-2.9.0/types_aiobotocore_appfabric/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    20315 2023-12-13 19:41:00.000000 types-aiobotocore-appfabric-2.9.0/types_aiobotocore_appfabric/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:40:59.000000 types-aiobotocore-appfabric-2.9.0/types_aiobotocore_appfabric/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:33.866102 types-aiobotocore-appfabric-2.9.0/types_aiobotocore_appfabric.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13573 2023-12-13 19:58:33.000000 types-aiobotocore-appfabric-2.9.0/types_aiobotocore_appfabric.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      851 2023-12-13 19:58:33.000000 types-aiobotocore-appfabric-2.9.0/types_aiobotocore_appfabric.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:33.000000 types-aiobotocore-appfabric-2.9.0/types_aiobotocore_appfabric.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:33.000000 types-aiobotocore-appfabric-2.9.0/types_aiobotocore_appfabric.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:33.000000 types-aiobotocore-appfabric-2.9.0/types_aiobotocore_appfabric.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-12-13 19:58:33.000000 types-aiobotocore-appfabric-2.9.0/types_aiobotocore_appfabric.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:02.021519 types-aiobotocore-appfabric-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:02:59.000000 types-aiobotocore-appfabric-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13593 2024-01-18 01:20:02.021519 types-aiobotocore-appfabric-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12002 2024-01-18 01:02:59.000000 types-aiobotocore-appfabric-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:02.021519 types-aiobotocore-appfabric-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-01-18 01:02:58.000000 types-aiobotocore-appfabric-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:02.017519 types-aiobotocore-appfabric-2.9.1/types_aiobotocore_appfabric/
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-01-18 01:02:59.000000 types-aiobotocore-appfabric-2.9.1/types_aiobotocore_appfabric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-01-18 01:02:59.000000 types-aiobotocore-appfabric-2.9.1/types_aiobotocore_appfabric/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-01-18 01:02:59.000000 types-aiobotocore-appfabric-2.9.1/types_aiobotocore_appfabric/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23032 2024-01-18 01:02:59.000000 types-aiobotocore-appfabric-2.9.1/types_aiobotocore_appfabric/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23029 2024-01-18 01:02:59.000000 types-aiobotocore-appfabric-2.9.1/types_aiobotocore_appfabric/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9432 2024-01-18 01:02:59.000000 types-aiobotocore-appfabric-2.9.1/types_aiobotocore_appfabric/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9432 2024-01-18 01:02:59.000000 types-aiobotocore-appfabric-2.9.1/types_aiobotocore_appfabric/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5593 2024-01-18 01:02:59.000000 types-aiobotocore-appfabric-2.9.1/types_aiobotocore_appfabric/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-01-18 01:02:59.000000 types-aiobotocore-appfabric-2.9.1/types_aiobotocore_appfabric/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:02:59.000000 types-aiobotocore-appfabric-2.9.1/types_aiobotocore_appfabric/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    20315 2024-01-18 01:02:59.000000 types-aiobotocore-appfabric-2.9.1/types_aiobotocore_appfabric/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20315 2024-01-18 01:02:59.000000 types-aiobotocore-appfabric-2.9.1/types_aiobotocore_appfabric/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:02:59.000000 types-aiobotocore-appfabric-2.9.1/types_aiobotocore_appfabric/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:02.021519 types-aiobotocore-appfabric-2.9.1/types_aiobotocore_appfabric.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13593 2024-01-18 01:20:01.000000 types-aiobotocore-appfabric-2.9.1/types_aiobotocore_appfabric.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-01-18 01:20:01.000000 types-aiobotocore-appfabric-2.9.1/types_aiobotocore_appfabric.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:01.000000 types-aiobotocore-appfabric-2.9.1/types_aiobotocore_appfabric.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:01.000000 types-aiobotocore-appfabric-2.9.1/types_aiobotocore_appfabric.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:01.000000 types-aiobotocore-appfabric-2.9.1/types_aiobotocore_appfabric.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-18 01:20:01.000000 types-aiobotocore-appfabric-2.9.1/types_aiobotocore_appfabric.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-appfabric-2.9.0/LICENSE` & `types-aiobotocore-appfabric-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-appfabric-2.9.0/PKG-INFO` & `types-aiobotocore-appfabric-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-appfabric
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.AppFabric 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.AppFabric 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appfabric/
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
 
 <a id="types-aiobotocore-appfabric"></a>
 
 # types-aiobotocore-appfabric
 
 [![PyPI - types-aiobotocore-appfabric](https://img.shields.io/pypi/v/types-aiobotocore-appfabric.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appfabric)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appfabric.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appfabric)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appfabric/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appfabric)](https://pepy.tech/project/types-aiobotocore-appfabric)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AppFabric 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric)
+[aiobotocore.AppFabric 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric)
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
 [types-aiobotocore-appfabric docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appfabric/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-appfabric-2.9.0/README.md` & `types-aiobotocore-appfabric-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appfabric.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appfabric)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appfabric/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appfabric)](https://pepy.tech/project/types-aiobotocore-appfabric)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AppFabric 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric)
+[aiobotocore.AppFabric 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric)
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
 [types-aiobotocore-appfabric docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appfabric/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-appfabric-2.9.0/setup.py` & `types-aiobotocore-appfabric-2.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-appfabric",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_appfabric"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.AppFabric 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.AppFabric 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore appfabric type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_appfabric": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appfabric/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-appfabric-2.9.0/types_aiobotocore_appfabric/__init__.py` & `types-aiobotocore-appfabric-2.9.1/types_aiobotocore_appfabric/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     ListAppBundlesPaginator,
     ListIngestionDestinationsPaginator,
     ListIngestionsPaginator,
 )
 
 Client = AppFabricClient
 
-
 __all__ = (
     "AppFabricClient",
     "Client",
     "ListAppAuthorizationsPaginator",
     "ListAppBundlesPaginator",
     "ListIngestionDestinationsPaginator",
     "ListIngestionsPaginator",
```

### Comparing `types-aiobotocore-appfabric-2.9.0/types_aiobotocore_appfabric/__init__.pyi` & `types-aiobotocore-appfabric-2.9.1/types_aiobotocore_appfabric/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appfabric-2.9.0/types_aiobotocore_appfabric/__main__.py` & `types-aiobotocore-appfabric-2.9.1/types_aiobotocore_appfabric/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.AppFabric 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.AppFabric 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appfabric//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric\nOther"
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

### Comparing `types-aiobotocore-appfabric-2.9.0/types_aiobotocore_appfabric/client.py` & `types-aiobotocore-appfabric-2.9.1/types_aiobotocore_appfabric/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("AppFabricClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -127,15 +126,15 @@
         """
 
     async def connect_app_authorization(
         self,
         *,
         appBundleIdentifier: str,
         appAuthorizationIdentifier: str,
-        authRequest: AuthRequestTypeDef = ...
+        authRequest: AuthRequestTypeDef = ...,
     ) -> ConnectAppAuthorizationResponseTypeDef:
         """
         Establishes a connection between Amazon Web Services AppFabric and an
         application, which allows AppFabric to call the APIs of the
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Client.connect_app_authorization)
@@ -147,15 +146,15 @@
         *,
         appBundleIdentifier: str,
         app: str,
         credential: CredentialTypeDef,
         tenant: TenantTypeDef,
         authType: AuthTypeType,
         clientToken: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateAppAuthorizationResponseTypeDef:
         """
         Creates an app authorization within an app bundle, which allows AppFabric to
         connect to an
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Client.create_app_authorization)
@@ -163,15 +162,15 @@
         """
 
     async def create_app_bundle(
         self,
         *,
         clientToken: str = ...,
         customerManagedKeyIdentifier: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateAppBundleResponseTypeDef:
         """
         Creates an app bundle to collect data from an application using AppFabric.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Client.create_app_bundle)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appfabric/client/#create_app_bundle)
         """
@@ -180,15 +179,15 @@
         self,
         *,
         appBundleIdentifier: str,
         app: str,
         tenantId: str,
         ingestionType: Literal["auditLog"],
         clientToken: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateIngestionResponseTypeDef:
         """
         Creates a data ingestion for an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Client.create_ingestion)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appfabric/client/#create_ingestion)
         """
@@ -197,15 +196,15 @@
         self,
         *,
         appBundleIdentifier: str,
         ingestionIdentifier: str,
         processingConfiguration: ProcessingConfigurationTypeDef,
         destinationConfiguration: DestinationConfigurationTypeDef,
         clientToken: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateIngestionDestinationResponseTypeDef:
         """
         Creates an ingestion destination, which specifies how an application's ingested
         data is processed by Amazon Web Services AppFabric and where it's
         delivered.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Client.create_ingestion_destination)
@@ -241,15 +240,15 @@
         """
 
     async def delete_ingestion_destination(
         self,
         *,
         appBundleIdentifier: str,
         ingestionIdentifier: str,
-        ingestionDestinationIdentifier: str
+        ingestionDestinationIdentifier: str,
     ) -> Dict[str, Any]:
         """
         Deletes an ingestion destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Client.delete_ingestion_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appfabric/client/#delete_ingestion_destination)
         """
@@ -297,15 +296,15 @@
         """
 
     async def get_ingestion_destination(
         self,
         *,
         appBundleIdentifier: str,
         ingestionIdentifier: str,
-        ingestionDestinationIdentifier: str
+        ingestionDestinationIdentifier: str,
     ) -> GetIngestionDestinationResponseTypeDef:
         """
         Returns information about an ingestion destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Client.get_ingestion_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appfabric/client/#get_ingestion_destination)
         """
@@ -332,15 +331,15 @@
 
     async def list_ingestion_destinations(
         self,
         *,
         appBundleIdentifier: str,
         ingestionIdentifier: str,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListIngestionDestinationsResponseTypeDef:
         """
         Returns a list of all ingestion destinations configured for an ingestion.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Client.list_ingestion_destinations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appfabric/client/#list_ingestion_destinations)
         """
@@ -413,15 +412,15 @@
 
     async def update_app_authorization(
         self,
         *,
         appBundleIdentifier: str,
         appAuthorizationIdentifier: str,
         credential: CredentialTypeDef = ...,
-        tenant: TenantTypeDef = ...
+        tenant: TenantTypeDef = ...,
     ) -> UpdateAppAuthorizationResponseTypeDef:
         """
         Updates an app authorization within an app bundle, which allows AppFabric to
         connect to an
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Client.update_app_authorization)
@@ -430,15 +429,15 @@
 
     async def update_ingestion_destination(
         self,
         *,
         appBundleIdentifier: str,
         ingestionIdentifier: str,
         ingestionDestinationIdentifier: str,
-        destinationConfiguration: DestinationConfigurationTypeDef
+        destinationConfiguration: DestinationConfigurationTypeDef,
     ) -> UpdateIngestionDestinationResponseTypeDef:
         """
         Updates an ingestion destination, which specifies how an application's ingested
         data is processed by Amazon Web Services AppFabric and where it's
         delivered.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Client.update_ingestion_destination)
```

### Comparing `types-aiobotocore-appfabric-2.9.0/types_aiobotocore_appfabric/client.pyi` & `types-aiobotocore-appfabric-2.9.1/types_aiobotocore_appfabric/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -123,15 +123,15 @@
         """
 
     async def connect_app_authorization(
         self,
         *,
         appBundleIdentifier: str,
         appAuthorizationIdentifier: str,
-        authRequest: AuthRequestTypeDef = ...
+        authRequest: AuthRequestTypeDef = ...,
     ) -> ConnectAppAuthorizationResponseTypeDef:
         """
         Establishes a connection between Amazon Web Services AppFabric and an
         application, which allows AppFabric to call the APIs of the
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Client.connect_app_authorization)
@@ -143,15 +143,15 @@
         *,
         appBundleIdentifier: str,
         app: str,
         credential: CredentialTypeDef,
         tenant: TenantTypeDef,
         authType: AuthTypeType,
         clientToken: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateAppAuthorizationResponseTypeDef:
         """
         Creates an app authorization within an app bundle, which allows AppFabric to
         connect to an
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Client.create_app_authorization)
@@ -159,15 +159,15 @@
         """
 
     async def create_app_bundle(
         self,
         *,
         clientToken: str = ...,
         customerManagedKeyIdentifier: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateAppBundleResponseTypeDef:
         """
         Creates an app bundle to collect data from an application using AppFabric.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Client.create_app_bundle)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appfabric/client/#create_app_bundle)
         """
@@ -176,15 +176,15 @@
         self,
         *,
         appBundleIdentifier: str,
         app: str,
         tenantId: str,
         ingestionType: Literal["auditLog"],
         clientToken: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateIngestionResponseTypeDef:
         """
         Creates a data ingestion for an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Client.create_ingestion)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appfabric/client/#create_ingestion)
         """
@@ -193,15 +193,15 @@
         self,
         *,
         appBundleIdentifier: str,
         ingestionIdentifier: str,
         processingConfiguration: ProcessingConfigurationTypeDef,
         destinationConfiguration: DestinationConfigurationTypeDef,
         clientToken: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateIngestionDestinationResponseTypeDef:
         """
         Creates an ingestion destination, which specifies how an application's ingested
         data is processed by Amazon Web Services AppFabric and where it's
         delivered.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Client.create_ingestion_destination)
@@ -237,15 +237,15 @@
         """
 
     async def delete_ingestion_destination(
         self,
         *,
         appBundleIdentifier: str,
         ingestionIdentifier: str,
-        ingestionDestinationIdentifier: str
+        ingestionDestinationIdentifier: str,
     ) -> Dict[str, Any]:
         """
         Deletes an ingestion destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Client.delete_ingestion_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appfabric/client/#delete_ingestion_destination)
         """
@@ -293,15 +293,15 @@
         """
 
     async def get_ingestion_destination(
         self,
         *,
         appBundleIdentifier: str,
         ingestionIdentifier: str,
-        ingestionDestinationIdentifier: str
+        ingestionDestinationIdentifier: str,
     ) -> GetIngestionDestinationResponseTypeDef:
         """
         Returns information about an ingestion destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Client.get_ingestion_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appfabric/client/#get_ingestion_destination)
         """
@@ -328,15 +328,15 @@
 
     async def list_ingestion_destinations(
         self,
         *,
         appBundleIdentifier: str,
         ingestionIdentifier: str,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListIngestionDestinationsResponseTypeDef:
         """
         Returns a list of all ingestion destinations configured for an ingestion.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Client.list_ingestion_destinations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appfabric/client/#list_ingestion_destinations)
         """
@@ -409,15 +409,15 @@
 
     async def update_app_authorization(
         self,
         *,
         appBundleIdentifier: str,
         appAuthorizationIdentifier: str,
         credential: CredentialTypeDef = ...,
-        tenant: TenantTypeDef = ...
+        tenant: TenantTypeDef = ...,
     ) -> UpdateAppAuthorizationResponseTypeDef:
         """
         Updates an app authorization within an app bundle, which allows AppFabric to
         connect to an
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Client.update_app_authorization)
@@ -426,15 +426,15 @@
 
     async def update_ingestion_destination(
         self,
         *,
         appBundleIdentifier: str,
         ingestionIdentifier: str,
         ingestionDestinationIdentifier: str,
-        destinationConfiguration: DestinationConfigurationTypeDef
+        destinationConfiguration: DestinationConfigurationTypeDef,
     ) -> UpdateIngestionDestinationResponseTypeDef:
         """
         Updates an ingestion destination, which specifies how an application's ingested
         data is processed by Amazon Web Services AppFabric and where it's
         delivered.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Client.update_ingestion_destination)
```

### Comparing `types-aiobotocore-appfabric-2.9.0/types_aiobotocore_appfabric/literals.py` & `types-aiobotocore-appfabric-2.9.1/types_aiobotocore_appfabric/literals.py`

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
     "AppAuthorizationStatusType",
     "AuthTypeType",
     "FormatType",
     "IngestionDestinationStatusType",
     "IngestionStateType",
     "IngestionTypeType",
@@ -36,15 +35,14 @@
     "SchemaType",
     "AppFabricServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 AppAuthorizationStatusType = Literal[
     "Connected", "ConnectionValidationFailed", "PendingConnect", "TokenAutoRotationFailed"
 ]
 AuthTypeType = Literal["apiKey", "oauth2"]
 FormatType = Literal["json", "parquet"]
 IngestionDestinationStatusType = Literal["Active", "Failed"]
 IngestionStateType = Literal["disabled", "enabled"]
```

### Comparing `types-aiobotocore-appfabric-2.9.0/types_aiobotocore_appfabric/literals.pyi` & `types-aiobotocore-appfabric-2.9.1/types_aiobotocore_appfabric/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appfabric-2.9.0/types_aiobotocore_appfabric/paginator.py` & `types-aiobotocore-appfabric-2.9.1/types_aiobotocore_appfabric/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 __all__ = (
     "ListAppAuthorizationsPaginator",
     "ListAppBundlesPaginator",
     "ListIngestionDestinationsPaginator",
     "ListIngestionsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -95,15 +94,15 @@
     """
 
     def paginate(
         self,
         *,
         appBundleIdentifier: str,
         ingestionIdentifier: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListIngestionDestinationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Paginator.ListIngestionDestinations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appfabric/paginators/#listingestiondestinationspaginator)
         """
```

### Comparing `types-aiobotocore-appfabric-2.9.0/types_aiobotocore_appfabric/paginator.pyi` & `types-aiobotocore-appfabric-2.9.1/types_aiobotocore_appfabric/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     """
 
     def paginate(
         self,
         *,
         appBundleIdentifier: str,
         ingestionIdentifier: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListIngestionDestinationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Paginator.ListIngestionDestinations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appfabric/paginators/#listingestiondestinationspaginator)
         """
 
 class ListIngestionsPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-appfabric-2.9.0/types_aiobotocore_appfabric/type_defs.py` & `types-aiobotocore-appfabric-2.9.1/types_aiobotocore_appfabric/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ApiKeyCredentialTypeDef",
     "TenantTypeDef",
     "AppBundleSummaryTypeDef",
     "AppBundleTypeDef",
     "AuditLogProcessingConfigurationTypeDef",
     "AuthRequestTypeDef",
```

### Comparing `types-aiobotocore-appfabric-2.9.0/types_aiobotocore_appfabric/type_defs.pyi` & `types-aiobotocore-appfabric-2.9.1/types_aiobotocore_appfabric/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appfabric-2.9.0/types_aiobotocore_appfabric.egg-info/PKG-INFO` & `types-aiobotocore-appfabric-2.9.1/types_aiobotocore_appfabric.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-appfabric
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.AppFabric 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.AppFabric 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appfabric/
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
 
 <a id="types-aiobotocore-appfabric"></a>
 
 # types-aiobotocore-appfabric
 
 [![PyPI - types-aiobotocore-appfabric](https://img.shields.io/pypi/v/types-aiobotocore-appfabric.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appfabric)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appfabric.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appfabric)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appfabric/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appfabric)](https://pepy.tech/project/types-aiobotocore-appfabric)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AppFabric 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric)
+[aiobotocore.AppFabric 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric)
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
 [types-aiobotocore-appfabric docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appfabric/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-appfabric-2.9.0/types_aiobotocore_appfabric.egg-info/SOURCES.txt` & `types-aiobotocore-appfabric-2.9.1/types_aiobotocore_appfabric.egg-info/SOURCES.txt`

 * *Files identical despite different names*

