# Comparing `tmp/types-aiobotocore-redshift-2.9.0.tar.gz` & `tmp/types-aiobotocore-redshift-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-redshift-2.9.0.tar", last modified: Wed Dec 13 20:00:16 2023, max compression
+gzip compressed data, was "types-aiobotocore-redshift-2.9.1.tar", last modified: Thu Jan 18 01:21:35 2024, max compression
```

## Comparing `types-aiobotocore-redshift-2.9.0.tar` & `types-aiobotocore-redshift-2.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:16.221261 types-aiobotocore-redshift-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:54:22.000000 types-aiobotocore-redshift-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    20755 2023-12-13 20:00:16.221261 types-aiobotocore-redshift-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19188 2023-12-13 19:54:22.000000 types-aiobotocore-redshift-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:16.221261 types-aiobotocore-redshift-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2023-12-13 19:54:21.000000 types-aiobotocore-redshift-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:16.221261 types-aiobotocore-redshift-2.9.0/types_aiobotocore_redshift/
--rw-r--r--   0 runner    (1001) docker     (127)    10569 2023-12-13 19:54:22.000000 types-aiobotocore-redshift-2.9.0/types_aiobotocore_redshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10568 2023-12-13 19:54:22.000000 types-aiobotocore-redshift-2.9.0/types_aiobotocore_redshift/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      936 2023-12-13 19:54:22.000000 types-aiobotocore-redshift-2.9.0/types_aiobotocore_redshift/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)   128424 2023-12-13 19:54:22.000000 types-aiobotocore-redshift-2.9.0/types_aiobotocore_redshift/client.py
--rw-r--r--   0 runner    (1001) docker     (127)   128420 2023-12-13 19:54:22.000000 types-aiobotocore-redshift-2.9.0/types_aiobotocore_redshift/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    18478 2023-12-13 19:54:23.000000 types-aiobotocore-redshift-2.9.0/types_aiobotocore_redshift/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    18476 2023-12-13 19:54:23.000000 types-aiobotocore-redshift-2.9.0/types_aiobotocore_redshift/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    47750 2023-12-13 19:54:23.000000 types-aiobotocore-redshift-2.9.0/types_aiobotocore_redshift/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    47713 2023-12-13 19:54:23.000000 types-aiobotocore-redshift-2.9.0/types_aiobotocore_redshift/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:54:22.000000 types-aiobotocore-redshift-2.9.0/types_aiobotocore_redshift/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   132240 2023-12-13 19:54:25.000000 types-aiobotocore-redshift-2.9.0/types_aiobotocore_redshift/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   132239 2023-12-13 19:54:24.000000 types-aiobotocore-redshift-2.9.0/types_aiobotocore_redshift/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:54:22.000000 types-aiobotocore-redshift-2.9.0/types_aiobotocore_redshift/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5584 2023-12-13 19:54:23.000000 types-aiobotocore-redshift-2.9.0/types_aiobotocore_redshift/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5580 2023-12-13 19:54:23.000000 types-aiobotocore-redshift-2.9.0/types_aiobotocore_redshift/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:16.221261 types-aiobotocore-redshift-2.9.0/types_aiobotocore_redshift.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20755 2023-12-13 20:00:16.000000 types-aiobotocore-redshift-2.9.0/types_aiobotocore_redshift.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      907 2023-12-13 20:00:16.000000 types-aiobotocore-redshift-2.9.0/types_aiobotocore_redshift.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:16.000000 types-aiobotocore-redshift-2.9.0/types_aiobotocore_redshift.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:16.000000 types-aiobotocore-redshift-2.9.0/types_aiobotocore_redshift.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:16.000000 types-aiobotocore-redshift-2.9.0/types_aiobotocore_redshift.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-13 20:00:16.000000 types-aiobotocore-redshift-2.9.0/types_aiobotocore_redshift.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:35.933092 types-aiobotocore-redshift-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:15:56.000000 types-aiobotocore-redshift-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    20775 2024-01-18 01:21:35.933092 types-aiobotocore-redshift-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19188 2024-01-18 01:15:56.000000 types-aiobotocore-redshift-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:35.933092 types-aiobotocore-redshift-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-01-18 01:15:56.000000 types-aiobotocore-redshift-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:35.933092 types-aiobotocore-redshift-2.9.1/types_aiobotocore_redshift/
+-rw-r--r--   0 runner    (1001) docker     (127)    10568 2024-01-18 01:15:56.000000 types-aiobotocore-redshift-2.9.1/types_aiobotocore_redshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10568 2024-01-18 01:15:56.000000 types-aiobotocore-redshift-2.9.1/types_aiobotocore_redshift/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-01-18 01:15:56.000000 types-aiobotocore-redshift-2.9.1/types_aiobotocore_redshift/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   128490 2024-01-18 01:15:57.000000 types-aiobotocore-redshift-2.9.1/types_aiobotocore_redshift/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   128487 2024-01-18 01:15:56.000000 types-aiobotocore-redshift-2.9.1/types_aiobotocore_redshift/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    18476 2024-01-18 01:15:58.000000 types-aiobotocore-redshift-2.9.1/types_aiobotocore_redshift/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18476 2024-01-18 01:15:58.000000 types-aiobotocore-redshift-2.9.1/types_aiobotocore_redshift/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    47777 2024-01-18 01:15:57.000000 types-aiobotocore-redshift-2.9.1/types_aiobotocore_redshift/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47741 2024-01-18 01:15:57.000000 types-aiobotocore-redshift-2.9.1/types_aiobotocore_redshift/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:15:56.000000 types-aiobotocore-redshift-2.9.1/types_aiobotocore_redshift/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   132239 2024-01-18 01:16:03.000000 types-aiobotocore-redshift-2.9.1/types_aiobotocore_redshift/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   132239 2024-01-18 01:15:59.000000 types-aiobotocore-redshift-2.9.1/types_aiobotocore_redshift/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:15:56.000000 types-aiobotocore-redshift-2.9.1/types_aiobotocore_redshift/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-01-18 01:15:57.000000 types-aiobotocore-redshift-2.9.1/types_aiobotocore_redshift/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-01-18 01:15:57.000000 types-aiobotocore-redshift-2.9.1/types_aiobotocore_redshift/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:35.933092 types-aiobotocore-redshift-2.9.1/types_aiobotocore_redshift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20775 2024-01-18 01:21:35.000000 types-aiobotocore-redshift-2.9.1/types_aiobotocore_redshift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-01-18 01:21:35.000000 types-aiobotocore-redshift-2.9.1/types_aiobotocore_redshift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:35.000000 types-aiobotocore-redshift-2.9.1/types_aiobotocore_redshift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:35.000000 types-aiobotocore-redshift-2.9.1/types_aiobotocore_redshift.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:35.000000 types-aiobotocore-redshift-2.9.1/types_aiobotocore_redshift.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-18 01:21:35.000000 types-aiobotocore-redshift-2.9.1/types_aiobotocore_redshift.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-redshift-2.9.0/LICENSE` & `types-aiobotocore-redshift-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-redshift-2.9.0/PKG-INFO` & `types-aiobotocore-redshift-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-redshift
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Redshift 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Redshift 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/
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
 
 <a id="types-aiobotocore-redshift"></a>
 
 # types-aiobotocore-redshift
 
 [![PyPI - types-aiobotocore-redshift](https://img.shields.io/pypi/v/types-aiobotocore-redshift.svg?color=blue)](https://pypi.org/project/types-aiobotocore-redshift)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-redshift.svg?color=blue)](https://pypi.org/project/types-aiobotocore-redshift)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-redshift)](https://pepy.tech/project/types-aiobotocore-redshift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Redshift 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift)
+[aiobotocore.Redshift 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift)
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
 [types-aiobotocore-redshift docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-redshift-2.9.0/README.md` & `types-aiobotocore-redshift-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-redshift.svg?color=blue)](https://pypi.org/project/types-aiobotocore-redshift)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-redshift)](https://pepy.tech/project/types-aiobotocore-redshift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Redshift 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift)
+[aiobotocore.Redshift 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift)
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
 [types-aiobotocore-redshift docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-redshift-2.9.0/setup.py` & `types-aiobotocore-redshift-2.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-redshift",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_redshift"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Redshift 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.Redshift 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore redshift type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_redshift": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-redshift-2.9.0/types_aiobotocore_redshift/__init__.py` & `types-aiobotocore-redshift-2.9.1/types_aiobotocore_redshift/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,14 @@
     ClusterDeletedWaiter,
     ClusterRestoredWaiter,
     SnapshotAvailableWaiter,
 )
 
 Client = RedshiftClient
 
-
 __all__ = (
     "Client",
     "ClusterAvailableWaiter",
     "ClusterDeletedWaiter",
     "ClusterRestoredWaiter",
     "DescribeClusterDbRevisionsPaginator",
     "DescribeClusterParameterGroupsPaginator",
```

### Comparing `types-aiobotocore-redshift-2.9.0/types_aiobotocore_redshift/__init__.pyi` & `types-aiobotocore-redshift-2.9.1/types_aiobotocore_redshift/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-2.9.0/types_aiobotocore_redshift/__main__.py` & `types-aiobotocore-redshift-2.9.1/types_aiobotocore_redshift/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Redshift 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Redshift 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift\nOther"
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

### Comparing `types-aiobotocore-redshift-2.9.0/types_aiobotocore_redshift/client.py` & `types-aiobotocore-redshift-2.9.1/types_aiobotocore_redshift/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,15 +194,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("RedshiftClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -392,15 +391,15 @@
     async def associate_data_share_consumer(
         self,
         *,
         DataShareArn: str,
         AssociateEntireAccount: bool = ...,
         ConsumerArn: str = ...,
         ConsumerRegion: str = ...,
-        AllowWrites: bool = ...
+        AllowWrites: bool = ...,
     ) -> DataShareResponseTypeDef:
         """
         From a datashare consumer account, associates a datashare with the account
         (AssociateEntireAccount) or the specified namespace
         (ConsumerArn).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.associate_data_share_consumer)
@@ -409,15 +408,15 @@
 
     async def authorize_cluster_security_group_ingress(
         self,
         *,
         ClusterSecurityGroupName: str,
         CIDRIP: str = ...,
         EC2SecurityGroupName: str = ...,
-        EC2SecurityGroupOwnerId: str = ...
+        EC2SecurityGroupOwnerId: str = ...,
     ) -> AuthorizeClusterSecurityGroupIngressResultTypeDef:
         """
         Adds an inbound (ingress) rule to an Amazon Redshift security group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.authorize_cluster_security_group_ingress)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#authorize_cluster_security_group_ingress)
         """
@@ -446,15 +445,15 @@
 
     async def authorize_snapshot_access(
         self,
         *,
         AccountWithRestoreAccess: str,
         SnapshotIdentifier: str = ...,
         SnapshotArn: str = ...,
-        SnapshotClusterIdentifier: str = ...
+        SnapshotClusterIdentifier: str = ...,
     ) -> AuthorizeSnapshotAccessResultTypeDef:
         """
         Authorizes the specified Amazon Web Services account to restore the specified
         snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.authorize_snapshot_access)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#authorize_snapshot_access)
@@ -471,15 +470,15 @@
         """
 
     async def batch_modify_cluster_snapshots(
         self,
         *,
         SnapshotIdentifierList: Sequence[str],
         ManualSnapshotRetentionPeriod: int = ...,
-        Force: bool = ...
+        Force: bool = ...,
     ) -> BatchModifyClusterSnapshotsOutputMessageTypeDef:
         """
         Modifies the settings for a set of cluster snapshots.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.batch_modify_cluster_snapshots)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#batch_modify_cluster_snapshots)
         """
@@ -510,15 +509,15 @@
 
     async def copy_cluster_snapshot(
         self,
         *,
         SourceSnapshotIdentifier: str,
         TargetSnapshotIdentifier: str,
         SourceSnapshotClusterIdentifier: str = ...,
-        ManualSnapshotRetentionPeriod: int = ...
+        ManualSnapshotRetentionPeriod: int = ...,
     ) -> CopyClusterSnapshotResultTypeDef:
         """
         Copies the specified automated cluster snapshot to a new manual cluster
         snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.copy_cluster_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#copy_cluster_snapshot)
