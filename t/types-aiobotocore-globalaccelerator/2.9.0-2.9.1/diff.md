# Comparing `tmp/types-aiobotocore-globalaccelerator-2.9.0.tar.gz` & `tmp/types-aiobotocore-globalaccelerator-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-globalaccelerator-2.9.0.tar", last modified: Wed Dec 13 19:59:23 2023, max compression
+gzip compressed data, was "types-aiobotocore-globalaccelerator-2.9.1.tar", last modified: Thu Jan 18 01:20:47 2024, max compression
```

## Comparing `types-aiobotocore-globalaccelerator-2.9.0.tar` & `types-aiobotocore-globalaccelerator-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:23.149730 types-aiobotocore-globalaccelerator-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:46:41.000000 types-aiobotocore-globalaccelerator-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15465 2023-12-13 19:59:23.149730 types-aiobotocore-globalaccelerator-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13862 2023-12-13 19:46:41.000000 types-aiobotocore-globalaccelerator-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:23.149730 types-aiobotocore-globalaccelerator-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2023-12-13 19:46:41.000000 types-aiobotocore-globalaccelerator-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:23.149730 types-aiobotocore-globalaccelerator-2.9.0/types_aiobotocore_globalaccelerator/
--rw-r--r--   0 runner    (1001) docker     (127)     3390 2023-12-13 19:46:41.000000 types-aiobotocore-globalaccelerator-2.9.0/types_aiobotocore_globalaccelerator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2023-12-13 19:46:41.000000 types-aiobotocore-globalaccelerator-2.9.0/types_aiobotocore_globalaccelerator/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      972 2023-12-13 19:46:41.000000 types-aiobotocore-globalaccelerator-2.9.0/types_aiobotocore_globalaccelerator/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    50714 2023-12-13 19:46:42.000000 types-aiobotocore-globalaccelerator-2.9.0/types_aiobotocore_globalaccelerator/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    50710 2023-12-13 19:46:41.000000 types-aiobotocore-globalaccelerator-2.9.0/types_aiobotocore_globalaccelerator/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11157 2023-12-13 19:46:42.000000 types-aiobotocore-globalaccelerator-2.9.0/types_aiobotocore_globalaccelerator/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11155 2023-12-13 19:46:42.000000 types-aiobotocore-globalaccelerator-2.9.0/types_aiobotocore_globalaccelerator/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    15068 2023-12-13 19:46:42.000000 types-aiobotocore-globalaccelerator-2.9.0/types_aiobotocore_globalaccelerator/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    15055 2023-12-13 19:46:42.000000 types-aiobotocore-globalaccelerator-2.9.0/types_aiobotocore_globalaccelerator/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:46:41.000000 types-aiobotocore-globalaccelerator-2.9.0/types_aiobotocore_globalaccelerator/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    42534 2023-12-13 19:46:42.000000 types-aiobotocore-globalaccelerator-2.9.0/types_aiobotocore_globalaccelerator/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    42533 2023-12-13 19:46:42.000000 types-aiobotocore-globalaccelerator-2.9.0/types_aiobotocore_globalaccelerator/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:46:41.000000 types-aiobotocore-globalaccelerator-2.9.0/types_aiobotocore_globalaccelerator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:23.149730 types-aiobotocore-globalaccelerator-2.9.0/types_aiobotocore_globalaccelerator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15465 2023-12-13 19:59:23.000000 types-aiobotocore-globalaccelerator-2.9.0/types_aiobotocore_globalaccelerator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2023-12-13 19:59:23.000000 types-aiobotocore-globalaccelerator-2.9.0/types_aiobotocore_globalaccelerator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:23.000000 types-aiobotocore-globalaccelerator-2.9.0/types_aiobotocore_globalaccelerator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:23.000000 types-aiobotocore-globalaccelerator-2.9.0/types_aiobotocore_globalaccelerator.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:23.000000 types-aiobotocore-globalaccelerator-2.9.0/types_aiobotocore_globalaccelerator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-13 19:59:23.000000 types-aiobotocore-globalaccelerator-2.9.0/types_aiobotocore_globalaccelerator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:47.297312 types-aiobotocore-globalaccelerator-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:08:34.000000 types-aiobotocore-globalaccelerator-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15485 2024-01-18 01:20:47.297312 types-aiobotocore-globalaccelerator-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13862 2024-01-18 01:08:34.000000 types-aiobotocore-globalaccelerator-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:47.297312 types-aiobotocore-globalaccelerator-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-01-18 01:08:34.000000 types-aiobotocore-globalaccelerator-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:47.293312 types-aiobotocore-globalaccelerator-2.9.1/types_aiobotocore_globalaccelerator/
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-01-18 01:08:34.000000 types-aiobotocore-globalaccelerator-2.9.1/types_aiobotocore_globalaccelerator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-01-18 01:08:34.000000 types-aiobotocore-globalaccelerator-2.9.1/types_aiobotocore_globalaccelerator/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-01-18 01:08:34.000000 types-aiobotocore-globalaccelerator-2.9.1/types_aiobotocore_globalaccelerator/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50733 2024-01-18 01:08:35.000000 types-aiobotocore-globalaccelerator-2.9.1/types_aiobotocore_globalaccelerator/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50730 2024-01-18 01:08:35.000000 types-aiobotocore-globalaccelerator-2.9.1/types_aiobotocore_globalaccelerator/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11155 2024-01-18 01:08:35.000000 types-aiobotocore-globalaccelerator-2.9.1/types_aiobotocore_globalaccelerator/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11155 2024-01-18 01:08:35.000000 types-aiobotocore-globalaccelerator-2.9.1/types_aiobotocore_globalaccelerator/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    15070 2024-01-18 01:08:35.000000 types-aiobotocore-globalaccelerator-2.9.1/types_aiobotocore_globalaccelerator/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15058 2024-01-18 01:08:35.000000 types-aiobotocore-globalaccelerator-2.9.1/types_aiobotocore_globalaccelerator/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:08:34.000000 types-aiobotocore-globalaccelerator-2.9.1/types_aiobotocore_globalaccelerator/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    42533 2024-01-18 01:08:36.000000 types-aiobotocore-globalaccelerator-2.9.1/types_aiobotocore_globalaccelerator/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42533 2024-01-18 01:08:35.000000 types-aiobotocore-globalaccelerator-2.9.1/types_aiobotocore_globalaccelerator/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:08:34.000000 types-aiobotocore-globalaccelerator-2.9.1/types_aiobotocore_globalaccelerator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:47.297312 types-aiobotocore-globalaccelerator-2.9.1/types_aiobotocore_globalaccelerator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15485 2024-01-18 01:20:47.000000 types-aiobotocore-globalaccelerator-2.9.1/types_aiobotocore_globalaccelerator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-01-18 01:20:47.000000 types-aiobotocore-globalaccelerator-2.9.1/types_aiobotocore_globalaccelerator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:47.000000 types-aiobotocore-globalaccelerator-2.9.1/types_aiobotocore_globalaccelerator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:47.000000 types-aiobotocore-globalaccelerator-2.9.1/types_aiobotocore_globalaccelerator.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:47.000000 types-aiobotocore-globalaccelerator-2.9.1/types_aiobotocore_globalaccelerator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-01-18 01:20:47.000000 types-aiobotocore-globalaccelerator-2.9.1/types_aiobotocore_globalaccelerator.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-globalaccelerator-2.9.0/LICENSE` & `types-aiobotocore-globalaccelerator-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-globalaccelerator-2.9.0/PKG-INFO` & `types-aiobotocore-globalaccelerator-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-globalaccelerator
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.GlobalAccelerator 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.GlobalAccelerator 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator/
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
 
 <a id="types-aiobotocore-globalaccelerator"></a>
 
 # types-aiobotocore-globalaccelerator
 
 [![PyPI - types-aiobotocore-globalaccelerator](https://img.shields.io/pypi/v/types-aiobotocore-globalaccelerator.svg?color=blue)](https://pypi.org/project/types-aiobotocore-globalaccelerator)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-globalaccelerator.svg?color=blue)](https://pypi.org/project/types-aiobotocore-globalaccelerator)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-globalaccelerator)](https://pepy.tech/project/types-aiobotocore-globalaccelerator)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.GlobalAccelerator 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator)
+[aiobotocore.GlobalAccelerator 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator)
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
 [types-aiobotocore-globalaccelerator docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-globalaccelerator-2.9.0/README.md` & `types-aiobotocore-globalaccelerator-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-globalaccelerator.svg?color=blue)](https://pypi.org/project/types-aiobotocore-globalaccelerator)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-globalaccelerator)](https://pepy.tech/project/types-aiobotocore-globalaccelerator)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.GlobalAccelerator 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator)
+[aiobotocore.GlobalAccelerator 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator)
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
 [types-aiobotocore-globalaccelerator docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-globalaccelerator-2.9.0/setup.py` & `types-aiobotocore-globalaccelerator-2.9.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-globalaccelerator",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_globalaccelerator"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.GlobalAccelerator 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.GlobalAccelerator 2.9.1 service generated with"
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
     keywords="aiobotocore globalaccelerator type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_globalaccelerator": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-globalaccelerator-2.9.0/types_aiobotocore_globalaccelerator/__init__.py` & `types-aiobotocore-globalaccelerator-2.9.1/types_aiobotocore_globalaccelerator/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,14 @@
     ListCustomRoutingPortMappingsPaginator,
     ListEndpointGroupsPaginator,
     ListListenersPaginator,
 )
 
 Client = GlobalAcceleratorClient
 
-
 __all__ = (
     "Client",
     "GlobalAcceleratorClient",
     "ListAcceleratorsPaginator",
     "ListByoipCidrsPaginator",
     "ListCrossAccountAttachmentsPaginator",
     "ListCrossAccountResourcesPaginator",
```

### Comparing `types-aiobotocore-globalaccelerator-2.9.0/types_aiobotocore_globalaccelerator/__init__.pyi` & `types-aiobotocore-globalaccelerator-2.9.1/types_aiobotocore_globalaccelerator/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-globalaccelerator-2.9.0/types_aiobotocore_globalaccelerator/__main__.py` & `types-aiobotocore-globalaccelerator-2.9.1/types_aiobotocore_globalaccelerator/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.GlobalAccelerator 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.GlobalAccelerator 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator\nOther"
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

### Comparing `types-aiobotocore-globalaccelerator-2.9.0/types_aiobotocore_globalaccelerator/client.py` & `types-aiobotocore-globalaccelerator-2.9.1/types_aiobotocore_globalaccelerator/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("GlobalAcceleratorClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -149,30 +148,30 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator/client/#exceptions)
         """
 
     async def add_custom_routing_endpoints(
         self,
         *,
         EndpointConfigurations: Sequence[CustomRoutingEndpointConfigurationTypeDef],
-        EndpointGroupArn: str
+        EndpointGroupArn: str,
     ) -> AddCustomRoutingEndpointsResponseTypeDef:
         """
         Associate a virtual private cloud (VPC) subnet endpoint with your custom
         routing
         accelerator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Client.add_custom_routing_endpoints)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator/client/#add_custom_routing_endpoints)
         """
 
     async def add_endpoints(
         self,
         *,
         EndpointConfigurations: Sequence[EndpointConfigurationTypeDef],
-        EndpointGroupArn: str
+        EndpointGroupArn: str,
     ) -> AddEndpointsResponseTypeDef:
         """
         Add endpoints to an endpoint group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Client.add_endpoints)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator/client/#add_endpoints)
         """
@@ -190,15 +189,15 @@
     async def allow_custom_routing_traffic(
         self,
         *,
         EndpointGroupArn: str,
         EndpointId: str,
         DestinationAddresses: Sequence[str] = ...,
         DestinationPorts: Sequence[int] = ...,
-        AllowAllTrafficToEndpoint: bool = ...
+        AllowAllTrafficToEndpoint: bool = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Specify the Amazon EC2 instance (destination) IP addresses and ports for a VPC
         subnet endpoint that can receive traffic for a custom routing
         accelerator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Client.allow_custom_routing_traffic)
@@ -225,15 +224,15 @@
         self,
         *,
         Name: str,
         IdempotencyToken: str,
         IpAddressType: IpAddressTypeType = ...,
         IpAddresses: Sequence[str] = ...,
         Enabled: bool = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateAcceleratorResponseTypeDef:
         """
         Create an accelerator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Client.create_accelerator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator/client/#create_accelerator)
         """
@@ -241,15 +240,15 @@
     async def create_cross_account_attachment(
         self,
         *,
         Name: str,
         IdempotencyToken: str,
         Principals: Sequence[str] = ...,
         Resources: Sequence[ResourceTypeDef] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateCrossAccountAttachmentResponseTypeDef:
         """
         Create a cross-account attachment in Global Accelerator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Client.create_cross_account_attachment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator/client/#create_cross_account_attachment)
         """
@@ -258,30 +257,30 @@
         self,
         *,
         Name: str,
         IdempotencyToken: str,
         IpAddressType: IpAddressTypeType = ...,
         IpAddresses: Sequence[str] = ...,
         Enabled: bool = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateCustomRoutingAcceleratorResponseTypeDef:
         """
         Create a custom routing accelerator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Client.create_custom_routing_accelerator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator/client/#create_custom_routing_accelerator)
         """
 
     async def create_custom_routing_endpoint_group(
         self,
         *,
         ListenerArn: str,
         EndpointGroupRegion: str,
         DestinationConfigurations: Sequence[CustomRoutingDestinationConfigurationTypeDef],
-        IdempotencyToken: str
+        IdempotencyToken: str,
     ) -> CreateCustomRoutingEndpointGroupResponseTypeDef:
         """
         Create an endpoint group for the specified listener for a custom routing
         accelerator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Client.create_custom_routing_endpoint_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator/client/#create_custom_routing_endpoint_group)
@@ -308,15 +307,15 @@
         EndpointConfigurations: Sequence[EndpointConfigurationTypeDef] = ...,
         TrafficDialPercentage: float = ...,
         HealthCheckPort: int = ...,
         HealthCheckProtocol: HealthCheckProtocolType = ...,
         HealthCheckPath: str = ...,
         HealthCheckIntervalSeconds: int = ...,
         ThresholdCount: int = ...,
-        PortOverrides: Sequence[PortOverrideTypeDef] = ...
+        PortOverrides: Sequence[PortOverrideTypeDef] = ...,
     ) -> CreateEndpointGroupResponseTypeDef:
         """
         Create an endpoint group for the specified listener.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Client.create_endpoint_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator/client/#create_endpoint_group)
         """
