# Comparing `tmp/types-aiobotocore-clouddirectory-2.9.0.tar.gz` & `tmp/types-aiobotocore-clouddirectory-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-clouddirectory-2.9.0.tar", last modified: Wed Dec 13 19:58:48 2023, max compression
+gzip compressed data, was "types-aiobotocore-clouddirectory-2.9.1.tar", last modified: Thu Jan 18 01:20:15 2024, max compression
```

## Comparing `types-aiobotocore-clouddirectory-2.9.0.tar` & `types-aiobotocore-clouddirectory-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:48.453981 types-aiobotocore-clouddirectory-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:42:15.000000 types-aiobotocore-clouddirectory-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16342 2023-12-13 19:58:48.453981 types-aiobotocore-clouddirectory-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14751 2023-12-13 19:42:15.000000 types-aiobotocore-clouddirectory-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:48.453981 types-aiobotocore-clouddirectory-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2023-12-13 19:42:15.000000 types-aiobotocore-clouddirectory-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:48.449981 types-aiobotocore-clouddirectory-2.9.0/types_aiobotocore_clouddirectory/
--rw-r--r--   0 runner    (1001) docker     (127)     4840 2023-12-13 19:42:15.000000 types-aiobotocore-clouddirectory-2.9.0/types_aiobotocore_clouddirectory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4839 2023-12-13 19:42:15.000000 types-aiobotocore-clouddirectory-2.9.0/types_aiobotocore_clouddirectory/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      960 2023-12-13 19:42:15.000000 types-aiobotocore-clouddirectory-2.9.0/types_aiobotocore_clouddirectory/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    59804 2023-12-13 19:42:15.000000 types-aiobotocore-clouddirectory-2.9.0/types_aiobotocore_clouddirectory/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    59800 2023-12-13 19:42:15.000000 types-aiobotocore-clouddirectory-2.9.0/types_aiobotocore_clouddirectory/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12445 2023-12-13 19:42:16.000000 types-aiobotocore-clouddirectory-2.9.0/types_aiobotocore_clouddirectory/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    12443 2023-12-13 19:42:15.000000 types-aiobotocore-clouddirectory-2.9.0/types_aiobotocore_clouddirectory/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    25497 2023-12-13 19:42:15.000000 types-aiobotocore-clouddirectory-2.9.0/types_aiobotocore_clouddirectory/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    25476 2023-12-13 19:42:15.000000 types-aiobotocore-clouddirectory-2.9.0/types_aiobotocore_clouddirectory/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:42:15.000000 types-aiobotocore-clouddirectory-2.9.0/types_aiobotocore_clouddirectory/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    73910 2023-12-13 19:42:18.000000 types-aiobotocore-clouddirectory-2.9.0/types_aiobotocore_clouddirectory/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    73909 2023-12-13 19:42:17.000000 types-aiobotocore-clouddirectory-2.9.0/types_aiobotocore_clouddirectory/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:42:15.000000 types-aiobotocore-clouddirectory-2.9.0/types_aiobotocore_clouddirectory/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:48.449981 types-aiobotocore-clouddirectory-2.9.0/types_aiobotocore_clouddirectory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16342 2023-12-13 19:58:48.000000 types-aiobotocore-clouddirectory-2.9.0/types_aiobotocore_clouddirectory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      946 2023-12-13 19:58:48.000000 types-aiobotocore-clouddirectory-2.9.0/types_aiobotocore_clouddirectory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:48.000000 types-aiobotocore-clouddirectory-2.9.0/types_aiobotocore_clouddirectory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:48.000000 types-aiobotocore-clouddirectory-2.9.0/types_aiobotocore_clouddirectory.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:48.000000 types-aiobotocore-clouddirectory-2.9.0/types_aiobotocore_clouddirectory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-13 19:58:48.000000 types-aiobotocore-clouddirectory-2.9.0/types_aiobotocore_clouddirectory.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:15.297466 types-aiobotocore-clouddirectory-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:04:12.000000 types-aiobotocore-clouddirectory-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16362 2024-01-18 01:20:15.297466 types-aiobotocore-clouddirectory-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14751 2024-01-18 01:04:12.000000 types-aiobotocore-clouddirectory-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:15.297466 types-aiobotocore-clouddirectory-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-01-18 01:04:12.000000 types-aiobotocore-clouddirectory-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:15.297466 types-aiobotocore-clouddirectory-2.9.1/types_aiobotocore_clouddirectory/
+-rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-01-18 01:04:12.000000 types-aiobotocore-clouddirectory-2.9.1/types_aiobotocore_clouddirectory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-01-18 01:04:12.000000 types-aiobotocore-clouddirectory-2.9.1/types_aiobotocore_clouddirectory/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-01-18 01:04:12.000000 types-aiobotocore-clouddirectory-2.9.1/types_aiobotocore_clouddirectory/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59835 2024-01-18 01:04:12.000000 types-aiobotocore-clouddirectory-2.9.1/types_aiobotocore_clouddirectory/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59832 2024-01-18 01:04:12.000000 types-aiobotocore-clouddirectory-2.9.1/types_aiobotocore_clouddirectory/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12443 2024-01-18 01:04:12.000000 types-aiobotocore-clouddirectory-2.9.1/types_aiobotocore_clouddirectory/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12443 2024-01-18 01:04:12.000000 types-aiobotocore-clouddirectory-2.9.1/types_aiobotocore_clouddirectory/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    25506 2024-01-18 01:04:12.000000 types-aiobotocore-clouddirectory-2.9.1/types_aiobotocore_clouddirectory/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25486 2024-01-18 01:04:12.000000 types-aiobotocore-clouddirectory-2.9.1/types_aiobotocore_clouddirectory/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:04:12.000000 types-aiobotocore-clouddirectory-2.9.1/types_aiobotocore_clouddirectory/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    73909 2024-01-18 01:04:14.000000 types-aiobotocore-clouddirectory-2.9.1/types_aiobotocore_clouddirectory/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73909 2024-01-18 01:04:14.000000 types-aiobotocore-clouddirectory-2.9.1/types_aiobotocore_clouddirectory/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:04:12.000000 types-aiobotocore-clouddirectory-2.9.1/types_aiobotocore_clouddirectory/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:15.297466 types-aiobotocore-clouddirectory-2.9.1/types_aiobotocore_clouddirectory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16362 2024-01-18 01:20:15.000000 types-aiobotocore-clouddirectory-2.9.1/types_aiobotocore_clouddirectory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-01-18 01:20:15.000000 types-aiobotocore-clouddirectory-2.9.1/types_aiobotocore_clouddirectory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:15.000000 types-aiobotocore-clouddirectory-2.9.1/types_aiobotocore_clouddirectory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:15.000000 types-aiobotocore-clouddirectory-2.9.1/types_aiobotocore_clouddirectory.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:15.000000 types-aiobotocore-clouddirectory-2.9.1/types_aiobotocore_clouddirectory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-18 01:20:15.000000 types-aiobotocore-clouddirectory-2.9.1/types_aiobotocore_clouddirectory.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-clouddirectory-2.9.0/LICENSE` & `types-aiobotocore-clouddirectory-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-clouddirectory-2.9.0/PKG-INFO` & `types-aiobotocore-clouddirectory-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-clouddirectory
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CloudDirectory 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CloudDirectory 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/
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
 
 <a id="types-aiobotocore-clouddirectory"></a>
 
 # types-aiobotocore-clouddirectory
 
 [![PyPI - types-aiobotocore-clouddirectory](https://img.shields.io/pypi/v/types-aiobotocore-clouddirectory.svg?color=blue)](https://pypi.org/project/types-aiobotocore-clouddirectory)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-clouddirectory.svg?color=blue)](https://pypi.org/project/types-aiobotocore-clouddirectory)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-clouddirectory)](https://pepy.tech/project/types-aiobotocore-clouddirectory)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudDirectory 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory)
+[aiobotocore.CloudDirectory 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory)
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
 [types-aiobotocore-clouddirectory docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-clouddirectory-2.9.0/README.md` & `types-aiobotocore-clouddirectory-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-clouddirectory.svg?color=blue)](https://pypi.org/project/types-aiobotocore-clouddirectory)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-clouddirectory)](https://pepy.tech/project/types-aiobotocore-clouddirectory)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudDirectory 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory)
+[aiobotocore.CloudDirectory 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory)
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
 [types-aiobotocore-clouddirectory docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-clouddirectory-2.9.0/setup.py` & `types-aiobotocore-clouddirectory-2.9.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-clouddirectory",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_clouddirectory"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CloudDirectory 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.CloudDirectory 2.9.1 service generated with"
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
     keywords="aiobotocore clouddirectory type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_clouddirectory": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-clouddirectory-2.9.0/types_aiobotocore_clouddirectory/__init__.py` & `types-aiobotocore-clouddirectory-2.9.1/types_aiobotocore_clouddirectory/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,14 @@
     ListTypedLinkFacetAttributesPaginator,
     ListTypedLinkFacetNamesPaginator,
     LookupPolicyPaginator,
 )
 
 Client = CloudDirectoryClient
 
-
 __all__ = (
     "Client",
     "CloudDirectoryClient",
     "ListAppliedSchemaArnsPaginator",
     "ListAttachedIndicesPaginator",
     "ListDevelopmentSchemaArnsPaginator",
     "ListDirectoriesPaginator",
```

### Comparing `types-aiobotocore-clouddirectory-2.9.0/types_aiobotocore_clouddirectory/__init__.pyi` & `types-aiobotocore-clouddirectory-2.9.1/types_aiobotocore_clouddirectory/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-clouddirectory-2.9.0/types_aiobotocore_clouddirectory/__main__.py` & `types-aiobotocore-clouddirectory-2.9.1/types_aiobotocore_clouddirectory/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CloudDirectory 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.CloudDirectory 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory\nOther"
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

### Comparing `types-aiobotocore-clouddirectory-2.9.0/types_aiobotocore_clouddirectory/client.py` & `types-aiobotocore-clouddirectory-2.9.1/types_aiobotocore_clouddirectory/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("CloudDirectoryClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -191,15 +190,15 @@
 
     async def add_facet_to_object(
         self,
         *,
         DirectoryArn: str,
         SchemaFacet: SchemaFacetTypeDef,
         ObjectReference: ObjectReferenceTypeDef,
-        ObjectAttributeList: Sequence[AttributeKeyAndValueTypeDef] = ...
+        ObjectAttributeList: Sequence[AttributeKeyAndValueTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Adds a new  Facet to an object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.add_facet_to_object)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#add_facet_to_object)
         """
@@ -218,43 +217,43 @@
 
     async def attach_object(
         self,
         *,
         DirectoryArn: str,
         ParentReference: ObjectReferenceTypeDef,
         ChildReference: ObjectReferenceTypeDef,
-        LinkName: str
+        LinkName: str,
     ) -> AttachObjectResponseTypeDef:
         """
         Attaches an existing object to another object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.attach_object)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#attach_object)
         """
 
     async def attach_policy(
         self,
         *,
         DirectoryArn: str,
         PolicyReference: ObjectReferenceTypeDef,
-        ObjectReference: ObjectReferenceTypeDef
+        ObjectReference: ObjectReferenceTypeDef,
     ) -> Dict[str, Any]:
         """
         Attaches a policy object to a regular object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.attach_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#attach_policy)
         """
 
     async def attach_to_index(
         self,
         *,
         DirectoryArn: str,
         IndexReference: ObjectReferenceTypeDef,
-        TargetReference: ObjectReferenceTypeDef
+        TargetReference: ObjectReferenceTypeDef,
     ) -> AttachToIndexResponseTypeDef:
         """
         Attaches the specified object to the specified index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.attach_to_index)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#attach_to_index)
         """
@@ -262,29 +261,29 @@
     async def attach_typed_link(
         self,
         *,
         DirectoryArn: str,
         SourceObjectReference: ObjectReferenceTypeDef,
         TargetObjectReference: ObjectReferenceTypeDef,
         TypedLinkFacet: TypedLinkSchemaAndFacetNameTypeDef,
-        Attributes: Sequence[AttributeNameAndValueTypeDef]
+        Attributes: Sequence[AttributeNameAndValueTypeDef],
     ) -> AttachTypedLinkResponseTypeDef:
         """
         Attaches a typed link to a specified source and target object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.attach_typed_link)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#attach_typed_link)
         """
 
     async def batch_read(
         self,
         *,
         DirectoryArn: str,
         Operations: Sequence[BatchReadOperationTypeDef],
-        ConsistencyLevel: ConsistencyLevelType = ...
+        ConsistencyLevel: ConsistencyLevelType = ...,
     ) -> BatchReadResponseTypeDef:
         """
         Performs all the read operations in a batch.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.batch_read)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#batch_read)
         """
@@ -328,15 +327,15 @@
     async def create_facet(
         self,
         *,
         SchemaArn: str,
         Name: str,
         Attributes: Sequence[FacetAttributeTypeDef] = ...,
         ObjectType: ObjectTypeType = ...,
-        FacetStyle: FacetStyleType = ...
+        FacetStyle: FacetStyleType = ...,
     ) -> Dict[str, Any]:
         """
         Creates a new  Facet in a schema.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.create_facet)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#create_facet)
         """
@@ -344,15 +343,15 @@
     async def create_index(
         self,
         *,
         DirectoryArn: str,
         OrderedIndexedAttributeList: Sequence[AttributeKeyTypeDef],
         IsUnique: bool,
         ParentReference: ObjectReferenceTypeDef = ...,
-        LinkName: str = ...
+        LinkName: str = ...,
     ) -> CreateIndexResponseTypeDef:
         """
         Creates an index object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.create_index)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#create_index)
         """
@@ -360,15 +359,15 @@
     async def create_object(
         self,
         *,
         DirectoryArn: str,
         SchemaFacets: Sequence[SchemaFacetTypeDef],
         ObjectAttributeList: Sequence[AttributeKeyAndValueTypeDef] = ...,
         ParentReference: ObjectReferenceTypeDef = ...,
-        LinkName: str = ...
+        LinkName: str = ...,
     ) -> CreateObjectResponseTypeDef:
         """
         Creates an object in a  Directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.create_object)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#create_object)
         """
@@ -434,15 +433,15 @@
         """
 
     async def detach_from_index(
         self,
         *,
         DirectoryArn: str,
         IndexReference: ObjectReferenceTypeDef,
-        TargetReference: ObjectReferenceTypeDef
+        TargetReference: ObjectReferenceTypeDef,
     ) -> DetachFromIndexResponseTypeDef:
         """
         Detaches the specified object from the specified index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.detach_from_index)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#detach_from_index)
         """