@@ -571,30 +570,30 @@
         AquaConfigurationStatus: AquaConfigurationStatusType = ...,
         DefaultIamRoleArn: str = ...,
         LoadSampleData: str = ...,
         ManageMasterPassword: bool = ...,
         MasterPasswordSecretKmsKeyId: str = ...,
         IpAddressType: str = ...,
         MultiAZ: bool = ...,
-        RedshiftIdcApplicationArn: str = ...
+        RedshiftIdcApplicationArn: str = ...,
     ) -> CreateClusterResultTypeDef:
         """
         Creates a new cluster with the specified parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#create_cluster)
         """
 
     async def create_cluster_parameter_group(
         self,
         *,
         ParameterGroupName: str,
         ParameterGroupFamily: str,
         Description: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateClusterParameterGroupResultTypeDef:
         """
         Creates an Amazon Redshift parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_cluster_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#create_cluster_parameter_group)
         """
@@ -611,30 +610,30 @@
 
     async def create_cluster_snapshot(
         self,
         *,
         SnapshotIdentifier: str,
         ClusterIdentifier: str,
         ManualSnapshotRetentionPeriod: int = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateClusterSnapshotResultTypeDef:
         """
         Creates a manual snapshot of the specified cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_cluster_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#create_cluster_snapshot)
         """
 
     async def create_cluster_subnet_group(
         self,
         *,
         ClusterSubnetGroupName: str,
         Description: str,
         SubnetIds: Sequence[str],
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateClusterSubnetGroupResultTypeDef:
         """
         Creates a new Amazon Redshift subnet group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_cluster_subnet_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#create_cluster_subnet_group)
         """
@@ -652,15 +651,15 @@
     async def create_endpoint_access(
         self,
         *,
         EndpointName: str,
         SubnetGroupName: str,
         ClusterIdentifier: str = ...,
         ResourceOwner: str = ...,
-        VpcSecurityGroupIds: Sequence[str] = ...
+        VpcSecurityGroupIds: Sequence[str] = ...,
     ) -> EndpointAccessResponseTypeDef:
         """
         Creates a Redshift-managed VPC endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_endpoint_access)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#create_endpoint_access)
         """
@@ -671,15 +670,15 @@
         SubscriptionName: str,
         SnsTopicArn: str,
         SourceType: str = ...,
         SourceIds: Sequence[str] = ...,
         EventCategories: Sequence[str] = ...,
         Severity: str = ...,
         Enabled: bool = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateEventSubscriptionResultTypeDef:
         """
         Creates an Amazon Redshift event notification subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_event_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#create_event_subscription)
         """
@@ -702,15 +701,15 @@
         *,
         HsmConfigurationIdentifier: str,
         Description: str,
         HsmIpAddress: str,
         HsmPartitionName: str,
         HsmPartitionPassword: str,
         HsmServerPublicCertificate: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateHsmConfigurationResultTypeDef:
         """
         Creates an HSM configuration that contains the information required by an
         Amazon Redshift cluster to store and use database encryption keys in a Hardware
         Security Module
         (HSM).
 
@@ -723,15 +722,15 @@
         *,
         IdcInstanceArn: str,
         RedshiftIdcApplicationName: str,
         IdcDisplayName: str,
         IamRoleArn: str,
         IdentityNamespace: str = ...,
         AuthorizedTokenIssuerList: Sequence[AuthorizedTokenIssuerTypeDef] = ...,
-        ServiceIntegrations: Sequence[ServiceIntegrationsUnionTypeDef] = ...
+        ServiceIntegrations: Sequence[ServiceIntegrationsUnionTypeDef] = ...,
     ) -> CreateRedshiftIdcApplicationResultTypeDef:
         """
         Creates an Amazon Redshift application for use with IAM Identity Center.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_redshift_idc_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#create_redshift_idc_application)
         """
@@ -742,15 +741,15 @@
         ScheduledActionName: str,
         TargetAction: ScheduledActionTypeTypeDef,
         Schedule: str,
         IamRole: str,
         ScheduledActionDescription: str = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
-        Enable: bool = ...
+        Enable: bool = ...,
     ) -> ScheduledActionResponseTypeDef:
         """
         Creates a scheduled action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_scheduled_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#create_scheduled_action)
         """
@@ -772,15 +771,15 @@
         self,
         *,
         ScheduleDefinitions: Sequence[str] = ...,
         ScheduleIdentifier: str = ...,
         ScheduleDescription: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DryRun: bool = ...,
-        NextInvocations: int = ...
+        NextInvocations: int = ...,
     ) -> SnapshotScheduleResponseTypeDef:
         """
         Create a snapshot schedule that can be associated to a cluster and which
         overrides the default system backup
         schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_snapshot_schedule)
@@ -802,15 +801,15 @@
         *,
         ClusterIdentifier: str,
         FeatureType: UsageLimitFeatureTypeType,
         LimitType: UsageLimitLimitTypeType,
         Amount: int,
         Period: UsageLimitPeriodType = ...,
         BreachAction: UsageLimitBreachActionType = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> UsageLimitResponseTypeDef:
         """
         Creates a usage limit for a specified Amazon Redshift feature on a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_usage_limit)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#create_usage_limit)
         """
@@ -838,15 +837,15 @@
 
     async def delete_cluster(
         self,
         *,
         ClusterIdentifier: str,
         SkipFinalClusterSnapshot: bool = ...,
         FinalClusterSnapshotIdentifier: str = ...,
-        FinalClusterSnapshotRetentionPeriod: int = ...
+        FinalClusterSnapshotRetentionPeriod: int = ...,
     ) -> DeleteClusterResultTypeDef:
         """
         Deletes a previously provisioned cluster without its final snapshot being
         created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.delete_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#delete_cluster)
@@ -1050,15 +1049,15 @@
     async def describe_cluster_parameter_groups(
         self,
         *,
         ParameterGroupName: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         TagKeys: Sequence[str] = ...,
-        TagValues: Sequence[str] = ...
+        TagValues: Sequence[str] = ...,
     ) -> ClusterParameterGroupsMessageTypeDef:
         """
         Returns a list of Amazon Redshift parameter groups, including parameter groups
         you created and the default parameter
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_cluster_parameter_groups)
@@ -1067,15 +1066,15 @@
 
     async def describe_cluster_parameters(
         self,
         *,
         ParameterGroupName: str,
         Source: str = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> ClusterParameterGroupDetailsTypeDef:
         """
         Returns a detailed list of parameters contained within the specified Amazon
         Redshift parameter
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_cluster_parameters)
@@ -1085,15 +1084,15 @@
     async def describe_cluster_security_groups(
         self,
         *,
         ClusterSecurityGroupName: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         TagKeys: Sequence[str] = ...,
-        TagValues: Sequence[str] = ...
+        TagValues: Sequence[str] = ...,
     ) -> ClusterSecurityGroupMessageTypeDef:
         """
         Returns information about Amazon Redshift security groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_cluster_security_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_cluster_security_groups)
         """
@@ -1109,15 +1108,15 @@
         EndTime: TimestampTypeDef = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         OwnerAccount: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
         ClusterExists: bool = ...,
-        SortingEntities: Sequence[SnapshotSortingEntityTypeDef] = ...
+        SortingEntities: Sequence[SnapshotSortingEntityTypeDef] = ...,
     ) -> SnapshotMessageTypeDef:
         """
         Returns one or more snapshot objects, which contain metadata about your cluster
         snapshots.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_cluster_snapshots)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_cluster_snapshots)
@@ -1126,15 +1125,15 @@
     async def describe_cluster_subnet_groups(
         self,
         *,
         ClusterSubnetGroupName: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         TagKeys: Sequence[str] = ...,
-        TagValues: Sequence[str] = ...
+        TagValues: Sequence[str] = ...,
     ) -> ClusterSubnetGroupMessageTypeDef:
         """
         Returns one or more cluster subnet group objects, which contain metadata about
         your cluster subnet
         groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_cluster_subnet_groups)
@@ -1153,15 +1152,15 @@
 
     async def describe_cluster_versions(
         self,
         *,
         ClusterVersion: str = ...,
         ClusterParameterGroupFamily: str = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> ClusterVersionsMessageTypeDef:
         """
         Returns descriptions of the available Amazon Redshift cluster versions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_cluster_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_cluster_versions)
         """
@@ -1169,15 +1168,15 @@
     async def describe_clusters(
         self,
         *,
         ClusterIdentifier: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         TagKeys: Sequence[str] = ...,
-        TagValues: Sequence[str] = ...
+        TagValues: Sequence[str] = ...,
     ) -> ClustersMessageTypeDef:
         """
         Returns properties of provisioned clusters including general cluster
         properties, cluster database properties, maintenance and backup properties, and
         security and access
         properties.
 
@@ -1187,15 +1186,15 @@
 
     async def describe_custom_domain_associations(
         self,
         *,
         CustomDomainName: str = ...,
         CustomDomainCertificateArn: str = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> CustomDomainAssociationsMessageTypeDef:
         """
         Contains information about custom domain associations for a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_custom_domain_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_custom_domain_associations)
         """
@@ -1214,15 +1213,15 @@
 
     async def describe_data_shares_for_consumer(
         self,
         *,
         ConsumerArn: str = ...,
         Status: DataShareStatusForConsumerType = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DescribeDataSharesForConsumerResultTypeDef:
         """
         Returns a list of datashares where the account identifier being called is a
         consumer account
         identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_data_shares_for_consumer)
@@ -1231,15 +1230,15 @@
 
     async def describe_data_shares_for_producer(
         self,
         *,
         ProducerArn: str = ...,
         Status: DataShareStatusForProducerType = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DescribeDataSharesForProducerResultTypeDef:
         """
         Returns a list of datashares when the account identifier being called is a
         producer account
         identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_data_shares_for_producer)
@@ -1260,15 +1259,15 @@
         self,
         *,
         ClusterIdentifier: str = ...,
         ResourceOwner: str = ...,
         EndpointName: str = ...,
         VpcId: str = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> EndpointAccessListTypeDef:
         """
         Describes a Redshift-managed VPC endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_endpoint_access)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_endpoint_access)
         """
@@ -1276,15 +1275,15 @@
     async def describe_endpoint_authorization(
         self,
         *,
         ClusterIdentifier: str = ...,
         Account: str = ...,
         Grantee: bool = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> EndpointAuthorizationListTypeDef:
         """
         Describes an endpoint authorization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_endpoint_authorization)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_endpoint_authorization)
         """
@@ -1304,15 +1303,15 @@
     async def describe_event_subscriptions(
         self,
         *,
         SubscriptionName: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         TagKeys: Sequence[str] = ...,
-        TagValues: Sequence[str] = ...
+        TagValues: Sequence[str] = ...,
     ) -> EventSubscriptionsMessageTypeDef:
         """
         Lists descriptions of all the Amazon Redshift event notification subscriptions
         for a customer
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_event_subscriptions)
@@ -1324,15 +1323,15 @@
         *,
         SourceIdentifier: str = ...,
         SourceType: SourceTypeType = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         Duration: int = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> EventsMessageTypeDef:
         """
         Returns events related to clusters, security groups, snapshots, and parameter
         groups for the past 14
         days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_events)
@@ -1342,15 +1341,15 @@
     async def describe_hsm_client_certificates(
         self,
         *,
         HsmClientCertificateIdentifier: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         TagKeys: Sequence[str] = ...,
-        TagValues: Sequence[str] = ...
+        TagValues: Sequence[str] = ...,
     ) -> HsmClientCertificateMessageTypeDef:
         """
         Returns information about the specified HSM client certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_hsm_client_certificates)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_hsm_client_certificates)
         """
@@ -1358,30 +1357,30 @@
     async def describe_hsm_configurations(
         self,
         *,
         HsmConfigurationIdentifier: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         TagKeys: Sequence[str] = ...,
-        TagValues: Sequence[str] = ...
+        TagValues: Sequence[str] = ...,
     ) -> HsmConfigurationMessageTypeDef:
         """
         Returns information about the specified Amazon Redshift HSM configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_hsm_configurations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_hsm_configurations)
         """
 
     async def describe_inbound_integrations(
         self,
         *,
         IntegrationArn: str = ...,
         TargetArn: str = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> InboundIntegrationsMessageTypeDef:
         """
         Returns a list of inbound integrations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_inbound_integrations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_inbound_integrations)
         """
@@ -1402,15 +1401,15 @@
         ActionType: ActionTypeType,
         ClusterIdentifier: str = ...,
         SnapshotIdentifier: str = ...,
         SnapshotArn: str = ...,
         OwnerAccount: str = ...,
         Filters: Sequence[NodeConfigurationOptionsFilterTypeDef] = ...,
         Marker: str = ...,
-        MaxRecords: int = ...
+        MaxRecords: int = ...,
     ) -> NodeConfigurationOptionsMessageTypeDef:
         """
         Returns properties of possible node configurations such as node type, number of
         nodes, and disk usage for the specified action
         type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_node_configuration_options)
@@ -1419,30 +1418,30 @@
 
     async def describe_orderable_cluster_options(
         self,
         *,
         ClusterVersion: str = ...,
         NodeType: str = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> OrderableClusterOptionsMessageTypeDef:
         """
         Returns a list of orderable cluster options.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_orderable_cluster_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_orderable_cluster_options)
         """
 
     async def describe_partners(
         self,
         *,
         AccountId: str,
         ClusterIdentifier: str,
         DatabaseName: str = ...,
-        PartnerName: str = ...
+        PartnerName: str = ...,
     ) -> DescribePartnersOutputMessageTypeDef:
         """
         Returns information about the partner integrations defined for a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_partners)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_partners)
         """
@@ -1459,15 +1458,15 @@
 
     async def describe_reserved_node_exchange_status(
         self,
         *,
         ReservedNodeId: str = ...,
         ReservedNodeExchangeRequestId: str = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DescribeReservedNodeExchangeStatusOutputMessageTypeDef:
         """
         Returns exchange status details and associated metadata for a reserved-node
         exchange.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_reserved_node_exchange_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_reserved_node_exchange_status)