@@ -324,15 +323,15 @@
     async def create_listener(
         self,
         *,
         AcceleratorArn: str,
         PortRanges: Sequence[PortRangeTypeDef],
         Protocol: ProtocolType,
         IdempotencyToken: str,
-        ClientAffinity: ClientAffinityType = ...
+        ClientAffinity: ClientAffinityType = ...,
     ) -> CreateListenerResponseTypeDef:
         """
         Create a listener to process inbound connections from clients to an accelerator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Client.create_listener)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator/client/#create_listener)
         """
@@ -404,15 +403,15 @@
     async def deny_custom_routing_traffic(
         self,
         *,
         EndpointGroupArn: str,
         EndpointId: str,
         DestinationAddresses: Sequence[str] = ...,
         DestinationPorts: Sequence[int] = ...,
-        DenyAllTrafficToEndpoint: bool = ...
+        DenyAllTrafficToEndpoint: bool = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Specify the Amazon EC2 instance (destination) IP addresses and ports for a VPC
         subnet endpoint that cannot receive traffic for a custom routing
         accelerator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Client.deny_custom_routing_traffic)
@@ -577,15 +576,15 @@
 
     async def list_cross_account_resources(
         self,
         *,
         ResourceOwnerAwsAccountId: str,
         AcceleratorArn: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListCrossAccountResourcesResponseTypeDef:
         """
         List the cross-account endpoints available to add to an accelerator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Client.list_cross_account_resources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator/client/#list_cross_account_resources)
         """
@@ -624,15 +623,15 @@
 
     async def list_custom_routing_port_mappings(
         self,
         *,
         AcceleratorArn: str,
         EndpointGroupArn: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListCustomRoutingPortMappingsResponseTypeDef:
         """
         Provides a complete mapping from the public accelerator IP address and port to
         destination EC2 instance IP addresses and ports in the virtual public cloud
         (VPC) subnet endpoint for a custom routing
         accelerator.
 
@@ -642,15 +641,15 @@
 
     async def list_custom_routing_port_mappings_by_destination(
         self,
         *,
         EndpointId: str,
         DestinationAddress: str,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListCustomRoutingPortMappingsByDestinationResponseTypeDef:
         """
         List the port mappings for a specific EC2 instance (destination) in a VPC
         subnet
         endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Client.list_custom_routing_port_mappings_by_destination)
@@ -737,15 +736,15 @@
 
     async def update_accelerator(
         self,
         *,
         AcceleratorArn: str,
         Name: str = ...,
         IpAddressType: IpAddressTypeType = ...,
-        Enabled: bool = ...
+        Enabled: bool = ...,
     ) -> UpdateAcceleratorResponseTypeDef:
         """
         Update an accelerator to make changes, such as the following: * Change the name
         of the
         accelerator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Client.update_accelerator)
@@ -754,15 +753,15 @@
 
     async def update_accelerator_attributes(
         self,
         *,
         AcceleratorArn: str,
         FlowLogsEnabled: bool = ...,
         FlowLogsS3Bucket: str = ...,
-        FlowLogsS3Prefix: str = ...
+        FlowLogsS3Prefix: str = ...,
     ) -> UpdateAcceleratorAttributesResponseTypeDef:
         """
         Update the attributes for an accelerator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Client.update_accelerator_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator/client/#update_accelerator_attributes)
         """
@@ -771,45 +770,45 @@
         self,
         *,
         AttachmentArn: str,
         Name: str = ...,
         AddPrincipals: Sequence[str] = ...,
         RemovePrincipals: Sequence[str] = ...,
         AddResources: Sequence[ResourceTypeDef] = ...,
-        RemoveResources: Sequence[ResourceTypeDef] = ...
+        RemoveResources: Sequence[ResourceTypeDef] = ...,
     ) -> UpdateCrossAccountAttachmentResponseTypeDef:
         """
         Update a cross-account attachment to add or remove principals or resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Client.update_cross_account_attachment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator/client/#update_cross_account_attachment)
         """
 
     async def update_custom_routing_accelerator(
         self,
         *,
         AcceleratorArn: str,
         Name: str = ...,
         IpAddressType: IpAddressTypeType = ...,
-        Enabled: bool = ...
+        Enabled: bool = ...,
     ) -> UpdateCustomRoutingAcceleratorResponseTypeDef:
         """
         Update a custom routing accelerator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Client.update_custom_routing_accelerator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator/client/#update_custom_routing_accelerator)
         """
 
     async def update_custom_routing_accelerator_attributes(
         self,
         *,
         AcceleratorArn: str,
         FlowLogsEnabled: bool = ...,
         FlowLogsS3Bucket: str = ...,
-        FlowLogsS3Prefix: str = ...
+        FlowLogsS3Prefix: str = ...,
     ) -> UpdateCustomRoutingAcceleratorAttributesResponseTypeDef:
         """
         Update the attributes for a custom routing accelerator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Client.update_custom_routing_accelerator_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator/client/#update_custom_routing_accelerator_attributes)
         """
@@ -831,30 +830,30 @@
         EndpointConfigurations: Sequence[EndpointConfigurationTypeDef] = ...,
         TrafficDialPercentage: float = ...,
         HealthCheckPort: int = ...,
         HealthCheckProtocol: HealthCheckProtocolType = ...,
         HealthCheckPath: str = ...,
         HealthCheckIntervalSeconds: int = ...,
         ThresholdCount: int = ...,
-        PortOverrides: Sequence[PortOverrideTypeDef] = ...
+        PortOverrides: Sequence[PortOverrideTypeDef] = ...,
     ) -> UpdateEndpointGroupResponseTypeDef:
         """
         Update an endpoint group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Client.update_endpoint_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator/client/#update_endpoint_group)
         """
 
     async def update_listener(
         self,
         *,
         ListenerArn: str,
         PortRanges: Sequence[PortRangeTypeDef] = ...,
         Protocol: ProtocolType = ...,
-        ClientAffinity: ClientAffinityType = ...
+        ClientAffinity: ClientAffinityType = ...,
     ) -> UpdateListenerResponseTypeDef:
         """
         Update a listener.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Client.update_listener)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator/client/#update_listener)
         """
```

### Comparing `types-aiobotocore-globalaccelerator-2.9.0/types_aiobotocore_globalaccelerator/client.pyi` & `types-aiobotocore-globalaccelerator-2.9.1/types_aiobotocore_globalaccelerator/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -145,30 +145,30 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator/client/#exceptions)
         """
 
     async def add_custom_routing_endpoints(
         self,
         *,
         EndpointConfigurations: Sequence[CustomRoutingEndpointConfigurationTypeDef],
-        EndpointGroupArn: str
+        EndpointGroupArn: str,
     ) -> AddCustomRoutingEndpointsResponseTypeDef:
         """
         Associate a virtual private cloud (VPC) subnet endpoint with your custom
         routing
         accelerator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Client.add_custom_routing_endpoints)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator/client/#add_custom_routing_endpoints)
         """
 
     async def add_endpoints(
         self,
         *,
         EndpointConfigurations: Sequence[EndpointConfigurationTypeDef],
-        EndpointGroupArn: str
+        EndpointGroupArn: str,
     ) -> AddEndpointsResponseTypeDef:
         """
         Add endpoints to an endpoint group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Client.add_endpoints)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator/client/#add_endpoints)
         """
