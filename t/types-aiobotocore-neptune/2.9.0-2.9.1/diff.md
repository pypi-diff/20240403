# Comparing `tmp/types-aiobotocore-neptune-2.9.0.tar.gz` & `tmp/types-aiobotocore-neptune-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-neptune-2.9.0.tar", last modified: Wed Dec 13 20:00:00 2023, max compression
+gzip compressed data, was "types-aiobotocore-neptune-2.9.1.tar", last modified: Thu Jan 18 01:21:21 2024, max compression
```

## Comparing `types-aiobotocore-neptune-2.9.0.tar` & `types-aiobotocore-neptune-2.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:00.577397 types-aiobotocore-neptune-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:50:45.000000 types-aiobotocore-neptune-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16696 2023-12-13 20:00:00.577397 types-aiobotocore-neptune-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15133 2023-12-13 19:50:45.000000 types-aiobotocore-neptune-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:00.577397 types-aiobotocore-neptune-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2023-12-13 19:50:45.000000 types-aiobotocore-neptune-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:00.577397 types-aiobotocore-neptune-2.9.0/types_aiobotocore_neptune/
--rw-r--r--   0 runner    (1001) docker     (127)     5034 2023-12-13 19:50:45.000000 types-aiobotocore-neptune-2.9.0/types_aiobotocore_neptune/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5033 2023-12-13 19:50:45.000000 types-aiobotocore-neptune-2.9.0/types_aiobotocore_neptune/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      932 2023-12-13 19:50:45.000000 types-aiobotocore-neptune-2.9.0/types_aiobotocore_neptune/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    70806 2023-12-13 19:50:46.000000 types-aiobotocore-neptune-2.9.0/types_aiobotocore_neptune/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    70802 2023-12-13 19:50:46.000000 types-aiobotocore-neptune-2.9.0/types_aiobotocore_neptune/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11850 2023-12-13 19:50:46.000000 types-aiobotocore-neptune-2.9.0/types_aiobotocore_neptune/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11848 2023-12-13 19:50:46.000000 types-aiobotocore-neptune-2.9.0/types_aiobotocore_neptune/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    22184 2023-12-13 19:50:46.000000 types-aiobotocore-neptune-2.9.0/types_aiobotocore_neptune/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    22166 2023-12-13 19:50:46.000000 types-aiobotocore-neptune-2.9.0/types_aiobotocore_neptune/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:50:45.000000 types-aiobotocore-neptune-2.9.0/types_aiobotocore_neptune/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    77905 2023-12-13 19:50:49.000000 types-aiobotocore-neptune-2.9.0/types_aiobotocore_neptune/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    77904 2023-12-13 19:50:47.000000 types-aiobotocore-neptune-2.9.0/types_aiobotocore_neptune/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:50:45.000000 types-aiobotocore-neptune-2.9.0/types_aiobotocore_neptune/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2023-12-13 19:50:46.000000 types-aiobotocore-neptune-2.9.0/types_aiobotocore_neptune/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2023-12-13 19:50:46.000000 types-aiobotocore-neptune-2.9.0/types_aiobotocore_neptune/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:00.577397 types-aiobotocore-neptune-2.9.0/types_aiobotocore_neptune.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16696 2023-12-13 20:00:00.000000 types-aiobotocore-neptune-2.9.0/types_aiobotocore_neptune.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      886 2023-12-13 20:00:00.000000 types-aiobotocore-neptune-2.9.0/types_aiobotocore_neptune.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:00.000000 types-aiobotocore-neptune-2.9.0/types_aiobotocore_neptune.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:00.000000 types-aiobotocore-neptune-2.9.0/types_aiobotocore_neptune.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:00.000000 types-aiobotocore-neptune-2.9.0/types_aiobotocore_neptune.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-13 20:00:00.000000 types-aiobotocore-neptune-2.9.0/types_aiobotocore_neptune.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:21.817155 types-aiobotocore-neptune-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:12:27.000000 types-aiobotocore-neptune-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16716 2024-01-18 01:21:21.817155 types-aiobotocore-neptune-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15133 2024-01-18 01:12:27.000000 types-aiobotocore-neptune-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:21.817155 types-aiobotocore-neptune-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-01-18 01:12:27.000000 types-aiobotocore-neptune-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:21.817155 types-aiobotocore-neptune-2.9.1/types_aiobotocore_neptune/
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-01-18 01:12:27.000000 types-aiobotocore-neptune-2.9.1/types_aiobotocore_neptune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-01-18 01:12:27.000000 types-aiobotocore-neptune-2.9.1/types_aiobotocore_neptune/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-01-18 01:12:27.000000 types-aiobotocore-neptune-2.9.1/types_aiobotocore_neptune/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70846 2024-01-18 01:12:28.000000 types-aiobotocore-neptune-2.9.1/types_aiobotocore_neptune/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70843 2024-01-18 01:12:27.000000 types-aiobotocore-neptune-2.9.1/types_aiobotocore_neptune/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11848 2024-01-18 01:12:28.000000 types-aiobotocore-neptune-2.9.1/types_aiobotocore_neptune/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11848 2024-01-18 01:12:28.000000 types-aiobotocore-neptune-2.9.1/types_aiobotocore_neptune/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    22198 2024-01-18 01:12:28.000000 types-aiobotocore-neptune-2.9.1/types_aiobotocore_neptune/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22181 2024-01-18 01:12:28.000000 types-aiobotocore-neptune-2.9.1/types_aiobotocore_neptune/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:12:27.000000 types-aiobotocore-neptune-2.9.1/types_aiobotocore_neptune/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    77904 2024-01-18 01:12:29.000000 types-aiobotocore-neptune-2.9.1/types_aiobotocore_neptune/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77904 2024-01-18 01:12:29.000000 types-aiobotocore-neptune-2.9.1/types_aiobotocore_neptune/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:12:27.000000 types-aiobotocore-neptune-2.9.1/types_aiobotocore_neptune/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-01-18 01:12:28.000000 types-aiobotocore-neptune-2.9.1/types_aiobotocore_neptune/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-01-18 01:12:28.000000 types-aiobotocore-neptune-2.9.1/types_aiobotocore_neptune/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:21.817155 types-aiobotocore-neptune-2.9.1/types_aiobotocore_neptune.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16716 2024-01-18 01:21:21.000000 types-aiobotocore-neptune-2.9.1/types_aiobotocore_neptune.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-01-18 01:21:21.000000 types-aiobotocore-neptune-2.9.1/types_aiobotocore_neptune.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:21.000000 types-aiobotocore-neptune-2.9.1/types_aiobotocore_neptune.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:21.000000 types-aiobotocore-neptune-2.9.1/types_aiobotocore_neptune.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:21.000000 types-aiobotocore-neptune-2.9.1/types_aiobotocore_neptune.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-01-18 01:21:21.000000 types-aiobotocore-neptune-2.9.1/types_aiobotocore_neptune.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-neptune-2.9.0/LICENSE` & `types-aiobotocore-neptune-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-neptune-2.9.0/PKG-INFO` & `types-aiobotocore-neptune-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-neptune
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Neptune 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Neptune 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/
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
 
 <a id="types-aiobotocore-neptune"></a>
 
 # types-aiobotocore-neptune
 
 [![PyPI - types-aiobotocore-neptune](https://img.shields.io/pypi/v/types-aiobotocore-neptune.svg?color=blue)](https://pypi.org/project/types-aiobotocore-neptune)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-neptune.svg?color=blue)](https://pypi.org/project/types-aiobotocore-neptune)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-neptune)](https://pepy.tech/project/types-aiobotocore-neptune)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Neptune 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune)
+[aiobotocore.Neptune 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune)
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
 [types-aiobotocore-neptune docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-neptune-2.9.0/README.md` & `types-aiobotocore-neptune-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-neptune.svg?color=blue)](https://pypi.org/project/types-aiobotocore-neptune)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-neptune)](https://pepy.tech/project/types-aiobotocore-neptune)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Neptune 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune)
+[aiobotocore.Neptune 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune)
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
 [types-aiobotocore-neptune docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-neptune-2.9.0/setup.py` & `types-aiobotocore-neptune-2.9.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-neptune",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_neptune"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Neptune 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.Neptune 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore neptune type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_neptune": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-neptune-2.9.0/types_aiobotocore_neptune/__init__.py` & `types-aiobotocore-neptune-2.9.1/types_aiobotocore_neptune/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,14 @@
     DescribeOrderableDBInstanceOptionsPaginator,
     DescribePendingMaintenanceActionsPaginator,
 )
 from .waiter import DBInstanceAvailableWaiter, DBInstanceDeletedWaiter
 
 Client = NeptuneClient
 
-
 __all__ = (
     "Client",
     "DBInstanceAvailableWaiter",
     "DBInstanceDeletedWaiter",
     "DescribeDBClusterEndpointsPaginator",
     "DescribeDBClusterParameterGroupsPaginator",
     "DescribeDBClusterParametersPaginator",
```

### Comparing `types-aiobotocore-neptune-2.9.0/types_aiobotocore_neptune/__init__.pyi` & `types-aiobotocore-neptune-2.9.1/types_aiobotocore_neptune/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-neptune-2.9.0/types_aiobotocore_neptune/__main__.py` & `types-aiobotocore-neptune-2.9.1/types_aiobotocore_neptune/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Neptune 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Neptune 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune\nOther"
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

### Comparing `types-aiobotocore-neptune-2.9.0/types_aiobotocore_neptune/client.py` & `types-aiobotocore-neptune-2.9.1/types_aiobotocore_neptune/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,14 @@
 from .waiter import DBInstanceAvailableWaiter, DBInstanceDeletedWaiter
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("NeptuneClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -276,15 +275,15 @@
 
     async def copy_db_cluster_parameter_group(
         self,
         *,
         SourceDBClusterParameterGroupIdentifier: str,
         TargetDBClusterParameterGroupIdentifier: str,
         TargetDBClusterParameterGroupDescription: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CopyDBClusterParameterGroupResultTypeDef:
         """
         Copies the specified DB cluster parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.copy_db_cluster_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#copy_db_cluster_parameter_group)
         """
@@ -294,30 +293,30 @@
         *,
         SourceDBClusterSnapshotIdentifier: str,
         TargetDBClusterSnapshotIdentifier: str,
         KmsKeyId: str = ...,
         PreSignedUrl: str = ...,
         CopyTags: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        SourceRegion: str = ...
+        SourceRegion: str = ...,
     ) -> CopyDBClusterSnapshotResultTypeDef:
         """
         Copies a snapshot of a DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.copy_db_cluster_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#copy_db_cluster_snapshot)
         """
 
     async def copy_db_parameter_group(
         self,
         *,
         SourceDBParameterGroupIdentifier: str,
         TargetDBParameterGroupIdentifier: str,
         TargetDBParameterGroupDescription: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CopyDBParameterGroupResultTypeDef:
         """
         Copies the specified DB parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.copy_db_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#copy_db_parameter_group)
         """
@@ -349,15 +348,15 @@
         PreSignedUrl: str = ...,
         EnableIAMDatabaseAuthentication: bool = ...,
         EnableCloudwatchLogsExports: Sequence[str] = ...,
         DeletionProtection: bool = ...,
         ServerlessV2ScalingConfiguration: ServerlessV2ScalingConfigurationTypeDef = ...,
         GlobalClusterIdentifier: str = ...,
         StorageType: str = ...,
-        SourceRegion: str = ...
+        SourceRegion: str = ...,
     ) -> CreateDBClusterResultTypeDef:
         """
         Creates a new Amazon Neptune DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.create_db_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#create_db_cluster)
         """
@@ -366,15 +365,15 @@
         self,
         *,
         DBClusterIdentifier: str,
         DBClusterEndpointIdentifier: str,
         EndpointType: str,
         StaticMembers: Sequence[str] = ...,
         ExcludedMembers: Sequence[str] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDBClusterEndpointOutputTypeDef:
         """
         Creates a new custom endpoint and associates it with an Amazon Neptune DB
         cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.create_db_cluster_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#create_db_cluster_endpoint)
@@ -382,29 +381,29 @@
 
     async def create_db_cluster_parameter_group(
         self,
         *,
         DBClusterParameterGroupName: str,
         DBParameterGroupFamily: str,
         Description: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDBClusterParameterGroupResultTypeDef:
         """
         Creates a new DB cluster parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.create_db_cluster_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#create_db_cluster_parameter_group)
         """
 
     async def create_db_cluster_snapshot(
         self,
         *,
         DBClusterSnapshotIdentifier: str,
         DBClusterIdentifier: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDBClusterSnapshotResultTypeDef:
         """
         Creates a snapshot of a DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.create_db_cluster_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#create_db_cluster_snapshot)
         """
@@ -450,45 +449,45 @@
         DomainIAMRoleName: str = ...,
         PromotionTier: int = ...,
         Timezone: str = ...,
         EnableIAMDatabaseAuthentication: bool = ...,
         EnablePerformanceInsights: bool = ...,
         PerformanceInsightsKMSKeyId: str = ...,
         EnableCloudwatchLogsExports: Sequence[str] = ...,
-        DeletionProtection: bool = ...
+        DeletionProtection: bool = ...,
     ) -> CreateDBInstanceResultTypeDef:
         """
         Creates a new DB instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.create_db_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#create_db_instance)
         """
 
     async def create_db_parameter_group(
         self,
         *,
         DBParameterGroupName: str,
         DBParameterGroupFamily: str,
         Description: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDBParameterGroupResultTypeDef:
         """
         Creates a new DB parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.create_db_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#create_db_parameter_group)
         """
 
     async def create_db_subnet_group(
         self,
         *,
         DBSubnetGroupName: str,
         DBSubnetGroupDescription: str,
         SubnetIds: Sequence[str],
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDBSubnetGroupResultTypeDef:
         """
         Creates a new DB subnet group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.create_db_subnet_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#create_db_subnet_group)
         """
@@ -498,15 +497,15 @@
         *,
         SubscriptionName: str,
         SnsTopicArn: str,
         SourceType: str = ...,
         EventCategories: Sequence[str] = ...,
         SourceIds: Sequence[str] = ...,
         Enabled: bool = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateEventSubscriptionResultTypeDef:
         """
         Creates an event notification subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.create_event_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#create_event_subscription)
         """
@@ -515,29 +514,29 @@
         self,
         *,
         GlobalClusterIdentifier: str,
         SourceDBClusterIdentifier: str = ...,
         Engine: str = ...,
         EngineVersion: str = ...,
         DeletionProtection: bool = ...,
-        StorageEncrypted: bool = ...
+        StorageEncrypted: bool = ...,
     ) -> CreateGlobalClusterResultTypeDef:
         """
         Creates a Neptune global database spread across multiple Amazon Regions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.create_global_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#create_global_cluster)
         """
 
     async def delete_db_cluster(
         self,
         *,
         DBClusterIdentifier: str,
         SkipFinalSnapshot: bool = ...,
-        FinalDBSnapshotIdentifier: str = ...
+        FinalDBSnapshotIdentifier: str = ...,
     ) -> DeleteDBClusterResultTypeDef:
         """
         The DeleteDBCluster action deletes a previously provisioned DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.delete_db_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#delete_db_cluster)
         """
@@ -573,15 +572,15 @@
         """
 
     async def delete_db_instance(
         self,
         *,
         DBInstanceIdentifier: str,
         SkipFinalSnapshot: bool = ...,
-        FinalDBSnapshotIdentifier: str = ...
+        FinalDBSnapshotIdentifier: str = ...,
     ) -> DeleteDBInstanceResultTypeDef:
         """
         The DeleteDBInstance action deletes a previously provisioned DB instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.delete_db_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#delete_db_instance)
         """
@@ -629,30 +628,30 @@
     async def describe_db_cluster_endpoints(
         self,
         *,
         DBClusterIdentifier: str = ...,
         DBClusterEndpointIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DBClusterEndpointMessageTypeDef:
         """
         Returns information about endpoints for an Amazon Neptune DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.describe_db_cluster_endpoints)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#describe_db_cluster_endpoints)
         """
 
     async def describe_db_cluster_parameter_groups(
         self,
         *,
         DBClusterParameterGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DBClusterParameterGroupsMessageTypeDef:
         """
         Returns a list of `DBClusterParameterGroup` descriptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.describe_db_cluster_parameter_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#describe_db_cluster_parameter_groups)
         """
@@ -660,15 +659,15 @@
     async def describe_db_cluster_parameters(
         self,
         *,
         DBClusterParameterGroupName: str,
         Source: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DBClusterParameterGroupDetailsTypeDef:
         """
         Returns the detailed parameter list for a particular DB cluster parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.describe_db_cluster_parameters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#describe_db_cluster_parameters)
         """
@@ -691,30 +690,30 @@
         DBClusterIdentifier: str = ...,
         DBClusterSnapshotIdentifier: str = ...,
         SnapshotType: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         IncludeShared: bool = ...,
-        IncludePublic: bool = ...
+        IncludePublic: bool = ...,
     ) -> DBClusterSnapshotMessageTypeDef:
         """
         Returns information about DB cluster snapshots.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.describe_db_cluster_snapshots)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#describe_db_cluster_snapshots)
         """
 
     async def describe_db_clusters(
         self,
         *,
         DBClusterIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DBClusterMessageTypeDef:
         """
         Returns information about provisioned DB clusters, and supports pagination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.describe_db_clusters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#describe_db_clusters)
         """
@@ -726,45 +725,45 @@
         EngineVersion: str = ...,
         DBParameterGroupFamily: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         DefaultOnly: bool = ...,
         ListSupportedCharacterSets: bool = ...,
-        ListSupportedTimezones: bool = ...
+        ListSupportedTimezones: bool = ...,
     ) -> DBEngineVersionMessageTypeDef:
         """
         Returns a list of the available DB engines.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.describe_db_engine_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#describe_db_engine_versions)
         """
 
     async def describe_db_instances(
         self,
         *,
         DBInstanceIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DBInstanceMessageTypeDef:
         """
         Returns information about provisioned instances, and supports pagination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.describe_db_instances)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#describe_db_instances)
         """
 
     async def describe_db_parameter_groups(
         self,
         *,
         DBParameterGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DBParameterGroupsMessageTypeDef:
         """
         Returns a list of `DBParameterGroup` descriptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.describe_db_parameter_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#describe_db_parameter_groups)
         """
@@ -772,45 +771,45 @@
     async def describe_db_parameters(
         self,
         *,
         DBParameterGroupName: str,
         Source: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DBParameterGroupDetailsTypeDef:
         """
         Returns the detailed parameter list for a particular DB parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.describe_db_parameters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#describe_db_parameters)
         """
 
     async def describe_db_subnet_groups(
         self,
         *,
         DBSubnetGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DBSubnetGroupMessageTypeDef:
         """
         Returns a list of DBSubnetGroup descriptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.describe_db_subnet_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#describe_db_subnet_groups)
         """
 
     async def describe_engine_default_cluster_parameters(
         self,
         *,
         DBParameterGroupFamily: str,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DescribeEngineDefaultClusterParametersResultTypeDef:
         """
         Returns the default engine and system parameter information for the cluster
         database
         engine.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.describe_engine_default_cluster_parameters)
@@ -819,15 +818,15 @@
 
     async def describe_engine_default_parameters(
         self,
         *,
         DBParameterGroupFamily: str,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DescribeEngineDefaultParametersResultTypeDef:
         """
         Returns the default engine and system parameter information for the specified
         database
         engine.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.describe_engine_default_parameters)
@@ -848,15 +847,15 @@
 
     async def describe_event_subscriptions(
         self,
         *,
         SubscriptionName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> EventSubscriptionsMessageTypeDef:
         """
         Lists all the subscription descriptions for a customer account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.describe_event_subscriptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#describe_event_subscriptions)
         """
@@ -868,15 +867,15 @@
         SourceType: SourceTypeType = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         Duration: int = ...,
         EventCategories: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> EventsMessageTypeDef:
         """
         Returns events related to DB instances, DB security groups, DB snapshots, and
         DB parameter groups for the past 14
         days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.describe_events)
@@ -899,30 +898,30 @@
         Engine: str,
         EngineVersion: str = ...,
         DBInstanceClass: str = ...,
         LicenseModel: str = ...,
         Vpc: bool = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> OrderableDBInstanceOptionsMessageTypeDef:
         """
         Returns a list of orderable DB instance options for the specified engine.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.describe_orderable_db_instance_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#describe_orderable_db_instance_options)
         """
 
     async def describe_pending_maintenance_actions(
         self,
         *,
         ResourceIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         Marker: str = ...,
-        MaxRecords: int = ...
+        MaxRecords: int = ...,
     ) -> PendingMaintenanceActionsMessageTypeDef:
         """
         Returns a list of resources (for example, DB instances) that have at least one
         pending maintenance
         action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.describe_pending_maintenance_actions)
@@ -1003,30 +1002,30 @@
         CloudwatchLogsExportConfiguration: CloudwatchLogsExportConfigurationTypeDef = ...,
         EngineVersion: str = ...,
         AllowMajorVersionUpgrade: bool = ...,
         DBInstanceParameterGroupName: str = ...,
         DeletionProtection: bool = ...,
         CopyTagsToSnapshot: bool = ...,
         ServerlessV2ScalingConfiguration: ServerlessV2ScalingConfigurationTypeDef = ...,
-        StorageType: str = ...
+        StorageType: str = ...,
     ) -> ModifyDBClusterResultTypeDef:
         """
         Modify a setting for a DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.modify_db_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#modify_db_cluster)
         """
 
     async def modify_db_cluster_endpoint(
         self,
         *,
         DBClusterEndpointIdentifier: str,
         EndpointType: str = ...,
         StaticMembers: Sequence[str] = ...,
-        ExcludedMembers: Sequence[str] = ...
+        ExcludedMembers: Sequence[str] = ...,
     ) -> ModifyDBClusterEndpointOutputTypeDef:
         """
         Modifies the properties of an endpoint in an Amazon Neptune DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.modify_db_cluster_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#modify_db_cluster_endpoint)
         """
@@ -1043,15 +1042,15 @@
 
     async def modify_db_cluster_snapshot_attribute(
         self,
         *,
         DBClusterSnapshotIdentifier: str,
         AttributeName: str,
         ValuesToAdd: Sequence[str] = ...,
-        ValuesToRemove: Sequence[str] = ...
+        ValuesToRemove: Sequence[str] = ...,
     ) -> ModifyDBClusterSnapshotAttributeResultTypeDef:
         """
         Adds an attribute and values to, or removes an attribute and values from, a
         manual DB cluster
         snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.modify_db_cluster_snapshot_attribute)
@@ -1093,15 +1092,15 @@
         MonitoringRoleArn: str = ...,
         DomainIAMRoleName: str = ...,
         PromotionTier: int = ...,
         EnableIAMDatabaseAuthentication: bool = ...,
         EnablePerformanceInsights: bool = ...,
         PerformanceInsightsKMSKeyId: str = ...,
         CloudwatchLogsExportConfiguration: CloudwatchLogsExportConfigurationTypeDef = ...,
-        DeletionProtection: bool = ...
+        DeletionProtection: bool = ...,
     ) -> ModifyDBInstanceResultTypeDef:
         """
         Modifies settings for a DB instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.modify_db_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#modify_db_instance)
         """
@@ -1117,15 +1116,15 @@
         """
 
     async def modify_db_subnet_group(
         self,
         *,
         DBSubnetGroupName: str,
         SubnetIds: Sequence[str],
-        DBSubnetGroupDescription: str = ...
+        DBSubnetGroupDescription: str = ...,
     ) -> ModifyDBSubnetGroupResultTypeDef:
         """
         Modifies an existing DB subnet group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.modify_db_subnet_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#modify_db_subnet_group)
         """
@@ -1133,15 +1132,15 @@
     async def modify_event_subscription(
         self,
         *,
         SubscriptionName: str,
         SnsTopicArn: str = ...,
         SourceType: str = ...,
         EventCategories: Sequence[str] = ...,
-        Enabled: bool = ...
+        Enabled: bool = ...,
     ) -> ModifyEventSubscriptionResultTypeDef:
         """
         Modifies an existing event notification subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.modify_event_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#modify_event_subscription)
         """
@@ -1149,15 +1148,15 @@
     async def modify_global_cluster(
         self,
         *,
         GlobalClusterIdentifier: str,
         NewGlobalClusterIdentifier: str = ...,
         DeletionProtection: bool = ...,
         EngineVersion: str = ...,
-        AllowMajorVersionUpgrade: bool = ...
+        AllowMajorVersionUpgrade: bool = ...,
     ) -> ModifyGlobalClusterResultTypeDef:
         """
         Modify a setting for an Amazon Neptune global cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.modify_global_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#modify_global_cluster)
         """
@@ -1223,29 +1222,29 @@
         """
 
     async def reset_db_cluster_parameter_group(
         self,
         *,
         DBClusterParameterGroupName: str,
         ResetAllParameters: bool = ...,
-        Parameters: Sequence[ParameterTypeDef] = ...
+        Parameters: Sequence[ParameterTypeDef] = ...,
     ) -> DBClusterParameterGroupNameMessageTypeDef:
         """
         Modifies the parameters of a DB cluster parameter group to the default value.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.reset_db_cluster_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#reset_db_cluster_parameter_group)
         """
 
     async def reset_db_parameter_group(
         self,
         *,
         DBParameterGroupName: str,
         ResetAllParameters: bool = ...,
-        Parameters: Sequence[ParameterTypeDef] = ...
+        Parameters: Sequence[ParameterTypeDef] = ...,
     ) -> DBParameterGroupNameMessageTypeDef:
         """
         Modifies the parameters of a DB parameter group to the engine/system default
         value.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.reset_db_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#reset_db_parameter_group)
@@ -1268,15 +1267,15 @@
         KmsKeyId: str = ...,
         EnableIAMDatabaseAuthentication: bool = ...,
         EnableCloudwatchLogsExports: Sequence[str] = ...,
         DBClusterParameterGroupName: str = ...,
         DeletionProtection: bool = ...,
         CopyTagsToSnapshot: bool = ...,
         ServerlessV2ScalingConfiguration: ServerlessV2ScalingConfigurationTypeDef = ...,
-        StorageType: str = ...
+        StorageType: str = ...,
     ) -> RestoreDBClusterFromSnapshotResultTypeDef:
         """
         Creates a new DB cluster from a DB snapshot or DB cluster snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.restore_db_cluster_from_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#restore_db_cluster_from_snapshot)
         """
@@ -1296,15 +1295,15 @@
         Tags: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...,
         EnableIAMDatabaseAuthentication: bool = ...,
         EnableCloudwatchLogsExports: Sequence[str] = ...,
         DBClusterParameterGroupName: str = ...,
         DeletionProtection: bool = ...,
         ServerlessV2ScalingConfiguration: ServerlessV2ScalingConfigurationTypeDef = ...,
-        StorageType: str = ...
+        StorageType: str = ...,
     ) -> RestoreDBClusterToPointInTimeResultTypeDef:
         """
         Restores a DB cluster to an arbitrary point in time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.restore_db_cluster_to_point_in_time)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#restore_db_cluster_to_point_in_time)
         """
```

### Comparing `types-aiobotocore-neptune-2.9.0/types_aiobotocore_neptune/client.pyi` & `types-aiobotocore-neptune-2.9.1/types_aiobotocore_neptune/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -272,15 +272,15 @@
 
     async def copy_db_cluster_parameter_group(
         self,
         *,
         SourceDBClusterParameterGroupIdentifier: str,
         TargetDBClusterParameterGroupIdentifier: str,
         TargetDBClusterParameterGroupDescription: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CopyDBClusterParameterGroupResultTypeDef:
         """
         Copies the specified DB cluster parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.copy_db_cluster_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#copy_db_cluster_parameter_group)
         """
@@ -290,30 +290,30 @@
         *,
         SourceDBClusterSnapshotIdentifier: str,
         TargetDBClusterSnapshotIdentifier: str,
         KmsKeyId: str = ...,
         PreSignedUrl: str = ...,
         CopyTags: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        SourceRegion: str = ...
+        SourceRegion: str = ...,
     ) -> CopyDBClusterSnapshotResultTypeDef:
         """
         Copies a snapshot of a DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.copy_db_cluster_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#copy_db_cluster_snapshot)
         """
 
     async def copy_db_parameter_group(
         self,
         *,
         SourceDBParameterGroupIdentifier: str,
         TargetDBParameterGroupIdentifier: str,
         TargetDBParameterGroupDescription: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CopyDBParameterGroupResultTypeDef:
         """
         Copies the specified DB parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.copy_db_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#copy_db_parameter_group)
         """
@@ -345,15 +345,15 @@
         PreSignedUrl: str = ...,
         EnableIAMDatabaseAuthentication: bool = ...,
         EnableCloudwatchLogsExports: Sequence[str] = ...,
         DeletionProtection: bool = ...,
         ServerlessV2ScalingConfiguration: ServerlessV2ScalingConfigurationTypeDef = ...,
         GlobalClusterIdentifier: str = ...,
         StorageType: str = ...,
-        SourceRegion: str = ...
+        SourceRegion: str = ...,
     ) -> CreateDBClusterResultTypeDef:
         """
         Creates a new Amazon Neptune DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.create_db_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#create_db_cluster)
         """
@@ -362,15 +362,15 @@
         self,
         *,
         DBClusterIdentifier: str,
         DBClusterEndpointIdentifier: str,
         EndpointType: str,
         StaticMembers: Sequence[str] = ...,
         ExcludedMembers: Sequence[str] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDBClusterEndpointOutputTypeDef:
         """
         Creates a new custom endpoint and associates it with an Amazon Neptune DB
         cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.create_db_cluster_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#create_db_cluster_endpoint)
@@ -378,29 +378,29 @@
 
     async def create_db_cluster_parameter_group(
         self,
         *,
         DBClusterParameterGroupName: str,
         DBParameterGroupFamily: str,
         Description: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDBClusterParameterGroupResultTypeDef:
         """
         Creates a new DB cluster parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.create_db_cluster_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#create_db_cluster_parameter_group)
         """
 
     async def create_db_cluster_snapshot(
         self,
         *,
         DBClusterSnapshotIdentifier: str,
         DBClusterIdentifier: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDBClusterSnapshotResultTypeDef:
         """
         Creates a snapshot of a DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.create_db_cluster_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#create_db_cluster_snapshot)
         """
@@ -446,45 +446,45 @@
         DomainIAMRoleName: str = ...,
         PromotionTier: int = ...,
         Timezone: str = ...,
         EnableIAMDatabaseAuthentication: bool = ...,
         EnablePerformanceInsights: bool = ...,
         PerformanceInsightsKMSKeyId: str = ...,
         EnableCloudwatchLogsExports: Sequence[str] = ...,
-        DeletionProtection: bool = ...
+        DeletionProtection: bool = ...,
     ) -> CreateDBInstanceResultTypeDef:
         """
         Creates a new DB instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.create_db_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#create_db_instance)
         """
 
     async def create_db_parameter_group(
         self,
         *,
         DBParameterGroupName: str,
         DBParameterGroupFamily: str,
         Description: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDBParameterGroupResultTypeDef:
         """
         Creates a new DB parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.create_db_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#create_db_parameter_group)
         """
 
     async def create_db_subnet_group(
         self,
         *,
         DBSubnetGroupName: str,
         DBSubnetGroupDescription: str,
         SubnetIds: Sequence[str],
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDBSubnetGroupResultTypeDef:
         """
         Creates a new DB subnet group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.create_db_subnet_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#create_db_subnet_group)
         """
@@ -494,15 +494,15 @@
         *,
         SubscriptionName: str,
         SnsTopicArn: str,
         SourceType: str = ...,
         EventCategories: Sequence[str] = ...,
         SourceIds: Sequence[str] = ...,
         Enabled: bool = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateEventSubscriptionResultTypeDef:
         """
         Creates an event notification subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.create_event_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#create_event_subscription)
         """
@@ -511,29 +511,29 @@
         self,
         *,
         GlobalClusterIdentifier: str,
         SourceDBClusterIdentifier: str = ...,
         Engine: str = ...,
         EngineVersion: str = ...,
         DeletionProtection: bool = ...,
-        StorageEncrypted: bool = ...
+        StorageEncrypted: bool = ...,
     ) -> CreateGlobalClusterResultTypeDef:
         """
         Creates a Neptune global database spread across multiple Amazon Regions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.create_global_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#create_global_cluster)
         """
 
     async def delete_db_cluster(
         self,
         *,
         DBClusterIdentifier: str,
         SkipFinalSnapshot: bool = ...,
-        FinalDBSnapshotIdentifier: str = ...
+        FinalDBSnapshotIdentifier: str = ...,
     ) -> DeleteDBClusterResultTypeDef:
         """
         The DeleteDBCluster action deletes a previously provisioned DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.delete_db_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#delete_db_cluster)
         """
@@ -569,15 +569,15 @@
         """
 
     async def delete_db_instance(
         self,
         *,
         DBInstanceIdentifier: str,
         SkipFinalSnapshot: bool = ...,
-        FinalDBSnapshotIdentifier: str = ...
+        FinalDBSnapshotIdentifier: str = ...,
     ) -> DeleteDBInstanceResultTypeDef:
         """
         The DeleteDBInstance action deletes a previously provisioned DB instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.delete_db_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#delete_db_instance)
         """
@@ -625,30 +625,30 @@
     async def describe_db_cluster_endpoints(
         self,
         *,
         DBClusterIdentifier: str = ...,
         DBClusterEndpointIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DBClusterEndpointMessageTypeDef:
         """
         Returns information about endpoints for an Amazon Neptune DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.describe_db_cluster_endpoints)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#describe_db_cluster_endpoints)
         """
 
     async def describe_db_cluster_parameter_groups(
         self,
         *,
         DBClusterParameterGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DBClusterParameterGroupsMessageTypeDef:
         """
         Returns a list of `DBClusterParameterGroup` descriptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.describe_db_cluster_parameter_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#describe_db_cluster_parameter_groups)
         """
@@ -656,15 +656,15 @@
     async def describe_db_cluster_parameters(
         self,
         *,
         DBClusterParameterGroupName: str,
         Source: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DBClusterParameterGroupDetailsTypeDef:
         """
         Returns the detailed parameter list for a particular DB cluster parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.describe_db_cluster_parameters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#describe_db_cluster_parameters)
         """
@@ -687,30 +687,30 @@
         DBClusterIdentifier: str = ...,
         DBClusterSnapshotIdentifier: str = ...,
         SnapshotType: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         IncludeShared: bool = ...,
-        IncludePublic: bool = ...
+        IncludePublic: bool = ...,
     ) -> DBClusterSnapshotMessageTypeDef:
         """
         Returns information about DB cluster snapshots.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.describe_db_cluster_snapshots)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#describe_db_cluster_snapshots)
         """
 
     async def describe_db_clusters(
         self,
         *,
         DBClusterIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DBClusterMessageTypeDef:
         """
         Returns information about provisioned DB clusters, and supports pagination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.describe_db_clusters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#describe_db_clusters)
         """
@@ -722,45 +722,45 @@
         EngineVersion: str = ...,
         DBParameterGroupFamily: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         DefaultOnly: bool = ...,
         ListSupportedCharacterSets: bool = ...,
-        ListSupportedTimezones: bool = ...
+        ListSupportedTimezones: bool = ...,
     ) -> DBEngineVersionMessageTypeDef:
         """
         Returns a list of the available DB engines.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.describe_db_engine_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#describe_db_engine_versions)
         """
 
     async def describe_db_instances(
         self,
         *,
         DBInstanceIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DBInstanceMessageTypeDef:
         """
         Returns information about provisioned instances, and supports pagination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.describe_db_instances)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#describe_db_instances)
         """
 
     async def describe_db_parameter_groups(
         self,
         *,
         DBParameterGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DBParameterGroupsMessageTypeDef:
         """
         Returns a list of `DBParameterGroup` descriptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.describe_db_parameter_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#describe_db_parameter_groups)
         """
@@ -768,45 +768,45 @@
     async def describe_db_parameters(
         self,
         *,
         DBParameterGroupName: str,
         Source: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DBParameterGroupDetailsTypeDef:
         """
         Returns the detailed parameter list for a particular DB parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.describe_db_parameters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#describe_db_parameters)
         """
 
     async def describe_db_subnet_groups(
         self,
         *,
         DBSubnetGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DBSubnetGroupMessageTypeDef:
         """
         Returns a list of DBSubnetGroup descriptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.describe_db_subnet_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#describe_db_subnet_groups)
         """
 
     async def describe_engine_default_cluster_parameters(
         self,
         *,
         DBParameterGroupFamily: str,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DescribeEngineDefaultClusterParametersResultTypeDef:
         """
         Returns the default engine and system parameter information for the cluster
         database
         engine.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.describe_engine_default_cluster_parameters)
@@ -815,15 +815,15 @@
 
     async def describe_engine_default_parameters(
         self,
         *,
         DBParameterGroupFamily: str,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DescribeEngineDefaultParametersResultTypeDef:
         """
         Returns the default engine and system parameter information for the specified
         database
         engine.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.describe_engine_default_parameters)
@@ -844,15 +844,15 @@
 
     async def describe_event_subscriptions(
         self,
         *,
         SubscriptionName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> EventSubscriptionsMessageTypeDef:
         """
         Lists all the subscription descriptions for a customer account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.describe_event_subscriptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#describe_event_subscriptions)
         """
@@ -864,15 +864,15 @@
         SourceType: SourceTypeType = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         Duration: int = ...,
         EventCategories: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> EventsMessageTypeDef:
         """
         Returns events related to DB instances, DB security groups, DB snapshots, and
         DB parameter groups for the past 14
         days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.describe_events)
@@ -895,30 +895,30 @@
         Engine: str,
         EngineVersion: str = ...,
         DBInstanceClass: str = ...,
         LicenseModel: str = ...,
         Vpc: bool = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> OrderableDBInstanceOptionsMessageTypeDef:
         """
         Returns a list of orderable DB instance options for the specified engine.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.describe_orderable_db_instance_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#describe_orderable_db_instance_options)
         """
 
     async def describe_pending_maintenance_actions(
         self,
         *,
         ResourceIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         Marker: str = ...,
-        MaxRecords: int = ...
+        MaxRecords: int = ...,
     ) -> PendingMaintenanceActionsMessageTypeDef:
         """
         Returns a list of resources (for example, DB instances) that have at least one
         pending maintenance
         action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.describe_pending_maintenance_actions)
@@ -999,30 +999,30 @@
         CloudwatchLogsExportConfiguration: CloudwatchLogsExportConfigurationTypeDef = ...,
         EngineVersion: str = ...,
         AllowMajorVersionUpgrade: bool = ...,
         DBInstanceParameterGroupName: str = ...,
         DeletionProtection: bool = ...,
         CopyTagsToSnapshot: bool = ...,
         ServerlessV2ScalingConfiguration: ServerlessV2ScalingConfigurationTypeDef = ...,
-        StorageType: str = ...
+        StorageType: str = ...,
     ) -> ModifyDBClusterResultTypeDef:
         """
         Modify a setting for a DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.modify_db_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#modify_db_cluster)
         """
 
     async def modify_db_cluster_endpoint(
         self,
         *,
         DBClusterEndpointIdentifier: str,
         EndpointType: str = ...,
         StaticMembers: Sequence[str] = ...,
-        ExcludedMembers: Sequence[str] = ...
+        ExcludedMembers: Sequence[str] = ...,
     ) -> ModifyDBClusterEndpointOutputTypeDef:
         """
         Modifies the properties of an endpoint in an Amazon Neptune DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.modify_db_cluster_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#modify_db_cluster_endpoint)
         """
@@ -1039,15 +1039,15 @@
 
     async def modify_db_cluster_snapshot_attribute(
         self,
         *,
         DBClusterSnapshotIdentifier: str,
         AttributeName: str,
         ValuesToAdd: Sequence[str] = ...,
-        ValuesToRemove: Sequence[str] = ...
+        ValuesToRemove: Sequence[str] = ...,
     ) -> ModifyDBClusterSnapshotAttributeResultTypeDef:
         """
         Adds an attribute and values to, or removes an attribute and values from, a
         manual DB cluster
         snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.modify_db_cluster_snapshot_attribute)
@@ -1089,15 +1089,15 @@
         MonitoringRoleArn: str = ...,
         DomainIAMRoleName: str = ...,
         PromotionTier: int = ...,
         EnableIAMDatabaseAuthentication: bool = ...,
         EnablePerformanceInsights: bool = ...,
         PerformanceInsightsKMSKeyId: str = ...,
         CloudwatchLogsExportConfiguration: CloudwatchLogsExportConfigurationTypeDef = ...,
-        DeletionProtection: bool = ...
+        DeletionProtection: bool = ...,
     ) -> ModifyDBInstanceResultTypeDef:
         """
         Modifies settings for a DB instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.modify_db_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#modify_db_instance)
         """
@@ -1113,15 +1113,15 @@
         """
 
     async def modify_db_subnet_group(
         self,
         *,
         DBSubnetGroupName: str,
         SubnetIds: Sequence[str],
-        DBSubnetGroupDescription: str = ...
+        DBSubnetGroupDescription: str = ...,
     ) -> ModifyDBSubnetGroupResultTypeDef:
         """
         Modifies an existing DB subnet group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.modify_db_subnet_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#modify_db_subnet_group)
         """
@@ -1129,15 +1129,15 @@
     async def modify_event_subscription(
         self,
         *,
         SubscriptionName: str,
         SnsTopicArn: str = ...,
         SourceType: str = ...,
         EventCategories: Sequence[str] = ...,
-        Enabled: bool = ...
+        Enabled: bool = ...,
     ) -> ModifyEventSubscriptionResultTypeDef:
         """
         Modifies an existing event notification subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.modify_event_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#modify_event_subscription)
         """
@@ -1145,15 +1145,15 @@
     async def modify_global_cluster(
         self,
         *,
         GlobalClusterIdentifier: str,
         NewGlobalClusterIdentifier: str = ...,
         DeletionProtection: bool = ...,
         EngineVersion: str = ...,
-        AllowMajorVersionUpgrade: bool = ...
+        AllowMajorVersionUpgrade: bool = ...,
     ) -> ModifyGlobalClusterResultTypeDef:
         """
         Modify a setting for an Amazon Neptune global cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.modify_global_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#modify_global_cluster)
         """
@@ -1219,29 +1219,29 @@
         """
 
     async def reset_db_cluster_parameter_group(
         self,
         *,
         DBClusterParameterGroupName: str,
         ResetAllParameters: bool = ...,
-        Parameters: Sequence[ParameterTypeDef] = ...
+        Parameters: Sequence[ParameterTypeDef] = ...,
     ) -> DBClusterParameterGroupNameMessageTypeDef:
         """
         Modifies the parameters of a DB cluster parameter group to the default value.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.reset_db_cluster_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#reset_db_cluster_parameter_group)
         """
 
     async def reset_db_parameter_group(
         self,
         *,
         DBParameterGroupName: str,
         ResetAllParameters: bool = ...,
-        Parameters: Sequence[ParameterTypeDef] = ...
+        Parameters: Sequence[ParameterTypeDef] = ...,
     ) -> DBParameterGroupNameMessageTypeDef:
         """
         Modifies the parameters of a DB parameter group to the engine/system default
         value.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.reset_db_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#reset_db_parameter_group)
@@ -1264,15 +1264,15 @@
         KmsKeyId: str = ...,
         EnableIAMDatabaseAuthentication: bool = ...,
         EnableCloudwatchLogsExports: Sequence[str] = ...,
         DBClusterParameterGroupName: str = ...,
         DeletionProtection: bool = ...,
         CopyTagsToSnapshot: bool = ...,
         ServerlessV2ScalingConfiguration: ServerlessV2ScalingConfigurationTypeDef = ...,
-        StorageType: str = ...
+        StorageType: str = ...,
     ) -> RestoreDBClusterFromSnapshotResultTypeDef:
         """
         Creates a new DB cluster from a DB snapshot or DB cluster snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.restore_db_cluster_from_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#restore_db_cluster_from_snapshot)
         """
@@ -1292,15 +1292,15 @@
         Tags: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...,
         EnableIAMDatabaseAuthentication: bool = ...,
         EnableCloudwatchLogsExports: Sequence[str] = ...,
         DBClusterParameterGroupName: str = ...,
         DeletionProtection: bool = ...,
         ServerlessV2ScalingConfiguration: ServerlessV2ScalingConfigurationTypeDef = ...,
-        StorageType: str = ...
+        StorageType: str = ...,
     ) -> RestoreDBClusterToPointInTimeResultTypeDef:
         """
         Restores a DB cluster to an arbitrary point in time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.restore_db_cluster_to_point_in_time)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#restore_db_cluster_to_point_in_time)
         """
```

### Comparing `types-aiobotocore-neptune-2.9.0/types_aiobotocore_neptune/literals.py` & `types-aiobotocore-neptune-2.9.1/types_aiobotocore_neptune/literals.py`

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
     "ApplyMethodType",
     "DBInstanceAvailableWaiterName",
     "DBInstanceDeletedWaiterName",
     "DescribeDBClusterEndpointsPaginatorName",
     "DescribeDBClusterParameterGroupsPaginatorName",
     "DescribeDBClusterParametersPaginatorName",
@@ -45,15 +44,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 ApplyMethodType = Literal["immediate", "pending-reboot"]
 DBInstanceAvailableWaiterName = Literal["db_instance_available"]
 DBInstanceDeletedWaiterName = Literal["db_instance_deleted"]
 DescribeDBClusterEndpointsPaginatorName = Literal["describe_db_cluster_endpoints"]
 DescribeDBClusterParameterGroupsPaginatorName = Literal["describe_db_cluster_parameter_groups"]
 DescribeDBClusterParametersPaginatorName = Literal["describe_db_cluster_parameters"]
 DescribeDBClusterSnapshotsPaginatorName = Literal["describe_db_cluster_snapshots"]
```

### Comparing `types-aiobotocore-neptune-2.9.0/types_aiobotocore_neptune/literals.pyi` & `types-aiobotocore-neptune-2.9.1/types_aiobotocore_neptune/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-neptune-2.9.0/types_aiobotocore_neptune/paginator.py` & `types-aiobotocore-neptune-2.9.1/types_aiobotocore_neptune/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -94,84 +94,78 @@
     "DescribeEventSubscriptionsPaginator",
     "DescribeEventsPaginator",
     "DescribeGlobalClustersPaginator",
     "DescribeOrderableDBInstanceOptionsPaginator",
     "DescribePendingMaintenanceActionsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class DescribeDBClusterEndpointsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBClusterEndpoints)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbclusterendpointspaginator)
     """
 
     def paginate(
         self,
         *,
         DBClusterIdentifier: str = ...,
         DBClusterEndpointIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBClusterEndpointMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBClusterEndpoints.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbclusterendpointspaginator)
         """
 
-
 class DescribeDBClusterParameterGroupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBClusterParameterGroups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbclusterparametergroupspaginator)
     """
 
     def paginate(
         self,
         *,
         DBClusterParameterGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBClusterParameterGroupsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBClusterParameterGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbclusterparametergroupspaginator)
         """
 
-
 class DescribeDBClusterParametersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBClusterParameters)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbclusterparameterspaginator)
     """
 
     def paginate(
         self,
         *,
         DBClusterParameterGroupName: str,
         Source: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBClusterParameterGroupDetailsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBClusterParameters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbclusterparameterspaginator)
         """
 
-
 class DescribeDBClusterSnapshotsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBClusterSnapshots)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbclustersnapshotspaginator)
     """
 
     def paginate(
@@ -179,41 +173,39 @@
         *,
         DBClusterIdentifier: str = ...,
         DBClusterSnapshotIdentifier: str = ...,
         SnapshotType: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         IncludeShared: bool = ...,
         IncludePublic: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBClusterSnapshotMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBClusterSnapshots.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbclustersnapshotspaginator)
         """
 
-
 class DescribeDBClustersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBClusters)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbclusterspaginator)
     """
 
     def paginate(
         self,
         *,
         DBClusterIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBClusterMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBClusters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbclusterspaginator)
         """
 
-
 class DescribeDBEngineVersionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBEngineVersions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbengineversionspaginator)
     """
 
     def paginate(
@@ -222,137 +214,130 @@
         Engine: str = ...,
         EngineVersion: str = ...,
         DBParameterGroupFamily: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         DefaultOnly: bool = ...,
         ListSupportedCharacterSets: bool = ...,
         ListSupportedTimezones: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBEngineVersionMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBEngineVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbengineversionspaginator)
         """
 
-
 class DescribeDBInstancesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBInstances)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbinstancespaginator)
     """
 
     def paginate(
         self,
         *,
         DBInstanceIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBInstanceMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbinstancespaginator)
         """
 