@@ -1510,15 +1509,15 @@
         ScheduledActionName: str = ...,
         TargetActionType: ScheduledActionTypeValuesType = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         Active: bool = ...,
         Filters: Sequence[ScheduledActionFilterTypeDef] = ...,
         Marker: str = ...,
-        MaxRecords: int = ...
+        MaxRecords: int = ...,
     ) -> ScheduledActionsMessageTypeDef:
         """
         Describes properties of scheduled actions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_scheduled_actions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_scheduled_actions)
         """
@@ -1526,15 +1525,15 @@
     async def describe_snapshot_copy_grants(
         self,
         *,
         SnapshotCopyGrantName: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         TagKeys: Sequence[str] = ...,
-        TagValues: Sequence[str] = ...
+        TagValues: Sequence[str] = ...,
     ) -> SnapshotCopyGrantMessageTypeDef:
         """
         Returns a list of snapshot copy grants owned by the Amazon Web Services account
         in the destination
         region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_snapshot_copy_grants)
@@ -1545,15 +1544,15 @@
         self,
         *,
         ClusterIdentifier: str = ...,
         ScheduleIdentifier: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
         Marker: str = ...,
-        MaxRecords: int = ...
+        MaxRecords: int = ...,
     ) -> DescribeSnapshotSchedulesOutputMessageTypeDef:
         """
         Returns a list of snapshot schedules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_snapshot_schedules)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_snapshot_schedules)
         """
@@ -1568,15 +1567,15 @@
 
     async def describe_table_restore_status(
         self,
         *,
         ClusterIdentifier: str = ...,
         TableRestoreRequestId: str = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> TableRestoreStatusMessageTypeDef:
         """
         Lists the status of one or more table restore requests made using the
         RestoreTableFromClusterSnapshot API
         action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_table_restore_status)
@@ -1587,15 +1586,15 @@
         self,
         *,
         ResourceName: str = ...,
         ResourceType: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         TagKeys: Sequence[str] = ...,
-        TagValues: Sequence[str] = ...
+        TagValues: Sequence[str] = ...,
     ) -> TaggedResourceListMessageTypeDef:
         """
         Returns a list of tags.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_tags)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_tags)
         """
@@ -1605,15 +1604,15 @@
         *,
         UsageLimitId: str = ...,
         ClusterIdentifier: str = ...,
         FeatureType: UsageLimitFeatureTypeType = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         TagKeys: Sequence[str] = ...,
-        TagValues: Sequence[str] = ...
+        TagValues: Sequence[str] = ...,
     ) -> UsageLimitListTypeDef:
         """
         Shows usage limits on a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_usage_limits)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_usage_limits)
         """
@@ -1642,15 +1641,15 @@
 
     async def disassociate_data_share_consumer(
         self,
         *,
         DataShareArn: str,
         DisassociateEntireAccount: bool = ...,
         ConsumerArn: str = ...,
-        ConsumerRegion: str = ...
+        ConsumerRegion: str = ...,
     ) -> DataShareResponseTypeDef:
         """
         From a datashare consumer account, remove association for the specified
         datashare.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.disassociate_data_share_consumer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#disassociate_data_share_consumer)
@@ -1659,15 +1658,15 @@
     async def enable_logging(
         self,
         *,
         ClusterIdentifier: str,
         BucketName: str = ...,
         S3KeyPrefix: str = ...,
         LogDestinationType: LogDestinationTypeType = ...,
-        LogExports: Sequence[str] = ...
+        LogExports: Sequence[str] = ...,
     ) -> LoggingStatusTypeDef:
         """
         Starts logging information, such as queries and connection attempts, for the
         specified Amazon Redshift
         cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.enable_logging)
@@ -1677,15 +1676,15 @@
     async def enable_snapshot_copy(
         self,
         *,
         ClusterIdentifier: str,
         DestinationRegion: str,
         RetentionPeriod: int = ...,
         SnapshotCopyGrantName: str = ...,
-        ManualSnapshotRetentionPeriod: int = ...
+        ManualSnapshotRetentionPeriod: int = ...,
     ) -> EnableSnapshotCopyResultTypeDef:
         """
         Enables the automatic copy of snapshots from one region to another region for a
         specified
         cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.enable_snapshot_copy)
@@ -1723,15 +1722,15 @@
         *,
         DbUser: str,
         DbName: str = ...,
         ClusterIdentifier: str = ...,
         DurationSeconds: int = ...,
         AutoCreate: bool = ...,
         DbGroups: Sequence[str] = ...,
-        CustomDomainName: str = ...
+        CustomDomainName: str = ...,
     ) -> ClusterCredentialsTypeDef:
         """
         Returns a database user name and temporary password with temporary
         authorization to log on to an Amazon Redshift
         database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_cluster_credentials)
@@ -1740,15 +1739,15 @@
 
     async def get_cluster_credentials_with_iam(
         self,
         *,
         DbName: str = ...,
         ClusterIdentifier: str = ...,
         DurationSeconds: int = ...,
-        CustomDomainName: str = ...
+        CustomDomainName: str = ...,
     ) -> ClusterExtendedCredentialsTypeDef:
         """
         Returns a database user name and temporary password with temporary
         authorization to log in to an Amazon Redshift
         database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_cluster_credentials_with_iam)
@@ -1758,15 +1757,15 @@
     async def get_reserved_node_exchange_configuration_options(
         self,
         *,
         ActionType: ReservedNodeExchangeActionTypeType,
         ClusterIdentifier: str = ...,
         SnapshotIdentifier: str = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> GetReservedNodeExchangeConfigurationOptionsOutputMessageTypeDef:
         """
         Gets the configuration options for the reserved-node exchange.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_reserved_node_exchange_configuration_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_reserved_node_exchange_configuration_options)
         """
@@ -1838,15 +1837,15 @@
         KmsKeyId: str = ...,
         AvailabilityZoneRelocation: bool = ...,
         AvailabilityZone: str = ...,
         Port: int = ...,
         ManageMasterPassword: bool = ...,
         MasterPasswordSecretKmsKeyId: str = ...,
         IpAddressType: str = ...,
-        MultiAZ: bool = ...
+        MultiAZ: bool = ...,
     ) -> ModifyClusterResultTypeDef:
         """
         Modifies the settings for a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#modify_cluster)
         """
@@ -1863,15 +1862,15 @@
 
     async def modify_cluster_iam_roles(
         self,
         *,
         ClusterIdentifier: str,
         AddIamRoles: Sequence[str] = ...,
         RemoveIamRoles: Sequence[str] = ...,
-        DefaultIamRoleArn: str = ...
+        DefaultIamRoleArn: str = ...,
     ) -> ModifyClusterIamRolesResultTypeDef:
         """
         Modifies the list of Identity and Access Management (IAM) roles that can be
         used by the cluster to access other Amazon Web Services
         services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_cluster_iam_roles)
@@ -1882,15 +1881,15 @@
         self,
         *,
         ClusterIdentifier: str,
         DeferMaintenance: bool = ...,
         DeferMaintenanceIdentifier: str = ...,
         DeferMaintenanceStartTime: TimestampTypeDef = ...,
         DeferMaintenanceEndTime: TimestampTypeDef = ...,
-        DeferMaintenanceDuration: int = ...
+        DeferMaintenanceDuration: int = ...,
     ) -> ModifyClusterMaintenanceResultTypeDef:
         """
         Modifies the maintenance settings of a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_cluster_maintenance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#modify_cluster_maintenance)
         """
@@ -1906,29 +1905,29 @@
         """
 
     async def modify_cluster_snapshot(
         self,
         *,
         SnapshotIdentifier: str,
         ManualSnapshotRetentionPeriod: int = ...,
-        Force: bool = ...
+        Force: bool = ...,
     ) -> ModifyClusterSnapshotResultTypeDef:
         """
         Modifies the settings for a snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_cluster_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#modify_cluster_snapshot)
         """
 
     async def modify_cluster_snapshot_schedule(
         self,
         *,
         ClusterIdentifier: str,
         ScheduleIdentifier: str = ...,
-        DisassociateSchedule: bool = ...
+        DisassociateSchedule: bool = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Modifies a snapshot schedule for a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_cluster_snapshot_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#modify_cluster_snapshot_schedule)
         """
@@ -1968,15 +1967,15 @@
         *,
         SubscriptionName: str,
         SnsTopicArn: str = ...,
         SourceType: str = ...,
         SourceIds: Sequence[str] = ...,
         EventCategories: Sequence[str] = ...,
         Severity: str = ...,
-        Enabled: bool = ...
+        Enabled: bool = ...,
     ) -> ModifyEventSubscriptionResultTypeDef:
         """
         Modifies an existing Amazon Redshift event notification subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_event_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#modify_event_subscription)
         """
@@ -1985,15 +1984,15 @@
         self,
         *,
         RedshiftIdcApplicationArn: str,
         IdentityNamespace: str = ...,
         IamRoleArn: str = ...,
         IdcDisplayName: str = ...,
         AuthorizedTokenIssuerList: Sequence[AuthorizedTokenIssuerTypeDef] = ...,
-        ServiceIntegrations: Sequence[ServiceIntegrationsUnionTypeDef] = ...
+        ServiceIntegrations: Sequence[ServiceIntegrationsUnionTypeDef] = ...,
     ) -> ModifyRedshiftIdcApplicationResultTypeDef:
         """
         Changes an existing Amazon Redshift IAM Identity Center application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_redshift_idc_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#modify_redshift_idc_application)
         """