@@ -186,15 +186,15 @@
     async def allow_custom_routing_traffic(
         self,
         *,
         EndpointGroupArn: str,
         EndpointId: str,
         DestinationAddresses: Sequence[str] = ...,
         DestinationPorts: Sequence[int] = ...,
-        AllowAllTrafficToEndpoint: bool = ...
+        AllowAllTrafficToEndpoint: bool = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Specify the Amazon EC2 instance (destination) IP addresses and ports for a VPC
         subnet endpoint that can receive traffic for a custom routing
         accelerator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Client.allow_custom_routing_traffic)
@@ -221,15 +221,15 @@
         self,
         *,
         Name: str,
         IdempotencyToken: str,
         IpAddressType: IpAddressTypeType = ...,
         IpAddresses: Sequence[str] = ...,
         Enabled: bool = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateAcceleratorResponseTypeDef:
         """
         Create an accelerator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Client.create_accelerator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator/client/#create_accelerator)
         """
@@ -237,15 +237,15 @@
     async def create_cross_account_attachment(
         self,
         *,
         Name: str,
         IdempotencyToken: str,
         Principals: Sequence[str] = ...,
         Resources: Sequence[ResourceTypeDef] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateCrossAccountAttachmentResponseTypeDef:
         """
         Create a cross-account attachment in Global Accelerator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Client.create_cross_account_attachment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator/client/#create_cross_account_attachment)
         """
@@ -254,30 +254,30 @@
         self,
         *,
         Name: str,
         IdempotencyToken: str,
         IpAddressType: IpAddressTypeType = ...,
         IpAddresses: Sequence[str] = ...,
         Enabled: bool = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateCustomRoutingAcceleratorResponseTypeDef:
         """
         Create a custom routing accelerator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Client.create_custom_routing_accelerator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator/client/#create_custom_routing_accelerator)
         """
 
     async def create_custom_routing_endpoint_group(
         self,
         *,
         ListenerArn: str,
         EndpointGroupRegion: str,
         DestinationConfigurations: Sequence[CustomRoutingDestinationConfigurationTypeDef],
-        IdempotencyToken: str
+        IdempotencyToken: str,
     ) -> CreateCustomRoutingEndpointGroupResponseTypeDef:
         """
         Create an endpoint group for the specified listener for a custom routing
         accelerator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Client.create_custom_routing_endpoint_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator/client/#create_custom_routing_endpoint_group)
@@ -304,15 +304,15 @@
         EndpointConfigurations: Sequence[EndpointConfigurationTypeDef] = ...,
         TrafficDialPercentage: float = ...,
         HealthCheckPort: int = ...,
         HealthCheckProtocol: HealthCheckProtocolType = ...,
         HealthCheckPath: str = ...,
         HealthCheckIntervalSeconds: int = ...,
         ThresholdCount: int = ...,
-        PortOverrides: Sequence[PortOverrideTypeDef] = ...
+        PortOverrides: Sequence[PortOverrideTypeDef] = ...,
     ) -> CreateEndpointGroupResponseTypeDef:
         """
         Create an endpoint group for the specified listener.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Client.create_endpoint_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator/client/#create_endpoint_group)
         """
@@ -320,15 +320,15 @@
     async def create_listener(
         self,
         *,
         AcceleratorArn: str,
         PortRanges: Sequence[PortRangeTypeDef],
         Protocol: ProtocolType,
         IdempotencyToken: str,
-        ClientAffinity: ClientAffinityType = ...
+        ClientAffinity: ClientAffinityType = ...,
     ) -> CreateListenerResponseTypeDef:
         """
         Create a listener to process inbound connections from clients to an accelerator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Client.create_listener)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator/client/#create_listener)
         """
@@ -400,15 +400,15 @@
     async def deny_custom_routing_traffic(
         self,
         *,
         EndpointGroupArn: str,
         EndpointId: str,
         DestinationAddresses: Sequence[str] = ...,
         DestinationPorts: Sequence[int] = ...,
-        DenyAllTrafficToEndpoint: bool = ...
+        DenyAllTrafficToEndpoint: bool = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Specify the Amazon EC2 instance (destination) IP addresses and ports for a VPC
         subnet endpoint that cannot receive traffic for a custom routing
         accelerator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Client.deny_custom_routing_traffic)
@@ -573,15 +573,15 @@
 
     async def list_cross_account_resources(
         self,
         *,
         ResourceOwnerAwsAccountId: str,
         AcceleratorArn: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListCrossAccountResourcesResponseTypeDef:
         """
         List the cross-account endpoints available to add to an accelerator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Client.list_cross_account_resources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator/client/#list_cross_account_resources)
         """
@@ -620,15 +620,15 @@
 
     async def list_custom_routing_port_mappings(
         self,
         *,
         AcceleratorArn: str,
         EndpointGroupArn: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListCustomRoutingPortMappingsResponseTypeDef:
         """
         Provides a complete mapping from the public accelerator IP address and port to
         destination EC2 instance IP addresses and ports in the virtual public cloud
         (VPC) subnet endpoint for a custom routing
         accelerator.
 