-
 class DescribeDBParameterGroupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBParameterGroups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbparametergroupspaginator)
     """
 
     def paginate(
         self,
         *,
         DBParameterGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBParameterGroupsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBParameterGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbparametergroupspaginator)
         """
 
-
 class DescribeDBParametersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBParameters)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbparameterspaginator)
     """
 
     def paginate(
         self,
         *,
         DBParameterGroupName: str,
         Source: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBParameterGroupDetailsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBParameters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbparameterspaginator)
         """
 
-
 class DescribeDBSubnetGroupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBSubnetGroups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbsubnetgroupspaginator)
     """
 
     def paginate(
         self,
         *,
         DBSubnetGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBSubnetGroupMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBSubnetGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbsubnetgroupspaginator)
         """
 
-
 class DescribeEngineDefaultParametersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeEngineDefaultParameters)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describeenginedefaultparameterspaginator)
     """
 
     def paginate(
         self,
         *,
         DBParameterGroupFamily: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeEngineDefaultParametersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeEngineDefaultParameters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describeenginedefaultparameterspaginator)
         """
 
-
 class DescribeEventSubscriptionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeEventSubscriptions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describeeventsubscriptionspaginator)
     """
 
     def paginate(
         self,
         *,
         SubscriptionName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[EventSubscriptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeEventSubscriptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describeeventsubscriptionspaginator)
         """
 
