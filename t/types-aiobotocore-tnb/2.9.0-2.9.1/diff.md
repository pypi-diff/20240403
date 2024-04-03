# Comparing `tmp/types-aiobotocore-tnb-2.9.0.tar.gz` & `tmp/types-aiobotocore-tnb-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-tnb-2.9.0.tar", last modified: Wed Dec 13 20:00:41 2023, max compression
+gzip compressed data, was "types-aiobotocore-tnb-2.9.1.tar", last modified: Thu Jan 18 01:21:58 2024, max compression
```

## Comparing `types-aiobotocore-tnb-2.9.0.tar` & `types-aiobotocore-tnb-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:41.489044 types-aiobotocore-tnb-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:57:21.000000 types-aiobotocore-tnb-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13659 2023-12-13 20:00:41.489044 types-aiobotocore-tnb-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12096 2023-12-13 19:57:21.000000 types-aiobotocore-tnb-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:41.489044 types-aiobotocore-tnb-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2023-12-13 19:57:21.000000 types-aiobotocore-tnb-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:41.485044 types-aiobotocore-tnb-2.9.0/types_aiobotocore_tnb/
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2023-12-13 19:57:21.000000 types-aiobotocore-tnb-2.9.0/types_aiobotocore_tnb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2023-12-13 19:57:21.000000 types-aiobotocore-tnb-2.9.0/types_aiobotocore_tnb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      937 2023-12-13 19:57:22.000000 types-aiobotocore-tnb-2.9.0/types_aiobotocore_tnb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27006 2023-12-13 19:57:22.000000 types-aiobotocore-tnb-2.9.0/types_aiobotocore_tnb/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    27002 2023-12-13 19:57:22.000000 types-aiobotocore-tnb-2.9.0/types_aiobotocore_tnb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10708 2023-12-13 19:57:22.000000 types-aiobotocore-tnb-2.9.0/types_aiobotocore_tnb/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10706 2023-12-13 19:57:22.000000 types-aiobotocore-tnb-2.9.0/types_aiobotocore_tnb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6827 2023-12-13 19:57:22.000000 types-aiobotocore-tnb-2.9.0/types_aiobotocore_tnb/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6820 2023-12-13 19:57:22.000000 types-aiobotocore-tnb-2.9.0/types_aiobotocore_tnb/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:57:22.000000 types-aiobotocore-tnb-2.9.0/types_aiobotocore_tnb/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    30011 2023-12-13 19:57:22.000000 types-aiobotocore-tnb-2.9.0/types_aiobotocore_tnb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    30010 2023-12-13 19:57:22.000000 types-aiobotocore-tnb-2.9.0/types_aiobotocore_tnb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:57:21.000000 types-aiobotocore-tnb-2.9.0/types_aiobotocore_tnb/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:41.489044 types-aiobotocore-tnb-2.9.0/types_aiobotocore_tnb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13659 2023-12-13 20:00:41.000000 types-aiobotocore-tnb-2.9.0/types_aiobotocore_tnb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      737 2023-12-13 20:00:41.000000 types-aiobotocore-tnb-2.9.0/types_aiobotocore_tnb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:41.000000 types-aiobotocore-tnb-2.9.0/types_aiobotocore_tnb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:41.000000 types-aiobotocore-tnb-2.9.0/types_aiobotocore_tnb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:41.000000 types-aiobotocore-tnb-2.9.0/types_aiobotocore_tnb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-13 20:00:41.000000 types-aiobotocore-tnb-2.9.0/types_aiobotocore_tnb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:58.856989 types-aiobotocore-tnb-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:18:50.000000 types-aiobotocore-tnb-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13679 2024-01-18 01:21:58.856989 types-aiobotocore-tnb-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12096 2024-01-18 01:18:50.000000 types-aiobotocore-tnb-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:58.856989 types-aiobotocore-tnb-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-01-18 01:18:50.000000 types-aiobotocore-tnb-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:58.852989 types-aiobotocore-tnb-2.9.1/types_aiobotocore_tnb/
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-01-18 01:18:50.000000 types-aiobotocore-tnb-2.9.1/types_aiobotocore_tnb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-01-18 01:18:50.000000 types-aiobotocore-tnb-2.9.1/types_aiobotocore_tnb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-01-18 01:18:50.000000 types-aiobotocore-tnb-2.9.1/types_aiobotocore_tnb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27008 2024-01-18 01:18:50.000000 types-aiobotocore-tnb-2.9.1/types_aiobotocore_tnb/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27005 2024-01-18 01:18:50.000000 types-aiobotocore-tnb-2.9.1/types_aiobotocore_tnb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10706 2024-01-18 01:18:50.000000 types-aiobotocore-tnb-2.9.1/types_aiobotocore_tnb/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10706 2024-01-18 01:18:50.000000 types-aiobotocore-tnb-2.9.1/types_aiobotocore_tnb/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6826 2024-01-18 01:18:50.000000 types-aiobotocore-tnb-2.9.1/types_aiobotocore_tnb/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6820 2024-01-18 01:18:50.000000 types-aiobotocore-tnb-2.9.1/types_aiobotocore_tnb/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:18:50.000000 types-aiobotocore-tnb-2.9.1/types_aiobotocore_tnb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    30010 2024-01-18 01:18:51.000000 types-aiobotocore-tnb-2.9.1/types_aiobotocore_tnb/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30010 2024-01-18 01:18:51.000000 types-aiobotocore-tnb-2.9.1/types_aiobotocore_tnb/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:18:50.000000 types-aiobotocore-tnb-2.9.1/types_aiobotocore_tnb/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:58.852989 types-aiobotocore-tnb-2.9.1/types_aiobotocore_tnb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13679 2024-01-18 01:21:58.000000 types-aiobotocore-tnb-2.9.1/types_aiobotocore_tnb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-01-18 01:21:58.000000 types-aiobotocore-tnb-2.9.1/types_aiobotocore_tnb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:58.000000 types-aiobotocore-tnb-2.9.1/types_aiobotocore_tnb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:58.000000 types-aiobotocore-tnb-2.9.1/types_aiobotocore_tnb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:58.000000 types-aiobotocore-tnb-2.9.1/types_aiobotocore_tnb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-18 01:21:58.000000 types-aiobotocore-tnb-2.9.1/types_aiobotocore_tnb.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-tnb-2.9.0/LICENSE` & `types-aiobotocore-tnb-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-tnb-2.9.0/PKG-INFO` & `types-aiobotocore-tnb-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-tnb
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.TelcoNetworkBuilder 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.TelcoNetworkBuilder 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/
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
 
 <a id="types-aiobotocore-tnb"></a>
 
 # types-aiobotocore-tnb
 
 [![PyPI - types-aiobotocore-tnb](https://img.shields.io/pypi/v/types-aiobotocore-tnb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-tnb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-tnb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-tnb)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-tnb)](https://pepy.tech/project/types-aiobotocore-tnb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.TelcoNetworkBuilder 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder)
+[aiobotocore.TelcoNetworkBuilder 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder)
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
 [types-aiobotocore-tnb docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-tnb-2.9.0/README.md` & `types-aiobotocore-tnb-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-tnb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-tnb)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-tnb)](https://pepy.tech/project/types-aiobotocore-tnb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.TelcoNetworkBuilder 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder)
+[aiobotocore.TelcoNetworkBuilder 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder)
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
 [types-aiobotocore-tnb docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-tnb-2.9.0/setup.py` & `types-aiobotocore-tnb-2.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-tnb",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_tnb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.TelcoNetworkBuilder 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.TelcoNetworkBuilder 2.9.1 service generated with"
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
     keywords="aiobotocore tnb type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_tnb": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-tnb-2.9.0/types_aiobotocore_tnb/__init__.py` & `types-aiobotocore-tnb-2.9.1/types_aiobotocore_tnb/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     ListSolNetworkInstancesPaginator,
     ListSolNetworkOperationsPaginator,
     ListSolNetworkPackagesPaginator,
 )
 
 Client = TelcoNetworkBuilderClient
 
-
 __all__ = (
     "Client",
     "ListSolFunctionInstancesPaginator",
     "ListSolFunctionPackagesPaginator",
     "ListSolNetworkInstancesPaginator",
     "ListSolNetworkOperationsPaginator",
     "ListSolNetworkPackagesPaginator",
```

### Comparing `types-aiobotocore-tnb-2.9.0/types_aiobotocore_tnb/__init__.pyi` & `types-aiobotocore-tnb-2.9.1/types_aiobotocore_tnb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-tnb-2.9.0/types_aiobotocore_tnb/__main__.py` & `types-aiobotocore-tnb-2.9.1/types_aiobotocore_tnb/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.TelcoNetworkBuilder 2.9.0\nVersion:        "
-        " 2.9.0\nBuilder version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.TelcoNetworkBuilder 2.9.1\nVersion:        "
+        " 2.9.1\nBuilder version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder\nOther"
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

### Comparing `types-aiobotocore-tnb-2.9.0/types_aiobotocore_tnb/client.py` & `types-aiobotocore-tnb-2.9.1/types_aiobotocore_tnb/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("TelcoNetworkBuilderClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -144,15 +143,15 @@
 
     async def create_sol_network_instance(
         self,
         *,
         nsName: str,
         nsdInfoId: str,
         nsDescription: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateSolNetworkInstanceOutputTypeDef:
         """
         Creates a network instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Client.create_sol_network_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/client/#create_sol_network_instance)
         """
@@ -303,15 +302,15 @@
 
     async def instantiate_sol_network_instance(
         self,
         *,
         nsInstanceId: str,
         additionalParamsForNs: Mapping[str, Any] = ...,
         dryRun: bool = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> InstantiateSolNetworkInstanceOutputTypeDef:
         """
         Instantiates a network instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Client.instantiate_sol_network_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/client/#instantiate_sol_network_instance)
         """
@@ -434,15 +433,15 @@
 
     async def update_sol_network_instance(
         self,
         *,
         nsInstanceId: str,
         updateType: Literal["MODIFY_VNF_INFORMATION"],
         modifyVnfInfoData: UpdateSolNetworkModifyTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> UpdateSolNetworkInstanceOutputTypeDef:
         """
         Update a network instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Client.update_sol_network_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/client/#update_sol_network_instance)
         """
```

### Comparing `types-aiobotocore-tnb-2.9.0/types_aiobotocore_tnb/client.pyi` & `types-aiobotocore-tnb-2.9.1/types_aiobotocore_tnb/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,15 @@
 
     async def create_sol_network_instance(
         self,
         *,
         nsName: str,
         nsdInfoId: str,
         nsDescription: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateSolNetworkInstanceOutputTypeDef:
         """
         Creates a network instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Client.create_sol_network_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/client/#create_sol_network_instance)
         """
@@ -299,15 +299,15 @@
 
     async def instantiate_sol_network_instance(
         self,
         *,
         nsInstanceId: str,
         additionalParamsForNs: Mapping[str, Any] = ...,
         dryRun: bool = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> InstantiateSolNetworkInstanceOutputTypeDef:
         """
         Instantiates a network instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Client.instantiate_sol_network_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/client/#instantiate_sol_network_instance)
         """
@@ -430,15 +430,15 @@
 
     async def update_sol_network_instance(
         self,
         *,
         nsInstanceId: str,
         updateType: Literal["MODIFY_VNF_INFORMATION"],
         modifyVnfInfoData: UpdateSolNetworkModifyTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> UpdateSolNetworkInstanceOutputTypeDef:
         """
         Update a network instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Client.update_sol_network_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/client/#update_sol_network_instance)
         """
```

### Comparing `types-aiobotocore-tnb-2.9.0/types_aiobotocore_tnb/literals.py` & `types-aiobotocore-tnb-2.9.1/types_aiobotocore_tnb/literals.py`

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
     "DescriptorContentTypeType",
     "LcmOperationTypeType",
     "ListSolFunctionInstancesPaginatorName",
     "ListSolFunctionPackagesPaginatorName",
     "ListSolNetworkInstancesPaginatorName",
     "ListSolNetworkOperationsPaginatorName",
@@ -44,15 +43,14 @@
     "TelcoNetworkBuilderServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 DescriptorContentTypeType = Literal["text/plain"]
 LcmOperationTypeType = Literal["INSTANTIATE", "TERMINATE", "UPDATE"]
 ListSolFunctionInstancesPaginatorName = Literal["list_sol_function_instances"]
 ListSolFunctionPackagesPaginatorName = Literal["list_sol_function_packages"]
 ListSolNetworkInstancesPaginatorName = Literal["list_sol_network_instances"]
 ListSolNetworkOperationsPaginatorName = Literal["list_sol_network_operations"]
 ListSolNetworkPackagesPaginatorName = Literal["list_sol_network_packages"]
```

### Comparing `types-aiobotocore-tnb-2.9.0/types_aiobotocore_tnb/literals.pyi` & `types-aiobotocore-tnb-2.9.1/types_aiobotocore_tnb/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-tnb-2.9.0/types_aiobotocore_tnb/paginator.py` & `types-aiobotocore-tnb-2.9.1/types_aiobotocore_tnb/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,14 @@
     "ListSolFunctionInstancesPaginator",
     "ListSolFunctionPackagesPaginator",
     "ListSolNetworkInstancesPaginator",
     "ListSolNetworkOperationsPaginator",
     "ListSolNetworkPackagesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
```

### Comparing `types-aiobotocore-tnb-2.9.0/types_aiobotocore_tnb/paginator.pyi` & `types-aiobotocore-tnb-2.9.1/types_aiobotocore_tnb/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-tnb-2.9.0/types_aiobotocore_tnb/type_defs.py` & `types-aiobotocore-tnb-2.9.1/types_aiobotocore_tnb/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "BlobTypeDef",
     "CancelSolNetworkOperationInputRequestTypeDef",
     "CreateSolFunctionPackageInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CreateSolNetworkInstanceInputRequestTypeDef",
     "CreateSolNetworkPackageInputRequestTypeDef",
```

### Comparing `types-aiobotocore-tnb-2.9.0/types_aiobotocore_tnb/type_defs.pyi` & `types-aiobotocore-tnb-2.9.1/types_aiobotocore_tnb/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-tnb-2.9.0/types_aiobotocore_tnb.egg-info/PKG-INFO` & `types-aiobotocore-tnb-2.9.1/types_aiobotocore_tnb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-tnb
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.TelcoNetworkBuilder 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.TelcoNetworkBuilder 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/
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
 
 <a id="types-aiobotocore-tnb"></a>
 
 # types-aiobotocore-tnb
 
 [![PyPI - types-aiobotocore-tnb](https://img.shields.io/pypi/v/types-aiobotocore-tnb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-tnb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-tnb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-tnb)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-tnb)](https://pepy.tech/project/types-aiobotocore-tnb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.TelcoNetworkBuilder 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder)
+[aiobotocore.TelcoNetworkBuilder 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder)
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
 [types-aiobotocore-tnb docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-tnb-2.9.0/types_aiobotocore_tnb.egg-info/SOURCES.txt` & `types-aiobotocore-tnb-2.9.1/types_aiobotocore_tnb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