@@ -638,15 +638,15 @@
 
     async def list_custom_routing_port_mappings_by_destination(
         self,
         *,
         EndpointId: str,
         DestinationAddress: str,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListCustomRoutingPortMappingsByDestinationResponseTypeDef:
         """
         List the port mappings for a specific EC2 instance (destination) in a VPC
         subnet
         endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Client.list_custom_routing_port_mappings_by_destination)
@@ -733,15 +733,15 @@
 
     async def update_accelerator(
         self,
         *,
         AcceleratorArn: str,
         Name: str = ...,
         IpAddressType: IpAddressTypeType = ...,
-        Enabled: bool = ...
+        Enabled: bool = ...,
     ) -> UpdateAcceleratorResponseTypeDef:
         """
         Update an accelerator to make changes, such as the following: * Change the name
         of the
         accelerator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Client.update_accelerator)
@@ -750,15 +750,15 @@
 
     async def update_accelerator_attributes(
         self,
         *,
         AcceleratorArn: str,
         FlowLogsEnabled: bool = ...,
         FlowLogsS3Bucket: str = ...,
-        FlowLogsS3Prefix: str = ...
+        FlowLogsS3Prefix: str = ...,
     ) -> UpdateAcceleratorAttributesResponseTypeDef:
         """
         Update the attributes for an accelerator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Client.update_accelerator_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator/client/#update_accelerator_attributes)
         """
