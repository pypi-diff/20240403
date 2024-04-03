# Comparing `tmp/types-aiobotocore-finspace-data-2.9.0.tar.gz` & `tmp/types-aiobotocore-finspace-data-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-finspace-data-2.9.0.tar", last modified: Wed Dec 13 19:59:18 2023, max compression
+gzip compressed data, was "types-aiobotocore-finspace-data-2.9.1.tar", last modified: Thu Jan 18 01:20:43 2024, max compression
```

## Comparing `types-aiobotocore-finspace-data-2.9.0.tar` & `types-aiobotocore-finspace-data-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:18.669747 types-aiobotocore-finspace-data-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:46:12.000000 types-aiobotocore-finspace-data-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13865 2023-12-13 19:59:18.669747 types-aiobotocore-finspace-data-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12279 2023-12-13 19:46:12.000000 types-aiobotocore-finspace-data-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:18.669747 types-aiobotocore-finspace-data-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2023-12-13 19:46:12.000000 types-aiobotocore-finspace-data-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:18.669747 types-aiobotocore-finspace-data-2.9.0/types_aiobotocore_finspace_data/
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2023-12-13 19:46:12.000000 types-aiobotocore-finspace-data-2.9.0/types_aiobotocore_finspace_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2023-12-13 19:46:12.000000 types-aiobotocore-finspace-data-2.9.0/types_aiobotocore_finspace_data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      954 2023-12-13 19:46:12.000000 types-aiobotocore-finspace-data-2.9.0/types_aiobotocore_finspace_data/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27118 2023-12-13 19:46:12.000000 types-aiobotocore-finspace-data-2.9.0/types_aiobotocore_finspace_data/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    27114 2023-12-13 19:46:12.000000 types-aiobotocore-finspace-data-2.9.0/types_aiobotocore_finspace_data/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10646 2023-12-13 19:46:12.000000 types-aiobotocore-finspace-data-2.9.0/types_aiobotocore_finspace_data/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10644 2023-12-13 19:46:12.000000 types-aiobotocore-finspace-data-2.9.0/types_aiobotocore_finspace_data/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6489 2023-12-13 19:46:12.000000 types-aiobotocore-finspace-data-2.9.0/types_aiobotocore_finspace_data/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6482 2023-12-13 19:46:12.000000 types-aiobotocore-finspace-data-2.9.0/types_aiobotocore_finspace_data/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:46:12.000000 types-aiobotocore-finspace-data-2.9.0/types_aiobotocore_finspace_data/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    30037 2023-12-13 19:46:13.000000 types-aiobotocore-finspace-data-2.9.0/types_aiobotocore_finspace_data/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    30036 2023-12-13 19:46:13.000000 types-aiobotocore-finspace-data-2.9.0/types_aiobotocore_finspace_data/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:46:12.000000 types-aiobotocore-finspace-data-2.9.0/types_aiobotocore_finspace_data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:18.669747 types-aiobotocore-finspace-data-2.9.0/types_aiobotocore_finspace_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13865 2023-12-13 19:59:18.000000 types-aiobotocore-finspace-data-2.9.0/types_aiobotocore_finspace_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      927 2023-12-13 19:59:18.000000 types-aiobotocore-finspace-data-2.9.0/types_aiobotocore_finspace_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:18.000000 types-aiobotocore-finspace-data-2.9.0/types_aiobotocore_finspace_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:18.000000 types-aiobotocore-finspace-data-2.9.0/types_aiobotocore_finspace_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:18.000000 types-aiobotocore-finspace-data-2.9.0/types_aiobotocore_finspace_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-13 19:59:18.000000 types-aiobotocore-finspace-data-2.9.0/types_aiobotocore_finspace_data.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:43.189331 types-aiobotocore-finspace-data-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:08:06.000000 types-aiobotocore-finspace-data-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13885 2024-01-18 01:20:43.189331 types-aiobotocore-finspace-data-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12279 2024-01-18 01:08:06.000000 types-aiobotocore-finspace-data-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:43.189331 types-aiobotocore-finspace-data-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-01-18 01:08:06.000000 types-aiobotocore-finspace-data-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:43.189331 types-aiobotocore-finspace-data-2.9.1/types_aiobotocore_finspace_data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-01-18 01:08:06.000000 types-aiobotocore-finspace-data-2.9.1/types_aiobotocore_finspace_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-01-18 01:08:06.000000 types-aiobotocore-finspace-data-2.9.1/types_aiobotocore_finspace_data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-01-18 01:08:06.000000 types-aiobotocore-finspace-data-2.9.1/types_aiobotocore_finspace_data/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27126 2024-01-18 01:08:06.000000 types-aiobotocore-finspace-data-2.9.1/types_aiobotocore_finspace_data/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27123 2024-01-18 01:08:06.000000 types-aiobotocore-finspace-data-2.9.1/types_aiobotocore_finspace_data/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10644 2024-01-18 01:08:06.000000 types-aiobotocore-finspace-data-2.9.1/types_aiobotocore_finspace_data/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10644 2024-01-18 01:08:06.000000 types-aiobotocore-finspace-data-2.9.1/types_aiobotocore_finspace_data/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-01-18 01:08:06.000000 types-aiobotocore-finspace-data-2.9.1/types_aiobotocore_finspace_data/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6482 2024-01-18 01:08:06.000000 types-aiobotocore-finspace-data-2.9.1/types_aiobotocore_finspace_data/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:08:06.000000 types-aiobotocore-finspace-data-2.9.1/types_aiobotocore_finspace_data/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    30036 2024-01-18 01:08:07.000000 types-aiobotocore-finspace-data-2.9.1/types_aiobotocore_finspace_data/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30036 2024-01-18 01:08:07.000000 types-aiobotocore-finspace-data-2.9.1/types_aiobotocore_finspace_data/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:08:06.000000 types-aiobotocore-finspace-data-2.9.1/types_aiobotocore_finspace_data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:43.189331 types-aiobotocore-finspace-data-2.9.1/types_aiobotocore_finspace_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13885 2024-01-18 01:20:43.000000 types-aiobotocore-finspace-data-2.9.1/types_aiobotocore_finspace_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-01-18 01:20:43.000000 types-aiobotocore-finspace-data-2.9.1/types_aiobotocore_finspace_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:43.000000 types-aiobotocore-finspace-data-2.9.1/types_aiobotocore_finspace_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:43.000000 types-aiobotocore-finspace-data-2.9.1/types_aiobotocore_finspace_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:43.000000 types-aiobotocore-finspace-data-2.9.1/types_aiobotocore_finspace_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-01-18 01:20:43.000000 types-aiobotocore-finspace-data-2.9.1/types_aiobotocore_finspace_data.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-finspace-data-2.9.0/LICENSE` & `types-aiobotocore-finspace-data-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-finspace-data-2.9.0/PKG-INFO` & `types-aiobotocore-finspace-data-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-finspace-data
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.FinSpaceData 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.FinSpaceData 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace_data/
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
 
 <a id="types-aiobotocore-finspace-data"></a>
 
 # types-aiobotocore-finspace-data
 
 [![PyPI - types-aiobotocore-finspace-data](https://img.shields.io/pypi/v/types-aiobotocore-finspace-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-finspace-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-finspace-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-finspace-data)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-finspace-data)](https://pepy.tech/project/types-aiobotocore-finspace-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.FinSpaceData 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData)
+[aiobotocore.FinSpaceData 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData)
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
 [types-aiobotocore-finspace-data docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace_data/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-finspace-data-2.9.0/README.md` & `types-aiobotocore-finspace-data-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-finspace-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-finspace-data)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-finspace-data)](https://pepy.tech/project/types-aiobotocore-finspace-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.FinSpaceData 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData)
+[aiobotocore.FinSpaceData 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData)
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
 [types-aiobotocore-finspace-data docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace_data/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-finspace-data-2.9.0/setup.py` & `types-aiobotocore-finspace-data-2.9.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-finspace-data",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_finspace_data"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.FinSpaceData 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.FinSpaceData 2.9.1 service generated with"
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
     keywords="aiobotocore finspace-data type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_finspace_data": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace_data/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-finspace-data-2.9.0/types_aiobotocore_finspace_data/__init__.py` & `types-aiobotocore-finspace-data-2.9.1/types_aiobotocore_finspace_data/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     ListDataViewsPaginator,
     ListPermissionGroupsPaginator,
     ListUsersPaginator,
 )
 
 Client = FinSpaceDataClient
 
-
 __all__ = (
     "Client",
     "FinSpaceDataClient",
     "ListChangesetsPaginator",
     "ListDataViewsPaginator",
     "ListDatasetsPaginator",
     "ListPermissionGroupsPaginator",
```

### Comparing `types-aiobotocore-finspace-data-2.9.0/types_aiobotocore_finspace_data/__init__.pyi` & `types-aiobotocore-finspace-data-2.9.1/types_aiobotocore_finspace_data/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-finspace-data-2.9.0/types_aiobotocore_finspace_data/__main__.py` & `types-aiobotocore-finspace-data-2.9.1/types_aiobotocore_finspace_data/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.FinSpaceData 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.FinSpaceData 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace_data//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData\nOther"
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

### Comparing `types-aiobotocore-finspace-data-2.9.0/types_aiobotocore_finspace_data/client.py` & `types-aiobotocore-finspace-data-2.9.1/types_aiobotocore_finspace_data/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("FinSpaceDataClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -150,15 +149,15 @@
     async def create_changeset(
         self,
         *,
         datasetId: str,
         changeType: ChangeTypeType,
         sourceParams: Mapping[str, str],
         formatParams: Mapping[str, str],
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> CreateChangesetResponseTypeDef:
         """
         Creates a new Changeset in a FinSpace Dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.create_changeset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace_data/client/#create_changeset)
         """
@@ -168,15 +167,15 @@
         *,
         datasetId: str,
         destinationTypeParams: DataViewDestinationTypeParamsTypeDef,
         clientToken: str = ...,
         autoUpdate: bool = ...,
         sortColumns: Sequence[str] = ...,
         partitionColumns: Sequence[str] = ...,
-        asOfTimestamp: int = ...
+        asOfTimestamp: int = ...,
     ) -> CreateDataViewResponseTypeDef:
         """
         Creates a Dataview for a Dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.create_data_view)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace_data/client/#create_data_view)
         """
@@ -187,30 +186,30 @@
         datasetTitle: str,
         kind: DatasetKindType,
         permissionGroupParams: PermissionGroupParamsTypeDef,
         clientToken: str = ...,
         datasetDescription: str = ...,
         ownerInfo: DatasetOwnerInfoTypeDef = ...,
         alias: str = ...,
-        schemaDefinition: SchemaUnionTypeDef = ...
+        schemaDefinition: SchemaUnionTypeDef = ...,
     ) -> CreateDatasetResponseTypeDef:
         """
         Creates a new FinSpace Dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.create_dataset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace_data/client/#create_dataset)
         """
 
     async def create_permission_group(
         self,
         *,
         name: str,
         applicationPermissions: Sequence[ApplicationPermissionType],
         description: str = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> CreatePermissionGroupResponseTypeDef:
         """
         Creates a group of permissions for various actions that a user can perform in
         FinSpace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.create_permission_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace_data/client/#create_permission_group)
@@ -221,15 +220,15 @@
         *,
         emailAddress: str,
         type: UserTypeType,
         firstName: str = ...,
         lastName: str = ...,
         apiAccess: ApiAccessType = ...,
         apiAccessPrincipalArn: str = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> CreateUserResponseTypeDef:
         """
         Creates a new user in FinSpace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.create_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace_data/client/#create_user)
         """
@@ -457,15 +456,15 @@
     async def update_changeset(
         self,
         *,
         datasetId: str,
         changesetId: str,
         sourceParams: Mapping[str, str],
         formatParams: Mapping[str, str],
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> UpdateChangesetResponseTypeDef:
         """
         Updates a FinSpace Changeset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.update_changeset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace_data/client/#update_changeset)
         """
@@ -475,15 +474,15 @@
         *,
         datasetId: str,
         datasetTitle: str,
         kind: DatasetKindType,
         clientToken: str = ...,
         datasetDescription: str = ...,
         alias: str = ...,
-        schemaDefinition: SchemaUnionTypeDef = ...
+        schemaDefinition: SchemaUnionTypeDef = ...,
     ) -> UpdateDatasetResponseTypeDef:
         """
         Updates a FinSpace Dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.update_dataset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace_data/client/#update_dataset)
         """
@@ -491,15 +490,15 @@
     async def update_permission_group(
         self,
         *,
         permissionGroupId: str,
         name: str = ...,
         description: str = ...,
         applicationPermissions: Sequence[ApplicationPermissionType] = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> UpdatePermissionGroupResponseTypeDef:
         """
         Modifies the details of a permission group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.update_permission_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace_data/client/#update_permission_group)
         """
@@ -509,15 +508,15 @@
         *,
         userId: str,
         type: UserTypeType = ...,
         firstName: str = ...,
         lastName: str = ...,
         apiAccess: ApiAccessType = ...,
         apiAccessPrincipalArn: str = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> UpdateUserResponseTypeDef:
         """
         Modifies the details of the specified user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.update_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace_data/client/#update_user)
         """
```

### Comparing `types-aiobotocore-finspace-data-2.9.0/types_aiobotocore_finspace_data/client.pyi` & `types-aiobotocore-finspace-data-2.9.1/types_aiobotocore_finspace_data/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,15 @@
     async def create_changeset(
         self,
         *,
         datasetId: str,
         changeType: ChangeTypeType,
         sourceParams: Mapping[str, str],
         formatParams: Mapping[str, str],
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> CreateChangesetResponseTypeDef:
         """
         Creates a new Changeset in a FinSpace Dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.create_changeset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace_data/client/#create_changeset)
         """
@@ -164,15 +164,15 @@
         *,
         datasetId: str,
         destinationTypeParams: DataViewDestinationTypeParamsTypeDef,
         clientToken: str = ...,
         autoUpdate: bool = ...,
         sortColumns: Sequence[str] = ...,
         partitionColumns: Sequence[str] = ...,
-        asOfTimestamp: int = ...
+        asOfTimestamp: int = ...,
     ) -> CreateDataViewResponseTypeDef:
         """
         Creates a Dataview for a Dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.create_data_view)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace_data/client/#create_data_view)
         """
@@ -183,30 +183,30 @@
         datasetTitle: str,
         kind: DatasetKindType,
         permissionGroupParams: PermissionGroupParamsTypeDef,
         clientToken: str = ...,
         datasetDescription: str = ...,
         ownerInfo: DatasetOwnerInfoTypeDef = ...,
         alias: str = ...,
-        schemaDefinition: SchemaUnionTypeDef = ...
+        schemaDefinition: SchemaUnionTypeDef = ...,
     ) -> CreateDatasetResponseTypeDef:
         """
         Creates a new FinSpace Dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.create_dataset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace_data/client/#create_dataset)
         """
 
     async def create_permission_group(
         self,
         *,
         name: str,
         applicationPermissions: Sequence[ApplicationPermissionType],
         description: str = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> CreatePermissionGroupResponseTypeDef:
         """
         Creates a group of permissions for various actions that a user can perform in
         FinSpace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.create_permission_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace_data/client/#create_permission_group)
@@ -217,15 +217,15 @@
         *,
         emailAddress: str,
         type: UserTypeType,
         firstName: str = ...,
         lastName: str = ...,
         apiAccess: ApiAccessType = ...,
         apiAccessPrincipalArn: str = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> CreateUserResponseTypeDef:
         """
         Creates a new user in FinSpace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.create_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace_data/client/#create_user)
         """
@@ -453,15 +453,15 @@
     async def update_changeset(
         self,
         *,
         datasetId: str,
         changesetId: str,
         sourceParams: Mapping[str, str],
         formatParams: Mapping[str, str],
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> UpdateChangesetResponseTypeDef:
         """
         Updates a FinSpace Changeset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.update_changeset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace_data/client/#update_changeset)
         """
@@ -471,15 +471,15 @@
         *,
         datasetId: str,
         datasetTitle: str,
         kind: DatasetKindType,
         clientToken: str = ...,
         datasetDescription: str = ...,
         alias: str = ...,
-        schemaDefinition: SchemaUnionTypeDef = ...
+        schemaDefinition: SchemaUnionTypeDef = ...,
     ) -> UpdateDatasetResponseTypeDef:
         """
         Updates a FinSpace Dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.update_dataset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace_data/client/#update_dataset)
         """
@@ -487,15 +487,15 @@
     async def update_permission_group(
         self,
         *,
         permissionGroupId: str,
         name: str = ...,
         description: str = ...,
         applicationPermissions: Sequence[ApplicationPermissionType] = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> UpdatePermissionGroupResponseTypeDef:
         """
         Modifies the details of a permission group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.update_permission_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace_data/client/#update_permission_group)
         """
@@ -505,15 +505,15 @@
         *,
         userId: str,
         type: UserTypeType = ...,
         firstName: str = ...,
         lastName: str = ...,
         apiAccess: ApiAccessType = ...,
         apiAccessPrincipalArn: str = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> UpdateUserResponseTypeDef:
         """
         Modifies the details of the specified user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.update_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace_data/client/#update_user)
         """
```

### Comparing `types-aiobotocore-finspace-data-2.9.0/types_aiobotocore_finspace_data/literals.py` & `types-aiobotocore-finspace-data-2.9.1/types_aiobotocore_finspace_data/literals.py`

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
     "ApiAccessType",
     "ApplicationPermissionType",
     "ChangeTypeType",
     "ColumnDataTypeType",
     "DataViewStatusType",
     "DatasetKindType",
@@ -43,15 +42,14 @@
     "FinSpaceDataServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ApiAccessType = Literal["DISABLED", "ENABLED"]
 ApplicationPermissionType = Literal[
     "AccessNotebooks",
     "CreateDataset",
     "GetTemporaryCredentials",
     "ManageAttributeSets",
     "ManageClusters",
```

### Comparing `types-aiobotocore-finspace-data-2.9.0/types_aiobotocore_finspace_data/literals.pyi` & `types-aiobotocore-finspace-data-2.9.1/types_aiobotocore_finspace_data/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-finspace-data-2.9.0/types_aiobotocore_finspace_data/paginator.py` & `types-aiobotocore-finspace-data-2.9.1/types_aiobotocore_finspace_data/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,14 @@
     "ListChangesetsPaginator",
     "ListDataViewsPaginator",
     "ListDatasetsPaginator",
     "ListPermissionGroupsPaginator",
     "ListUsersPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
```

### Comparing `types-aiobotocore-finspace-data-2.9.0/types_aiobotocore_finspace_data/paginator.pyi` & `types-aiobotocore-finspace-data-2.9.1/types_aiobotocore_finspace_data/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-finspace-data-2.9.0/types_aiobotocore_finspace_data/type_defs.py` & `types-aiobotocore-finspace-data-2.9.1/types_aiobotocore_finspace_data/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AssociateUserToPermissionGroupRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AwsCredentialsTypeDef",
     "ChangesetErrorInfoTypeDef",
     "ColumnDefinitionTypeDef",
     "CreateChangesetRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-finspace-data-2.9.0/types_aiobotocore_finspace_data/type_defs.pyi` & `types-aiobotocore-finspace-data-2.9.1/types_aiobotocore_finspace_data/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-finspace-data-2.9.0/types_aiobotocore_finspace_data.egg-info/PKG-INFO` & `types-aiobotocore-finspace-data-2.9.1/types_aiobotocore_finspace_data.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-finspace-data
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.FinSpaceData 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.FinSpaceData 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace_data/
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
 
 <a id="types-aiobotocore-finspace-data"></a>
 
 # types-aiobotocore-finspace-data
 
 [![PyPI - types-aiobotocore-finspace-data](https://img.shields.io/pypi/v/types-aiobotocore-finspace-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-finspace-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-finspace-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-finspace-data)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-finspace-data)](https://pepy.tech/project/types-aiobotocore-finspace-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.FinSpaceData 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData)
+[aiobotocore.FinSpaceData 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData)
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
 [types-aiobotocore-finspace-data docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace_data/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-finspace-data-2.9.0/types_aiobotocore_finspace_data.egg-info/SOURCES.txt` & `types-aiobotocore-finspace-data-2.9.1/types_aiobotocore_finspace_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

