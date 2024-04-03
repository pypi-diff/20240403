# Comparing `tmp/types-aiobotocore-entityresolution-2.9.0.tar.gz` & `tmp/types-aiobotocore-entityresolution-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-entityresolution-2.9.0.tar", last modified: Wed Dec 13 19:59:17 2023, max compression
+gzip compressed data, was "types-aiobotocore-entityresolution-2.9.1.tar", last modified: Thu Jan 18 01:20:41 2024, max compression
```

## Comparing `types-aiobotocore-entityresolution-2.9.0.tar` & `types-aiobotocore-entityresolution-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:17.173748 types-aiobotocore-entityresolution-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:46:00.000000 types-aiobotocore-entityresolution-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14374 2023-12-13 19:59:17.173748 types-aiobotocore-entityresolution-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12775 2023-12-13 19:46:00.000000 types-aiobotocore-entityresolution-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:17.173748 types-aiobotocore-entityresolution-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2023-12-13 19:45:59.000000 types-aiobotocore-entityresolution-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:17.173748 types-aiobotocore-entityresolution-2.9.0/types_aiobotocore_entityresolution/
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2023-12-13 19:46:00.000000 types-aiobotocore-entityresolution-2.9.0/types_aiobotocore_entityresolution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2023-12-13 19:46:00.000000 types-aiobotocore-entityresolution-2.9.0/types_aiobotocore_entityresolution/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      968 2023-12-13 19:46:00.000000 types-aiobotocore-entityresolution-2.9.0/types_aiobotocore_entityresolution/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25855 2023-12-13 19:46:00.000000 types-aiobotocore-entityresolution-2.9.0/types_aiobotocore_entityresolution/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    25851 2023-12-13 19:46:00.000000 types-aiobotocore-entityresolution-2.9.0/types_aiobotocore_entityresolution/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9993 2023-12-13 19:46:00.000000 types-aiobotocore-entityresolution-2.9.0/types_aiobotocore_entityresolution/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9991 2023-12-13 19:46:00.000000 types-aiobotocore-entityresolution-2.9.0/types_aiobotocore_entityresolution/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8091 2023-12-13 19:46:00.000000 types-aiobotocore-entityresolution-2.9.0/types_aiobotocore_entityresolution/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8083 2023-12-13 19:46:00.000000 types-aiobotocore-entityresolution-2.9.0/types_aiobotocore_entityresolution/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:46:00.000000 types-aiobotocore-entityresolution-2.9.0/types_aiobotocore_entityresolution/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    25442 2023-12-13 19:46:00.000000 types-aiobotocore-entityresolution-2.9.0/types_aiobotocore_entityresolution/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    25441 2023-12-13 19:46:00.000000 types-aiobotocore-entityresolution-2.9.0/types_aiobotocore_entityresolution/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:46:00.000000 types-aiobotocore-entityresolution-2.9.0/types_aiobotocore_entityresolution/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:17.173748 types-aiobotocore-entityresolution-2.9.0/types_aiobotocore_entityresolution.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14374 2023-12-13 19:59:17.000000 types-aiobotocore-entityresolution-2.9.0/types_aiobotocore_entityresolution.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      984 2023-12-13 19:59:17.000000 types-aiobotocore-entityresolution-2.9.0/types_aiobotocore_entityresolution.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:17.000000 types-aiobotocore-entityresolution-2.9.0/types_aiobotocore_entityresolution.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:17.000000 types-aiobotocore-entityresolution-2.9.0/types_aiobotocore_entityresolution.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:17.000000 types-aiobotocore-entityresolution-2.9.0/types_aiobotocore_entityresolution.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-13 19:59:17.000000 types-aiobotocore-entityresolution-2.9.0/types_aiobotocore_entityresolution.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:41.821337 types-aiobotocore-entityresolution-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:07:55.000000 types-aiobotocore-entityresolution-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14394 2024-01-18 01:20:41.821337 types-aiobotocore-entityresolution-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12775 2024-01-18 01:07:55.000000 types-aiobotocore-entityresolution-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:41.821337 types-aiobotocore-entityresolution-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-01-18 01:07:55.000000 types-aiobotocore-entityresolution-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:41.817337 types-aiobotocore-entityresolution-2.9.1/types_aiobotocore_entityresolution/
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-01-18 01:07:55.000000 types-aiobotocore-entityresolution-2.9.1/types_aiobotocore_entityresolution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-01-18 01:07:55.000000 types-aiobotocore-entityresolution-2.9.1/types_aiobotocore_entityresolution/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-01-18 01:07:55.000000 types-aiobotocore-entityresolution-2.9.1/types_aiobotocore_entityresolution/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25860 2024-01-18 01:07:55.000000 types-aiobotocore-entityresolution-2.9.1/types_aiobotocore_entityresolution/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25857 2024-01-18 01:07:55.000000 types-aiobotocore-entityresolution-2.9.1/types_aiobotocore_entityresolution/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9991 2024-01-18 01:07:55.000000 types-aiobotocore-entityresolution-2.9.1/types_aiobotocore_entityresolution/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9991 2024-01-18 01:07:55.000000 types-aiobotocore-entityresolution-2.9.1/types_aiobotocore_entityresolution/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8090 2024-01-18 01:07:55.000000 types-aiobotocore-entityresolution-2.9.1/types_aiobotocore_entityresolution/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8083 2024-01-18 01:07:55.000000 types-aiobotocore-entityresolution-2.9.1/types_aiobotocore_entityresolution/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:07:55.000000 types-aiobotocore-entityresolution-2.9.1/types_aiobotocore_entityresolution/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    25441 2024-01-18 01:07:56.000000 types-aiobotocore-entityresolution-2.9.1/types_aiobotocore_entityresolution/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25441 2024-01-18 01:07:56.000000 types-aiobotocore-entityresolution-2.9.1/types_aiobotocore_entityresolution/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:07:55.000000 types-aiobotocore-entityresolution-2.9.1/types_aiobotocore_entityresolution/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:41.821337 types-aiobotocore-entityresolution-2.9.1/types_aiobotocore_entityresolution.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14394 2024-01-18 01:20:41.000000 types-aiobotocore-entityresolution-2.9.1/types_aiobotocore_entityresolution.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-01-18 01:20:41.000000 types-aiobotocore-entityresolution-2.9.1/types_aiobotocore_entityresolution.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:41.000000 types-aiobotocore-entityresolution-2.9.1/types_aiobotocore_entityresolution.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:41.000000 types-aiobotocore-entityresolution-2.9.1/types_aiobotocore_entityresolution.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:41.000000 types-aiobotocore-entityresolution-2.9.1/types_aiobotocore_entityresolution.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-18 01:20:41.000000 types-aiobotocore-entityresolution-2.9.1/types_aiobotocore_entityresolution.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-entityresolution-2.9.0/LICENSE` & `types-aiobotocore-entityresolution-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-entityresolution-2.9.0/PKG-INFO` & `types-aiobotocore-entityresolution-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-entityresolution
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.EntityResolution 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.EntityResolution 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_entityresolution/
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
 
 <a id="types-aiobotocore-entityresolution"></a>
 
 # types-aiobotocore-entityresolution
 
 [![PyPI - types-aiobotocore-entityresolution](https://img.shields.io/pypi/v/types-aiobotocore-entityresolution.svg?color=blue)](https://pypi.org/project/types-aiobotocore-entityresolution)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-entityresolution.svg?color=blue)](https://pypi.org/project/types-aiobotocore-entityresolution)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_entityresolution/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-entityresolution)](https://pepy.tech/project/types-aiobotocore-entityresolution)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EntityResolution 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution)
+[aiobotocore.EntityResolution 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution)
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
 [types-aiobotocore-entityresolution docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_entityresolution/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-entityresolution-2.9.0/README.md` & `types-aiobotocore-entityresolution-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-entityresolution.svg?color=blue)](https://pypi.org/project/types-aiobotocore-entityresolution)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_entityresolution/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-entityresolution)](https://pepy.tech/project/types-aiobotocore-entityresolution)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EntityResolution 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution)
+[aiobotocore.EntityResolution 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution)
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
 [types-aiobotocore-entityresolution docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_entityresolution/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-entityresolution-2.9.0/setup.py` & `types-aiobotocore-entityresolution-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-entityresolution",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_entityresolution"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.EntityResolution 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.EntityResolution 2.9.1 service generated with"
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
     keywords="aiobotocore entityresolution type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_entityresolution": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_entityresolution/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-entityresolution-2.9.0/types_aiobotocore_entityresolution/__init__.py` & `types-aiobotocore-entityresolution-2.9.1/types_aiobotocore_entityresolution/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,14 @@
     ListMatchingWorkflowsPaginator,
     ListProviderServicesPaginator,
     ListSchemaMappingsPaginator,
 )
 
 Client = EntityResolutionClient
 
-
 __all__ = (
     "Client",
     "EntityResolutionClient",
     "ListIdMappingJobsPaginator",
     "ListIdMappingWorkflowsPaginator",
     "ListMatchingJobsPaginator",
     "ListMatchingWorkflowsPaginator",
```

### Comparing `types-aiobotocore-entityresolution-2.9.0/types_aiobotocore_entityresolution/__init__.pyi` & `types-aiobotocore-entityresolution-2.9.1/types_aiobotocore_entityresolution/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-entityresolution-2.9.0/types_aiobotocore_entityresolution/__main__.py` & `types-aiobotocore-entityresolution-2.9.1/types_aiobotocore_entityresolution/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.EntityResolution 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.EntityResolution 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_entityresolution//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution\nOther"
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

### Comparing `types-aiobotocore-entityresolution-2.9.0/types_aiobotocore_entityresolution/client.py` & `types-aiobotocore-entityresolution-2.9.1/types_aiobotocore_entityresolution/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("EntityResolutionClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -131,15 +130,15 @@
         *,
         idMappingTechniques: IdMappingTechniquesTypeDef,
         inputSourceConfig: Sequence[IdMappingWorkflowInputSourceTypeDef],
         outputSourceConfig: Sequence[IdMappingWorkflowOutputSourceTypeDef],
         roleArn: str,
         workflowName: str,
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateIdMappingWorkflowOutputTypeDef:
         """
         Creates an `IdMappingWorkflow` object which stores the configuration of the
         data processing job to be
         run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.create_id_mapping_workflow)
@@ -152,15 +151,15 @@
         inputSourceConfig: Sequence[InputSourceTypeDef],
         outputSourceConfig: Sequence[OutputSourceTypeDef],
         resolutionTechniques: ResolutionTechniquesTypeDef,
         roleArn: str,
         workflowName: str,
         description: str = ...,
         incrementalRunConfig: IncrementalRunConfigTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateMatchingWorkflowOutputTypeDef:
         """
         Creates a `MatchingWorkflow` object which stores the configuration of the data
         processing job to be
         run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.create_matching_workflow)
@@ -169,15 +168,15 @@
 
     async def create_schema_mapping(
         self,
         *,
         mappedInputFields: Sequence[SchemaInputAttributeTypeDef],
         schemaName: str,
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateSchemaMappingOutputTypeDef:
         """
         Creates a schema mapping, which defines the schema of the input customer
         records
         table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.create_schema_mapping)
@@ -410,15 +409,15 @@
         self,
         *,
         idMappingTechniques: IdMappingTechniquesTypeDef,
         inputSourceConfig: Sequence[IdMappingWorkflowInputSourceTypeDef],
         outputSourceConfig: Sequence[IdMappingWorkflowOutputSourceTypeDef],
         roleArn: str,
         workflowName: str,
-        description: str = ...
+        description: str = ...,
     ) -> UpdateIdMappingWorkflowOutputTypeDef:
         """
         Updates an existing `IdMappingWorkflow`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.update_id_mapping_workflow)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_entityresolution/client/#update_id_mapping_workflow)
         """
@@ -428,29 +427,29 @@
         *,
         inputSourceConfig: Sequence[InputSourceTypeDef],
         outputSourceConfig: Sequence[OutputSourceTypeDef],
         resolutionTechniques: ResolutionTechniquesTypeDef,
         roleArn: str,
         workflowName: str,
         description: str = ...,
-        incrementalRunConfig: IncrementalRunConfigTypeDef = ...
+        incrementalRunConfig: IncrementalRunConfigTypeDef = ...,
     ) -> UpdateMatchingWorkflowOutputTypeDef:
         """
         Updates an existing `MatchingWorkflow`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.update_matching_workflow)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_entityresolution/client/#update_matching_workflow)
         """
 
     async def update_schema_mapping(
         self,
         *,
         mappedInputFields: Sequence[SchemaInputAttributeTypeDef],
         schemaName: str,
-        description: str = ...
+        description: str = ...,
     ) -> UpdateSchemaMappingOutputTypeDef:
         """
         Updates a schema mapping.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.update_schema_mapping)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_entityresolution/client/#update_schema_mapping)
         """
```

### Comparing `types-aiobotocore-entityresolution-2.9.0/types_aiobotocore_entityresolution/client.pyi` & `types-aiobotocore-entityresolution-2.9.1/types_aiobotocore_entityresolution/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,15 @@
         *,
         idMappingTechniques: IdMappingTechniquesTypeDef,
         inputSourceConfig: Sequence[IdMappingWorkflowInputSourceTypeDef],
         outputSourceConfig: Sequence[IdMappingWorkflowOutputSourceTypeDef],
         roleArn: str,
         workflowName: str,
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateIdMappingWorkflowOutputTypeDef:
         """
         Creates an `IdMappingWorkflow` object which stores the configuration of the
         data processing job to be
         run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.create_id_mapping_workflow)