@@ -2004,15 +2003,15 @@
         ScheduledActionName: str,
         TargetAction: ScheduledActionTypeTypeDef = ...,
         Schedule: str = ...,
         IamRole: str = ...,
         ScheduledActionDescription: str = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
-        Enable: bool = ...
+        Enable: bool = ...,
     ) -> ScheduledActionResponseTypeDef:
         """
         Modifies a scheduled action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_scheduled_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#modify_scheduled_action)
         """
@@ -2040,15 +2039,15 @@
         """
 
     async def modify_usage_limit(
         self,
         *,
         UsageLimitId: str,
         Amount: int = ...,
-        BreachAction: UsageLimitBreachActionType = ...
+        BreachAction: UsageLimitBreachActionType = ...,
     ) -> UsageLimitResponseTypeDef:
         """
         Modifies a usage limit in a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_usage_limit)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#modify_usage_limit)
         """
@@ -2098,15 +2097,15 @@
         """
 
     async def reset_cluster_parameter_group(
         self,
         *,
         ParameterGroupName: str,
         ResetAllParameters: bool = ...,
-        Parameters: Sequence[ParameterTypeDef] = ...
+        Parameters: Sequence[ParameterTypeDef] = ...,
     ) -> ClusterParameterGroupNameMessageTypeDef:
         """
         Sets one or more parameters of the specified parameter group to their default
         values and sets the source values of the parameters to
         "engine-default".
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.reset_cluster_parameter_group)
@@ -2118,15 +2117,15 @@
         *,
         ClusterIdentifier: str,
         ClusterType: str = ...,
         NodeType: str = ...,
         NumberOfNodes: int = ...,
         Classic: bool = ...,
         ReservedNodeId: str = ...,
-        TargetReservedNodeOfferingId: str = ...
+        TargetReservedNodeOfferingId: str = ...,
     ) -> ResizeClusterResultTypeDef:
         """
         Changes the size of the cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.resize_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#resize_cluster)
         """
@@ -2166,15 +2165,15 @@
         DefaultIamRoleArn: str = ...,
         ReservedNodeId: str = ...,
         TargetReservedNodeOfferingId: str = ...,
         Encrypted: bool = ...,
         ManageMasterPassword: bool = ...,
         MasterPasswordSecretKmsKeyId: str = ...,
         IpAddressType: str = ...,
-        MultiAZ: bool = ...
+        MultiAZ: bool = ...,
     ) -> RestoreFromClusterSnapshotResultTypeDef:
         """
         Creates a new cluster from a snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.restore_from_cluster_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#restore_from_cluster_snapshot)
         """
@@ -2186,15 +2185,15 @@
         SnapshotIdentifier: str,
         SourceDatabaseName: str,
         SourceTableName: str,
         NewTableName: str,
         SourceSchemaName: str = ...,
         TargetDatabaseName: str = ...,
         TargetSchemaName: str = ...,
-        EnableCaseSensitiveIdentifier: bool = ...
+        EnableCaseSensitiveIdentifier: bool = ...,
     ) -> RestoreTableFromClusterSnapshotResultTypeDef:
         """
         Creates a new table from a table in an Amazon Redshift cluster snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.restore_table_from_cluster_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#restore_table_from_cluster_snapshot)
         """
@@ -2209,15 +2208,15 @@
 
     async def revoke_cluster_security_group_ingress(
         self,
         *,
         ClusterSecurityGroupName: str,
         CIDRIP: str = ...,
         EC2SecurityGroupName: str = ...,
-        EC2SecurityGroupOwnerId: str = ...
+        EC2SecurityGroupOwnerId: str = ...,
     ) -> RevokeClusterSecurityGroupIngressResultTypeDef:
         """
         Revokes an ingress rule in an Amazon Redshift security group for a previously
         authorized IP range or Amazon EC2 security
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.revoke_cluster_security_group_ingress)
@@ -2226,30 +2225,30 @@
 
     async def revoke_endpoint_access(
         self,
         *,
         ClusterIdentifier: str = ...,
         Account: str = ...,
         VpcIds: Sequence[str] = ...,
-        Force: bool = ...
+        Force: bool = ...,
     ) -> EndpointAuthorizationResponseTypeDef:
         """
         Revokes access to a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.revoke_endpoint_access)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#revoke_endpoint_access)
         """
 
     async def revoke_snapshot_access(
         self,
         *,
         AccountWithRestoreAccess: str,
         SnapshotIdentifier: str = ...,
         SnapshotArn: str = ...,
-        SnapshotClusterIdentifier: str = ...
+        SnapshotClusterIdentifier: str = ...,
     ) -> RevokeSnapshotAccessResultTypeDef:
         """
         Removes the ability of the specified Amazon Web Services account to restore the
         specified
         snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.revoke_snapshot_access)
@@ -2270,15 +2269,15 @@
         self,
         *,
         AccountId: str,
         ClusterIdentifier: str,
         DatabaseName: str,
         PartnerName: str,
         Status: PartnerIntegrationStatusType,
-        StatusMessage: str = ...
+        StatusMessage: str = ...,
     ) -> PartnerIntegrationOutputMessageTypeDef:
         """
         Updates the status of a partner integration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.update_partner_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#update_partner_status)
         """
```

### Comparing `types-aiobotocore-redshift-2.9.0/types_aiobotocore_redshift/client.pyi` & `types-aiobotocore-redshift-2.9.1/types_aiobotocore_redshift/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -388,15 +388,15 @@
     async def associate_data_share_consumer(
         self,
         *,
         DataShareArn: str,
         AssociateEntireAccount: bool = ...,
         ConsumerArn: str = ...,
         ConsumerRegion: str = ...,
-        AllowWrites: bool = ...
+        AllowWrites: bool = ...,
     ) -> DataShareResponseTypeDef:
         """
         From a datashare consumer account, associates a datashare with the account
         (AssociateEntireAccount) or the specified namespace
         (ConsumerArn).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.associate_data_share_consumer)
@@ -405,15 +405,15 @@
 
     async def authorize_cluster_security_group_ingress(
         self,
         *,
         ClusterSecurityGroupName: str,
         CIDRIP: str = ...,
         EC2SecurityGroupName: str = ...,
-        EC2SecurityGroupOwnerId: str = ...
+        EC2SecurityGroupOwnerId: str = ...,
     ) -> AuthorizeClusterSecurityGroupIngressResultTypeDef:
         """
         Adds an inbound (ingress) rule to an Amazon Redshift security group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.authorize_cluster_security_group_ingress)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#authorize_cluster_security_group_ingress)
         """
@@ -442,15 +442,15 @@
 
     async def authorize_snapshot_access(
         self,
         *,
         AccountWithRestoreAccess: str,
         SnapshotIdentifier: str = ...,
         SnapshotArn: str = ...,
-        SnapshotClusterIdentifier: str = ...
+        SnapshotClusterIdentifier: str = ...,
     ) -> AuthorizeSnapshotAccessResultTypeDef:
         """
         Authorizes the specified Amazon Web Services account to restore the specified
         snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.authorize_snapshot_access)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#authorize_snapshot_access)
@@ -467,15 +467,15 @@
         """
 
     async def batch_modify_cluster_snapshots(
         self,
         *,
         SnapshotIdentifierList: Sequence[str],
         ManualSnapshotRetentionPeriod: int = ...,
-        Force: bool = ...
+        Force: bool = ...,
     ) -> BatchModifyClusterSnapshotsOutputMessageTypeDef:
         """
         Modifies the settings for a set of cluster snapshots.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.batch_modify_cluster_snapshots)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#batch_modify_cluster_snapshots)
         """
@@ -506,15 +506,15 @@
 
     async def copy_cluster_snapshot(
         self,
         *,
         SourceSnapshotIdentifier: str,
         TargetSnapshotIdentifier: str,
         SourceSnapshotClusterIdentifier: str = ...,
-        ManualSnapshotRetentionPeriod: int = ...
+        ManualSnapshotRetentionPeriod: int = ...,
     ) -> CopyClusterSnapshotResultTypeDef:
         """
         Copies the specified automated cluster snapshot to a new manual cluster
         snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.copy_cluster_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#copy_cluster_snapshot)
@@ -567,30 +567,30 @@
         AquaConfigurationStatus: AquaConfigurationStatusType = ...,
         DefaultIamRoleArn: str = ...,
         LoadSampleData: str = ...,
         ManageMasterPassword: bool = ...,
         MasterPasswordSecretKmsKeyId: str = ...,
         IpAddressType: str = ...,
         MultiAZ: bool = ...,
-        RedshiftIdcApplicationArn: str = ...
+        RedshiftIdcApplicationArn: str = ...,
     ) -> CreateClusterResultTypeDef:
         """
         Creates a new cluster with the specified parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#create_cluster)
         """
 
     async def create_cluster_parameter_group(
         self,
         *,
         ParameterGroupName: str,
         ParameterGroupFamily: str,
         Description: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateClusterParameterGroupResultTypeDef:
         """
         Creates an Amazon Redshift parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_cluster_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#create_cluster_parameter_group)
         """
@@ -607,30 +607,30 @@
 
     async def create_cluster_snapshot(
         self,
         *,
         SnapshotIdentifier: str,
         ClusterIdentifier: str,
         ManualSnapshotRetentionPeriod: int = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateClusterSnapshotResultTypeDef:
         """
         Creates a manual snapshot of the specified cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_cluster_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#create_cluster_snapshot)
         """
 
     async def create_cluster_subnet_group(
         self,
         *,
         ClusterSubnetGroupName: str,
         Description: str,
         SubnetIds: Sequence[str],
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateClusterSubnetGroupResultTypeDef:
         """
         Creates a new Amazon Redshift subnet group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_cluster_subnet_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#create_cluster_subnet_group)
         """
@@ -648,15 +648,15 @@
     async def create_endpoint_access(
         self,
         *,
         EndpointName: str,
         SubnetGroupName: str,
         ClusterIdentifier: str = ...,
         ResourceOwner: str = ...,
-        VpcSecurityGroupIds: Sequence[str] = ...
+        VpcSecurityGroupIds: Sequence[str] = ...,
     ) -> EndpointAccessResponseTypeDef:
         """
         Creates a Redshift-managed VPC endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_endpoint_access)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#create_endpoint_access)
         """
@@ -667,15 +667,15 @@
         SubscriptionName: str,
         SnsTopicArn: str,
         SourceType: str = ...,
         SourceIds: Sequence[str] = ...,
         EventCategories: Sequence[str] = ...,
         Severity: str = ...,
         Enabled: bool = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateEventSubscriptionResultTypeDef:
         """
         Creates an Amazon Redshift event notification subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_event_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#create_event_subscription)
         """
@@ -698,15 +698,15 @@
         *,
         HsmConfigurationIdentifier: str,
         Description: str,
         HsmIpAddress: str,
         HsmPartitionName: str,
         HsmPartitionPassword: str,
         HsmServerPublicCertificate: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateHsmConfigurationResultTypeDef:
         """
         Creates an HSM configuration that contains the information required by an
         Amazon Redshift cluster to store and use database encryption keys in a Hardware
         Security Module
         (HSM).
 
@@ -719,15 +719,15 @@
         *,
         IdcInstanceArn: str,
         RedshiftIdcApplicationName: str,
         IdcDisplayName: str,
         IamRoleArn: str,
         IdentityNamespace: str = ...,
         AuthorizedTokenIssuerList: Sequence[AuthorizedTokenIssuerTypeDef] = ...,
-        ServiceIntegrations: Sequence[ServiceIntegrationsUnionTypeDef] = ...
+        ServiceIntegrations: Sequence[ServiceIntegrationsUnionTypeDef] = ...,
     ) -> CreateRedshiftIdcApplicationResultTypeDef:
         """
         Creates an Amazon Redshift application for use with IAM Identity Center.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_redshift_idc_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#create_redshift_idc_application)
         """