@@ -458,15 +457,15 @@
         """
 
     async def detach_policy(
         self,
         *,
         DirectoryArn: str,
         PolicyReference: ObjectReferenceTypeDef,
-        ObjectReference: ObjectReferenceTypeDef
+        ObjectReference: ObjectReferenceTypeDef,
     ) -> Dict[str, Any]:
         """
         Detaches a policy from an object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.detach_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#detach_policy)
         """
@@ -540,15 +539,15 @@
 
     async def get_link_attributes(
         self,
         *,
         DirectoryArn: str,
         TypedLinkSpecifier: TypedLinkSpecifierTypeDef,
         AttributeNames: Sequence[str],
-        ConsistencyLevel: ConsistencyLevelType = ...
+        ConsistencyLevel: ConsistencyLevelType = ...,
     ) -> GetLinkAttributesResponseTypeDef:
         """
         Retrieves attributes that are associated with a typed link.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.get_link_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#get_link_attributes)
         """
@@ -556,29 +555,29 @@
     async def get_object_attributes(
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
         SchemaFacet: SchemaFacetTypeDef,
         AttributeNames: Sequence[str],
-        ConsistencyLevel: ConsistencyLevelType = ...
+        ConsistencyLevel: ConsistencyLevelType = ...,
     ) -> GetObjectAttributesResponseTypeDef:
         """
         Retrieves attributes within a facet that are associated with an object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.get_object_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#get_object_attributes)
         """
 
     async def get_object_information(
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
-        ConsistencyLevel: ConsistencyLevelType = ...
+        ConsistencyLevel: ConsistencyLevelType = ...,
     ) -> GetObjectInformationResponseTypeDef:
         """
         Retrieves metadata about an object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.get_object_information)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#get_object_information)
         """
@@ -603,15 +602,15 @@
 
     async def list_applied_schema_arns(
         self,
         *,
         DirectoryArn: str,
         SchemaArn: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListAppliedSchemaArnsResponseTypeDef:
         """
         Lists schema major versions applied to a directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.list_applied_schema_arns)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#list_applied_schema_arns)
         """
@@ -619,15 +618,15 @@
     async def list_attached_indices(
         self,
         *,
         DirectoryArn: str,
         TargetReference: ObjectReferenceTypeDef,
         NextToken: str = ...,
         MaxResults: int = ...,
-        ConsistencyLevel: ConsistencyLevelType = ...
+        ConsistencyLevel: ConsistencyLevelType = ...,
     ) -> ListAttachedIndicesResponseTypeDef:
         """
         Lists indices attached to the specified object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.list_attached_indices)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#list_attached_indices)
         """
@@ -677,15 +676,15 @@
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
         FilterAttributeRanges: Sequence[TypedLinkAttributeRangeTypeDef] = ...,
         FilterTypedLink: TypedLinkSchemaAndFacetNameTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        ConsistencyLevel: ConsistencyLevelType = ...
+        ConsistencyLevel: ConsistencyLevelType = ...,
     ) -> ListIncomingTypedLinksResponseTypeDef:
         """
         Returns a paginated list of all the incoming  TypedLinkSpecifier information
         for an
         object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.list_incoming_typed_links)