-
 class DescribeEventsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeEvents)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describeeventspaginator)
     """
 
     def paginate(
@@ -361,37 +346,35 @@
         SourceIdentifier: str = ...,
         SourceType: SourceTypeType = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         Duration: int = ...,
         EventCategories: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[EventsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describeeventspaginator)
         """
 
-
 class DescribeGlobalClustersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeGlobalClusters)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describeglobalclusterspaginator)
     """
 
     def paginate(
         self, *, GlobalClusterIdentifier: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GlobalClustersMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeGlobalClusters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describeglobalclusterspaginator)
         """
 
-
 class DescribeOrderableDBInstanceOptionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeOrderableDBInstanceOptions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describeorderabledbinstanceoptionspaginator)
     """
 
     def paginate(
@@ -399,32 +382,31 @@
         *,
         Engine: str,
         EngineVersion: str = ...,
         DBInstanceClass: str = ...,
         LicenseModel: str = ...,
         Vpc: bool = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[OrderableDBInstanceOptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeOrderableDBInstanceOptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describeorderabledbinstanceoptionspaginator)
         """
 
-
 class DescribePendingMaintenanceActionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribePendingMaintenanceActions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describependingmaintenanceactionspaginator)
     """
 
     def paginate(
         self,
         *,
         ResourceIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[PendingMaintenanceActionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribePendingMaintenanceActions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describependingmaintenanceactionspaginator)
         """