@@ -767,45 +767,45 @@
         self,
         *,
         AttachmentArn: str,
         Name: str = ...,
         AddPrincipals: Sequence[str] = ...,
         RemovePrincipals: Sequence[str] = ...,
         AddResources: Sequence[ResourceTypeDef] = ...,
-        RemoveResources: Sequence[ResourceTypeDef] = ...
+        RemoveResources: Sequence[ResourceTypeDef] = ...,
     ) -> UpdateCrossAccountAttachmentResponseTypeDef:
         """
         Update a cross-account attachment to add or remove principals or resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Client.update_cross_account_attachment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator/client/#update_cross_account_attachment)
         """
 
     async def update_custom_routing_accelerator(
         self,
         *,
         AcceleratorArn: str,
         Name: str = ...,
         IpAddressType: IpAddressTypeType = ...,
-        Enabled: bool = ...
+        Enabled: bool = ...,
     ) -> UpdateCustomRoutingAcceleratorResponseTypeDef:
         """
         Update a custom routing accelerator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Client.update_custom_routing_accelerator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator/client/#update_custom_routing_accelerator)
         """
 
     async def update_custom_routing_accelerator_attributes(
         self,
         *,
         AcceleratorArn: str,
         FlowLogsEnabled: bool = ...,
         FlowLogsS3Bucket: str = ...,
-        FlowLogsS3Prefix: str = ...
+        FlowLogsS3Prefix: str = ...,
     ) -> UpdateCustomRoutingAcceleratorAttributesResponseTypeDef:
         """
         Update the attributes for a custom routing accelerator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Client.update_custom_routing_accelerator_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator/client/#update_custom_routing_accelerator_attributes)
         """