@@ -696,15 +695,15 @@
         self,
         *,
         DirectoryArn: str,
         IndexReference: ObjectReferenceTypeDef,
         RangesOnIndexedValues: Sequence[ObjectAttributeRangeTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        ConsistencyLevel: ConsistencyLevelType = ...
+        ConsistencyLevel: ConsistencyLevelType = ...,
     ) -> ListIndexResponseTypeDef:
         """
         Lists objects attached to the specified index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.list_index)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#list_index)
         """
@@ -723,15 +722,15 @@
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
         NextToken: str = ...,
         MaxResults: int = ...,
         ConsistencyLevel: ConsistencyLevelType = ...,
-        FacetFilter: SchemaFacetTypeDef = ...
+        FacetFilter: SchemaFacetTypeDef = ...,
     ) -> ListObjectAttributesResponseTypeDef:
         """
         Lists all attributes that are associated with an object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.list_object_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#list_object_attributes)
         """
@@ -739,15 +738,15 @@
     async def list_object_children(
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
         NextToken: str = ...,
         MaxResults: int = ...,
-        ConsistencyLevel: ConsistencyLevelType = ...
+        ConsistencyLevel: ConsistencyLevelType = ...,
     ) -> ListObjectChildrenResponseTypeDef:
         """
         Returns a paginated list of child objects that are associated with a given
         object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.list_object_children)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#list_object_children)
@@ -755,15 +754,15 @@
 
     async def list_object_parent_paths(
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListObjectParentPathsResponseTypeDef:
         """
         Retrieves all available parent paths for any object type such as node, leaf
         node, policy node, and index node
         objects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.list_object_parent_paths)
