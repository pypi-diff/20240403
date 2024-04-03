# Comparing `tmp/types-aiobotocore-kinesisanalytics-2.9.0.tar.gz` & `tmp/types-aiobotocore-kinesisanalytics-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-kinesisanalytics-2.9.0.tar", last modified: Wed Dec 13 19:59:41 2023, max compression
+gzip compressed data, was "types-aiobotocore-kinesisanalytics-2.9.1.tar", last modified: Thu Jan 18 01:21:03 2024, max compression
```

## Comparing `types-aiobotocore-kinesisanalytics-2.9.0.tar` & `types-aiobotocore-kinesisanalytics-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:41.093563 types-aiobotocore-kinesisanalytics-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:48:35.000000 types-aiobotocore-kinesisanalytics-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12730 2023-12-13 19:59:41.093563 types-aiobotocore-kinesisanalytics-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11131 2023-12-13 19:48:35.000000 types-aiobotocore-kinesisanalytics-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:41.093563 types-aiobotocore-kinesisanalytics-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2023-12-13 19:48:35.000000 types-aiobotocore-kinesisanalytics-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:41.093563 types-aiobotocore-kinesisanalytics-2.9.0/types_aiobotocore_kinesisanalytics/
--rw-r--r--   0 runner    (1001) docker     (127)      515 2023-12-13 19:48:35.000000 types-aiobotocore-kinesisanalytics-2.9.0/types_aiobotocore_kinesisanalytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2023-12-13 19:48:35.000000 types-aiobotocore-kinesisanalytics-2.9.0/types_aiobotocore_kinesisanalytics/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      968 2023-12-13 19:48:35.000000 types-aiobotocore-kinesisanalytics-2.9.0/types_aiobotocore_kinesisanalytics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17022 2023-12-13 19:48:35.000000 types-aiobotocore-kinesisanalytics-2.9.0/types_aiobotocore_kinesisanalytics/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    17019 2023-12-13 19:48:35.000000 types-aiobotocore-kinesisanalytics-2.9.0/types_aiobotocore_kinesisanalytics/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9041 2023-12-13 19:48:35.000000 types-aiobotocore-kinesisanalytics-2.9.0/types_aiobotocore_kinesisanalytics/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9039 2023-12-13 19:48:35.000000 types-aiobotocore-kinesisanalytics-2.9.0/types_aiobotocore_kinesisanalytics/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:48:35.000000 types-aiobotocore-kinesisanalytics-2.9.0/types_aiobotocore_kinesisanalytics/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    23337 2023-12-13 19:48:35.000000 types-aiobotocore-kinesisanalytics-2.9.0/types_aiobotocore_kinesisanalytics/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    23336 2023-12-13 19:48:35.000000 types-aiobotocore-kinesisanalytics-2.9.0/types_aiobotocore_kinesisanalytics/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:48:35.000000 types-aiobotocore-kinesisanalytics-2.9.0/types_aiobotocore_kinesisanalytics/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:41.093563 types-aiobotocore-kinesisanalytics-2.9.0/types_aiobotocore_kinesisanalytics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12730 2023-12-13 19:59:41.000000 types-aiobotocore-kinesisanalytics-2.9.0/types_aiobotocore_kinesisanalytics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      887 2023-12-13 19:59:41.000000 types-aiobotocore-kinesisanalytics-2.9.0/types_aiobotocore_kinesisanalytics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:41.000000 types-aiobotocore-kinesisanalytics-2.9.0/types_aiobotocore_kinesisanalytics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:41.000000 types-aiobotocore-kinesisanalytics-2.9.0/types_aiobotocore_kinesisanalytics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:41.000000 types-aiobotocore-kinesisanalytics-2.9.0/types_aiobotocore_kinesisanalytics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-13 19:59:41.000000 types-aiobotocore-kinesisanalytics-2.9.0/types_aiobotocore_kinesisanalytics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:03.861237 types-aiobotocore-kinesisanalytics-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:10:23.000000 types-aiobotocore-kinesisanalytics-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12750 2024-01-18 01:21:03.861237 types-aiobotocore-kinesisanalytics-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11131 2024-01-18 01:10:23.000000 types-aiobotocore-kinesisanalytics-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:03.861237 types-aiobotocore-kinesisanalytics-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-01-18 01:10:23.000000 types-aiobotocore-kinesisanalytics-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:03.857237 types-aiobotocore-kinesisanalytics-2.9.1/types_aiobotocore_kinesisanalytics/
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-01-18 01:10:23.000000 types-aiobotocore-kinesisanalytics-2.9.1/types_aiobotocore_kinesisanalytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-01-18 01:10:23.000000 types-aiobotocore-kinesisanalytics-2.9.1/types_aiobotocore_kinesisanalytics/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-01-18 01:10:23.000000 types-aiobotocore-kinesisanalytics-2.9.1/types_aiobotocore_kinesisanalytics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17029 2024-01-18 01:10:23.000000 types-aiobotocore-kinesisanalytics-2.9.1/types_aiobotocore_kinesisanalytics/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17026 2024-01-18 01:10:23.000000 types-aiobotocore-kinesisanalytics-2.9.1/types_aiobotocore_kinesisanalytics/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9039 2024-01-18 01:10:23.000000 types-aiobotocore-kinesisanalytics-2.9.1/types_aiobotocore_kinesisanalytics/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9039 2024-01-18 01:10:23.000000 types-aiobotocore-kinesisanalytics-2.9.1/types_aiobotocore_kinesisanalytics/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:10:23.000000 types-aiobotocore-kinesisanalytics-2.9.1/types_aiobotocore_kinesisanalytics/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    23336 2024-01-18 01:10:24.000000 types-aiobotocore-kinesisanalytics-2.9.1/types_aiobotocore_kinesisanalytics/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23336 2024-01-18 01:10:24.000000 types-aiobotocore-kinesisanalytics-2.9.1/types_aiobotocore_kinesisanalytics/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:10:23.000000 types-aiobotocore-kinesisanalytics-2.9.1/types_aiobotocore_kinesisanalytics/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:03.861237 types-aiobotocore-kinesisanalytics-2.9.1/types_aiobotocore_kinesisanalytics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12750 2024-01-18 01:21:03.000000 types-aiobotocore-kinesisanalytics-2.9.1/types_aiobotocore_kinesisanalytics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-01-18 01:21:03.000000 types-aiobotocore-kinesisanalytics-2.9.1/types_aiobotocore_kinesisanalytics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:03.000000 types-aiobotocore-kinesisanalytics-2.9.1/types_aiobotocore_kinesisanalytics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:03.000000 types-aiobotocore-kinesisanalytics-2.9.1/types_aiobotocore_kinesisanalytics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:03.000000 types-aiobotocore-kinesisanalytics-2.9.1/types_aiobotocore_kinesisanalytics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-18 01:21:03.000000 types-aiobotocore-kinesisanalytics-2.9.1/types_aiobotocore_kinesisanalytics.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-kinesisanalytics-2.9.0/LICENSE` & `types-aiobotocore-kinesisanalytics-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-kinesisanalytics-2.9.0/PKG-INFO` & `types-aiobotocore-kinesisanalytics-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kinesisanalytics
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.KinesisAnalytics 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.KinesisAnalytics 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics/
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
 
 <a id="types-aiobotocore-kinesisanalytics"></a>
 
 # types-aiobotocore-kinesisanalytics
 
 [![PyPI - types-aiobotocore-kinesisanalytics](https://img.shields.io/pypi/v/types-aiobotocore-kinesisanalytics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesisanalytics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesisanalytics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesisanalytics)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kinesisanalytics)](https://pepy.tech/project/types-aiobotocore-kinesisanalytics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.KinesisAnalytics 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics)
+[aiobotocore.KinesisAnalytics 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics)
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
 [types-aiobotocore-kinesisanalytics docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-kinesisanalytics-2.9.0/README.md` & `types-aiobotocore-kinesisanalytics-2.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesisanalytics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesisanalytics)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kinesisanalytics)](https://pepy.tech/project/types-aiobotocore-kinesisanalytics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.KinesisAnalytics 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics)
+[aiobotocore.KinesisAnalytics 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics)
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
 [types-aiobotocore-kinesisanalytics docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-kinesisanalytics-2.9.0/setup.py` & `types-aiobotocore-kinesisanalytics-2.9.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-kinesisanalytics",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_kinesisanalytics"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.KinesisAnalytics 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.KinesisAnalytics 2.9.1 service generated with"
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
     keywords="aiobotocore kinesisanalytics type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_kinesisanalytics": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-kinesisanalytics-2.9.0/types_aiobotocore_kinesisanalytics/__init__.py` & `types-aiobotocore-kinesisanalytics-2.9.1/types_aiobotocore_kinesisanalytics/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,9 +18,8 @@
     ```
 """
 
 from .client import KinesisAnalyticsClient
 
 Client = KinesisAnalyticsClient
 
-
 __all__ = ("Client", "KinesisAnalyticsClient")
```

### Comparing `types-aiobotocore-kinesisanalytics-2.9.0/types_aiobotocore_kinesisanalytics/__init__.pyi` & `types-aiobotocore-kinesisanalytics-2.9.1/types_aiobotocore_kinesisanalytics/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisanalytics-2.9.0/types_aiobotocore_kinesisanalytics/__main__.py` & `types-aiobotocore-kinesisanalytics-2.9.1/types_aiobotocore_kinesisanalytics/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.KinesisAnalytics 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.KinesisAnalytics 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics\nOther"
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

### Comparing `types-aiobotocore-kinesisanalytics-2.9.0/types_aiobotocore_kinesisanalytics/client.py` & `types-aiobotocore-kinesisanalytics-2.9.1/types_aiobotocore_kinesisanalytics/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         """
 
     async def add_application_cloud_watch_logging_option(
         self,
         *,
         ApplicationName: str,
         CurrentApplicationVersionId: int,
-        CloudWatchLoggingOption: CloudWatchLoggingOptionTypeDef
+        CloudWatchLoggingOption: CloudWatchLoggingOptionTypeDef,
     ) -> Dict[str, Any]:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics.Client.add_application_cloud_watch_logging_option)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics/client/#add_application_cloud_watch_logging_option)
         """
@@ -109,15 +109,15 @@
 
     async def add_application_input_processing_configuration(
         self,
         *,
         ApplicationName: str,
         CurrentApplicationVersionId: int,
         InputId: str,
-        InputProcessingConfiguration: InputProcessingConfigurationTypeDef
+        InputProcessingConfiguration: InputProcessingConfigurationTypeDef,
     ) -> Dict[str, Any]:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics.Client.add_application_input_processing_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics/client/#add_application_input_processing_configuration)
         """
@@ -133,15 +133,15 @@
         """
 
     async def add_application_reference_data_source(
         self,
         *,
         ApplicationName: str,
         CurrentApplicationVersionId: int,
-        ReferenceDataSource: ReferenceDataSourceTypeDef
+        ReferenceDataSource: ReferenceDataSourceTypeDef,
     ) -> Dict[str, Any]:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics.Client.add_application_reference_data_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics/client/#add_application_reference_data_source)
         """
@@ -167,15 +167,15 @@
         *,
         ApplicationName: str,
         ApplicationDescription: str = ...,
         Inputs: Sequence[InputTypeDef] = ...,
         Outputs: Sequence[OutputTypeDef] = ...,
         CloudWatchLoggingOptions: Sequence[CloudWatchLoggingOptionTypeDef] = ...,
         ApplicationCode: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateApplicationResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics.Client.create_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics/client/#create_application)
         """
@@ -191,15 +191,15 @@
         """
 
     async def delete_application_cloud_watch_logging_option(
         self,
         *,
         ApplicationName: str,
         CurrentApplicationVersionId: int,
-        CloudWatchLoggingOptionId: str
+        CloudWatchLoggingOptionId: str,
     ) -> Dict[str, Any]:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics.Client.delete_application_cloud_watch_logging_option)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics/client/#delete_application_cloud_watch_logging_option)
         """
@@ -247,15 +247,15 @@
     async def discover_input_schema(
         self,
         *,
         ResourceARN: str = ...,
         RoleARN: str = ...,
         InputStartingPositionConfiguration: InputStartingPositionConfigurationTypeDef = ...,
         S3Configuration: S3ConfigurationTypeDef = ...,
-        InputProcessingConfiguration: InputProcessingConfigurationTypeDef = ...
+        InputProcessingConfiguration: InputProcessingConfigurationTypeDef = ...,
     ) -> DiscoverInputSchemaResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics.Client.discover_input_schema)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics/client/#discover_input_schema)
         """