@@ -738,15 +738,15 @@
         ScheduledActionName: str,
         TargetAction: ScheduledActionTypeTypeDef,
         Schedule: str,
         IamRole: str,
         ScheduledActionDescription: str = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
-        Enable: bool = ...
+        Enable: bool = ...,
     ) -> ScheduledActionResponseTypeDef:
         """
         Creates a scheduled action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_scheduled_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#create_scheduled_action)
         """
@@ -768,15 +768,15 @@
         self,
         *,
         ScheduleDefinitions: Sequence[str] = ...,
         ScheduleIdentifier: str = ...,
         ScheduleDescription: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DryRun: bool = ...,
-        NextInvocations: int = ...
+        NextInvocations: int = ...,
     ) -> SnapshotScheduleResponseTypeDef:
         """
         Create a snapshot schedule that can be associated to a cluster and which
         overrides the default system backup
         schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_snapshot_schedule)
@@ -798,15 +798,15 @@
         *,
         ClusterIdentifier: str,
         FeatureType: UsageLimitFeatureTypeType,
         LimitType: UsageLimitLimitTypeType,
         Amount: int,
         Period: UsageLimitPeriodType = ...,
         BreachAction: UsageLimitBreachActionType = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> UsageLimitResponseTypeDef:
         """
         Creates a usage limit for a specified Amazon Redshift feature on a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_usage_limit)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#create_usage_limit)
         """
@@ -834,15 +834,15 @@
 
     async def delete_cluster(
         self,
         *,
         ClusterIdentifier: str,
         SkipFinalClusterSnapshot: bool = ...,
         FinalClusterSnapshotIdentifier: str = ...,
-        FinalClusterSnapshotRetentionPeriod: int = ...
+        FinalClusterSnapshotRetentionPeriod: int = ...,
     ) -> DeleteClusterResultTypeDef:
         """
         Deletes a previously provisioned cluster without its final snapshot being
         created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.delete_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#delete_cluster)
@@ -1046,15 +1046,15 @@
     async def describe_cluster_parameter_groups(
         self,
         *,
         ParameterGroupName: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         TagKeys: Sequence[str] = ...,
-        TagValues: Sequence[str] = ...
+        TagValues: Sequence[str] = ...,
     ) -> ClusterParameterGroupsMessageTypeDef:
         """
         Returns a list of Amazon Redshift parameter groups, including parameter groups
         you created and the default parameter
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_cluster_parameter_groups)
@@ -1063,15 +1063,15 @@
 
     async def describe_cluster_parameters(
         self,
         *,
         ParameterGroupName: str,
         Source: str = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> ClusterParameterGroupDetailsTypeDef:
         """
         Returns a detailed list of parameters contained within the specified Amazon
         Redshift parameter
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_cluster_parameters)
@@ -1081,15 +1081,15 @@
     async def describe_cluster_security_groups(
         self,
         *,
         ClusterSecurityGroupName: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         TagKeys: Sequence[str] = ...,
-        TagValues: Sequence[str] = ...
+        TagValues: Sequence[str] = ...,
     ) -> ClusterSecurityGroupMessageTypeDef:
         """
         Returns information about Amazon Redshift security groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_cluster_security_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_cluster_security_groups)
         """
@@ -1105,15 +1105,15 @@
         EndTime: TimestampTypeDef = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         OwnerAccount: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
         ClusterExists: bool = ...,
-        SortingEntities: Sequence[SnapshotSortingEntityTypeDef] = ...
+        SortingEntities: Sequence[SnapshotSortingEntityTypeDef] = ...,
     ) -> SnapshotMessageTypeDef:
         """
         Returns one or more snapshot objects, which contain metadata about your cluster
         snapshots.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_cluster_snapshots)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_cluster_snapshots)
@@ -1122,15 +1122,15 @@
     async def describe_cluster_subnet_groups(
         self,
         *,
         ClusterSubnetGroupName: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         TagKeys: Sequence[str] = ...,
-        TagValues: Sequence[str] = ...
+        TagValues: Sequence[str] = ...,
     ) -> ClusterSubnetGroupMessageTypeDef:
         """
         Returns one or more cluster subnet group objects, which contain metadata about
         your cluster subnet
         groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_cluster_subnet_groups)
@@ -1149,15 +1149,15 @@
 
     async def describe_cluster_versions(
         self,
         *,
         ClusterVersion: str = ...,
         ClusterParameterGroupFamily: str = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> ClusterVersionsMessageTypeDef:
         """
         Returns descriptions of the available Amazon Redshift cluster versions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_cluster_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_cluster_versions)
         """
@@ -1165,15 +1165,15 @@
     async def describe_clusters(
         self,
         *,
         ClusterIdentifier: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         TagKeys: Sequence[str] = ...,
-        TagValues: Sequence[str] = ...
+        TagValues: Sequence[str] = ...,
     ) -> ClustersMessageTypeDef:
         """
         Returns properties of provisioned clusters including general cluster
         properties, cluster database properties, maintenance and backup properties, and
         security and access
         properties.
 
@@ -1183,15 +1183,15 @@
 
     async def describe_custom_domain_associations(
         self,
         *,
         CustomDomainName: str = ...,
         CustomDomainCertificateArn: str = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> CustomDomainAssociationsMessageTypeDef:
         """
         Contains information about custom domain associations for a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_custom_domain_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_custom_domain_associations)
         """
@@ -1210,15 +1210,15 @@
 
     async def describe_data_shares_for_consumer(
         self,
         *,
         ConsumerArn: str = ...,
         Status: DataShareStatusForConsumerType = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DescribeDataSharesForConsumerResultTypeDef:
         """
         Returns a list of datashares where the account identifier being called is a
         consumer account
         identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_data_shares_for_consumer)
@@ -1227,15 +1227,15 @@
 
     async def describe_data_shares_for_producer(
         self,
         *,
         ProducerArn: str = ...,
         Status: DataShareStatusForProducerType = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DescribeDataSharesForProducerResultTypeDef:
         """
         Returns a list of datashares when the account identifier being called is a
         producer account
         identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_data_shares_for_producer)
@@ -1256,15 +1256,15 @@
         self,
         *,
         ClusterIdentifier: str = ...,
         ResourceOwner: str = ...,
         EndpointName: str = ...,
         VpcId: str = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> EndpointAccessListTypeDef:
         """
         Describes a Redshift-managed VPC endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_endpoint_access)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_endpoint_access)
         """
@@ -1272,15 +1272,15 @@
     async def describe_endpoint_authorization(
         self,
         *,
         ClusterIdentifier: str = ...,
         Account: str = ...,
         Grantee: bool = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> EndpointAuthorizationListTypeDef:
         """
         Describes an endpoint authorization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_endpoint_authorization)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_endpoint_authorization)
         """
@@ -1300,15 +1300,15 @@
     async def describe_event_subscriptions(
         self,
         *,
         SubscriptionName: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         TagKeys: Sequence[str] = ...,
-        TagValues: Sequence[str] = ...
+        TagValues: Sequence[str] = ...,
     ) -> EventSubscriptionsMessageTypeDef:
         """
         Lists descriptions of all the Amazon Redshift event notification subscriptions
         for a customer
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_event_subscriptions)
@@ -1320,15 +1320,15 @@
         *,
         SourceIdentifier: str = ...,
         SourceType: SourceTypeType = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         Duration: int = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> EventsMessageTypeDef:
         """
         Returns events related to clusters, security groups, snapshots, and parameter
         groups for the past 14
         days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_events)
@@ -1338,15 +1338,15 @@
     async def describe_hsm_client_certificates(
         self,
         *,
         HsmClientCertificateIdentifier: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         TagKeys: Sequence[str] = ...,
-        TagValues: Sequence[str] = ...
+        TagValues: Sequence[str] = ...,
     ) -> HsmClientCertificateMessageTypeDef:
         """
         Returns information about the specified HSM client certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_hsm_client_certificates)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_hsm_client_certificates)
         """
@@ -1354,30 +1354,30 @@
     async def describe_hsm_configurations(
         self,
         *,
         HsmConfigurationIdentifier: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         TagKeys: Sequence[str] = ...,
-        TagValues: Sequence[str] = ...
+        TagValues: Sequence[str] = ...,
     ) -> HsmConfigurationMessageTypeDef:
         """
         Returns information about the specified Amazon Redshift HSM configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_hsm_configurations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_hsm_configurations)
         """
 
     async def describe_inbound_integrations(
         self,
         *,
         IntegrationArn: str = ...,
         TargetArn: str = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> InboundIntegrationsMessageTypeDef:
         """
         Returns a list of inbound integrations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_inbound_integrations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_inbound_integrations)
         """
@@ -1398,15 +1398,15 @@
         ActionType: ActionTypeType,
         ClusterIdentifier: str = ...,
         SnapshotIdentifier: str = ...,
         SnapshotArn: str = ...,
         OwnerAccount: str = ...,
         Filters: Sequence[NodeConfigurationOptionsFilterTypeDef] = ...,
         Marker: str = ...,
-        MaxRecords: int = ...
+        MaxRecords: int = ...,
     ) -> NodeConfigurationOptionsMessageTypeDef:
         """
         Returns properties of possible node configurations such as node type, number of
         nodes, and disk usage for the specified action
         type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_node_configuration_options)
@@ -1415,30 +1415,30 @@
 
     async def describe_orderable_cluster_options(
         self,
         *,
         ClusterVersion: str = ...,
         NodeType: str = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> OrderableClusterOptionsMessageTypeDef:
         """
         Returns a list of orderable cluster options.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_orderable_cluster_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_orderable_cluster_options)
         """
 
     async def describe_partners(
         self,
         *,
         AccountId: str,
         ClusterIdentifier: str,
         DatabaseName: str = ...,
-        PartnerName: str = ...
+        PartnerName: str = ...,
     ) -> DescribePartnersOutputMessageTypeDef:
         """
         Returns information about the partner integrations defined for a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_partners)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_partners)
         """
@@ -1455,15 +1455,15 @@
 
     async def describe_reserved_node_exchange_status(
         self,
         *,
         ReservedNodeId: str = ...,
         ReservedNodeExchangeRequestId: str = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DescribeReservedNodeExchangeStatusOutputMessageTypeDef:
         """
         Returns exchange status details and associated metadata for a reserved-node
         exchange.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_reserved_node_exchange_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_reserved_node_exchange_status)
@@ -1506,15 +1506,15 @@
         ScheduledActionName: str = ...,
         TargetActionType: ScheduledActionTypeValuesType = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         Active: bool = ...,
         Filters: Sequence[ScheduledActionFilterTypeDef] = ...,
         Marker: str = ...,
-        MaxRecords: int = ...
+        MaxRecords: int = ...,
     ) -> ScheduledActionsMessageTypeDef:
         """
         Describes properties of scheduled actions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_scheduled_actions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_scheduled_actions)
         """
@@ -1522,15 +1522,15 @@
     async def describe_snapshot_copy_grants(
         self,
         *,
         SnapshotCopyGrantName: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         TagKeys: Sequence[str] = ...,
-        TagValues: Sequence[str] = ...
+        TagValues: Sequence[str] = ...,
     ) -> SnapshotCopyGrantMessageTypeDef:
         """
         Returns a list of snapshot copy grants owned by the Amazon Web Services account
         in the destination
         region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_snapshot_copy_grants)
@@ -1541,15 +1541,15 @@
         self,
         *,
         ClusterIdentifier: str = ...,
         ScheduleIdentifier: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
         Marker: str = ...,
-        MaxRecords: int = ...
+        MaxRecords: int = ...,
     ) -> DescribeSnapshotSchedulesOutputMessageTypeDef:
         """
         Returns a list of snapshot schedules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_snapshot_schedules)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_snapshot_schedules)
         """