@@ -148,15 +148,15 @@
         inputSourceConfig: Sequence[InputSourceTypeDef],
         outputSourceConfig: Sequence[OutputSourceTypeDef],
         resolutionTechniques: ResolutionTechniquesTypeDef,
         roleArn: str,
         workflowName: str,
         description: str = ...,
         incrementalRunConfig: IncrementalRunConfigTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateMatchingWorkflowOutputTypeDef:
         """
         Creates a `MatchingWorkflow` object which stores the configuration of the data
         processing job to be
         run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.create_matching_workflow)
@@ -165,15 +165,15 @@
 
     async def create_schema_mapping(
         self,
         *,
         mappedInputFields: Sequence[SchemaInputAttributeTypeDef],
         schemaName: str,
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateSchemaMappingOutputTypeDef:
         """
         Creates a schema mapping, which defines the schema of the input customer
         records
         table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.create_schema_mapping)
@@ -406,15 +406,15 @@
         self,
         *,
         idMappingTechniques: IdMappingTechniquesTypeDef,
         inputSourceConfig: Sequence[IdMappingWorkflowInputSourceTypeDef],
         outputSourceConfig: Sequence[IdMappingWorkflowOutputSourceTypeDef],
         roleArn: str,
         workflowName: str,
-        description: str = ...
+        description: str = ...,
     ) -> UpdateIdMappingWorkflowOutputTypeDef:
         """
         Updates an existing `IdMappingWorkflow`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.update_id_mapping_workflow)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_entityresolution/client/#update_id_mapping_workflow)
         """