@@ -827,30 +827,30 @@
         EndpointConfigurations: Sequence[EndpointConfigurationTypeDef] = ...,
         TrafficDialPercentage: float = ...,
         HealthCheckPort: int = ...,
         HealthCheckProtocol: HealthCheckProtocolType = ...,
         HealthCheckPath: str = ...,
         HealthCheckIntervalSeconds: int = ...,
         ThresholdCount: int = ...,
-        PortOverrides: Sequence[PortOverrideTypeDef] = ...
+        PortOverrides: Sequence[PortOverrideTypeDef] = ...,
     ) -> UpdateEndpointGroupResponseTypeDef:
         """
         Update an endpoint group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Client.update_endpoint_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator/client/#update_endpoint_group)
         """
 
     async def update_listener(
         self,
         *,
         ListenerArn: str,
         PortRanges: Sequence[PortRangeTypeDef] = ...,
         Protocol: ProtocolType = ...,
-        ClientAffinity: ClientAffinityType = ...
+        ClientAffinity: ClientAffinityType = ...,
     ) -> UpdateListenerResponseTypeDef:
         """
         Update a listener.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Client.update_listener)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator/client/#update_listener)
         """
```

### Comparing `types-aiobotocore-globalaccelerator-2.9.0/types_aiobotocore_globalaccelerator/literals.py` & `types-aiobotocore-globalaccelerator-2.9.1/types_aiobotocore_globalaccelerator/literals.py`

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
     "AcceleratorStatusType",
     "ByoipCidrStateType",
     "ClientAffinityType",
     "CustomRoutingAcceleratorStatusType",
     "CustomRoutingDestinationTrafficStateType",
     "CustomRoutingProtocolType",
@@ -45,15 +44,14 @@
     "ProtocolType",
     "GlobalAcceleratorServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 AcceleratorStatusType = Literal["DEPLOYED", "IN_PROGRESS"]
 ByoipCidrStateType = Literal[
     "ADVERTISING",
     "DEPROVISIONED",
     "FAILED_ADVERTISING",
     "FAILED_DEPROVISION",
     "FAILED_PROVISION",
```