@@ -329,15 +329,15 @@
         """
 
     async def update_application(
         self,
         *,
         ApplicationName: str,
         CurrentApplicationVersionId: int,
-        ApplicationUpdate: ApplicationUpdateTypeDef
+        ApplicationUpdate: ApplicationUpdateTypeDef,
     ) -> Dict[str, Any]:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics.Client.update_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics/client/#update_application)
         """
```

### Comparing `types-aiobotocore-kinesisanalytics-2.9.0/types_aiobotocore_kinesisanalytics/client.pyi` & `types-aiobotocore-kinesisanalytics-2.9.1/types_aiobotocore_kinesisanalytics/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         """
 
     async def add_application_cloud_watch_logging_option(
         self,
         *,
         ApplicationName: str,
         CurrentApplicationVersionId: int,
-        CloudWatchLoggingOption: CloudWatchLoggingOptionTypeDef
+        CloudWatchLoggingOption: CloudWatchLoggingOptionTypeDef,
     ) -> Dict[str, Any]:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics.Client.add_application_cloud_watch_logging_option)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics/client/#add_application_cloud_watch_logging_option)
         """
@@ -106,15 +106,15 @@
 
     async def add_application_input_processing_configuration(
         self,
         *,
         ApplicationName: str,
         CurrentApplicationVersionId: int,
         InputId: str,
-        InputProcessingConfiguration: InputProcessingConfigurationTypeDef
+        InputProcessingConfiguration: InputProcessingConfigurationTypeDef,
     ) -> Dict[str, Any]:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics.Client.add_application_input_processing_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics/client/#add_application_input_processing_configuration)
         """
@@ -130,15 +130,15 @@
         """
 
     async def add_application_reference_data_source(
         self,
         *,
         ApplicationName: str,
         CurrentApplicationVersionId: int,
-        ReferenceDataSource: ReferenceDataSourceTypeDef
+        ReferenceDataSource: ReferenceDataSourceTypeDef,
     ) -> Dict[str, Any]:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics.Client.add_application_reference_data_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics/client/#add_application_reference_data_source)
         """
@@ -164,15 +164,15 @@
         *,
         ApplicationName: str,
         ApplicationDescription: str = ...,
         Inputs: Sequence[InputTypeDef] = ...,
         Outputs: Sequence[OutputTypeDef] = ...,
         CloudWatchLoggingOptions: Sequence[CloudWatchLoggingOptionTypeDef] = ...,
         ApplicationCode: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateApplicationResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics.Client.create_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics/client/#create_application)
         """