@@ -424,29 +424,29 @@
         *,
         inputSourceConfig: Sequence[InputSourceTypeDef],
         outputSourceConfig: Sequence[OutputSourceTypeDef],
         resolutionTechniques: ResolutionTechniquesTypeDef,
         roleArn: str,
         workflowName: str,
         description: str = ...,
-        incrementalRunConfig: IncrementalRunConfigTypeDef = ...
+        incrementalRunConfig: IncrementalRunConfigTypeDef = ...,
     ) -> UpdateMatchingWorkflowOutputTypeDef:
         """
         Updates an existing `MatchingWorkflow`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.update_matching_workflow)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_entityresolution/client/#update_matching_workflow)
         """
 
     async def update_schema_mapping(
         self,
         *,
         mappedInputFields: Sequence[SchemaInputAttributeTypeDef],
         schemaName: str,
-        description: str = ...
+        description: str = ...,
     ) -> UpdateSchemaMappingOutputTypeDef:
         """
         Updates a schema mapping.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.update_schema_mapping)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_entityresolution/client/#update_schema_mapping)
         """
```

### Comparing `types-aiobotocore-entityresolution-2.9.0/types_aiobotocore_entityresolution/literals.py` & `types-aiobotocore-entityresolution-2.9.1/types_aiobotocore_entityresolution/literals.py`

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
     "AttributeMatchingModelType",
     "IdMappingTypeType",
     "IncrementalRunTypeType",
     "JobStatusType",
     "ListIdMappingJobsPaginatorName",
     "ListIdMappingWorkflowsPaginatorName",
@@ -36,15 +35,14 @@
     "ServiceTypeType",
     "EntityResolutionServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 AttributeMatchingModelType = Literal["MANY_TO_MANY", "ONE_TO_ONE"]
 IdMappingTypeType = Literal["PROVIDER"]
 IncrementalRunTypeType = Literal["IMMEDIATE"]
 JobStatusType = Literal["FAILED", "QUEUED", "RUNNING", "SUCCEEDED"]
 ListIdMappingJobsPaginatorName = Literal["list_id_mapping_jobs"]
 ListIdMappingWorkflowsPaginatorName = Literal["list_id_mapping_workflows"]
 ListMatchingJobsPaginatorName = Literal["list_matching_jobs"]
```