### Comparing `types-aiobotocore-globalaccelerator-2.9.0/types_aiobotocore_globalaccelerator/literals.pyi` & `types-aiobotocore-globalaccelerator-2.9.1/types_aiobotocore_globalaccelerator/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-globalaccelerator-2.9.0/types_aiobotocore_globalaccelerator/paginator.py` & `types-aiobotocore-globalaccelerator-2.9.1/types_aiobotocore_globalaccelerator/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,14 @@
     "ListCustomRoutingListenersPaginator",
     "ListCustomRoutingPortMappingsPaginator",
     "ListCustomRoutingPortMappingsByDestinationPaginator",
     "ListEndpointGroupsPaginator",
     "ListListenersPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -138,15 +137,15 @@
     """
 
     def paginate(
         self,
         *,
         ResourceOwnerAwsAccountId: str,
         AcceleratorArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCrossAccountResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListCrossAccountResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator/paginators/#listcrossaccountresourcespaginator)
         """
 
 
@@ -202,15 +201,15 @@
     """
 
     def paginate(
         self,
         *,
         AcceleratorArn: str,
         EndpointGroupArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCustomRoutingPortMappingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListCustomRoutingPortMappings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator/paginators/#listcustomroutingportmappingspaginator)
         """
 
 