```

### Comparing `types-aiobotocore-neptune-2.9.0/types_aiobotocore_neptune/paginator.pyi` & `types-aiobotocore-neptune-2.9.1/types_aiobotocore_neptune/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,76 +96,81 @@
     "DescribeGlobalClustersPaginator",
     "DescribeOrderableDBInstanceOptionsPaginator",
     "DescribePendingMaintenanceActionsPaginator",
 )
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class DescribeDBClusterEndpointsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBClusterEndpoints)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbclusterendpointspaginator)
     """
 
     def paginate(
         self,
         *,
         DBClusterIdentifier: str = ...,
         DBClusterEndpointIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBClusterEndpointMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBClusterEndpoints.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbclusterendpointspaginator)
         """
 
+
 class DescribeDBClusterParameterGroupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBClusterParameterGroups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbclusterparametergroupspaginator)
     """
 
     def paginate(
         self,
         *,
         DBClusterParameterGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBClusterParameterGroupsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBClusterParameterGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbclusterparametergroupspaginator)
         """
 
+
 class DescribeDBClusterParametersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBClusterParameters)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbclusterparameterspaginator)
     """
 
     def paginate(
         self,
         *,
         DBClusterParameterGroupName: str,
         Source: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBClusterParameterGroupDetailsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBClusterParameters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbclusterparameterspaginator)
         """
 