@@ -1564,15 +1564,15 @@
 
     async def describe_table_restore_status(
         self,
         *,
         ClusterIdentifier: str = ...,
         TableRestoreRequestId: str = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> TableRestoreStatusMessageTypeDef:
         """
         Lists the status of one or more table restore requests made using the
         RestoreTableFromClusterSnapshot API
         action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_table_restore_status)
@@ -1583,15 +1583,15 @@
         self,
         *,
         ResourceName: str = ...,
         ResourceType: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         TagKeys: Sequence[str] = ...,
-        TagValues: Sequence[str] = ...
+        TagValues: Sequence[str] = ...,
     ) -> TaggedResourceListMessageTypeDef:
         """
         Returns a list of tags.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_tags)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_tags)
         """
@@ -1601,15 +1601,15 @@
         *,
         UsageLimitId: str = ...,
         ClusterIdentifier: str = ...,
         FeatureType: UsageLimitFeatureTypeType = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         TagKeys: Sequence[str] = ...,
-        TagValues: Sequence[str] = ...
+        TagValues: Sequence[str] = ...,
     ) -> UsageLimitListTypeDef:
         """
         Shows usage limits on a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_usage_limits)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_usage_limits)
         """
@@ -1638,15 +1638,15 @@
 
     async def disassociate_data_share_consumer(
         self,
         *,
         DataShareArn: str,
         DisassociateEntireAccount: bool = ...,
         ConsumerArn: str = ...,
-        ConsumerRegion: str = ...
+        ConsumerRegion: str = ...,
     ) -> DataShareResponseTypeDef:
         """
         From a datashare consumer account, remove association for the specified
         datashare.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.disassociate_data_share_consumer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#disassociate_data_share_consumer)
@@ -1655,15 +1655,15 @@
     async def enable_logging(
         self,
         *,
         ClusterIdentifier: str,
         BucketName: str = ...,
         S3KeyPrefix: str = ...,
         LogDestinationType: LogDestinationTypeType = ...,
-        LogExports: Sequence[str] = ...
+        LogExports: Sequence[str] = ...,
     ) -> LoggingStatusTypeDef:
         """
         Starts logging information, such as queries and connection attempts, for the
         specified Amazon Redshift
         cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.enable_logging)
@@ -1673,15 +1673,15 @@
     async def enable_snapshot_copy(
         self,
         *,
         ClusterIdentifier: str,
         DestinationRegion: str,
         RetentionPeriod: int = ...,
         SnapshotCopyGrantName: str = ...,
-        ManualSnapshotRetentionPeriod: int = ...
+        ManualSnapshotRetentionPeriod: int = ...,
     ) -> EnableSnapshotCopyResultTypeDef:
         """
         Enables the automatic copy of snapshots from one region to another region for a
         specified
         cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.enable_snapshot_copy)
@@ -1719,15 +1719,15 @@
         *,
         DbUser: str,
         DbName: str = ...,
         ClusterIdentifier: str = ...,
         DurationSeconds: int = ...,
         AutoCreate: bool = ...,
         DbGroups: Sequence[str] = ...,
-        CustomDomainName: str = ...
+        CustomDomainName: str = ...,
     ) -> ClusterCredentialsTypeDef:
         """
         Returns a database user name and temporary password with temporary
         authorization to log on to an Amazon Redshift
         database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_cluster_credentials)
@@ -1736,15 +1736,15 @@
 
     async def get_cluster_credentials_with_iam(
         self,
         *,
         DbName: str = ...,
         ClusterIdentifier: str = ...,
         DurationSeconds: int = ...,
-        CustomDomainName: str = ...
+        CustomDomainName: str = ...,
     ) -> ClusterExtendedCredentialsTypeDef:
         """
         Returns a database user name and temporary password with temporary
         authorization to log in to an Amazon Redshift
         database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_cluster_credentials_with_iam)
@@ -1754,15 +1754,15 @@
     async def get_reserved_node_exchange_configuration_options(
         self,
         *,
         ActionType: ReservedNodeExchangeActionTypeType,
         ClusterIdentifier: str = ...,
         SnapshotIdentifier: str = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> GetReservedNodeExchangeConfigurationOptionsOutputMessageTypeDef:
         """
         Gets the configuration options for the reserved-node exchange.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_reserved_node_exchange_configuration_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_reserved_node_exchange_configuration_options)
         """
@@ -1834,15 +1834,15 @@
         KmsKeyId: str = ...,
         AvailabilityZoneRelocation: bool = ...,
         AvailabilityZone: str = ...,
         Port: int = ...,
         ManageMasterPassword: bool = ...,
         MasterPasswordSecretKmsKeyId: str = ...,
         IpAddressType: str = ...,
-        MultiAZ: bool = ...
+        MultiAZ: bool = ...,
     ) -> ModifyClusterResultTypeDef:
         """
         Modifies the settings for a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#modify_cluster)
         """
@@ -1859,15 +1859,15 @@
 
     async def modify_cluster_iam_roles(
         self,
         *,
         ClusterIdentifier: str,
         AddIamRoles: Sequence[str] = ...,
         RemoveIamRoles: Sequence[str] = ...,
-        DefaultIamRoleArn: str = ...
+        DefaultIamRoleArn: str = ...,
     ) -> ModifyClusterIamRolesResultTypeDef:
         """
         Modifies the list of Identity and Access Management (IAM) roles that can be
         used by the cluster to access other Amazon Web Services
         services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_cluster_iam_roles)
@@ -1878,15 +1878,15 @@
         self,
         *,
         ClusterIdentifier: str,
         DeferMaintenance: bool = ...,
         DeferMaintenanceIdentifier: str = ...,
         DeferMaintenanceStartTime: TimestampTypeDef = ...,
         DeferMaintenanceEndTime: TimestampTypeDef = ...,
-        DeferMaintenanceDuration: int = ...
+        DeferMaintenanceDuration: int = ...,
     ) -> ModifyClusterMaintenanceResultTypeDef:
         """
         Modifies the maintenance settings of a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_cluster_maintenance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#modify_cluster_maintenance)
         """
@@ -1902,29 +1902,29 @@
         """
 
     async def modify_cluster_snapshot(
         self,
         *,
         SnapshotIdentifier: str,
         ManualSnapshotRetentionPeriod: int = ...,
-        Force: bool = ...
+        Force: bool = ...,
     ) -> ModifyClusterSnapshotResultTypeDef:
         """
         Modifies the settings for a snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_cluster_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#modify_cluster_snapshot)
         """
 
     async def modify_cluster_snapshot_schedule(
         self,
         *,
         ClusterIdentifier: str,
         ScheduleIdentifier: str = ...,
-        DisassociateSchedule: bool = ...
+        DisassociateSchedule: bool = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Modifies a snapshot schedule for a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_cluster_snapshot_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#modify_cluster_snapshot_schedule)
         """
@@ -1964,15 +1964,15 @@
         *,
         SubscriptionName: str,
         SnsTopicArn: str = ...,
         SourceType: str = ...,
         SourceIds: Sequence[str] = ...,
         EventCategories: Sequence[str] = ...,
         Severity: str = ...,
-        Enabled: bool = ...
+        Enabled: bool = ...,
     ) -> ModifyEventSubscriptionResultTypeDef:
         """
         Modifies an existing Amazon Redshift event notification subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_event_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#modify_event_subscription)
         """
@@ -1981,15 +1981,15 @@
         self,
         *,
         RedshiftIdcApplicationArn: str,
         IdentityNamespace: str = ...,
         IamRoleArn: str = ...,
         IdcDisplayName: str = ...,
         AuthorizedTokenIssuerList: Sequence[AuthorizedTokenIssuerTypeDef] = ...,
-        ServiceIntegrations: Sequence[ServiceIntegrationsUnionTypeDef] = ...
+        ServiceIntegrations: Sequence[ServiceIntegrationsUnionTypeDef] = ...,
     ) -> ModifyRedshiftIdcApplicationResultTypeDef:
         """
         Changes an existing Amazon Redshift IAM Identity Center application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_redshift_idc_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#modify_redshift_idc_application)
         """
@@ -2000,15 +2000,15 @@
         ScheduledActionName: str,
         TargetAction: ScheduledActionTypeTypeDef = ...,
         Schedule: str = ...,
         IamRole: str = ...,
         ScheduledActionDescription: str = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
-        Enable: bool = ...
+        Enable: bool = ...,
     ) -> ScheduledActionResponseTypeDef:
         """
         Modifies a scheduled action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_scheduled_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#modify_scheduled_action)
         """
@@ -2036,15 +2036,15 @@
         """
 
     async def modify_usage_limit(
         self,
         *,
         UsageLimitId: str,
         Amount: int = ...,
-        BreachAction: UsageLimitBreachActionType = ...
+        BreachAction: UsageLimitBreachActionType = ...,
     ) -> UsageLimitResponseTypeDef:
         """
         Modifies a usage limit in a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_usage_limit)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#modify_usage_limit)
         """
@@ -2094,15 +2094,15 @@
         """
 
     async def reset_cluster_parameter_group(
         self,
         *,
         ParameterGroupName: str,
         ResetAllParameters: bool = ...,
-        Parameters: Sequence[ParameterTypeDef] = ...
+        Parameters: Sequence[ParameterTypeDef] = ...,
     ) -> ClusterParameterGroupNameMessageTypeDef:
         """
         Sets one or more parameters of the specified parameter group to their default
         values and sets the source values of the parameters to
         "engine-default".
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.reset_cluster_parameter_group)
@@ -2114,15 +2114,15 @@
         *,
         ClusterIdentifier: str,
         ClusterType: str = ...,
         NodeType: str = ...,
         NumberOfNodes: int = ...,
         Classic: bool = ...,
         ReservedNodeId: str = ...,
-        TargetReservedNodeOfferingId: str = ...
+        TargetReservedNodeOfferingId: str = ...,
     ) -> ResizeClusterResultTypeDef:
         """
         Changes the size of the cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.resize_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#resize_cluster)
         """
@@ -2162,15 +2162,15 @@
         DefaultIamRoleArn: str = ...,
         ReservedNodeId: str = ...,
         TargetReservedNodeOfferingId: str = ...,
         Encrypted: bool = ...,
         ManageMasterPassword: bool = ...,
         MasterPasswordSecretKmsKeyId: str = ...,
         IpAddressType: str = ...,
-        MultiAZ: bool = ...
+        MultiAZ: bool = ...,
     ) -> RestoreFromClusterSnapshotResultTypeDef:
         """
         Creates a new cluster from a snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.restore_from_cluster_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#restore_from_cluster_snapshot)
         """
@@ -2182,15 +2182,15 @@
         SnapshotIdentifier: str,
         SourceDatabaseName: str,
         SourceTableName: str,
         NewTableName: str,
         SourceSchemaName: str = ...,
         TargetDatabaseName: str = ...,
         TargetSchemaName: str = ...,
-        EnableCaseSensitiveIdentifier: bool = ...
+        EnableCaseSensitiveIdentifier: bool = ...,
     ) -> RestoreTableFromClusterSnapshotResultTypeDef:
         """
         Creates a new table from a table in an Amazon Redshift cluster snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.restore_table_from_cluster_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#restore_table_from_cluster_snapshot)
         """