@@ -774,15 +773,15 @@
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
         NextToken: str = ...,
         MaxResults: int = ...,
         ConsistencyLevel: ConsistencyLevelType = ...,
-        IncludeAllLinksToEachParent: bool = ...
+        IncludeAllLinksToEachParent: bool = ...,
     ) -> ListObjectParentsResponseTypeDef:
         """
         Lists parent objects that are associated with a given object in pagination
         fashion.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.list_object_parents)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#list_object_parents)
@@ -791,15 +790,15 @@
     async def list_object_policies(
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
         NextToken: str = ...,
         MaxResults: int = ...,
-        ConsistencyLevel: ConsistencyLevelType = ...
+        ConsistencyLevel: ConsistencyLevelType = ...,
     ) -> ListObjectPoliciesResponseTypeDef:
         """
         Returns policies attached to an object in pagination fashion.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.list_object_policies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#list_object_policies)
         """
@@ -809,15 +808,15 @@
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
         FilterAttributeRanges: Sequence[TypedLinkAttributeRangeTypeDef] = ...,
         FilterTypedLink: TypedLinkSchemaAndFacetNameTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        ConsistencyLevel: ConsistencyLevelType = ...
+        ConsistencyLevel: ConsistencyLevelType = ...,
     ) -> ListOutgoingTypedLinksResponseTypeDef:
         """
         Returns a paginated list of all the outgoing  TypedLinkSpecifier information
         for an
         object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.list_outgoing_typed_links)
@@ -827,15 +826,15 @@
     async def list_policy_attachments(
         self,
         *,
         DirectoryArn: str,
         PolicyReference: ObjectReferenceTypeDef,
         NextToken: str = ...,
         MaxResults: int = ...,
-        ConsistencyLevel: ConsistencyLevelType = ...
+        ConsistencyLevel: ConsistencyLevelType = ...,
     ) -> ListPolicyAttachmentsResponseTypeDef:
         """
         Returns all of the `ObjectIdentifiers` to which a given policy is attached.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.list_policy_attachments)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#list_policy_attachments)
         """
@@ -883,15 +882,15 @@
 
     async def lookup_policy(
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> LookupPolicyResponseTypeDef:
         """
         Lists all policies from the root of the  Directory to the object specified.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.lookup_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#lookup_policy)
         """
@@ -918,15 +917,15 @@
         """
 
     async def remove_facet_from_object(
         self,
         *,
         DirectoryArn: str,
         SchemaFacet: SchemaFacetTypeDef,
-        ObjectReference: ObjectReferenceTypeDef
+        ObjectReference: ObjectReferenceTypeDef,
     ) -> Dict[str, Any]:
         """
         Removes the specified facet from the specified object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.remove_facet_from_object)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#remove_facet_from_object)
         """
@@ -949,43 +948,43 @@
 
     async def update_facet(
         self,
         *,
         SchemaArn: str,
         Name: str,
         AttributeUpdates: Sequence[FacetAttributeUpdateTypeDef] = ...,
-        ObjectType: ObjectTypeType = ...
+        ObjectType: ObjectTypeType = ...,
     ) -> Dict[str, Any]:
         """
         Does the following: * Adds new `Attributes`, `Rules`, or `ObjectTypes`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.update_facet)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#update_facet)
         """
 
     async def update_link_attributes(
         self,
         *,
         DirectoryArn: str,
         TypedLinkSpecifier: TypedLinkSpecifierTypeDef,
-        AttributeUpdates: Sequence[LinkAttributeUpdateTypeDef]
+        AttributeUpdates: Sequence[LinkAttributeUpdateTypeDef],
     ) -> Dict[str, Any]:
         """
         Updates a given typed link’s attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.update_link_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#update_link_attributes)
         """
 
     async def update_object_attributes(
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
-        AttributeUpdates: Sequence[ObjectAttributeUpdateTypeDef]
+        AttributeUpdates: Sequence[ObjectAttributeUpdateTypeDef],
     ) -> UpdateObjectAttributesResponseTypeDef:
         """
         Updates a given object's attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.update_object_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#update_object_attributes)
         """
@@ -1000,15 +999,15 @@
 
     async def update_typed_link_facet(
         self,
         *,
         SchemaArn: str,
         Name: str,
         AttributeUpdates: Sequence[TypedLinkFacetAttributeUpdateTypeDef],
-        IdentityAttributeOrder: Sequence[str]
+        IdentityAttributeOrder: Sequence[str],
     ) -> Dict[str, Any]:
         """
         Updates a  TypedLinkFacet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.update_typed_link_facet)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#update_typed_link_facet)
         """
@@ -1027,15 +1026,15 @@
 
     async def upgrade_published_schema(
         self,
         *,
         DevelopmentSchemaArn: str,
         PublishedSchemaArn: str,
         MinorVersion: str,
-        DryRun: bool = ...
+        DryRun: bool = ...,
     ) -> UpgradePublishedSchemaResponseTypeDef:
         """
         Upgrades a published schema under a new minor version revision using the
         current contents of
         `DevelopmentSchemaArn`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.upgrade_published_schema)