+
 class DescribeDBClusterSnapshotsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBClusterSnapshots)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbclustersnapshotspaginator)
     """
 
     def paginate(
@@ -173,39 +178,41 @@
         *,
         DBClusterIdentifier: str = ...,
         DBClusterSnapshotIdentifier: str = ...,
         SnapshotType: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         IncludeShared: bool = ...,
         IncludePublic: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBClusterSnapshotMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBClusterSnapshots.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbclustersnapshotspaginator)
         """
 
+
 class DescribeDBClustersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBClusters)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbclusterspaginator)
     """
 
     def paginate(
         self,
         *,
         DBClusterIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBClusterMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBClusters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbclusterspaginator)
         """
 
+
 class DescribeDBEngineVersionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBEngineVersions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbengineversionspaginator)
     """
 
     def paginate(
@@ -214,130 +221,137 @@
         Engine: str = ...,
         EngineVersion: str = ...,
         DBParameterGroupFamily: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         DefaultOnly: bool = ...,
         ListSupportedCharacterSets: bool = ...,
         ListSupportedTimezones: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBEngineVersionMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBEngineVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbengineversionspaginator)
         """
 
+
 class DescribeDBInstancesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBInstances)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbinstancespaginator)
     """
 
     def paginate(
         self,
         *,
         DBInstanceIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBInstanceMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbinstancespaginator)
         """
 
