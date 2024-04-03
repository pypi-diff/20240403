# Comparing `tmp/types-aiobotocore-mediastore-data-2.9.0.tar.gz` & `tmp/types-aiobotocore-mediastore-data-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-mediastore-data-2.9.0.tar", last modified: Wed Dec 13 19:59:54 2023, max compression
+gzip compressed data, was "types-aiobotocore-mediastore-data-2.9.1.tar", last modified: Thu Jan 18 01:21:16 2024, max compression
```

## Comparing `types-aiobotocore-mediastore-data-2.9.0.tar` & `types-aiobotocore-mediastore-data-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:54.597449 types-aiobotocore-mediastore-data-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:50:19.000000 types-aiobotocore-mediastore-data-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13349 2023-12-13 19:59:54.597449 types-aiobotocore-mediastore-data-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11755 2023-12-13 19:50:19.000000 types-aiobotocore-mediastore-data-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:54.597449 types-aiobotocore-mediastore-data-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2023-12-13 19:50:19.000000 types-aiobotocore-mediastore-data-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:54.597449 types-aiobotocore-mediastore-data-2.9.0/types_aiobotocore_mediastore_data/
--rw-r--r--   0 runner    (1001) docker     (127)      677 2023-12-13 19:50:19.000000 types-aiobotocore-mediastore-data-2.9.0/types_aiobotocore_mediastore_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      676 2023-12-13 19:50:19.000000 types-aiobotocore-mediastore-data-2.9.0/types_aiobotocore_mediastore_data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      962 2023-12-13 19:50:19.000000 types-aiobotocore-mediastore-data-2.9.0/types_aiobotocore_mediastore_data/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7768 2023-12-13 19:50:19.000000 types-aiobotocore-mediastore-data-2.9.0/types_aiobotocore_mediastore_data/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7764 2023-12-13 19:50:19.000000 types-aiobotocore-mediastore-data-2.9.0/types_aiobotocore_mediastore_data/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8685 2023-12-13 19:50:20.000000 types-aiobotocore-mediastore-data-2.9.0/types_aiobotocore_mediastore_data/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8683 2023-12-13 19:50:20.000000 types-aiobotocore-mediastore-data-2.9.0/types_aiobotocore_mediastore_data/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2023-12-13 19:50:19.000000 types-aiobotocore-mediastore-data-2.9.0/types_aiobotocore_mediastore_data/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2023-12-13 19:50:19.000000 types-aiobotocore-mediastore-data-2.9.0/types_aiobotocore_mediastore_data/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:50:19.000000 types-aiobotocore-mediastore-data-2.9.0/types_aiobotocore_mediastore_data/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4424 2023-12-13 19:50:20.000000 types-aiobotocore-mediastore-data-2.9.0/types_aiobotocore_mediastore_data/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4423 2023-12-13 19:50:20.000000 types-aiobotocore-mediastore-data-2.9.0/types_aiobotocore_mediastore_data/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:50:19.000000 types-aiobotocore-mediastore-data-2.9.0/types_aiobotocore_mediastore_data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:54.597449 types-aiobotocore-mediastore-data-2.9.0/types_aiobotocore_mediastore_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13349 2023-12-13 19:59:54.000000 types-aiobotocore-mediastore-data-2.9.0/types_aiobotocore_mediastore_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      965 2023-12-13 19:59:54.000000 types-aiobotocore-mediastore-data-2.9.0/types_aiobotocore_mediastore_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:54.000000 types-aiobotocore-mediastore-data-2.9.0/types_aiobotocore_mediastore_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:54.000000 types-aiobotocore-mediastore-data-2.9.0/types_aiobotocore_mediastore_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:54.000000 types-aiobotocore-mediastore-data-2.9.0/types_aiobotocore_mediastore_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-12-13 19:59:54.000000 types-aiobotocore-mediastore-data-2.9.0/types_aiobotocore_mediastore_data.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:16.409180 types-aiobotocore-mediastore-data-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:12:03.000000 types-aiobotocore-mediastore-data-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13369 2024-01-18 01:21:16.409180 types-aiobotocore-mediastore-data-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11755 2024-01-18 01:12:03.000000 types-aiobotocore-mediastore-data-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:16.409180 types-aiobotocore-mediastore-data-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-01-18 01:12:03.000000 types-aiobotocore-mediastore-data-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:16.409180 types-aiobotocore-mediastore-data-2.9.1/types_aiobotocore_mediastore_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-01-18 01:12:03.000000 types-aiobotocore-mediastore-data-2.9.1/types_aiobotocore_mediastore_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-01-18 01:12:03.000000 types-aiobotocore-mediastore-data-2.9.1/types_aiobotocore_mediastore_data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-01-18 01:12:03.000000 types-aiobotocore-mediastore-data-2.9.1/types_aiobotocore_mediastore_data/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7768 2024-01-18 01:12:03.000000 types-aiobotocore-mediastore-data-2.9.1/types_aiobotocore_mediastore_data/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7765 2024-01-18 01:12:03.000000 types-aiobotocore-mediastore-data-2.9.1/types_aiobotocore_mediastore_data/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8683 2024-01-18 01:12:03.000000 types-aiobotocore-mediastore-data-2.9.1/types_aiobotocore_mediastore_data/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8683 2024-01-18 01:12:03.000000 types-aiobotocore-mediastore-data-2.9.1/types_aiobotocore_mediastore_data/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-01-18 01:12:03.000000 types-aiobotocore-mediastore-data-2.9.1/types_aiobotocore_mediastore_data/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-01-18 01:12:03.000000 types-aiobotocore-mediastore-data-2.9.1/types_aiobotocore_mediastore_data/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:12:03.000000 types-aiobotocore-mediastore-data-2.9.1/types_aiobotocore_mediastore_data/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4423 2024-01-18 01:12:03.000000 types-aiobotocore-mediastore-data-2.9.1/types_aiobotocore_mediastore_data/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4423 2024-01-18 01:12:03.000000 types-aiobotocore-mediastore-data-2.9.1/types_aiobotocore_mediastore_data/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:12:03.000000 types-aiobotocore-mediastore-data-2.9.1/types_aiobotocore_mediastore_data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:16.409180 types-aiobotocore-mediastore-data-2.9.1/types_aiobotocore_mediastore_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13369 2024-01-18 01:21:16.000000 types-aiobotocore-mediastore-data-2.9.1/types_aiobotocore_mediastore_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-01-18 01:21:16.000000 types-aiobotocore-mediastore-data-2.9.1/types_aiobotocore_mediastore_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:16.000000 types-aiobotocore-mediastore-data-2.9.1/types_aiobotocore_mediastore_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:16.000000 types-aiobotocore-mediastore-data-2.9.1/types_aiobotocore_mediastore_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:16.000000 types-aiobotocore-mediastore-data-2.9.1/types_aiobotocore_mediastore_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-01-18 01:21:16.000000 types-aiobotocore-mediastore-data-2.9.1/types_aiobotocore_mediastore_data.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-mediastore-data-2.9.0/LICENSE` & `types-aiobotocore-mediastore-data-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-mediastore-data-2.9.0/PKG-INFO` & `types-aiobotocore-mediastore-data-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mediastore-data
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.MediaStoreData 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.MediaStoreData 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore_data/
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
 
 <a id="types-aiobotocore-mediastore-data"></a>
 
 # types-aiobotocore-mediastore-data
 
 [![PyPI - types-aiobotocore-mediastore-data](https://img.shields.io/pypi/v/types-aiobotocore-mediastore-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediastore-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mediastore-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediastore-data)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mediastore-data)](https://pepy.tech/project/types-aiobotocore-mediastore-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MediaStoreData 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData)
+[aiobotocore.MediaStoreData 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData)
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
 [types-aiobotocore-mediastore-data docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore_data/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-mediastore-data-2.9.0/README.md` & `types-aiobotocore-mediastore-data-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mediastore-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediastore-data)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mediastore-data)](https://pepy.tech/project/types-aiobotocore-mediastore-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MediaStoreData 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData)
+[aiobotocore.MediaStoreData 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData)
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
 [types-aiobotocore-mediastore-data docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore_data/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-mediastore-data-2.9.0/setup.py` & `types-aiobotocore-mediastore-data-2.9.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-mediastore-data",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_mediastore_data"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.MediaStoreData 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.MediaStoreData 2.9.1 service generated with"
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
     keywords="aiobotocore mediastore-data type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_mediastore_data": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore_data/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-mediastore-data-2.9.0/types_aiobotocore_mediastore_data/__init__.py` & `types-aiobotocore-mediastore-data-2.9.1/types_aiobotocore_mediastore_data/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,9 +22,8 @@
 """
 
 from .client import MediaStoreDataClient
 from .paginator import ListItemsPaginator
 
 Client = MediaStoreDataClient
 
-
 __all__ = ("Client", "ListItemsPaginator", "MediaStoreDataClient")
```

### Comparing `types-aiobotocore-mediastore-data-2.9.0/types_aiobotocore_mediastore_data/__init__.pyi` & `types-aiobotocore-mediastore-data-2.9.1/types_aiobotocore_mediastore_data/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediastore-data-2.9.0/types_aiobotocore_mediastore_data/__main__.py` & `types-aiobotocore-mediastore-data-2.9.1/types_aiobotocore_mediastore_data/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.MediaStoreData 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.MediaStoreData 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore_data//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData\nOther"
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

### Comparing `types-aiobotocore-mediastore-data-2.9.0/types_aiobotocore_mediastore_data/client.py` & `types-aiobotocore-mediastore-data-2.9.1/types_aiobotocore_mediastore_data/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("MediaStoreDataClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -142,15 +141,15 @@
         self,
         *,
         Body: BlobTypeDef,
         Path: str,
         ContentType: str = ...,
         CacheControl: str = ...,
         StorageClass: Literal["TEMPORAL"] = ...,
-        UploadAvailability: UploadAvailabilityType = ...
+        UploadAvailability: UploadAvailabilityType = ...,
     ) -> PutObjectResponseTypeDef:
         """
         Uploads an object to the specified path.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData.Client.put_object)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore_data/client/#put_object)
         """
```

### Comparing `types-aiobotocore-mediastore-data-2.9.0/types_aiobotocore_mediastore_data/client.pyi` & `types-aiobotocore-mediastore-data-2.9.1/types_aiobotocore_mediastore_data/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,15 @@
         self,
         *,
         Body: BlobTypeDef,
         Path: str,
         ContentType: str = ...,
         CacheControl: str = ...,
         StorageClass: Literal["TEMPORAL"] = ...,
-        UploadAvailability: UploadAvailabilityType = ...
+        UploadAvailability: UploadAvailabilityType = ...,
     ) -> PutObjectResponseTypeDef:
         """
         Uploads an object to the specified path.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData.Client.put_object)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore_data/client/#put_object)
         """
```

### Comparing `types-aiobotocore-mediastore-data-2.9.0/types_aiobotocore_mediastore_data/literals.py` & `types-aiobotocore-mediastore-data-2.9.1/types_aiobotocore_mediastore_data/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,28 +15,26 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ItemTypeType",
     "ListItemsPaginatorName",
     "StorageClassType",
     "UploadAvailabilityType",
     "MediaStoreDataServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ItemTypeType = Literal["FOLDER", "OBJECT"]
 ListItemsPaginatorName = Literal["list_items"]
 StorageClassType = Literal["TEMPORAL"]
 UploadAvailabilityType = Literal["STANDARD", "STREAMING"]
 MediaStoreDataServiceName = Literal["mediastore-data"]
 ServiceName = Literal[
     "accessanalyzer",
```

### Comparing `types-aiobotocore-mediastore-data-2.9.0/types_aiobotocore_mediastore_data/literals.pyi` & `types-aiobotocore-mediastore-data-2.9.1/types_aiobotocore_mediastore_data/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediastore-data-2.9.0/types_aiobotocore_mediastore_data/paginator.py` & `types-aiobotocore-mediastore-data-2.9.1/types_aiobotocore_mediastore_data/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .type_defs import ListItemsResponseTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListItemsPaginator",)
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
```

### Comparing `types-aiobotocore-mediastore-data-2.9.0/types_aiobotocore_mediastore_data/paginator.pyi` & `types-aiobotocore-mediastore-data-2.9.1/types_aiobotocore_mediastore_data/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediastore-data-2.9.0/types_aiobotocore_mediastore_data/type_defs.py` & `types-aiobotocore-mediastore-data-2.9.1/types_aiobotocore_mediastore_data/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "BlobTypeDef",
     "DeleteObjectRequestRequestTypeDef",
     "DescribeObjectRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "GetObjectRequestRequestTypeDef",
     "ItemTypeDef",
```

### Comparing `types-aiobotocore-mediastore-data-2.9.0/types_aiobotocore_mediastore_data/type_defs.pyi` & `types-aiobotocore-mediastore-data-2.9.1/types_aiobotocore_mediastore_data/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediastore-data-2.9.0/types_aiobotocore_mediastore_data.egg-info/PKG-INFO` & `types-aiobotocore-mediastore-data-2.9.1/types_aiobotocore_mediastore_data.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mediastore-data
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.MediaStoreData 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.MediaStoreData 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore_data/
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
 
 <a id="types-aiobotocore-mediastore-data"></a>
 
 # types-aiobotocore-mediastore-data
 
 [![PyPI - types-aiobotocore-mediastore-data](https://img.shields.io/pypi/v/types-aiobotocore-mediastore-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediastore-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mediastore-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediastore-data)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mediastore-data)](https://pepy.tech/project/types-aiobotocore-mediastore-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MediaStoreData 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData)
+[aiobotocore.MediaStoreData 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData)
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
 [types-aiobotocore-mediastore-data docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore_data/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-mediastore-data-2.9.0/types_aiobotocore_mediastore_data.egg-info/SOURCES.txt` & `types-aiobotocore-mediastore-data-2.9.1/types_aiobotocore_mediastore_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