```

### Comparing `types-aiobotocore-clouddirectory-2.9.0/types_aiobotocore_clouddirectory/client.pyi` & `types-aiobotocore-clouddirectory-2.9.1/types_aiobotocore_clouddirectory/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -187,15 +187,15 @@
 
     async def add_facet_to_object(
         self,
         *,
         DirectoryArn: str,
         SchemaFacet: SchemaFacetTypeDef,
         ObjectReference: ObjectReferenceTypeDef,
-        ObjectAttributeList: Sequence[AttributeKeyAndValueTypeDef] = ...
+        ObjectAttributeList: Sequence[AttributeKeyAndValueTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Adds a new  Facet to an object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.add_facet_to_object)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#add_facet_to_object)
         """
@@ -214,43 +214,43 @@
 
     async def attach_object(
         self,
         *,
         DirectoryArn: str,
         ParentReference: ObjectReferenceTypeDef,
         ChildReference: ObjectReferenceTypeDef,
-        LinkName: str
+        LinkName: str,
     ) -> AttachObjectResponseTypeDef:
         """
         Attaches an existing object to another object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.attach_object)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#attach_object)
         """
 
     async def attach_policy(
         self,
         *,
         DirectoryArn: str,
         PolicyReference: ObjectReferenceTypeDef,
-        ObjectReference: ObjectReferenceTypeDef
+        ObjectReference: ObjectReferenceTypeDef,
     ) -> Dict[str, Any]:
         """
         Attaches a policy object to a regular object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.attach_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#attach_policy)
         """
 
     async def attach_to_index(
         self,
         *,
         DirectoryArn: str,
         IndexReference: ObjectReferenceTypeDef,
-        TargetReference: ObjectReferenceTypeDef
+        TargetReference: ObjectReferenceTypeDef,
     ) -> AttachToIndexResponseTypeDef:
         """
         Attaches the specified object to the specified index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.attach_to_index)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#attach_to_index)
         """
@@ -258,29 +258,29 @@
     async def attach_typed_link(
         self,
         *,
         DirectoryArn: str,
         SourceObjectReference: ObjectReferenceTypeDef,
         TargetObjectReference: ObjectReferenceTypeDef,
         TypedLinkFacet: TypedLinkSchemaAndFacetNameTypeDef,
-        Attributes: Sequence[AttributeNameAndValueTypeDef]
+        Attributes: Sequence[AttributeNameAndValueTypeDef],
     ) -> AttachTypedLinkResponseTypeDef:
         """
         Attaches a typed link to a specified source and target object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.attach_typed_link)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#attach_typed_link)
         """
 
     async def batch_read(
         self,
         *,
         DirectoryArn: str,
         Operations: Sequence[BatchReadOperationTypeDef],
-        ConsistencyLevel: ConsistencyLevelType = ...
+        ConsistencyLevel: ConsistencyLevelType = ...,
     ) -> BatchReadResponseTypeDef:
         """
         Performs all the read operations in a batch.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.batch_read)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#batch_read)
         """
@@ -324,15 +324,15 @@
     async def create_facet(
         self,
         *,
         SchemaArn: str,
         Name: str,
         Attributes: Sequence[FacetAttributeTypeDef] = ...,
         ObjectType: ObjectTypeType = ...,
-        FacetStyle: FacetStyleType = ...
+        FacetStyle: FacetStyleType = ...,
     ) -> Dict[str, Any]:
         """
         Creates a new  Facet in a schema.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.create_facet)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#create_facet)
         """
@@ -340,15 +340,15 @@
     async def create_index(
         self,
         *,
         DirectoryArn: str,
         OrderedIndexedAttributeList: Sequence[AttributeKeyTypeDef],
         IsUnique: bool,
         ParentReference: ObjectReferenceTypeDef = ...,
-        LinkName: str = ...
+        LinkName: str = ...,
     ) -> CreateIndexResponseTypeDef:
         """
         Creates an index object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.create_index)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#create_index)
         """
@@ -356,15 +356,15 @@
     async def create_object(
         self,
         *,
         DirectoryArn: str,
         SchemaFacets: Sequence[SchemaFacetTypeDef],
         ObjectAttributeList: Sequence[AttributeKeyAndValueTypeDef] = ...,
         ParentReference: ObjectReferenceTypeDef = ...,
-        LinkName: str = ...
+        LinkName: str = ...,
     ) -> CreateObjectResponseTypeDef:
         """
         Creates an object in a  Directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.create_object)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#create_object)
         """
@@ -430,15 +430,15 @@
         """
 
     async def detach_from_index(
         self,
         *,
         DirectoryArn: str,
         IndexReference: ObjectReferenceTypeDef,
-        TargetReference: ObjectReferenceTypeDef
+        TargetReference: ObjectReferenceTypeDef,
     ) -> DetachFromIndexResponseTypeDef:
         """
         Detaches the specified object from the specified index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.detach_from_index)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#detach_from_index)
         """