+
 class DescribeDBParameterGroupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBParameterGroups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbparametergroupspaginator)
     """
 
     def paginate(
         self,
         *,
         DBParameterGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBParameterGroupsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBParameterGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbparametergroupspaginator)
         """
 
+
 class DescribeDBParametersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBParameters)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbparameterspaginator)
     """
 
     def paginate(
         self,
         *,
         DBParameterGroupName: str,
         Source: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBParameterGroupDetailsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBParameters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbparameterspaginator)
         """
 
+
 class DescribeDBSubnetGroupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBSubnetGroups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbsubnetgroupspaginator)
     """
 
     def paginate(
         self,
         *,
         DBSubnetGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBSubnetGroupMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBSubnetGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbsubnetgroupspaginator)
         """
 
+
 class DescribeEngineDefaultParametersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeEngineDefaultParameters)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describeenginedefaultparameterspaginator)
     """
 
     def paginate(
         self,
         *,
         DBParameterGroupFamily: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeEngineDefaultParametersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeEngineDefaultParameters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describeenginedefaultparameterspaginator)
         """
 
+
 class DescribeEventSubscriptionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeEventSubscriptions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describeeventsubscriptionspaginator)
     """
 
     def paginate(
         self,
         *,
         SubscriptionName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[EventSubscriptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeEventSubscriptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describeeventsubscriptionspaginator)
         """
 