@@ -188,15 +188,15 @@
         """
 
     async def delete_application_cloud_watch_logging_option(
         self,
         *,
         ApplicationName: str,
         CurrentApplicationVersionId: int,
-        CloudWatchLoggingOptionId: str
+        CloudWatchLoggingOptionId: str,
     ) -> Dict[str, Any]:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics.Client.delete_application_cloud_watch_logging_option)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics/client/#delete_application_cloud_watch_logging_option)
         """
@@ -244,15 +244,15 @@
     async def discover_input_schema(
         self,
         *,
         ResourceARN: str = ...,
         RoleARN: str = ...,
         InputStartingPositionConfiguration: InputStartingPositionConfigurationTypeDef = ...,
         S3Configuration: S3ConfigurationTypeDef = ...,
-        InputProcessingConfiguration: InputProcessingConfigurationTypeDef = ...
+        InputProcessingConfiguration: InputProcessingConfigurationTypeDef = ...,
     ) -> DiscoverInputSchemaResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics.Client.discover_input_schema)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics/client/#discover_input_schema)
         """
@@ -326,15 +326,15 @@
         """
 
     async def update_application(
         self,
         *,
         ApplicationName: str,
         CurrentApplicationVersionId: int,
-        ApplicationUpdate: ApplicationUpdateTypeDef
+        ApplicationUpdate: ApplicationUpdateTypeDef,
     ) -> Dict[str, Any]:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics.Client.update_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics/client/#update_application)
         """
```

### Comparing `types-aiobotocore-kinesisanalytics-2.9.0/types_aiobotocore_kinesisanalytics/literals.py` & `types-aiobotocore-kinesisanalytics-2.9.1/types_aiobotocore_kinesisanalytics/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,26 +15,24 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ApplicationStatusType",
     "InputStartingPositionType",
     "RecordFormatTypeType",
     "KinesisAnalyticsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 ApplicationStatusType = Literal["DELETING", "READY", "RUNNING", "STARTING", "STOPPING", "UPDATING"]
 InputStartingPositionType = Literal["LAST_STOPPED_POINT", "NOW", "TRIM_HORIZON"]
 RecordFormatTypeType = Literal["CSV", "JSON"]
 KinesisAnalyticsServiceName = Literal["kinesisanalytics"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
```

### Comparing `types-aiobotocore-kinesisanalytics-2.9.0/types_aiobotocore_kinesisanalytics/literals.pyi` & `types-aiobotocore-kinesisanalytics-2.9.1/types_aiobotocore_kinesisanalytics/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisanalytics-2.9.0/types_aiobotocore_kinesisanalytics/type_defs.py` & `types-aiobotocore-kinesisanalytics-2.9.1/types_aiobotocore_kinesisanalytics/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CloudWatchLoggingOptionTypeDef",
     "CloudWatchLoggingOptionDescriptionTypeDef",
     "ApplicationSummaryTypeDef",
     "CloudWatchLoggingOptionUpdateTypeDef",
     "CSVMappingParametersTypeDef",
     "TagTypeDef",
```

### Comparing `types-aiobotocore-kinesisanalytics-2.9.0/types_aiobotocore_kinesisanalytics/type_defs.pyi` & `types-aiobotocore-kinesisanalytics-2.9.1/types_aiobotocore_kinesisanalytics/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisanalytics-2.9.0/types_aiobotocore_kinesisanalytics.egg-info/PKG-INFO` & `types-aiobotocore-kinesisanalytics-2.9.1/types_aiobotocore_kinesisanalytics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kinesisanalytics
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.KinesisAnalytics 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.KinesisAnalytics 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics/
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
 
 <a id="types-aiobotocore-kinesisanalytics"></a>
 
 # types-aiobotocore-kinesisanalytics
 
 [![PyPI - types-aiobotocore-kinesisanalytics](https://img.shields.io/pypi/v/types-aiobotocore-kinesisanalytics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesisanalytics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesisanalytics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesisanalytics)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kinesisanalytics)](https://pepy.tech/project/types-aiobotocore-kinesisanalytics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.KinesisAnalytics 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics)
+[aiobotocore.KinesisAnalytics 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics)
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
 [types-aiobotocore-kinesisanalytics docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-kinesisanalytics-2.9.0/types_aiobotocore_kinesisanalytics.egg-info/SOURCES.txt` & `types-aiobotocore-kinesisanalytics-2.9.1/types_aiobotocore_kinesisanalytics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