@@ -454,15 +454,15 @@
         """
 
     async def detach_policy(
         self,
         *,
         DirectoryArn: str,
         PolicyReference: ObjectReferenceTypeDef,
-        ObjectReference: ObjectReferenceTypeDef
+        ObjectReference: ObjectReferenceTypeDef,
     ) -> Dict[str, Any]:
         """
         Detaches a policy from an object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.detach_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#detach_policy)
         """
@@ -536,15 +536,15 @@
 
     async def get_link_attributes(
         self,
         *,
         DirectoryArn: str,
         TypedLinkSpecifier: TypedLinkSpecifierTypeDef,
         AttributeNames: Sequence[str],
-        ConsistencyLevel: ConsistencyLevelType = ...
+        ConsistencyLevel: ConsistencyLevelType = ...,
     ) -> GetLinkAttributesResponseTypeDef:
         """
         Retrieves attributes that are associated with a typed link.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.get_link_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#get_link_attributes)
         """
@@ -552,29 +552,29 @@
     async def get_object_attributes(
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
         SchemaFacet: SchemaFacetTypeDef,
         AttributeNames: Sequence[str],
-        ConsistencyLevel: ConsistencyLevelType = ...
+        ConsistencyLevel: ConsistencyLevelType = ...,
     ) -> GetObjectAttributesResponseTypeDef:
         """
         Retrieves attributes within a facet that are associated with an object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.get_object_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#get_object_attributes)
         """
 
     async def get_object_information(
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
-        ConsistencyLevel: ConsistencyLevelType = ...
+        ConsistencyLevel: ConsistencyLevelType = ...,
     ) -> GetObjectInformationResponseTypeDef:
         """
         Retrieves metadata about an object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.get_object_information)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#get_object_information)
         """
@@ -599,15 +599,15 @@
 
     async def list_applied_schema_arns(
         self,
         *,
         DirectoryArn: str,
         SchemaArn: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListAppliedSchemaArnsResponseTypeDef:
         """
         Lists schema major versions applied to a directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.list_applied_schema_arns)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#list_applied_schema_arns)
         """
@@ -615,15 +615,15 @@
     async def list_attached_indices(
         self,
         *,
         DirectoryArn: str,
         TargetReference: ObjectReferenceTypeDef,
         NextToken: str = ...,
         MaxResults: int = ...,
-        ConsistencyLevel: ConsistencyLevelType = ...
+        ConsistencyLevel: ConsistencyLevelType = ...,
     ) -> ListAttachedIndicesResponseTypeDef:
         """
         Lists indices attached to the specified object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.list_attached_indices)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#list_attached_indices)
         """
@@ -673,15 +673,15 @@
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
         FilterAttributeRanges: Sequence[TypedLinkAttributeRangeTypeDef] = ...,
         FilterTypedLink: TypedLinkSchemaAndFacetNameTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        ConsistencyLevel: ConsistencyLevelType = ...
+        ConsistencyLevel: ConsistencyLevelType = ...,
     ) -> ListIncomingTypedLinksResponseTypeDef:
         """
         Returns a paginated list of all the incoming  TypedLinkSpecifier information
         for an
         object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.list_incoming_typed_links)
@@ -692,15 +692,15 @@
         self,
         *,
         DirectoryArn: str,
         IndexReference: ObjectReferenceTypeDef,
         RangesOnIndexedValues: Sequence[ObjectAttributeRangeTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        ConsistencyLevel: ConsistencyLevelType = ...
+        ConsistencyLevel: ConsistencyLevelType = ...,
     ) -> ListIndexResponseTypeDef:
         """
         Lists objects attached to the specified index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.list_index)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#list_index)
         """
@@ -719,15 +719,15 @@
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
         NextToken: str = ...,
         MaxResults: int = ...,
         ConsistencyLevel: ConsistencyLevelType = ...,
-        FacetFilter: SchemaFacetTypeDef = ...
+        FacetFilter: SchemaFacetTypeDef = ...,
     ) -> ListObjectAttributesResponseTypeDef:
         """
         Lists all attributes that are associated with an object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.list_object_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#list_object_attributes)
         """
@@ -735,15 +735,15 @@
     async def list_object_children(
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
         NextToken: str = ...,
         MaxResults: int = ...,
-        ConsistencyLevel: ConsistencyLevelType = ...
+        ConsistencyLevel: ConsistencyLevelType = ...,
     ) -> ListObjectChildrenResponseTypeDef:
         """
         Returns a paginated list of child objects that are associated with a given
         object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.list_object_children)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#list_object_children)
@@ -751,15 +751,15 @@
 
     async def list_object_parent_paths(
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListObjectParentPathsResponseTypeDef:
         """
         Retrieves all available parent paths for any object type such as node, leaf
         node, policy node, and index node
         objects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.list_object_parent_paths)
@@ -770,15 +770,15 @@
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
         NextToken: str = ...,
         MaxResults: int = ...,
         ConsistencyLevel: ConsistencyLevelType = ...,
-        IncludeAllLinksToEachParent: bool = ...
+        IncludeAllLinksToEachParent: bool = ...,
     ) -> ListObjectParentsResponseTypeDef:
         """
         Lists parent objects that are associated with a given object in pagination
         fashion.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.list_object_parents)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#list_object_parents)
@@ -787,15 +787,15 @@
     async def list_object_policies(
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
         NextToken: str = ...,
         MaxResults: int = ...,
-        ConsistencyLevel: ConsistencyLevelType = ...
+        ConsistencyLevel: ConsistencyLevelType = ...,
     ) -> ListObjectPoliciesResponseTypeDef:
         """
         Returns policies attached to an object in pagination fashion.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.list_object_policies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#list_object_policies)
         """
@@ -805,15 +805,15 @@
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
         FilterAttributeRanges: Sequence[TypedLinkAttributeRangeTypeDef] = ...,
         FilterTypedLink: TypedLinkSchemaAndFacetNameTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        ConsistencyLevel: ConsistencyLevelType = ...
+        ConsistencyLevel: ConsistencyLevelType = ...,
     ) -> ListOutgoingTypedLinksResponseTypeDef:
         """
         Returns a paginated list of all the outgoing  TypedLinkSpecifier information
         for an
         object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.list_outgoing_typed_links)
@@ -823,15 +823,15 @@
     async def list_policy_attachments(
         self,
         *,
         DirectoryArn: str,
         PolicyReference: ObjectReferenceTypeDef,
         NextToken: str = ...,
         MaxResults: int = ...,
-        ConsistencyLevel: ConsistencyLevelType = ...
+        ConsistencyLevel: ConsistencyLevelType = ...,
     ) -> ListPolicyAttachmentsResponseTypeDef:
         """
         Returns all of the `ObjectIdentifiers` to which a given policy is attached.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.list_policy_attachments)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#list_policy_attachments)
         """