### Comparing `types-aiobotocore-entityresolution-2.9.0/types_aiobotocore_entityresolution/literals.pyi` & `types-aiobotocore-entityresolution-2.9.1/types_aiobotocore_entityresolution/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-entityresolution-2.9.0/types_aiobotocore_entityresolution/paginator.py` & `types-aiobotocore-entityresolution-2.9.1/types_aiobotocore_entityresolution/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,14 @@
     "ListIdMappingWorkflowsPaginator",
     "ListMatchingJobsPaginator",
     "ListMatchingWorkflowsPaginator",
     "ListProviderServicesPaginator",
     "ListSchemaMappingsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
```

### Comparing `types-aiobotocore-entityresolution-2.9.0/types_aiobotocore_entityresolution/paginator.pyi` & `types-aiobotocore-entityresolution-2.9.1/types_aiobotocore_entityresolution/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-entityresolution-2.9.0/types_aiobotocore_entityresolution/type_defs.py` & `types-aiobotocore-entityresolution-2.9.1/types_aiobotocore_entityresolution/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "IdMappingWorkflowInputSourceTypeDef",
     "IdMappingWorkflowOutputSourceTypeDef",
     "ResponseMetadataTypeDef",
     "IncrementalRunConfigTypeDef",
     "InputSourceTypeDef",
     "SchemaInputAttributeTypeDef",