@@ -221,15 +220,15 @@
     """
 
     def paginate(
         self,
         *,
         EndpointId: str,
         DestinationAddress: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCustomRoutingPortMappingsByDestinationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListCustomRoutingPortMappingsByDestination.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator/paginators/#listcustomroutingportmappingsbydestinationpaginator)
         """
```

### Comparing `types-aiobotocore-globalaccelerator-2.9.0/types_aiobotocore_globalaccelerator/paginator.pyi` & `types-aiobotocore-globalaccelerator-2.9.1/types_aiobotocore_globalaccelerator/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
     """
 
     def paginate(
         self,
         *,
         ResourceOwnerAwsAccountId: str,
         AcceleratorArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCrossAccountResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListCrossAccountResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator/paginators/#listcrossaccountresourcespaginator)
         """
 
 class ListCustomRoutingAcceleratorsPaginator(AioPaginator):
@@ -192,15 +192,15 @@
     """
 
     def paginate(
         self,
         *,
         AcceleratorArn: str,
         EndpointGroupArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCustomRoutingPortMappingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListCustomRoutingPortMappings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator/paginators/#listcustomroutingportmappingspaginator)
         """
 
 class ListCustomRoutingPortMappingsByDestinationPaginator(AioPaginator):
@@ -210,15 +210,15 @@
     """
 
     def paginate(
         self,
         *,
         EndpointId: str,
         DestinationAddress: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCustomRoutingPortMappingsByDestinationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListCustomRoutingPortMappingsByDestination.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator/paginators/#listcustomroutingportmappingsbydestinationpaginator)
         """
 
 class ListEndpointGroupsPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-globalaccelerator-2.9.0/types_aiobotocore_globalaccelerator/type_defs.py` & `types-aiobotocore-globalaccelerator-2.9.1/types_aiobotocore_globalaccelerator/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AcceleratorAttributesTypeDef",
     "AcceleratorEventTypeDef",
     "IpSetTypeDef",
     "CustomRoutingEndpointConfigurationTypeDef",
     "CustomRoutingEndpointDescriptionTypeDef",
     "ResponseMetadataTypeDef",
```

### Comparing `types-aiobotocore-globalaccelerator-2.9.0/types_aiobotocore_globalaccelerator/type_defs.pyi` & `types-aiobotocore-globalaccelerator-2.9.1/types_aiobotocore_globalaccelerator/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-globalaccelerator-2.9.0/types_aiobotocore_globalaccelerator.egg-info/PKG-INFO` & `types-aiobotocore-globalaccelerator-2.9.1/types_aiobotocore_globalaccelerator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-globalaccelerator
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.GlobalAccelerator 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.GlobalAccelerator 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator/
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
 
 <a id="types-aiobotocore-globalaccelerator"></a>
 
 # types-aiobotocore-globalaccelerator
 
 [![PyPI - types-aiobotocore-globalaccelerator](https://img.shields.io/pypi/v/types-aiobotocore-globalaccelerator.svg?color=blue)](https://pypi.org/project/types-aiobotocore-globalaccelerator)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-globalaccelerator.svg?color=blue)](https://pypi.org/project/types-aiobotocore-globalaccelerator)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-globalaccelerator)](https://pepy.tech/project/types-aiobotocore-globalaccelerator)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.GlobalAccelerator 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator)
+[aiobotocore.GlobalAccelerator 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator)
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
 [types-aiobotocore-globalaccelerator docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-globalaccelerator-2.9.0/types_aiobotocore_globalaccelerator.egg-info/SOURCES.txt` & `types-aiobotocore-globalaccelerator-2.9.1/types_aiobotocore_globalaccelerator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