+
 class DescribeEventsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeEvents)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describeeventspaginator)
     """
 
     def paginate(
@@ -346,35 +360,37 @@
         SourceIdentifier: str = ...,
         SourceType: SourceTypeType = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         Duration: int = ...,
         EventCategories: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[EventsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describeeventspaginator)
         """
 
+
 class DescribeGlobalClustersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeGlobalClusters)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describeglobalclusterspaginator)
     """
 
     def paginate(
         self, *, GlobalClusterIdentifier: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GlobalClustersMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeGlobalClusters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describeglobalclusterspaginator)
         """
 
+
 class DescribeOrderableDBInstanceOptionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeOrderableDBInstanceOptions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describeorderabledbinstanceoptionspaginator)
     """
 
     def paginate(
@@ -382,31 +398,32 @@
         *,
         Engine: str,
         EngineVersion: str = ...,
         DBInstanceClass: str = ...,
         LicenseModel: str = ...,
         Vpc: bool = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[OrderableDBInstanceOptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeOrderableDBInstanceOptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describeorderabledbinstanceoptionspaginator)
         """
 
+
 class DescribePendingMaintenanceActionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribePendingMaintenanceActions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describependingmaintenanceactionspaginator)
     """
 
     def paginate(
         self,
         *,
         ResourceIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[PendingMaintenanceActionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribePendingMaintenanceActions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describependingmaintenanceactionspaginator)
         """