@@ -879,15 +879,15 @@
 
     async def lookup_policy(
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> LookupPolicyResponseTypeDef:
         """
         Lists all policies from the root of the  Directory to the object specified.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.lookup_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#lookup_policy)
         """
@@ -914,15 +914,15 @@
         """
 
     async def remove_facet_from_object(
         self,
         *,
         DirectoryArn: str,
         SchemaFacet: SchemaFacetTypeDef,
-        ObjectReference: ObjectReferenceTypeDef
+        ObjectReference: ObjectReferenceTypeDef,
     ) -> Dict[str, Any]:
         """
         Removes the specified facet from the specified object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.remove_facet_from_object)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#remove_facet_from_object)
         """
@@ -945,43 +945,43 @@
 
     async def update_facet(
         self,
         *,
         SchemaArn: str,
         Name: str,
         AttributeUpdates: Sequence[FacetAttributeUpdateTypeDef] = ...,
-        ObjectType: ObjectTypeType = ...
+        ObjectType: ObjectTypeType = ...,
     ) -> Dict[str, Any]:
         """
         Does the following: * Adds new `Attributes`, `Rules`, or `ObjectTypes`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.update_facet)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#update_facet)
         """
 
     async def update_link_attributes(
         self,
         *,
         DirectoryArn: str,
         TypedLinkSpecifier: TypedLinkSpecifierTypeDef,
-        AttributeUpdates: Sequence[LinkAttributeUpdateTypeDef]
+        AttributeUpdates: Sequence[LinkAttributeUpdateTypeDef],
     ) -> Dict[str, Any]:
         """
         Updates a given typed link’s attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.update_link_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#update_link_attributes)
         """
 
     async def update_object_attributes(
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
-        AttributeUpdates: Sequence[ObjectAttributeUpdateTypeDef]
+        AttributeUpdates: Sequence[ObjectAttributeUpdateTypeDef],
     ) -> UpdateObjectAttributesResponseTypeDef:
         """
         Updates a given object's attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.update_object_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#update_object_attributes)
         """
@@ -996,15 +996,15 @@
 
     async def update_typed_link_facet(
         self,
         *,
         SchemaArn: str,
         Name: str,
         AttributeUpdates: Sequence[TypedLinkFacetAttributeUpdateTypeDef],
-        IdentityAttributeOrder: Sequence[str]
+        IdentityAttributeOrder: Sequence[str],
     ) -> Dict[str, Any]:
         """
         Updates a  TypedLinkFacet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.update_typed_link_facet)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#update_typed_link_facet)
         """
@@ -1023,15 +1023,15 @@
 
     async def upgrade_published_schema(
         self,
         *,
         DevelopmentSchemaArn: str,
         PublishedSchemaArn: str,
         MinorVersion: str,
-        DryRun: bool = ...
+        DryRun: bool = ...,
     ) -> UpgradePublishedSchemaResponseTypeDef:
         """
         Upgrades a published schema under a new minor version revision using the
         current contents of
         `DevelopmentSchemaArn`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.upgrade_published_schema)
```

### Comparing `types-aiobotocore-clouddirectory-2.9.0/types_aiobotocore_clouddirectory/literals.py` & `types-aiobotocore-clouddirectory-2.9.1/types_aiobotocore_clouddirectory/literals.py`

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
     "BatchReadExceptionTypeType",
     "ConsistencyLevelType",
     "DirectoryStateType",
     "FacetAttributeTypeType",
     "FacetStyleType",
     "ListAppliedSchemaArnsPaginatorName",
@@ -53,15 +52,14 @@
     "CloudDirectoryServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 BatchReadExceptionTypeType = Literal[
     "AccessDeniedException",
     "CannotListParentOfRootException",
     "DirectoryNotEnabledException",
     "FacetValidationException",
     "InternalServiceException",
     "InvalidArnException",
```

### Comparing `types-aiobotocore-clouddirectory-2.9.0/types_aiobotocore_clouddirectory/literals.pyi` & `types-aiobotocore-clouddirectory-2.9.1/types_aiobotocore_clouddirectory/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-clouddirectory-2.9.0/types_aiobotocore_clouddirectory/paginator.py` & `types-aiobotocore-clouddirectory-2.9.1/types_aiobotocore_clouddirectory/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,14 @@
     "ListPublishedSchemaArnsPaginator",
     "ListTagsForResourcePaginator",
     "ListTypedLinkFacetAttributesPaginator",
     "ListTypedLinkFacetNamesPaginator",
     "LookupPolicyPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -131,15 +130,15 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryArn: str,
         SchemaArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAppliedSchemaArnsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListAppliedSchemaArns.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listappliedschemaarnspaginator)
         """
 
 
@@ -151,15 +150,15 @@
 
     def paginate(
         self,
         *,
         DirectoryArn: str,
         TargetReference: ObjectReferenceTypeDef,
         ConsistencyLevel: ConsistencyLevelType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAttachedIndicesResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListAttachedIndices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listattachedindicespaginator)
         """
 
 
@@ -233,15 +232,15 @@
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
         FilterAttributeRanges: Sequence[TypedLinkAttributeRangePaginatorTypeDef] = ...,
         FilterTypedLink: TypedLinkSchemaAndFacetNameTypeDef = ...,
         ConsistencyLevel: ConsistencyLevelType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListIncomingTypedLinksResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListIncomingTypedLinks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listincomingtypedlinkspaginator)
         """
 
 
@@ -254,15 +253,15 @@
     def paginate(
         self,
         *,
         DirectoryArn: str,
         IndexReference: ObjectReferenceTypeDef,
         RangesOnIndexedValues: Sequence[ObjectAttributeRangePaginatorTypeDef] = ...,
         ConsistencyLevel: ConsistencyLevelType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListIndexResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListIndex.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listindexpaginator)
         """
 
 
@@ -290,15 +289,15 @@
     def paginate(
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
         ConsistencyLevel: ConsistencyLevelType = ...,
         FacetFilter: SchemaFacetTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListObjectAttributesResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListObjectAttributes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listobjectattributespaginator)
         """
 
 
@@ -309,15 +308,15 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListObjectParentPathsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListObjectParentPaths.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listobjectparentpathspaginator)
         """
 
 
@@ -329,15 +328,15 @@
 
     def paginate(
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
         ConsistencyLevel: ConsistencyLevelType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListObjectPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListObjectPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listobjectpoliciespaginator)
         """
 
 
@@ -351,15 +350,15 @@
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
         FilterAttributeRanges: Sequence[TypedLinkAttributeRangePaginatorTypeDef] = ...,
         FilterTypedLink: TypedLinkSchemaAndFacetNameTypeDef = ...,
         ConsistencyLevel: ConsistencyLevelType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListOutgoingTypedLinksResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListOutgoingTypedLinks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listoutgoingtypedlinkspaginator)
         """
 
 