```

### Comparing `types-aiobotocore-entityresolution-2.9.0/types_aiobotocore_entityresolution/type_defs.pyi` & `types-aiobotocore-entityresolution-2.9.1/types_aiobotocore_entityresolution/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-entityresolution-2.9.0/types_aiobotocore_entityresolution.egg-info/PKG-INFO` & `types-aiobotocore-entityresolution-2.9.1/types_aiobotocore_entityresolution.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-entityresolution
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.EntityResolution 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.EntityResolution 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_entityresolution/
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
 
 <a id="types-aiobotocore-entityresolution"></a>
 
 # types-aiobotocore-entityresolution
 
 [![PyPI - types-aiobotocore-entityresolution](https://img.shields.io/pypi/v/types-aiobotocore-entityresolution.svg?color=blue)](https://pypi.org/project/types-aiobotocore-entityresolution)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-entityresolution.svg?color=blue)](https://pypi.org/project/types-aiobotocore-entityresolution)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_entityresolution/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-entityresolution)](https://pepy.tech/project/types-aiobotocore-entityresolution)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EntityResolution 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution)
+[aiobotocore.EntityResolution 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution)
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
 [types-aiobotocore-entityresolution docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_entityresolution/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-entityresolution-2.9.0/types_aiobotocore_entityresolution.egg-info/SOURCES.txt` & `types-aiobotocore-entityresolution-2.9.1/types_aiobotocore_entityresolution.egg-info/SOURCES.txt`

 * *Files identical despite different names*