```

### Comparing `types-aiobotocore-neptune-2.9.0/types_aiobotocore_neptune/type_defs.py` & `types-aiobotocore-neptune-2.9.1/types_aiobotocore_neptune/type_defs.py`

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
     "AddRoleToDBClusterMessageRequestTypeDef",
     "AddSourceIdentifierToSubscriptionMessageRequestTypeDef",
     "EventSubscriptionTypeDef",
     "ResponseMetadataTypeDef",
     "TagTypeDef",
     "ApplyPendingMaintenanceActionMessageRequestTypeDef",
```

### Comparing `types-aiobotocore-neptune-2.9.0/types_aiobotocore_neptune/type_defs.pyi` & `types-aiobotocore-neptune-2.9.1/types_aiobotocore_neptune/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-neptune-2.9.0/types_aiobotocore_neptune/waiter.py` & `types-aiobotocore-neptune-2.9.1/types_aiobotocore_neptune/waiter.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     async def wait(
         self,
         *,
         DBInstanceIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Waiter.DBInstanceAvailable.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/waiters/#dbinstanceavailablewaiter)
         """
 
 
@@ -62,13 +62,13 @@
     async def wait(
         self,
         *,
         DBInstanceIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Waiter.DBInstanceDeleted.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/waiters/#dbinstancedeletedwaiter)
         """
```

### Comparing `types-aiobotocore-neptune-2.9.0/types_aiobotocore_neptune/waiter.pyi` & `types-aiobotocore-neptune-2.9.1/types_aiobotocore_neptune/waiter.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     async def wait(
         self,
         *,
         DBInstanceIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Waiter.DBInstanceAvailable.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/waiters/#dbinstanceavailablewaiter)
         """
 
 class DBInstanceDeletedWaiter(AIOWaiter):
@@ -60,13 +60,13 @@
     async def wait(
         self,
         *,
         DBInstanceIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Waiter.DBInstanceDeleted.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/waiters/#dbinstancedeletedwaiter)
         """
```

### Comparing `types-aiobotocore-neptune-2.9.0/types_aiobotocore_neptune.egg-info/PKG-INFO` & `types-aiobotocore-neptune-2.9.1/types_aiobotocore_neptune.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-neptune
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Neptune 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Neptune 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/
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
 
 <a id="types-aiobotocore-neptune"></a>
 
 # types-aiobotocore-neptune
 
 [![PyPI - types-aiobotocore-neptune](https://img.shields.io/pypi/v/types-aiobotocore-neptune.svg?color=blue)](https://pypi.org/project/types-aiobotocore-neptune)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-neptune.svg?color=blue)](https://pypi.org/project/types-aiobotocore-neptune)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-neptune)](https://pepy.tech/project/types-aiobotocore-neptune)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Neptune 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune)
+[aiobotocore.Neptune 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune)
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
 [types-aiobotocore-neptune docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-neptune-2.9.0/types_aiobotocore_neptune.egg-info/SOURCES.txt` & `types-aiobotocore-neptune-2.9.1/types_aiobotocore_neptune.egg-info/SOURCES.txt`

 * *Files identical despite different names*