@@ -371,15 +370,15 @@
 
     def paginate(
         self,
         *,
         DirectoryArn: str,
         PolicyReference: ObjectReferenceTypeDef,
         ConsistencyLevel: ConsistencyLevelType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPolicyAttachmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListPolicyAttachments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listpolicyattachmentspaginator)
         """
 
 
@@ -450,13 +449,13 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[LookupPolicyResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.LookupPolicy.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#lookuppolicypaginator)
         """
```

### Comparing `types-aiobotocore-clouddirectory-2.9.0/types_aiobotocore_clouddirectory/paginator.pyi` & `types-aiobotocore-clouddirectory-2.9.1/types_aiobotocore_clouddirectory/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryArn: str,
         SchemaArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAppliedSchemaArnsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListAppliedSchemaArns.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listappliedschemaarnspaginator)
         """
 
 class ListAttachedIndicesPaginator(AioPaginator):
@@ -147,15 +147,15 @@
 
     def paginate(
         self,
         *,
         DirectoryArn: str,
         TargetReference: ObjectReferenceTypeDef,
         ConsistencyLevel: ConsistencyLevelType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAttachedIndicesResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListAttachedIndices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listattachedindicespaginator)
         """
 
 class ListDevelopmentSchemaArnsPaginator(AioPaginator):
@@ -224,15 +224,15 @@
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
         FilterAttributeRanges: Sequence[TypedLinkAttributeRangePaginatorTypeDef] = ...,
         FilterTypedLink: TypedLinkSchemaAndFacetNameTypeDef = ...,
         ConsistencyLevel: ConsistencyLevelType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListIncomingTypedLinksResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListIncomingTypedLinks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listincomingtypedlinkspaginator)
         """
 
 class ListIndexPaginator(AioPaginator):
@@ -244,15 +244,15 @@
     def paginate(
         self,
         *,
         DirectoryArn: str,
         IndexReference: ObjectReferenceTypeDef,
         RangesOnIndexedValues: Sequence[ObjectAttributeRangePaginatorTypeDef] = ...,
         ConsistencyLevel: ConsistencyLevelType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListIndexResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListIndex.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listindexpaginator)
         """
 
 class ListManagedSchemaArnsPaginator(AioPaginator):
@@ -278,15 +278,15 @@
     def paginate(
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
         ConsistencyLevel: ConsistencyLevelType = ...,
         FacetFilter: SchemaFacetTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListObjectAttributesResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListObjectAttributes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listobjectattributespaginator)
         """
 
 class ListObjectParentPathsPaginator(AioPaginator):
@@ -296,15 +296,15 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListObjectParentPathsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListObjectParentPaths.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listobjectparentpathspaginator)
         """
 
 class ListObjectPoliciesPaginator(AioPaginator):
@@ -315,15 +315,15 @@
 
     def paginate(
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
         ConsistencyLevel: ConsistencyLevelType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListObjectPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListObjectPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listobjectpoliciespaginator)
         """
 
 class ListOutgoingTypedLinksPaginator(AioPaginator):
@@ -336,15 +336,15 @@
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
         FilterAttributeRanges: Sequence[TypedLinkAttributeRangePaginatorTypeDef] = ...,
         FilterTypedLink: TypedLinkSchemaAndFacetNameTypeDef = ...,
         ConsistencyLevel: ConsistencyLevelType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListOutgoingTypedLinksResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListOutgoingTypedLinks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listoutgoingtypedlinkspaginator)
         """
 
 class ListPolicyAttachmentsPaginator(AioPaginator):
@@ -355,15 +355,15 @@
 
     def paginate(
         self,
         *,
         DirectoryArn: str,
         PolicyReference: ObjectReferenceTypeDef,
         ConsistencyLevel: ConsistencyLevelType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPolicyAttachmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListPolicyAttachments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listpolicyattachmentspaginator)
         """
 
 class ListPublishedSchemaArnsPaginator(AioPaginator):
@@ -429,13 +429,13 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[LookupPolicyResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.LookupPolicy.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#lookuppolicypaginator)
         """
```

### Comparing `types-aiobotocore-clouddirectory-2.9.0/types_aiobotocore_clouddirectory/type_defs.py` & `types-aiobotocore-clouddirectory-2.9.1/types_aiobotocore_clouddirectory/type_defs.py`

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
     "ObjectReferenceTypeDef",
     "SchemaFacetTypeDef",
     "ApplySchemaRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "TypedLinkSchemaAndFacetNameTypeDef",
     "AttributeKeyTypeDef",
```

### Comparing `types-aiobotocore-clouddirectory-2.9.0/types_aiobotocore_clouddirectory/type_defs.pyi` & `types-aiobotocore-clouddirectory-2.9.1/types_aiobotocore_clouddirectory/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-clouddirectory-2.9.0/types_aiobotocore_clouddirectory.egg-info/PKG-INFO` & `types-aiobotocore-clouddirectory-2.9.1/types_aiobotocore_clouddirectory.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-clouddirectory
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CloudDirectory 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CloudDirectory 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/
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
 
 <a id="types-aiobotocore-clouddirectory"></a>
 
 # types-aiobotocore-clouddirectory
 
 [![PyPI - types-aiobotocore-clouddirectory](https://img.shields.io/pypi/v/types-aiobotocore-clouddirectory.svg?color=blue)](https://pypi.org/project/types-aiobotocore-clouddirectory)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-clouddirectory.svg?color=blue)](https://pypi.org/project/types-aiobotocore-clouddirectory)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-clouddirectory)](https://pepy.tech/project/types-aiobotocore-clouddirectory)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudDirectory 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory)
+[aiobotocore.CloudDirectory 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory)
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
 [types-aiobotocore-clouddirectory docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-clouddirectory-2.9.0/types_aiobotocore_clouddirectory.egg-info/SOURCES.txt` & `types-aiobotocore-clouddirectory-2.9.1/types_aiobotocore_clouddirectory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

