# Comparing `tmp/types-aiobotocore-greengrass-2.9.0.tar.gz` & `tmp/types-aiobotocore-greengrass-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-greengrass-2.9.0.tar", last modified: Wed Dec 13 19:59:24 2023, max compression
+gzip compressed data, was "types-aiobotocore-greengrass-2.9.1.tar", last modified: Thu Jan 18 01:20:48 2024, max compression
```

## Comparing `types-aiobotocore-greengrass-2.9.0.tar` & `types-aiobotocore-greengrass-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:24.305721 types-aiobotocore-greengrass-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:47:00.000000 types-aiobotocore-greengrass-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16526 2023-12-13 19:59:24.305721 types-aiobotocore-greengrass-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14951 2023-12-13 19:47:00.000000 types-aiobotocore-greengrass-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:24.305721 types-aiobotocore-greengrass-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2023-12-13 19:46:59.000000 types-aiobotocore-greengrass-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:24.305721 types-aiobotocore-greengrass-2.9.0/types_aiobotocore_greengrass/
--rw-r--r--   0 runner    (1001) docker     (127)     5326 2023-12-13 19:47:00.000000 types-aiobotocore-greengrass-2.9.0/types_aiobotocore_greengrass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5325 2023-12-13 19:47:00.000000 types-aiobotocore-greengrass-2.9.0/types_aiobotocore_greengrass/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      944 2023-12-13 19:47:00.000000 types-aiobotocore-greengrass-2.9.0/types_aiobotocore_greengrass/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    72446 2023-12-13 19:47:00.000000 types-aiobotocore-greengrass-2.9.0/types_aiobotocore_greengrass/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    72442 2023-12-13 19:47:00.000000 types-aiobotocore-greengrass-2.9.0/types_aiobotocore_greengrass/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12851 2023-12-13 19:47:00.000000 types-aiobotocore-greengrass-2.9.0/types_aiobotocore_greengrass/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    12849 2023-12-13 19:47:00.000000 types-aiobotocore-greengrass-2.9.0/types_aiobotocore_greengrass/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    24011 2023-12-13 19:47:00.000000 types-aiobotocore-greengrass-2.9.0/types_aiobotocore_greengrass/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    23990 2023-12-13 19:47:00.000000 types-aiobotocore-greengrass-2.9.0/types_aiobotocore_greengrass/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:47:00.000000 types-aiobotocore-greengrass-2.9.0/types_aiobotocore_greengrass/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    68945 2023-12-13 19:47:01.000000 types-aiobotocore-greengrass-2.9.0/types_aiobotocore_greengrass/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    68944 2023-12-13 19:47:01.000000 types-aiobotocore-greengrass-2.9.0/types_aiobotocore_greengrass/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:47:00.000000 types-aiobotocore-greengrass-2.9.0/types_aiobotocore_greengrass/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:24.305721 types-aiobotocore-greengrass-2.9.0/types_aiobotocore_greengrass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16526 2023-12-13 19:59:24.000000 types-aiobotocore-greengrass-2.9.0/types_aiobotocore_greengrass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      870 2023-12-13 19:59:24.000000 types-aiobotocore-greengrass-2.9.0/types_aiobotocore_greengrass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:24.000000 types-aiobotocore-greengrass-2.9.0/types_aiobotocore_greengrass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:24.000000 types-aiobotocore-greengrass-2.9.0/types_aiobotocore_greengrass.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:24.000000 types-aiobotocore-greengrass-2.9.0/types_aiobotocore_greengrass.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-13 19:59:24.000000 types-aiobotocore-greengrass-2.9.0/types_aiobotocore_greengrass.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:48.365307 types-aiobotocore-greengrass-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:08:52.000000 types-aiobotocore-greengrass-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16546 2024-01-18 01:20:48.365307 types-aiobotocore-greengrass-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14951 2024-01-18 01:08:52.000000 types-aiobotocore-greengrass-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:48.365307 types-aiobotocore-greengrass-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-01-18 01:08:52.000000 types-aiobotocore-greengrass-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:48.361307 types-aiobotocore-greengrass-2.9.1/types_aiobotocore_greengrass/
+-rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-01-18 01:08:52.000000 types-aiobotocore-greengrass-2.9.1/types_aiobotocore_greengrass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-01-18 01:08:52.000000 types-aiobotocore-greengrass-2.9.1/types_aiobotocore_greengrass/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-01-18 01:08:52.000000 types-aiobotocore-greengrass-2.9.1/types_aiobotocore_greengrass/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72465 2024-01-18 01:08:52.000000 types-aiobotocore-greengrass-2.9.1/types_aiobotocore_greengrass/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72462 2024-01-18 01:08:52.000000 types-aiobotocore-greengrass-2.9.1/types_aiobotocore_greengrass/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12849 2024-01-18 01:08:53.000000 types-aiobotocore-greengrass-2.9.1/types_aiobotocore_greengrass/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12849 2024-01-18 01:08:52.000000 types-aiobotocore-greengrass-2.9.1/types_aiobotocore_greengrass/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    24010 2024-01-18 01:08:52.000000 types-aiobotocore-greengrass-2.9.1/types_aiobotocore_greengrass/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23990 2024-01-18 01:08:52.000000 types-aiobotocore-greengrass-2.9.1/types_aiobotocore_greengrass/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:08:52.000000 types-aiobotocore-greengrass-2.9.1/types_aiobotocore_greengrass/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    68944 2024-01-18 01:08:54.000000 types-aiobotocore-greengrass-2.9.1/types_aiobotocore_greengrass/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68944 2024-01-18 01:08:53.000000 types-aiobotocore-greengrass-2.9.1/types_aiobotocore_greengrass/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:08:52.000000 types-aiobotocore-greengrass-2.9.1/types_aiobotocore_greengrass/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:48.365307 types-aiobotocore-greengrass-2.9.1/types_aiobotocore_greengrass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16546 2024-01-18 01:20:48.000000 types-aiobotocore-greengrass-2.9.1/types_aiobotocore_greengrass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-01-18 01:20:48.000000 types-aiobotocore-greengrass-2.9.1/types_aiobotocore_greengrass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:48.000000 types-aiobotocore-greengrass-2.9.1/types_aiobotocore_greengrass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:48.000000 types-aiobotocore-greengrass-2.9.1/types_aiobotocore_greengrass.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:48.000000 types-aiobotocore-greengrass-2.9.1/types_aiobotocore_greengrass.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-01-18 01:20:48.000000 types-aiobotocore-greengrass-2.9.1/types_aiobotocore_greengrass.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-greengrass-2.9.0/LICENSE` & `types-aiobotocore-greengrass-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-greengrass-2.9.0/PKG-INFO` & `types-aiobotocore-greengrass-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-greengrass
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Greengrass 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Greengrass 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/
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
 
 <a id="types-aiobotocore-greengrass"></a>
 
 # types-aiobotocore-greengrass
 
 [![PyPI - types-aiobotocore-greengrass](https://img.shields.io/pypi/v/types-aiobotocore-greengrass.svg?color=blue)](https://pypi.org/project/types-aiobotocore-greengrass)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-greengrass.svg?color=blue)](https://pypi.org/project/types-aiobotocore-greengrass)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-greengrass)](https://pepy.tech/project/types-aiobotocore-greengrass)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Greengrass 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass)
+[aiobotocore.Greengrass 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass)
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
 [types-aiobotocore-greengrass docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-greengrass-2.9.0/README.md` & `types-aiobotocore-greengrass-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-greengrass.svg?color=blue)](https://pypi.org/project/types-aiobotocore-greengrass)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-greengrass)](https://pepy.tech/project/types-aiobotocore-greengrass)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Greengrass 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass)
+[aiobotocore.Greengrass 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass)
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
 [types-aiobotocore-greengrass docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-greengrass-2.9.0/setup.py` & `types-aiobotocore-greengrass-2.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-greengrass",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_greengrass"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Greengrass 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.Greengrass 2.9.1 service generated with"
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
     keywords="aiobotocore greengrass type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_greengrass": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-greengrass-2.9.0/types_aiobotocore_greengrass/__init__.py` & `types-aiobotocore-greengrass-2.9.1/types_aiobotocore_greengrass/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,14 @@
     ListResourceDefinitionVersionsPaginator,
     ListSubscriptionDefinitionsPaginator,
     ListSubscriptionDefinitionVersionsPaginator,
 )
 
 Client = GreengrassClient
 
-
 __all__ = (
     "Client",
     "GreengrassClient",
     "ListBulkDeploymentDetailedReportsPaginator",
     "ListBulkDeploymentsPaginator",
     "ListConnectorDefinitionVersionsPaginator",
     "ListConnectorDefinitionsPaginator",
```

### Comparing `types-aiobotocore-greengrass-2.9.0/types_aiobotocore_greengrass/__init__.pyi` & `types-aiobotocore-greengrass-2.9.1/types_aiobotocore_greengrass/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-greengrass-2.9.0/types_aiobotocore_greengrass/__main__.py` & `types-aiobotocore-greengrass-2.9.1/types_aiobotocore_greengrass/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Greengrass 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Greengrass 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass\nOther"
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

### Comparing `types-aiobotocore-greengrass-2.9.0/types_aiobotocore_greengrass/client.py` & `types-aiobotocore-greengrass-2.9.1/types_aiobotocore_greengrass/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("GreengrassClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -221,58 +220,58 @@
 
     async def create_connector_definition(
         self,
         *,
         AmznClientToken: str = ...,
         InitialVersion: ConnectorDefinitionVersionTypeDef = ...,
         Name: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateConnectorDefinitionResponseTypeDef:
         """
         Creates a connector definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_connector_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#create_connector_definition)
         """
 
     async def create_connector_definition_version(
         self,
         *,
         ConnectorDefinitionId: str,
         AmznClientToken: str = ...,
-        Connectors: Sequence[ConnectorTypeDef] = ...
+        Connectors: Sequence[ConnectorTypeDef] = ...,
     ) -> CreateConnectorDefinitionVersionResponseTypeDef:
         """
         Creates a version of a connector definition which has already been defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_connector_definition_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#create_connector_definition_version)
         """
 
     async def create_core_definition(
         self,
         *,
         AmznClientToken: str = ...,
         InitialVersion: CoreDefinitionVersionTypeDef = ...,
         Name: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateCoreDefinitionResponseTypeDef:
         """
         Creates a core definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_core_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#create_core_definition)
         """
 
     async def create_core_definition_version(
         self,
         *,
         CoreDefinitionId: str,
         AmznClientToken: str = ...,
-        Cores: Sequence[CoreTypeDef] = ...
+        Cores: Sequence[CoreTypeDef] = ...,
     ) -> CreateCoreDefinitionVersionResponseTypeDef:
         """
         Creates a version of a core definition that has already been defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_core_definition_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#create_core_definition_version)
         """
@@ -280,59 +279,59 @@
     async def create_deployment(
         self,
         *,
         DeploymentType: DeploymentTypeType,
         GroupId: str,
         AmznClientToken: str = ...,
         DeploymentId: str = ...,
-        GroupVersionId: str = ...
+        GroupVersionId: str = ...,
     ) -> CreateDeploymentResponseTypeDef:
         """
         Creates a deployment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_deployment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#create_deployment)
         """
 
     async def create_device_definition(
         self,
         *,
         AmznClientToken: str = ...,
         InitialVersion: DeviceDefinitionVersionTypeDef = ...,
         Name: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateDeviceDefinitionResponseTypeDef:
         """
         Creates a device definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_device_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#create_device_definition)
         """
 
     async def create_device_definition_version(
         self,
         *,
         DeviceDefinitionId: str,
         AmznClientToken: str = ...,
-        Devices: Sequence[DeviceTypeDef] = ...
+        Devices: Sequence[DeviceTypeDef] = ...,
     ) -> CreateDeviceDefinitionVersionResponseTypeDef:
         """
         Creates a version of a device definition that has already been defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_device_definition_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#create_device_definition_version)
         """
 
     async def create_function_definition(
         self,
         *,
         AmznClientToken: str = ...,
         InitialVersion: FunctionDefinitionVersionTypeDef = ...,
         Name: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateFunctionDefinitionResponseTypeDef:
         """
         Creates a Lambda function definition which contains a list of Lambda functions
         and their configurations to be used in a
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_function_definition)
@@ -341,30 +340,30 @@
 
     async def create_function_definition_version(
         self,
         *,
         FunctionDefinitionId: str,
         AmznClientToken: str = ...,
         DefaultConfig: FunctionDefaultConfigTypeDef = ...,
-        Functions: Sequence[FunctionTypeDef] = ...
+        Functions: Sequence[FunctionTypeDef] = ...,
     ) -> CreateFunctionDefinitionVersionResponseTypeDef:
         """
         Creates a version of a Lambda function definition that has already been defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_function_definition_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#create_function_definition_version)
         """
 
     async def create_group(
         self,
         *,
         Name: str,
         AmznClientToken: str = ...,
         InitialVersion: GroupVersionTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateGroupResponseTypeDef:
         """
         Creates a group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#create_group)
         """
@@ -386,59 +385,59 @@
         AmznClientToken: str = ...,
         ConnectorDefinitionVersionArn: str = ...,
         CoreDefinitionVersionArn: str = ...,
         DeviceDefinitionVersionArn: str = ...,
         FunctionDefinitionVersionArn: str = ...,
         LoggerDefinitionVersionArn: str = ...,
         ResourceDefinitionVersionArn: str = ...,
-        SubscriptionDefinitionVersionArn: str = ...
+        SubscriptionDefinitionVersionArn: str = ...,
     ) -> CreateGroupVersionResponseTypeDef:
         """
         Creates a version of a group which has already been defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_group_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#create_group_version)
         """
 
     async def create_logger_definition(
         self,
         *,
         AmznClientToken: str = ...,
         InitialVersion: LoggerDefinitionVersionTypeDef = ...,
         Name: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateLoggerDefinitionResponseTypeDef:
         """
         Creates a logger definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_logger_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#create_logger_definition)
         """
 
     async def create_logger_definition_version(
         self,
         *,
         LoggerDefinitionId: str,
         AmznClientToken: str = ...,
-        Loggers: Sequence[LoggerTypeDef] = ...
+        Loggers: Sequence[LoggerTypeDef] = ...,
     ) -> CreateLoggerDefinitionVersionResponseTypeDef:
         """
         Creates a version of a logger definition that has already been defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_logger_definition_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#create_logger_definition_version)
         """
 
     async def create_resource_definition(
         self,
         *,
         AmznClientToken: str = ...,
         InitialVersion: ResourceDefinitionVersionTypeDef = ...,
         Name: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateResourceDefinitionResponseTypeDef:
         """
         Creates a resource definition which contains a list of resources to be used in
         a
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_resource_definition)
@@ -446,15 +445,15 @@
         """
 
     async def create_resource_definition_version(
         self,
         *,
         ResourceDefinitionId: str,
         AmznClientToken: str = ...,
-        Resources: Sequence[ResourceTypeDef] = ...
+        Resources: Sequence[ResourceTypeDef] = ...,
     ) -> CreateResourceDefinitionVersionResponseTypeDef:
         """
         Creates a version of a resource definition that has already been defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_resource_definition_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#create_resource_definition_version)
         """
@@ -464,15 +463,15 @@
         *,
         S3UrlSignerRole: str,
         SoftwareToUpdate: SoftwareToUpdateType,
         UpdateTargets: Sequence[str],
         UpdateTargetsArchitecture: UpdateTargetsArchitectureType,
         UpdateTargetsOperatingSystem: UpdateTargetsOperatingSystemType,
         AmznClientToken: str = ...,
-        UpdateAgentLogLevel: UpdateAgentLogLevelType = ...
+        UpdateAgentLogLevel: UpdateAgentLogLevelType = ...,
     ) -> CreateSoftwareUpdateJobResponseTypeDef:
         """
         Creates a software update for a core or group of cores (specified as an IoT
         thing group.) Use this to update the OTA Agent as well as the Greengrass core
         software.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_software_update_job)
@@ -481,29 +480,29 @@
 
     async def create_subscription_definition(
         self,
         *,
         AmznClientToken: str = ...,
         InitialVersion: SubscriptionDefinitionVersionTypeDef = ...,
         Name: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateSubscriptionDefinitionResponseTypeDef:
         """
         Creates a subscription definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_subscription_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#create_subscription_definition)
         """
 
     async def create_subscription_definition_version(
         self,
         *,
         SubscriptionDefinitionId: str,
         AmznClientToken: str = ...,
-        Subscriptions: Sequence[SubscriptionTypeDef] = ...
+        Subscriptions: Sequence[SubscriptionTypeDef] = ...,
     ) -> CreateSubscriptionDefinitionVersionResponseTypeDef:
         """
         Creates a version of a subscription definition which has already been defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_subscription_definition_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#create_subscription_definition_version)
         """
@@ -831,15 +830,15 @@
         """
 
     async def get_subscription_definition_version(
         self,
         *,
         SubscriptionDefinitionId: str,
         SubscriptionDefinitionVersionId: str,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetSubscriptionDefinitionVersionResponseTypeDef:
         """
         Retrieves information about a subscription definition version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.get_subscription_definition_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#get_subscription_definition_version)
         """
@@ -1079,15 +1078,15 @@
 
     async def start_bulk_deployment(
         self,
         *,
         ExecutionRoleArn: str,
         InputFileUri: str,
         AmznClientToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> StartBulkDeploymentResponseTypeDef:
         """
         Deploys multiple groups in one operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.start_bulk_deployment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#start_bulk_deployment)
         """
```

### Comparing `types-aiobotocore-greengrass-2.9.0/types_aiobotocore_greengrass/client.pyi` & `types-aiobotocore-greengrass-2.9.1/types_aiobotocore_greengrass/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -217,58 +217,58 @@
 
     async def create_connector_definition(
         self,
         *,
         AmznClientToken: str = ...,
         InitialVersion: ConnectorDefinitionVersionTypeDef = ...,
         Name: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateConnectorDefinitionResponseTypeDef:
         """
         Creates a connector definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_connector_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#create_connector_definition)
         """
 
     async def create_connector_definition_version(
         self,
         *,
         ConnectorDefinitionId: str,
         AmznClientToken: str = ...,
-        Connectors: Sequence[ConnectorTypeDef] = ...
+        Connectors: Sequence[ConnectorTypeDef] = ...,
     ) -> CreateConnectorDefinitionVersionResponseTypeDef:
         """
         Creates a version of a connector definition which has already been defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_connector_definition_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#create_connector_definition_version)
         """
 
     async def create_core_definition(
         self,
         *,
         AmznClientToken: str = ...,
         InitialVersion: CoreDefinitionVersionTypeDef = ...,
         Name: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateCoreDefinitionResponseTypeDef:
         """
         Creates a core definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_core_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#create_core_definition)
         """
 
     async def create_core_definition_version(
         self,
         *,
         CoreDefinitionId: str,
         AmznClientToken: str = ...,
-        Cores: Sequence[CoreTypeDef] = ...
+        Cores: Sequence[CoreTypeDef] = ...,
     ) -> CreateCoreDefinitionVersionResponseTypeDef:
         """
         Creates a version of a core definition that has already been defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_core_definition_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#create_core_definition_version)
         """
@@ -276,59 +276,59 @@
     async def create_deployment(
         self,
         *,
         DeploymentType: DeploymentTypeType,
         GroupId: str,
         AmznClientToken: str = ...,
         DeploymentId: str = ...,
-        GroupVersionId: str = ...
+        GroupVersionId: str = ...,
     ) -> CreateDeploymentResponseTypeDef:
         """
         Creates a deployment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_deployment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#create_deployment)
         """
 
     async def create_device_definition(
         self,
         *,
         AmznClientToken: str = ...,
         InitialVersion: DeviceDefinitionVersionTypeDef = ...,
         Name: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateDeviceDefinitionResponseTypeDef:
         """
         Creates a device definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_device_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#create_device_definition)
         """
 
     async def create_device_definition_version(
         self,
         *,
         DeviceDefinitionId: str,
         AmznClientToken: str = ...,
-        Devices: Sequence[DeviceTypeDef] = ...
+        Devices: Sequence[DeviceTypeDef] = ...,
     ) -> CreateDeviceDefinitionVersionResponseTypeDef:
         """
         Creates a version of a device definition that has already been defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_device_definition_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#create_device_definition_version)
         """
 
     async def create_function_definition(
         self,
         *,
         AmznClientToken: str = ...,
         InitialVersion: FunctionDefinitionVersionTypeDef = ...,
         Name: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateFunctionDefinitionResponseTypeDef:
         """
         Creates a Lambda function definition which contains a list of Lambda functions
         and their configurations to be used in a
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_function_definition)
@@ -337,30 +337,30 @@
 
     async def create_function_definition_version(
         self,
         *,
         FunctionDefinitionId: str,
         AmznClientToken: str = ...,
         DefaultConfig: FunctionDefaultConfigTypeDef = ...,
-        Functions: Sequence[FunctionTypeDef] = ...
+        Functions: Sequence[FunctionTypeDef] = ...,
     ) -> CreateFunctionDefinitionVersionResponseTypeDef:
         """
         Creates a version of a Lambda function definition that has already been defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_function_definition_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#create_function_definition_version)
         """
 
     async def create_group(
         self,
         *,
         Name: str,
         AmznClientToken: str = ...,
         InitialVersion: GroupVersionTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateGroupResponseTypeDef:
         """
         Creates a group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#create_group)
         """
@@ -382,59 +382,59 @@
         AmznClientToken: str = ...,
         ConnectorDefinitionVersionArn: str = ...,
         CoreDefinitionVersionArn: str = ...,
         DeviceDefinitionVersionArn: str = ...,
         FunctionDefinitionVersionArn: str = ...,
         LoggerDefinitionVersionArn: str = ...,
         ResourceDefinitionVersionArn: str = ...,
-        SubscriptionDefinitionVersionArn: str = ...
+        SubscriptionDefinitionVersionArn: str = ...,
     ) -> CreateGroupVersionResponseTypeDef:
         """
         Creates a version of a group which has already been defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_group_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#create_group_version)
         """
 
     async def create_logger_definition(
         self,
         *,
         AmznClientToken: str = ...,
         InitialVersion: LoggerDefinitionVersionTypeDef = ...,
         Name: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateLoggerDefinitionResponseTypeDef:
         """
         Creates a logger definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_logger_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#create_logger_definition)
         """
 
     async def create_logger_definition_version(
         self,
         *,
         LoggerDefinitionId: str,
         AmznClientToken: str = ...,
-        Loggers: Sequence[LoggerTypeDef] = ...
+        Loggers: Sequence[LoggerTypeDef] = ...,
     ) -> CreateLoggerDefinitionVersionResponseTypeDef:
         """
         Creates a version of a logger definition that has already been defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_logger_definition_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#create_logger_definition_version)
         """
 
     async def create_resource_definition(
         self,
         *,
         AmznClientToken: str = ...,
         InitialVersion: ResourceDefinitionVersionTypeDef = ...,
         Name: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateResourceDefinitionResponseTypeDef:
         """
         Creates a resource definition which contains a list of resources to be used in
         a
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_resource_definition)
@@ -442,15 +442,15 @@
         """
 
     async def create_resource_definition_version(
         self,
         *,
         ResourceDefinitionId: str,
         AmznClientToken: str = ...,
-        Resources: Sequence[ResourceTypeDef] = ...
+        Resources: Sequence[ResourceTypeDef] = ...,
     ) -> CreateResourceDefinitionVersionResponseTypeDef:
         """
         Creates a version of a resource definition that has already been defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_resource_definition_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#create_resource_definition_version)
         """
@@ -460,15 +460,15 @@
         *,
         S3UrlSignerRole: str,
         SoftwareToUpdate: SoftwareToUpdateType,
         UpdateTargets: Sequence[str],
         UpdateTargetsArchitecture: UpdateTargetsArchitectureType,
         UpdateTargetsOperatingSystem: UpdateTargetsOperatingSystemType,
         AmznClientToken: str = ...,
-        UpdateAgentLogLevel: UpdateAgentLogLevelType = ...
+        UpdateAgentLogLevel: UpdateAgentLogLevelType = ...,
     ) -> CreateSoftwareUpdateJobResponseTypeDef:
         """
         Creates a software update for a core or group of cores (specified as an IoT
         thing group.) Use this to update the OTA Agent as well as the Greengrass core
         software.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_software_update_job)
@@ -477,29 +477,29 @@
 
     async def create_subscription_definition(
         self,
         *,
         AmznClientToken: str = ...,
         InitialVersion: SubscriptionDefinitionVersionTypeDef = ...,
         Name: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateSubscriptionDefinitionResponseTypeDef:
         """
         Creates a subscription definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_subscription_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#create_subscription_definition)
         """
 
     async def create_subscription_definition_version(
         self,
         *,
         SubscriptionDefinitionId: str,
         AmznClientToken: str = ...,
-        Subscriptions: Sequence[SubscriptionTypeDef] = ...
+        Subscriptions: Sequence[SubscriptionTypeDef] = ...,
     ) -> CreateSubscriptionDefinitionVersionResponseTypeDef:
         """
         Creates a version of a subscription definition which has already been defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_subscription_definition_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#create_subscription_definition_version)
         """
@@ -827,15 +827,15 @@
         """
 
     async def get_subscription_definition_version(
         self,
         *,
         SubscriptionDefinitionId: str,
         SubscriptionDefinitionVersionId: str,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetSubscriptionDefinitionVersionResponseTypeDef:
         """
         Retrieves information about a subscription definition version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.get_subscription_definition_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#get_subscription_definition_version)
         """
@@ -1075,15 +1075,15 @@
 
     async def start_bulk_deployment(
         self,
         *,
         ExecutionRoleArn: str,
         InputFileUri: str,
         AmznClientToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> StartBulkDeploymentResponseTypeDef:
         """
         Deploys multiple groups in one operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.start_bulk_deployment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#start_bulk_deployment)
         """
```

### Comparing `types-aiobotocore-greengrass-2.9.0/types_aiobotocore_greengrass/literals.py` & `types-aiobotocore-greengrass-2.9.1/types_aiobotocore_greengrass/literals.py`

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
     "BulkDeploymentStatusType",
     "ConfigurationSyncStatusType",
     "DeploymentTypeType",
     "EncodingTypeType",
     "FunctionIsolationModeType",
     "ListBulkDeploymentDetailedReportsPaginatorName",
@@ -57,15 +56,14 @@
     "GreengrassServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 BulkDeploymentStatusType = Literal[
     "Completed", "Failed", "Initializing", "Running", "Stopped", "Stopping"
 ]
 ConfigurationSyncStatusType = Literal["InSync", "OutOfSync"]
 DeploymentTypeType = Literal[
     "ForceResetDeployment", "NewDeployment", "Redeployment", "ResetDeployment"
 ]
```

### Comparing `types-aiobotocore-greengrass-2.9.0/types_aiobotocore_greengrass/literals.pyi` & `types-aiobotocore-greengrass-2.9.1/types_aiobotocore_greengrass/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-greengrass-2.9.0/types_aiobotocore_greengrass/paginator.py` & `types-aiobotocore-greengrass-2.9.1/types_aiobotocore_greengrass/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,14 @@
     "ListLoggerDefinitionsPaginator",
     "ListResourceDefinitionVersionsPaginator",
     "ListResourceDefinitionsPaginator",
     "ListSubscriptionDefinitionVersionsPaginator",
     "ListSubscriptionDefinitionsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
```

### Comparing `types-aiobotocore-greengrass-2.9.0/types_aiobotocore_greengrass/paginator.pyi` & `types-aiobotocore-greengrass-2.9.1/types_aiobotocore_greengrass/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-greengrass-2.9.0/types_aiobotocore_greengrass/type_defs.py` & `types-aiobotocore-greengrass-2.9.1/types_aiobotocore_greengrass/type_defs.py`

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
     "AssociateRoleToGroupRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AssociateServiceRoleToAccountRequestRequestTypeDef",
     "BulkDeploymentMetricsTypeDef",
     "ErrorDetailTypeDef",
     "BulkDeploymentTypeDef",
```

### Comparing `types-aiobotocore-greengrass-2.9.0/types_aiobotocore_greengrass/type_defs.pyi` & `types-aiobotocore-greengrass-2.9.1/types_aiobotocore_greengrass/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-greengrass-2.9.0/types_aiobotocore_greengrass.egg-info/PKG-INFO` & `types-aiobotocore-greengrass-2.9.1/types_aiobotocore_greengrass.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-greengrass
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Greengrass 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Greengrass 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/
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
 
 <a id="types-aiobotocore-greengrass"></a>
 
 # types-aiobotocore-greengrass
 
 [![PyPI - types-aiobotocore-greengrass](https://img.shields.io/pypi/v/types-aiobotocore-greengrass.svg?color=blue)](https://pypi.org/project/types-aiobotocore-greengrass)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-greengrass.svg?color=blue)](https://pypi.org/project/types-aiobotocore-greengrass)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-greengrass)](https://pepy.tech/project/types-aiobotocore-greengrass)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Greengrass 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass)
+[aiobotocore.Greengrass 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass)
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
 [types-aiobotocore-greengrass docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-greengrass-2.9.0/types_aiobotocore_greengrass.egg-info/SOURCES.txt` & `types-aiobotocore-greengrass-2.9.1/types_aiobotocore_greengrass.egg-info/SOURCES.txt`

 * *Files identical despite different names*