@@ -2205,15 +2205,15 @@
 
     async def revoke_cluster_security_group_ingress(
         self,
         *,
         ClusterSecurityGroupName: str,
         CIDRIP: str = ...,
         EC2SecurityGroupName: str = ...,
-        EC2SecurityGroupOwnerId: str = ...
+        EC2SecurityGroupOwnerId: str = ...,
     ) -> RevokeClusterSecurityGroupIngressResultTypeDef:
         """
         Revokes an ingress rule in an Amazon Redshift security group for a previously
         authorized IP range or Amazon EC2 security
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.revoke_cluster_security_group_ingress)
@@ -2222,30 +2222,30 @@
 
     async def revoke_endpoint_access(
         self,
         *,
         ClusterIdentifier: str = ...,
         Account: str = ...,
         VpcIds: Sequence[str] = ...,
-        Force: bool = ...
+        Force: bool = ...,
     ) -> EndpointAuthorizationResponseTypeDef:
         """
         Revokes access to a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.revoke_endpoint_access)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#revoke_endpoint_access)
         """
 
     async def revoke_snapshot_access(
         self,
         *,
         AccountWithRestoreAccess: str,
         SnapshotIdentifier: str = ...,
         SnapshotArn: str = ...,
-        SnapshotClusterIdentifier: str = ...
+        SnapshotClusterIdentifier: str = ...,
     ) -> RevokeSnapshotAccessResultTypeDef:
         """
         Removes the ability of the specified Amazon Web Services account to restore the
         specified
         snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.revoke_snapshot_access)
@@ -2266,15 +2266,15 @@
         self,
         *,
         AccountId: str,
         ClusterIdentifier: str,
         DatabaseName: str,
         PartnerName: str,
         Status: PartnerIntegrationStatusType,
-        StatusMessage: str = ...
+        StatusMessage: str = ...,
     ) -> PartnerIntegrationOutputMessageTypeDef:
         """
         Updates the status of a partner integration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.update_partner_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#update_partner_status)
         """
```

### Comparing `types-aiobotocore-redshift-2.9.0/types_aiobotocore_redshift/literals.py` & `types-aiobotocore-redshift-2.9.1/types_aiobotocore_redshift/literals.py`

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
     "ActionTypeType",
     "AquaConfigurationStatusType",
     "AquaStatusType",
     "AuthorizationStatusType",
     "ClusterAvailableWaiterName",
     "ClusterDeletedWaiterName",
@@ -94,15 +93,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 ActionTypeType = Literal["recommend-node-config", "resize-cluster", "restore-cluster"]
 AquaConfigurationStatusType = Literal["auto", "disabled", "enabled"]
 AquaStatusType = Literal["applying", "disabled", "enabled"]
 AuthorizationStatusType = Literal["Authorized", "Revoking"]
 ClusterAvailableWaiterName = Literal["cluster_available"]
 ClusterDeletedWaiterName = Literal["cluster_deleted"]
 ClusterRestoredWaiterName = Literal["cluster_restored"]
```

### Comparing `types-aiobotocore-redshift-2.9.0/types_aiobotocore_redshift/literals.pyi` & `types-aiobotocore-redshift-2.9.1/types_aiobotocore_redshift/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-2.9.0/types_aiobotocore_redshift/paginator.py` & `types-aiobotocore-redshift-2.9.1/types_aiobotocore_redshift/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,14 @@
     "DescribeTableRestoreStatusPaginator",
     "DescribeTagsPaginator",
     "DescribeUsageLimitsPaginator",
     "GetReservedNodeExchangeConfigurationOptionsPaginator",
     "GetReservedNodeExchangeOfferingsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -218,15 +217,15 @@
 
     def paginate(
         self,
         *,
         ParameterGroupName: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ClusterParameterGroupsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterParameterGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeclusterparametergroupspaginator)
         """
 
 
@@ -237,15 +236,15 @@
     """
 
     def paginate(
         self,
         *,
         ParameterGroupName: str,
         Source: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ClusterParameterGroupDetailsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterParameters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeclusterparameterspaginator)
         """
 
 
@@ -257,15 +256,15 @@
 
     def paginate(
         self,
         *,
         ClusterSecurityGroupName: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ClusterSecurityGroupMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterSecurityGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeclustersecuritygroupspaginator)
         """
 
 
@@ -285,15 +284,15 @@
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         OwnerAccount: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
         ClusterExists: bool = ...,
         SortingEntities: Sequence[SnapshotSortingEntityTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SnapshotMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterSnapshots.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeclustersnapshotspaginator)
         """
 
 
@@ -305,15 +304,15 @@
 
     def paginate(
         self,
         *,
         ClusterSubnetGroupName: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ClusterSubnetGroupMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterSubnetGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeclustersubnetgroupspaginator)
         """
 
 
@@ -339,15 +338,15 @@
     """
 
     def paginate(
         self,
         *,
         ClusterVersion: str = ...,
         ClusterParameterGroupFamily: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ClusterVersionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeclusterversionspaginator)
         """
 
 
@@ -359,15 +358,15 @@
 
     def paginate(
         self,
         *,
         ClusterIdentifier: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ClustersMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeclusterspaginator)
         """
 
 
@@ -378,15 +377,15 @@
     """
 
     def paginate(
         self,
         *,
         CustomDomainName: str = ...,
         CustomDomainCertificateArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[CustomDomainAssociationsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeCustomDomainAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describecustomdomainassociationspaginator)
         """
 
 
@@ -412,15 +411,15 @@
     """
 
     def paginate(
         self,
         *,
         ConsumerArn: str = ...,
         Status: DataShareStatusForConsumerType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeDataSharesForConsumerResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeDataSharesForConsumer.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describedatasharesforconsumerpaginator)
         """
 
 
@@ -431,15 +430,15 @@
     """
 
     def paginate(
         self,
         *,
         ProducerArn: str = ...,
         Status: DataShareStatusForProducerType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeDataSharesForProducerResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeDataSharesForProducer.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describedatasharesforproducerpaginator)
         """
 
 
@@ -467,15 +466,15 @@
     def paginate(
         self,
         *,
         ClusterIdentifier: str = ...,
         ResourceOwner: str = ...,
         EndpointName: str = ...,
         VpcId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[EndpointAccessListTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeEndpointAccess.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeendpointaccesspaginator)
         """
 
 
@@ -487,15 +486,15 @@
 
     def paginate(
         self,
         *,
         ClusterIdentifier: str = ...,
         Account: str = ...,
         Grantee: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[EndpointAuthorizationListTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeEndpointAuthorization.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeendpointauthorizationpaginator)
         """
 
 
@@ -507,15 +506,15 @@
 
     def paginate(
         self,
         *,
         SubscriptionName: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[EventSubscriptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeEventSubscriptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeeventsubscriptionspaginator)
         """
 
 
@@ -529,15 +528,15 @@
         self,
         *,
         SourceIdentifier: str = ...,
         SourceType: SourceTypeType = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         Duration: int = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[EventsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeeventspaginator)
         """
 
 
@@ -549,15 +548,15 @@
 
     def paginate(
         self,
         *,
         HsmClientCertificateIdentifier: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[HsmClientCertificateMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeHsmClientCertificates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describehsmclientcertificatespaginator)
         """
 
 
@@ -569,15 +568,15 @@
 
     def paginate(
         self,
         *,
         HsmConfigurationIdentifier: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[HsmConfigurationMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeHsmConfigurations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describehsmconfigurationspaginator)
         """
 
 
@@ -588,15 +587,15 @@
     """
 
     def paginate(
         self,
         *,
         IntegrationArn: str = ...,
         TargetArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[InboundIntegrationsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeInboundIntegrations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeinboundintegrationspaginator)
         """
 
 
@@ -611,15 +610,15 @@
         *,
         ActionType: ActionTypeType,
         ClusterIdentifier: str = ...,
         SnapshotIdentifier: str = ...,
         SnapshotArn: str = ...,
         OwnerAccount: str = ...,
         Filters: Sequence[NodeConfigurationOptionsFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[NodeConfigurationOptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeNodeConfigurationOptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describenodeconfigurationoptionspaginator)
         """
 
 
@@ -630,15 +629,15 @@
     """
 
     def paginate(
         self,
         *,
         ClusterVersion: str = ...,
         NodeType: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[OrderableClusterOptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeOrderableClusterOptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeorderableclusteroptionspaginator)
         """
 
 
@@ -648,15 +647,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeredshiftidcapplicationspaginator)
     """
 
     def paginate(
         self,
         *,
         RedshiftIdcApplicationArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeRedshiftIdcApplicationsResultPaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeRedshiftIdcApplications.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeredshiftidcapplicationspaginator)
         """
 
 
@@ -667,15 +666,15 @@
     """
 
     def paginate(
         self,
         *,
         ReservedNodeId: str = ...,
         ReservedNodeExchangeRequestId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeReservedNodeExchangeStatusOutputMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeReservedNodeExchangeStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describereservednodeexchangestatuspaginator)
         """
 
 
@@ -720,15 +719,15 @@
         *,
         ScheduledActionName: str = ...,
         TargetActionType: ScheduledActionTypeValuesType = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         Active: bool = ...,
         Filters: Sequence[ScheduledActionFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ScheduledActionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeScheduledActions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describescheduledactionspaginator)
         """
 
 
@@ -740,15 +739,15 @@
 
     def paginate(
         self,
         *,
         SnapshotCopyGrantName: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SnapshotCopyGrantMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeSnapshotCopyGrants.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describesnapshotcopygrantspaginator)
         """
 
 
@@ -761,15 +760,15 @@
     def paginate(
         self,
         *,
         ClusterIdentifier: str = ...,
         ScheduleIdentifier: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeSnapshotSchedulesOutputMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeSnapshotSchedules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describesnapshotschedulespaginator)
         """
 
 
@@ -780,15 +779,15 @@
     """
 
     def paginate(
         self,
         *,
         ClusterIdentifier: str = ...,
         TableRestoreRequestId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[TableRestoreStatusMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeTableRestoreStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describetablerestorestatuspaginator)
         """
 
 
@@ -801,15 +800,15 @@
     def paginate(
         self,
         *,
         ResourceName: str = ...,
         ResourceType: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[TaggedResourceListMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describetagspaginator)
         """
 
 
@@ -823,15 +822,15 @@
         self,
         *,
         UsageLimitId: str = ...,
         ClusterIdentifier: str = ...,
         FeatureType: UsageLimitFeatureTypeType = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[UsageLimitListTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeUsageLimits.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeusagelimitspaginator)
         """
 
 
@@ -843,15 +842,15 @@
 
     def paginate(
         self,
         *,
         ActionType: ReservedNodeExchangeActionTypeType,
         ClusterIdentifier: str = ...,
         SnapshotIdentifier: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetReservedNodeExchangeConfigurationOptionsOutputMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.GetReservedNodeExchangeConfigurationOptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#getreservednodeexchangeconfigurationoptionspaginator)
         """
```

### Comparing `types-aiobotocore-redshift-2.9.0/types_aiobotocore_redshift/paginator.pyi` & `types-aiobotocore-redshift-2.9.1/types_aiobotocore_redshift/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -214,15 +214,15 @@
 
     def paginate(
         self,
         *,
         ParameterGroupName: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ClusterParameterGroupsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterParameterGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeclusterparametergroupspaginator)
         """
 
 class DescribeClusterParametersPaginator(AioPaginator):
@@ -232,15 +232,15 @@
     """
 
     def paginate(
         self,
         *,
         ParameterGroupName: str,
         Source: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ClusterParameterGroupDetailsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterParameters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeclusterparameterspaginator)
         """
 
 class DescribeClusterSecurityGroupsPaginator(AioPaginator):
@@ -251,15 +251,15 @@
 
     def paginate(
         self,
         *,
         ClusterSecurityGroupName: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ClusterSecurityGroupMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterSecurityGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeclustersecuritygroupspaginator)
         """
 
 class DescribeClusterSnapshotsPaginator(AioPaginator):
@@ -278,15 +278,15 @@
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         OwnerAccount: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
         ClusterExists: bool = ...,
         SortingEntities: Sequence[SnapshotSortingEntityTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SnapshotMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterSnapshots.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeclustersnapshotspaginator)
         """
 
 class DescribeClusterSubnetGroupsPaginator(AioPaginator):
@@ -297,15 +297,15 @@
 
     def paginate(
         self,
         *,
         ClusterSubnetGroupName: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ClusterSubnetGroupMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterSubnetGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeclustersubnetgroupspaginator)
         """
 
 class DescribeClusterTracksPaginator(AioPaginator):
@@ -329,15 +329,15 @@
     """
 
     def paginate(
         self,
         *,
         ClusterVersion: str = ...,
         ClusterParameterGroupFamily: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ClusterVersionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeclusterversionspaginator)
         """
 
 class DescribeClustersPaginator(AioPaginator):
@@ -348,15 +348,15 @@
 
     def paginate(
         self,
         *,
         ClusterIdentifier: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ClustersMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeclusterspaginator)
         """
 
 class DescribeCustomDomainAssociationsPaginator(AioPaginator):
@@ -366,15 +366,15 @@
     """
 
     def paginate(
         self,
         *,
         CustomDomainName: str = ...,
         CustomDomainCertificateArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[CustomDomainAssociationsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeCustomDomainAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describecustomdomainassociationspaginator)
         """
 
 class DescribeDataSharesPaginator(AioPaginator):
@@ -398,15 +398,15 @@
     """
 
     def paginate(
         self,
         *,
         ConsumerArn: str = ...,
         Status: DataShareStatusForConsumerType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeDataSharesForConsumerResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeDataSharesForConsumer.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describedatasharesforconsumerpaginator)
         """
 
 class DescribeDataSharesForProducerPaginator(AioPaginator):
@@ -416,15 +416,15 @@
     """
 
     def paginate(
         self,
         *,
         ProducerArn: str = ...,
         Status: DataShareStatusForProducerType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeDataSharesForProducerResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeDataSharesForProducer.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describedatasharesforproducerpaginator)
         """
 
 class DescribeDefaultClusterParametersPaginator(AioPaginator):
@@ -450,15 +450,15 @@
     def paginate(
         self,
         *,
         ClusterIdentifier: str = ...,
         ResourceOwner: str = ...,
         EndpointName: str = ...,
         VpcId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[EndpointAccessListTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeEndpointAccess.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeendpointaccesspaginator)
         """
 
 class DescribeEndpointAuthorizationPaginator(AioPaginator):
@@ -469,15 +469,15 @@
 
     def paginate(
         self,
         *,
         ClusterIdentifier: str = ...,
         Account: str = ...,
         Grantee: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[EndpointAuthorizationListTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeEndpointAuthorization.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeendpointauthorizationpaginator)
         """
 
 class DescribeEventSubscriptionsPaginator(AioPaginator):
@@ -488,15 +488,15 @@
 
     def paginate(
         self,
         *,
         SubscriptionName: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[EventSubscriptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeEventSubscriptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeeventsubscriptionspaginator)
         """
 
 class DescribeEventsPaginator(AioPaginator):
@@ -509,15 +509,15 @@
         self,
         *,
         SourceIdentifier: str = ...,
         SourceType: SourceTypeType = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         Duration: int = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[EventsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeeventspaginator)
         """
 
 class DescribeHsmClientCertificatesPaginator(AioPaginator):
@@ -528,15 +528,15 @@
 
     def paginate(
         self,
         *,
         HsmClientCertificateIdentifier: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[HsmClientCertificateMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeHsmClientCertificates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describehsmclientcertificatespaginator)
         """
 
 class DescribeHsmConfigurationsPaginator(AioPaginator):
@@ -547,15 +547,15 @@
 
     def paginate(
         self,
         *,
         HsmConfigurationIdentifier: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[HsmConfigurationMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeHsmConfigurations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describehsmconfigurationspaginator)
         """
 
 class DescribeInboundIntegrationsPaginator(AioPaginator):
@@ -565,15 +565,15 @@
     """
 
     def paginate(
         self,
         *,
         IntegrationArn: str = ...,
         TargetArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[InboundIntegrationsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeInboundIntegrations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeinboundintegrationspaginator)
         """
 
 class DescribeNodeConfigurationOptionsPaginator(AioPaginator):
@@ -587,15 +587,15 @@
         *,
         ActionType: ActionTypeType,
         ClusterIdentifier: str = ...,
         SnapshotIdentifier: str = ...,
         SnapshotArn: str = ...,
         OwnerAccount: str = ...,
         Filters: Sequence[NodeConfigurationOptionsFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[NodeConfigurationOptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeNodeConfigurationOptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describenodeconfigurationoptionspaginator)
         """
 
 class DescribeOrderableClusterOptionsPaginator(AioPaginator):
@@ -605,15 +605,15 @@
     """
 
     def paginate(
         self,
         *,
         ClusterVersion: str = ...,
         NodeType: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[OrderableClusterOptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeOrderableClusterOptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeorderableclusteroptionspaginator)
         """
 
 class DescribeRedshiftIdcApplicationsPaginator(AioPaginator):
@@ -622,15 +622,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeredshiftidcapplicationspaginator)
     """
 
     def paginate(
         self,
         *,
         RedshiftIdcApplicationArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeRedshiftIdcApplicationsResultPaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeRedshiftIdcApplications.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeredshiftidcapplicationspaginator)
         """
 
 class DescribeReservedNodeExchangeStatusPaginator(AioPaginator):
@@ -640,15 +640,15 @@
     """
 
     def paginate(
         self,
         *,
         ReservedNodeId: str = ...,
         ReservedNodeExchangeRequestId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeReservedNodeExchangeStatusOutputMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeReservedNodeExchangeStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describereservednodeexchangestatuspaginator)
         """
 
 class DescribeReservedNodeOfferingsPaginator(AioPaginator):
@@ -690,15 +690,15 @@
         *,
         ScheduledActionName: str = ...,
         TargetActionType: ScheduledActionTypeValuesType = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         Active: bool = ...,
         Filters: Sequence[ScheduledActionFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ScheduledActionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeScheduledActions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describescheduledactionspaginator)
         """
 
 class DescribeSnapshotCopyGrantsPaginator(AioPaginator):
@@ -709,15 +709,15 @@
 
     def paginate(
         self,
         *,
         SnapshotCopyGrantName: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SnapshotCopyGrantMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeSnapshotCopyGrants.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describesnapshotcopygrantspaginator)
         """
 
 class DescribeSnapshotSchedulesPaginator(AioPaginator):
@@ -729,15 +729,15 @@
     def paginate(
         self,
         *,
         ClusterIdentifier: str = ...,
         ScheduleIdentifier: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeSnapshotSchedulesOutputMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeSnapshotSchedules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describesnapshotschedulespaginator)
         """
 
 class DescribeTableRestoreStatusPaginator(AioPaginator):
@@ -747,15 +747,15 @@
     """
 
     def paginate(
         self,
         *,
         ClusterIdentifier: str = ...,
         TableRestoreRequestId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[TableRestoreStatusMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeTableRestoreStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describetablerestorestatuspaginator)
         """
 
 class DescribeTagsPaginator(AioPaginator):
@@ -767,15 +767,15 @@
     def paginate(
         self,
         *,
         ResourceName: str = ...,
         ResourceType: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[TaggedResourceListMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describetagspaginator)
         """
 
 class DescribeUsageLimitsPaginator(AioPaginator):
@@ -788,15 +788,15 @@
         self,
         *,
         UsageLimitId: str = ...,
         ClusterIdentifier: str = ...,
         FeatureType: UsageLimitFeatureTypeType = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[UsageLimitListTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeUsageLimits.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeusagelimitspaginator)
         """
 
 class GetReservedNodeExchangeConfigurationOptionsPaginator(AioPaginator):
@@ -807,15 +807,15 @@
 
     def paginate(
         self,
         *,
         ActionType: ReservedNodeExchangeActionTypeType,
         ClusterIdentifier: str = ...,
         SnapshotIdentifier: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetReservedNodeExchangeConfigurationOptionsOutputMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.GetReservedNodeExchangeConfigurationOptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#getreservednodeexchangeconfigurationoptionspaginator)
         """
 
 class GetReservedNodeExchangeOfferingsPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-redshift-2.9.0/types_aiobotocore_redshift/type_defs.py` & `types-aiobotocore-redshift-2.9.1/types_aiobotocore_redshift/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AcceptReservedNodeExchangeInputMessageRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AttributeValueTargetTypeDef",
     "AccountWithRestoreAccessTypeDef",
     "AquaConfigurationTypeDef",
     "AssociateDataShareConsumerMessageRequestTypeDef",
```

### Comparing `types-aiobotocore-redshift-2.9.0/types_aiobotocore_redshift/type_defs.pyi` & `types-aiobotocore-redshift-2.9.1/types_aiobotocore_redshift/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-2.9.0/types_aiobotocore_redshift/waiter.py` & `types-aiobotocore-redshift-2.9.1/types_aiobotocore_redshift/waiter.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         self,
         *,
         ClusterIdentifier: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Waiter.ClusterAvailable.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/waiters/#clusteravailablewaiter)
         """
 
 
@@ -73,15 +73,15 @@
         self,
         *,
         ClusterIdentifier: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Waiter.ClusterDeleted.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/waiters/#clusterdeletedwaiter)
         """
 
 
@@ -95,15 +95,15 @@
         self,
         *,
         ClusterIdentifier: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Waiter.ClusterRestored.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/waiters/#clusterrestoredwaiter)
         """
 
 
@@ -125,13 +125,13 @@
         MaxRecords: int = ...,
         Marker: str = ...,
         OwnerAccount: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
         ClusterExists: bool = ...,
         SortingEntities: Sequence[SnapshotSortingEntityTypeDef] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Waiter.SnapshotAvailable.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/waiters/#snapshotavailablewaiter)
         """
```

### Comparing `types-aiobotocore-redshift-2.9.0/types_aiobotocore_redshift/waiter.pyi` & `types-aiobotocore-redshift-2.9.1/types_aiobotocore_redshift/waiter.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         self,
         *,
         ClusterIdentifier: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Waiter.ClusterAvailable.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/waiters/#clusteravailablewaiter)
         """
 
 class ClusterDeletedWaiter(AIOWaiter):
@@ -71,15 +71,15 @@
         self,
         *,
         ClusterIdentifier: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Waiter.ClusterDeleted.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/waiters/#clusterdeletedwaiter)
         """
 
 class ClusterRestoredWaiter(AIOWaiter):
@@ -92,15 +92,15 @@
         self,
         *,
         ClusterIdentifier: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Waiter.ClusterRestored.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/waiters/#clusterrestoredwaiter)
         """
 
 class SnapshotAvailableWaiter(AIOWaiter):
@@ -121,13 +121,13 @@
         MaxRecords: int = ...,
         Marker: str = ...,
         OwnerAccount: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
         ClusterExists: bool = ...,
         SortingEntities: Sequence[SnapshotSortingEntityTypeDef] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Waiter.SnapshotAvailable.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/waiters/#snapshotavailablewaiter)
         """
```

### Comparing `types-aiobotocore-redshift-2.9.0/types_aiobotocore_redshift.egg-info/PKG-INFO` & `types-aiobotocore-redshift-2.9.1/types_aiobotocore_redshift.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-redshift
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Redshift 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Redshift 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/
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
 
 <a id="types-aiobotocore-redshift"></a>
 
 # types-aiobotocore-redshift
 
 [![PyPI - types-aiobotocore-redshift](https://img.shields.io/pypi/v/types-aiobotocore-redshift.svg?color=blue)](https://pypi.org/project/types-aiobotocore-redshift)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-redshift.svg?color=blue)](https://pypi.org/project/types-aiobotocore-redshift)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-redshift)](https://pepy.tech/project/types-aiobotocore-redshift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Redshift 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift)
+[aiobotocore.Redshift 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift)
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
 [types-aiobotocore-redshift docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-redshift-2.9.0/types_aiobotocore_redshift.egg-info/SOURCES.txt` & `types-aiobotocore-redshift-2.9.1/types_aiobotocore_redshift.egg-info/SOURCES.txt`

 * *Files identical despite different names*

