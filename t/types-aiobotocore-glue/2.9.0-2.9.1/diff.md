# Comparing `tmp/types-aiobotocore-glue-2.9.0.tar.gz` & `tmp/types-aiobotocore-glue-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-glue-2.9.0.tar", last modified: Wed Dec 13 19:59:23 2023, max compression
+gzip compressed data, was "types-aiobotocore-glue-2.9.1.tar", last modified: Thu Jan 18 01:20:47 2024, max compression
```

## Comparing `types-aiobotocore-glue-2.9.0.tar` & `types-aiobotocore-glue-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:23.521727 types-aiobotocore-glue-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:46:48.000000 types-aiobotocore-glue-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15244 2023-12-13 19:59:23.521727 types-aiobotocore-glue-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13693 2023-12-13 19:46:48.000000 types-aiobotocore-glue-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:23.521727 types-aiobotocore-glue-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2023-12-13 19:46:48.000000 types-aiobotocore-glue-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:23.521727 types-aiobotocore-glue-2.9.0/types_aiobotocore_glue/
--rw-r--r--   0 runner    (1001) docker     (127)     4160 2023-12-13 19:46:48.000000 types-aiobotocore-glue-2.9.0/types_aiobotocore_glue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4159 2023-12-13 19:46:48.000000 types-aiobotocore-glue-2.9.0/types_aiobotocore_glue/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      909 2023-12-13 19:46:48.000000 types-aiobotocore-glue-2.9.0/types_aiobotocore_glue/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)   151440 2023-12-13 19:46:49.000000 types-aiobotocore-glue-2.9.0/types_aiobotocore_glue/client.py
--rw-r--r--   0 runner    (1001) docker     (127)   151436 2023-12-13 19:46:49.000000 types-aiobotocore-glue-2.9.0/types_aiobotocore_glue/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    22293 2023-12-13 19:46:51.000000 types-aiobotocore-glue-2.9.0/types_aiobotocore_glue/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    22291 2023-12-13 19:46:51.000000 types-aiobotocore-glue-2.9.0/types_aiobotocore_glue/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    22314 2023-12-13 19:46:51.000000 types-aiobotocore-glue-2.9.0/types_aiobotocore_glue/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    22293 2023-12-13 19:46:51.000000 types-aiobotocore-glue-2.9.0/types_aiobotocore_glue/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:46:48.000000 types-aiobotocore-glue-2.9.0/types_aiobotocore_glue/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   236088 2023-12-13 19:46:57.000000 types-aiobotocore-glue-2.9.0/types_aiobotocore_glue/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   236087 2023-12-13 19:46:53.000000 types-aiobotocore-glue-2.9.0/types_aiobotocore_glue/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:46:48.000000 types-aiobotocore-glue-2.9.0/types_aiobotocore_glue/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:23.521727 types-aiobotocore-glue-2.9.0/types_aiobotocore_glue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15244 2023-12-13 19:59:23.000000 types-aiobotocore-glue-2.9.0/types_aiobotocore_glue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      756 2023-12-13 19:59:23.000000 types-aiobotocore-glue-2.9.0/types_aiobotocore_glue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:23.000000 types-aiobotocore-glue-2.9.0/types_aiobotocore_glue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:23.000000 types-aiobotocore-glue-2.9.0/types_aiobotocore_glue.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:23.000000 types-aiobotocore-glue-2.9.0/types_aiobotocore_glue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-13 19:59:23.000000 types-aiobotocore-glue-2.9.0/types_aiobotocore_glue.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:47.637310 types-aiobotocore-glue-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:08:41.000000 types-aiobotocore-glue-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15264 2024-01-18 01:20:47.637310 types-aiobotocore-glue-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13693 2024-01-18 01:08:41.000000 types-aiobotocore-glue-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:47.637310 types-aiobotocore-glue-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-01-18 01:08:41.000000 types-aiobotocore-glue-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:47.637310 types-aiobotocore-glue-2.9.1/types_aiobotocore_glue/
+-rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-01-18 01:08:41.000000 types-aiobotocore-glue-2.9.1/types_aiobotocore_glue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-01-18 01:08:41.000000 types-aiobotocore-glue-2.9.1/types_aiobotocore_glue/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-01-18 01:08:41.000000 types-aiobotocore-glue-2.9.1/types_aiobotocore_glue/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   151518 2024-01-18 01:08:43.000000 types-aiobotocore-glue-2.9.1/types_aiobotocore_glue/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   151515 2024-01-18 01:08:42.000000 types-aiobotocore-glue-2.9.1/types_aiobotocore_glue/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    22291 2024-01-18 01:08:45.000000 types-aiobotocore-glue-2.9.1/types_aiobotocore_glue/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22291 2024-01-18 01:08:44.000000 types-aiobotocore-glue-2.9.1/types_aiobotocore_glue/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    22321 2024-01-18 01:08:43.000000 types-aiobotocore-glue-2.9.1/types_aiobotocore_glue/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22301 2024-01-18 01:08:43.000000 types-aiobotocore-glue-2.9.1/types_aiobotocore_glue/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:08:41.000000 types-aiobotocore-glue-2.9.1/types_aiobotocore_glue/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   236087 2024-01-18 01:08:50.000000 types-aiobotocore-glue-2.9.1/types_aiobotocore_glue/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   236087 2024-01-18 01:08:47.000000 types-aiobotocore-glue-2.9.1/types_aiobotocore_glue/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:08:41.000000 types-aiobotocore-glue-2.9.1/types_aiobotocore_glue/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:47.637310 types-aiobotocore-glue-2.9.1/types_aiobotocore_glue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15264 2024-01-18 01:20:47.000000 types-aiobotocore-glue-2.9.1/types_aiobotocore_glue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-01-18 01:20:47.000000 types-aiobotocore-glue-2.9.1/types_aiobotocore_glue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:47.000000 types-aiobotocore-glue-2.9.1/types_aiobotocore_glue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:47.000000 types-aiobotocore-glue-2.9.1/types_aiobotocore_glue.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:47.000000 types-aiobotocore-glue-2.9.1/types_aiobotocore_glue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-01-18 01:20:47.000000 types-aiobotocore-glue-2.9.1/types_aiobotocore_glue.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-glue-2.9.0/LICENSE` & `types-aiobotocore-glue-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-glue-2.9.0/PKG-INFO` & `types-aiobotocore-glue-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-glue
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Glue 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Glue 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/
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
 
 <a id="types-aiobotocore-glue"></a>
 
 # types-aiobotocore-glue
 
 [![PyPI - types-aiobotocore-glue](https://img.shields.io/pypi/v/types-aiobotocore-glue.svg?color=blue)](https://pypi.org/project/types-aiobotocore-glue)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-glue.svg?color=blue)](https://pypi.org/project/types-aiobotocore-glue)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-glue)](https://pepy.tech/project/types-aiobotocore-glue)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Glue 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
+[aiobotocore.Glue 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
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
 [types-aiobotocore-glue docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-glue-2.9.0/README.md` & `types-aiobotocore-glue-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-glue.svg?color=blue)](https://pypi.org/project/types-aiobotocore-glue)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-glue)](https://pepy.tech/project/types-aiobotocore-glue)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Glue 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
+[aiobotocore.Glue 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
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
 [types-aiobotocore-glue docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-glue-2.9.0/setup.py` & `types-aiobotocore-glue-2.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-glue",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_glue"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Glue 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.Glue 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore glue type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_glue": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-glue-2.9.0/types_aiobotocore_glue/__init__.py` & `types-aiobotocore-glue-2.9.1/types_aiobotocore_glue/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,14 @@
     ListRegistriesPaginator,
     ListSchemasPaginator,
     ListSchemaVersionsPaginator,
 )
 
 Client = GlueClient
 
-
 __all__ = (
     "Client",
     "GetClassifiersPaginator",
     "GetConnectionsPaginator",
     "GetCrawlerMetricsPaginator",
     "GetCrawlersPaginator",
     "GetDatabasesPaginator",
```

### Comparing `types-aiobotocore-glue-2.9.0/types_aiobotocore_glue/__init__.pyi` & `types-aiobotocore-glue-2.9.1/types_aiobotocore_glue/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glue-2.9.0/types_aiobotocore_glue/__main__.py` & `types-aiobotocore-glue-2.9.1/types_aiobotocore_glue/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Glue 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Glue 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue\nOther"
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

### Comparing `types-aiobotocore-glue-2.9.0/types_aiobotocore_glue/client.py` & `types-aiobotocore-glue-2.9.1/types_aiobotocore_glue/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -294,15 +294,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("GlueClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -368,15 +367,15 @@
 
     async def batch_create_partition(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         PartitionInputList: Sequence[PartitionInputTypeDef],
-        CatalogId: str = ...
+        CatalogId: str = ...,
     ) -> BatchCreatePartitionResponseTypeDef:
         """
         Creates one or more partitions in a batch operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.batch_create_partition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#batch_create_partition)
         """
@@ -393,30 +392,30 @@
 
     async def batch_delete_partition(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         PartitionsToDelete: Sequence[PartitionValueListTypeDef],
-        CatalogId: str = ...
+        CatalogId: str = ...,
     ) -> BatchDeletePartitionResponseTypeDef:
         """
         Deletes one or more partitions in a batch operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.batch_delete_partition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#batch_delete_partition)
         """
 
     async def batch_delete_table(
         self,
         *,
         DatabaseName: str,
         TablesToDelete: Sequence[str],
         CatalogId: str = ...,
-        TransactionId: str = ...
+        TransactionId: str = ...,
     ) -> BatchDeleteTableResponseTypeDef:
         """
         Deletes multiple tables at once.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.batch_delete_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#batch_delete_table)
         """
@@ -432,15 +431,15 @@
         """
 
     async def batch_get_blueprints(
         self,
         *,
         Names: Sequence[str],
         IncludeBlueprint: bool = ...,
-        IncludeParameterSpec: bool = ...
+        IncludeParameterSpec: bool = ...,
     ) -> BatchGetBlueprintsResponseTypeDef:
         """
         Retrieves information about a list of blueprints.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.batch_get_blueprints)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#batch_get_blueprints)
         """
@@ -496,15 +495,15 @@
 
     async def batch_get_partition(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         PartitionsToGet: Sequence[PartitionValueListTypeDef],
-        CatalogId: str = ...
+        CatalogId: str = ...,
     ) -> BatchGetPartitionResponseTypeDef:
         """
         Retrieves partitions in a batch request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.batch_get_partition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#batch_get_partition)
         """
@@ -551,15 +550,15 @@
 
     async def batch_update_partition(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         Entries: Sequence[BatchUpdatePartitionRequestEntryTypeDef],
-        CatalogId: str = ...
+        CatalogId: str = ...,
     ) -> BatchUpdatePartitionResponseTypeDef:
         """
         Updates one or more partitions in a batch operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.batch_update_partition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#batch_update_partition)
         """
@@ -628,44 +627,44 @@
 
     async def create_blueprint(
         self,
         *,
         Name: str,
         BlueprintLocation: str,
         Description: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateBlueprintResponseTypeDef:
         """
         Registers a blueprint with Glue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_blueprint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#create_blueprint)
         """
 
     async def create_classifier(
         self,
         *,
         GrokClassifier: CreateGrokClassifierRequestTypeDef = ...,
         XMLClassifier: CreateXMLClassifierRequestTypeDef = ...,
         JsonClassifier: CreateJsonClassifierRequestTypeDef = ...,
-        CsvClassifier: CreateCsvClassifierRequestTypeDef = ...
+        CsvClassifier: CreateCsvClassifierRequestTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Creates a classifier in the user's account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_classifier)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#create_classifier)
         """
 
     async def create_connection(
         self,
         *,
         ConnectionInput: ConnectionInputTypeDef,
         CatalogId: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> Dict[str, Any]:
         """
         Creates a connection definition in the Data Catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#create_connection)
         """
@@ -683,15 +682,15 @@
         TablePrefix: str = ...,
         SchemaChangePolicy: SchemaChangePolicyTypeDef = ...,
         RecrawlPolicy: RecrawlPolicyTypeDef = ...,
         LineageConfiguration: LineageConfigurationTypeDef = ...,
         LakeFormationConfiguration: LakeFormationConfigurationTypeDef = ...,
         Configuration: str = ...,
         CrawlerSecurityConfiguration: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> Dict[str, Any]:
         """
         Creates a new crawler with specified targets, role, configuration, and optional
         schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_crawler)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#create_crawler)
@@ -699,15 +698,15 @@
 
     async def create_custom_entity_type(
         self,
         *,
         Name: str,
         RegexString: str,
         ContextWords: Sequence[str] = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateCustomEntityTypeResponseTypeDef:
         """
         Creates a custom pattern that is used to detect sensitive data across the
         columns and rows of your structured
         data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_custom_entity_type)
@@ -718,30 +717,30 @@
         self,
         *,
         Name: str,
         Ruleset: str,
         Description: str = ...,
         Tags: Mapping[str, str] = ...,
         TargetTable: DataQualityTargetTableTypeDef = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreateDataQualityRulesetResponseTypeDef:
         """
         Creates a data quality ruleset with DQDL rules applied to a specified Glue
         table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_data_quality_ruleset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#create_data_quality_ruleset)
         """
 
     async def create_database(
         self,
         *,
         DatabaseInput: DatabaseInputTypeDef,
         CatalogId: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> Dict[str, Any]:
         """
         Creates a new database in a Data Catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_database)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#create_database)
         """
@@ -759,15 +758,15 @@
         WorkerType: WorkerTypeType = ...,
         GlueVersion: str = ...,
         NumberOfWorkers: int = ...,
         ExtraPythonLibsS3Path: str = ...,
         ExtraJarsS3Path: str = ...,
         SecurityConfiguration: str = ...,
         Tags: Mapping[str, str] = ...,
-        Arguments: Mapping[str, str] = ...
+        Arguments: Mapping[str, str] = ...,
     ) -> CreateDevEndpointResponseTypeDef:
         """
         Creates a new development endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_dev_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#create_dev_endpoint)
         """
@@ -792,15 +791,15 @@
         Tags: Mapping[str, str] = ...,
         NotificationProperty: NotificationPropertyTypeDef = ...,
         GlueVersion: str = ...,
         NumberOfWorkers: int = ...,
         WorkerType: WorkerTypeType = ...,
         CodeGenConfigurationNodes: Mapping[str, CodeGenConfigurationNodeTypeDef] = ...,
         ExecutionClass: ExecutionClassType = ...,
-        SourceControlDetails: SourceControlDetailsTypeDef = ...
+        SourceControlDetails: SourceControlDetailsTypeDef = ...,
     ) -> CreateJobResponseTypeDef:
         """
         Creates a new job definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#create_job)
         """
@@ -816,45 +815,45 @@
         GlueVersion: str = ...,
         MaxCapacity: float = ...,
         WorkerType: WorkerTypeType = ...,
         NumberOfWorkers: int = ...,
         Timeout: int = ...,
         MaxRetries: int = ...,
         Tags: Mapping[str, str] = ...,
-        TransformEncryption: TransformEncryptionTypeDef = ...
+        TransformEncryption: TransformEncryptionTypeDef = ...,
     ) -> CreateMLTransformResponseTypeDef:
         """
         Creates an Glue machine learning transform.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_ml_transform)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#create_ml_transform)
         """
 
     async def create_partition(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         PartitionInput: PartitionInputTypeDef,
-        CatalogId: str = ...
+        CatalogId: str = ...,
     ) -> Dict[str, Any]:
         """
         Creates a new partition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_partition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#create_partition)
         """
 
     async def create_partition_index(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         PartitionIndex: PartitionIndexTypeDef,
-        CatalogId: str = ...
+        CatalogId: str = ...,
     ) -> Dict[str, Any]:
         """
         Creates a specified partition index in an existing table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_partition_index)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#create_partition_index)
         """
@@ -874,29 +873,29 @@
         *,
         SchemaName: str,
         DataFormat: DataFormatType,
         RegistryId: RegistryIdTypeDef = ...,
         Compatibility: CompatibilityType = ...,
         Description: str = ...,
         Tags: Mapping[str, str] = ...,
-        SchemaDefinition: str = ...
+        SchemaDefinition: str = ...,
     ) -> CreateSchemaResponseTypeDef:
         """
         Creates a new schema set and registers the schema definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_schema)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#create_schema)
         """
 
     async def create_script(
         self,
         *,
         DagNodes: Sequence[CodeGenNodeTypeDef] = ...,
         DagEdges: Sequence[CodeGenEdgeTypeDef] = ...,
-        Language: LanguageType = ...
+        Language: LanguageType = ...,
     ) -> CreateScriptResponseTypeDef:
         """
         Transforms a directed acyclic graph (DAG) into code.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_script)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#create_script)
         """
@@ -924,15 +923,15 @@
         Connections: ConnectionsListTypeDef = ...,
         MaxCapacity: float = ...,
         NumberOfWorkers: int = ...,
         WorkerType: WorkerTypeType = ...,
         SecurityConfiguration: str = ...,
         GlueVersion: str = ...,
         Tags: Mapping[str, str] = ...,
-        RequestOrigin: str = ...
+        RequestOrigin: str = ...,
     ) -> CreateSessionResponseTypeDef:
         """
         Creates a new session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_session)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#create_session)
         """
@@ -941,15 +940,15 @@
         self,
         *,
         DatabaseName: str,
         TableInput: TableInputTypeDef,
         CatalogId: str = ...,
         PartitionIndexes: Sequence[PartitionIndexTypeDef] = ...,
         TransactionId: str = ...,
-        OpenTableFormatInput: OpenTableFormatInputTypeDef = ...
+        OpenTableFormatInput: OpenTableFormatInputTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Creates a new table definition in the Data Catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#create_table)
         """
@@ -957,15 +956,15 @@
     async def create_table_optimizer(
         self,
         *,
         CatalogId: str,
         DatabaseName: str,
         TableName: str,
         Type: Literal["compaction"],
-        TableOptimizerConfiguration: TableOptimizerConfigurationTypeDef
+        TableOptimizerConfiguration: TableOptimizerConfigurationTypeDef,
     ) -> Dict[str, Any]:
         """
         Creates a new table optimizer for a specific function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_table_optimizer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#create_table_optimizer)
         """
@@ -978,29 +977,29 @@
         Actions: Sequence[ActionTypeDef],
         WorkflowName: str = ...,
         Schedule: str = ...,
         Predicate: PredicateTypeDef = ...,
         Description: str = ...,
         StartOnCreation: bool = ...,
         Tags: Mapping[str, str] = ...,
-        EventBatchingCondition: EventBatchingConditionTypeDef = ...
+        EventBatchingCondition: EventBatchingConditionTypeDef = ...,
     ) -> CreateTriggerResponseTypeDef:
         """
         Creates a new trigger.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_trigger)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#create_trigger)
         """
 
     async def create_user_defined_function(
         self,
         *,
         DatabaseName: str,
         FunctionInput: UserDefinedFunctionInputTypeDef,
-        CatalogId: str = ...
+        CatalogId: str = ...,
     ) -> Dict[str, Any]:
         """
         Creates a new function definition in the Data Catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_user_defined_function)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#create_user_defined_function)
         """
@@ -1008,15 +1007,15 @@
     async def create_workflow(
         self,
         *,
         Name: str,
         Description: str = ...,
         DefaultRunProperties: Mapping[str, str] = ...,
         Tags: Mapping[str, str] = ...,
-        MaxConcurrentRuns: int = ...
+        MaxConcurrentRuns: int = ...,
     ) -> CreateWorkflowResponseTypeDef:
         """
         Creates a new workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_workflow)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#create_workflow)
         """
@@ -1040,15 +1039,15 @@
     async def delete_column_statistics_for_partition(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         PartitionValues: Sequence[str],
         ColumnName: str,
-        CatalogId: str = ...
+        CatalogId: str = ...,
     ) -> Dict[str, Any]:
         """
         Delete the partition column statistics of a column.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.delete_column_statistics_for_partition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#delete_column_statistics_for_partition)
         """
@@ -1135,15 +1134,15 @@
 
     async def delete_partition(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         PartitionValues: Sequence[str],
-        CatalogId: str = ...
+        CatalogId: str = ...,
     ) -> Dict[str, Any]:
         """
         Deletes a specified partition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.delete_partition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#delete_partition)
         """
@@ -1345,15 +1344,15 @@
     async def get_column_statistics_for_partition(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         PartitionValues: Sequence[str],
         ColumnNames: Sequence[str],
-        CatalogId: str = ...
+        CatalogId: str = ...,
     ) -> GetColumnStatisticsForPartitionResponseTypeDef:
         """
         Retrieves partition statistics of columns.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_column_statistics_for_partition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#get_column_statistics_for_partition)
         """
@@ -1401,15 +1400,15 @@
     async def get_connections(
         self,
         *,
         CatalogId: str = ...,
         Filter: GetConnectionsFilterTypeDef = ...,
         HidePassword: bool = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> GetConnectionsResponseTypeDef:
         """
         Retrieves a list of connection definitions from the Data Catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_connections)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#get_connections)
         """
@@ -1508,15 +1507,15 @@
 
     async def get_databases(
         self,
         *,
         CatalogId: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        ResourceShareType: ResourceShareTypeType = ...
+        ResourceShareType: ResourceShareTypeType = ...,
     ) -> GetDatabasesResponseTypeDef:
         """
         Retrieves all databases defined in a given Data Catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_databases)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#get_databases)
         """
@@ -1598,15 +1597,15 @@
         """
 
     async def get_mapping(
         self,
         *,
         Source: CatalogEntryTypeDef,
         Sinks: Sequence[CatalogEntryTypeDef] = ...,
-        Location: LocationTypeDef = ...
+        Location: LocationTypeDef = ...,
     ) -> GetMappingResponseTypeDef:
         """
         Creates mappings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_mapping)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#get_mapping)
         """
@@ -1624,15 +1623,15 @@
     async def get_ml_task_runs(
         self,
         *,
         TransformId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         Filter: TaskRunFilterCriteriaTypeDef = ...,
-        Sort: TaskRunSortCriteriaTypeDef = ...
+        Sort: TaskRunSortCriteriaTypeDef = ...,
     ) -> GetMLTaskRunsResponseTypeDef:
         """
         Gets a list of runs for a machine learning transform.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_ml_task_runs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#get_ml_task_runs)
         """
@@ -1648,30 +1647,30 @@
 
     async def get_ml_transforms(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         Filter: TransformFilterCriteriaTypeDef = ...,
-        Sort: TransformSortCriteriaTypeDef = ...
+        Sort: TransformSortCriteriaTypeDef = ...,
     ) -> GetMLTransformsResponseTypeDef:
         """
         Gets a sortable, filterable list of existing Glue machine learning transforms.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_ml_transforms)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#get_ml_transforms)
         """
 
     async def get_partition(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         PartitionValues: Sequence[str],
-        CatalogId: str = ...
+        CatalogId: str = ...,
     ) -> GetPartitionResponseTypeDef:
         """
         Retrieves information about a specified partition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_partition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#get_partition)
         """
@@ -1694,15 +1693,15 @@
         CatalogId: str = ...,
         Expression: str = ...,
         NextToken: str = ...,
         Segment: SegmentTypeDef = ...,
         MaxResults: int = ...,
         ExcludeColumnSchema: bool = ...,
         TransactionId: str = ...,
-        QueryAsOfTime: TimestampTypeDef = ...
+        QueryAsOfTime: TimestampTypeDef = ...,
     ) -> GetPartitionsResponseTypeDef:
         """
         Retrieves information about the partitions in a table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_partitions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#get_partitions)
         """
@@ -1711,15 +1710,15 @@
         self,
         *,
         Mapping: Sequence[MappingEntryTypeDef],
         Source: CatalogEntryTypeDef,
         Sinks: Sequence[CatalogEntryTypeDef] = ...,
         Location: LocationTypeDef = ...,
         Language: LanguageType = ...,
-        AdditionalPlanOptionsMap: Mapping[str, str] = ...
+        AdditionalPlanOptionsMap: Mapping[str, str] = ...,
     ) -> GetPlanResponseTypeDef:
         """
         Gets code to perform a specified mapping.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_plan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#get_plan)
         """
@@ -1773,15 +1772,15 @@
         """
 
     async def get_schema_version(
         self,
         *,
         SchemaId: SchemaIdTypeDef = ...,
         SchemaVersionId: str = ...,
-        SchemaVersionNumber: SchemaVersionNumberTypeDef = ...
+        SchemaVersionNumber: SchemaVersionNumberTypeDef = ...,
     ) -> GetSchemaVersionResponseTypeDef:
         """
         Get the specified schema by its unique ID assigned when a version of the schema
         is created or
         registered.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_schema_version)
@@ -1790,15 +1789,15 @@
 
     async def get_schema_versions_diff(
         self,
         *,
         SchemaId: SchemaIdTypeDef,
         FirstSchemaVersionNumber: SchemaVersionNumberTypeDef,
         SecondSchemaVersionNumber: SchemaVersionNumberTypeDef,
-        SchemaDiffType: Literal["SYNTAX_DIFF"]
+        SchemaDiffType: Literal["SYNTAX_DIFF"],
     ) -> GetSchemaVersionsDiffResponseTypeDef:
         """
         Fetches the schema version difference in the specified difference type between
         two stored schema versions in the Schema
         Registry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_schema_versions_diff)
@@ -1846,15 +1845,15 @@
     async def get_table(
         self,
         *,
         DatabaseName: str,
         Name: str,
         CatalogId: str = ...,
         TransactionId: str = ...,
-        QueryAsOfTime: TimestampTypeDef = ...
+        QueryAsOfTime: TimestampTypeDef = ...,
     ) -> GetTableResponseTypeDef:
         """
         Retrieves the `Table` definition in a Data Catalog for a specified table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#get_table)
         """
@@ -1882,15 +1881,15 @@
     async def get_table_versions(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         CatalogId: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> GetTableVersionsResponseTypeDef:
         """
         Retrieves a list of strings that identify available versions of a specified
         table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_table_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#get_table_versions)
@@ -1901,15 +1900,15 @@
         *,
         DatabaseName: str,
         CatalogId: str = ...,
         Expression: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         TransactionId: str = ...,
-        QueryAsOfTime: TimestampTypeDef = ...
+        QueryAsOfTime: TimestampTypeDef = ...,
     ) -> GetTablesResponseTypeDef:
         """
         Retrieves the definitions of some or all of the tables in a given `Database`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_tables)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#get_tables)
         """
@@ -1944,15 +1943,15 @@
         self,
         *,
         CatalogId: str,
         DatabaseName: str,
         TableName: str,
         PartitionValues: Sequence[str],
         SupportedPermissionTypes: Sequence[PermissionTypeType],
-        AuditContext: AuditContextTypeDef = ...
+        AuditContext: AuditContextTypeDef = ...,
     ) -> GetUnfilteredPartitionMetadataResponseTypeDef:
         """
         Retrieves partition metadata from the Data Catalog that contains unfiltered
         metadata.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_unfiltered_partition_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#get_unfiltered_partition_metadata)
@@ -1965,15 +1964,15 @@
         DatabaseName: str,
         TableName: str,
         SupportedPermissionTypes: Sequence[PermissionTypeType],
         Expression: str = ...,
         AuditContext: AuditContextTypeDef = ...,
         NextToken: str = ...,
         Segment: SegmentTypeDef = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> GetUnfilteredPartitionsMetadataResponseTypeDef:
         """
         Retrieves partition metadata from the Data Catalog that contains unfiltered
         metadata.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_unfiltered_partitions_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#get_unfiltered_partitions_metadata)
@@ -1982,15 +1981,15 @@
     async def get_unfiltered_table_metadata(
         self,
         *,
         CatalogId: str,
         DatabaseName: str,
         Name: str,
         SupportedPermissionTypes: Sequence[PermissionTypeType],
-        AuditContext: AuditContextTypeDef = ...
+        AuditContext: AuditContextTypeDef = ...,
     ) -> GetUnfilteredTableMetadataResponseTypeDef:
         """
         Retrieves table metadata from the Data Catalog that contains unfiltered
         metadata.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_unfiltered_table_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#get_unfiltered_table_metadata)
@@ -2009,15 +2008,15 @@
     async def get_user_defined_functions(
         self,
         *,
         Pattern: str,
         CatalogId: str = ...,
         DatabaseName: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> GetUserDefinedFunctionsResponseTypeDef:
         """
         Retrieves multiple function definitions from the Data Catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_user_defined_functions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#get_user_defined_functions)
         """
@@ -2104,15 +2103,15 @@
 
     async def list_crawls(
         self,
         *,
         CrawlerName: str,
         MaxResults: int = ...,
         Filters: Sequence[CrawlsFilterTypeDef] = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListCrawlsResponseTypeDef:
         """
         Returns all the crawls of a specified crawler.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.list_crawls)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#list_crawls)
         """
@@ -2128,43 +2127,43 @@
         """
 
     async def list_data_quality_results(
         self,
         *,
         Filter: DataQualityResultFilterCriteriaTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListDataQualityResultsResponseTypeDef:
         """
         Returns all data quality execution results for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.list_data_quality_results)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#list_data_quality_results)
         """
 
     async def list_data_quality_rule_recommendation_runs(
         self,
         *,
         Filter: DataQualityRuleRecommendationRunFilterTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListDataQualityRuleRecommendationRunsResponseTypeDef:
         """
         Lists the recommendation runs meeting the filter criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.list_data_quality_rule_recommendation_runs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#list_data_quality_rule_recommendation_runs)
         """
 
     async def list_data_quality_ruleset_evaluation_runs(
         self,
         *,
         Filter: DataQualityRulesetEvaluationRunFilterTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListDataQualityRulesetEvaluationRunsResponseTypeDef:
         """
         Lists all the runs meeting the filter criteria, where a ruleset is evaluated
         against a data
         source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.list_data_quality_ruleset_evaluation_runs)
@@ -2173,15 +2172,15 @@
 
     async def list_data_quality_rulesets(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         Filter: DataQualityRulesetFilterCriteriaTypeDef = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> ListDataQualityRulesetsResponseTypeDef:
         """
         Returns a paginated list of rulesets for the specified list of Glue tables.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.list_data_quality_rulesets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#list_data_quality_rulesets)
         """
@@ -2213,15 +2212,15 @@
     async def list_ml_transforms(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         Filter: TransformFilterCriteriaTypeDef = ...,
         Sort: TransformSortCriteriaTypeDef = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> ListMLTransformsResponseTypeDef:
         """
         Retrieves a sortable, filterable list of existing Glue machine learning
         transforms in this Amazon Web Services account, or the resources with the
         specified
         tag.
 
@@ -2263,15 +2262,15 @@
 
     async def list_sessions(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         Tags: Mapping[str, str] = ...,
-        RequestOrigin: str = ...
+        RequestOrigin: str = ...,
     ) -> ListSessionsResponseTypeDef:
         """
         Retrieve a list of sessions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.list_sessions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#list_sessions)
         """
@@ -2290,30 +2289,30 @@
         self,
         *,
         CatalogId: str,
         DatabaseName: str,
         TableName: str,
         Type: Literal["compaction"],
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListTableOptimizerRunsResponseTypeDef:
         """
         Lists the history of previous optimizer runs for a specific table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.list_table_optimizer_runs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#list_table_optimizer_runs)
         """
 
     async def list_triggers(
         self,
         *,
         NextToken: str = ...,
         DependentJobName: str = ...,
         MaxResults: int = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> ListTriggersResponseTypeDef:
         """
         Retrieves the names of all trigger resources in this Amazon Web Services
         account, or the resources with the specified
         tag.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.list_triggers)
@@ -2330,15 +2329,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#list_workflows)
         """
 
     async def put_data_catalog_encryption_settings(
         self,
         *,
         DataCatalogEncryptionSettings: DataCatalogEncryptionSettingsTypeDef,
-        CatalogId: str = ...
+        CatalogId: str = ...,
     ) -> Dict[str, Any]:
         """
         Sets the security configuration for a specified catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.put_data_catalog_encryption_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#put_data_catalog_encryption_settings)
         """
@@ -2346,30 +2345,30 @@
     async def put_resource_policy(
         self,
         *,
         PolicyInJson: str,
         ResourceArn: str = ...,
         PolicyHashCondition: str = ...,
         PolicyExistsCondition: ExistConditionType = ...,
-        EnableHybrid: EnableHybridValuesType = ...
+        EnableHybrid: EnableHybridValuesType = ...,
     ) -> PutResourcePolicyResponseTypeDef:
         """
         Sets the Data Catalog resource policy for access control.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.put_resource_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#put_resource_policy)
         """
 
     async def put_schema_version_metadata(
         self,
         *,
         MetadataKeyValue: MetadataKeyValuePairTypeDef,
         SchemaId: SchemaIdTypeDef = ...,
         SchemaVersionNumber: SchemaVersionNumberTypeDef = ...,
-        SchemaVersionId: str = ...
+        SchemaVersionId: str = ...,
     ) -> PutSchemaVersionMetadataResponseTypeDef:
         """
         Puts the metadata key value pair for a specified schema version ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.put_schema_version_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#put_schema_version_metadata)
         """
@@ -2388,15 +2387,15 @@
         self,
         *,
         SchemaId: SchemaIdTypeDef = ...,
         SchemaVersionNumber: SchemaVersionNumberTypeDef = ...,
         SchemaVersionId: str = ...,
         MetadataList: Sequence[MetadataKeyValuePairTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> QuerySchemaVersionMetadataResponseTypeDef:
         """
         Queries for the schema version metadata information.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.query_schema_version_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#query_schema_version_metadata)
         """
@@ -2413,15 +2412,15 @@
 
     async def remove_schema_version_metadata(
         self,
         *,
         MetadataKeyValue: MetadataKeyValuePairTypeDef,
         SchemaId: SchemaIdTypeDef = ...,
         SchemaVersionNumber: SchemaVersionNumberTypeDef = ...,
-        SchemaVersionId: str = ...
+        SchemaVersionId: str = ...,
     ) -> RemoveSchemaVersionMetadataResponseTypeDef:
         """
         Removes a key value pair from the schema version metadata for the specified
         schema version
         ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.remove_schema_version_metadata)
@@ -2465,15 +2464,15 @@
         *,
         CatalogId: str = ...,
         NextToken: str = ...,
         Filters: Sequence[PropertyPredicateTypeDef] = ...,
         SearchText: str = ...,
         SortCriteria: Sequence[SortCriterionTypeDef] = ...,
         MaxResults: int = ...,
-        ResourceShareType: ResourceShareTypeType = ...
+        ResourceShareType: ResourceShareTypeType = ...,
     ) -> SearchTablesResponseTypeDef:
         """
         Searches a set of tables based on properties in the table metadata as well as
         on the parent
         database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.search_tables)
@@ -2495,15 +2494,15 @@
         *,
         DatabaseName: str,
         TableName: str,
         Role: str,
         ColumnNameList: Sequence[str] = ...,
         SampleSize: float = ...,
         CatalogID: str = ...,
-        SecurityConfiguration: str = ...
+        SecurityConfiguration: str = ...,
     ) -> StartColumnStatisticsTaskRunResponseTypeDef:
         """
         Starts a column statistics task run, for a specified table and columns.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.start_column_statistics_task_run)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#start_column_statistics_task_run)
         """
@@ -2530,15 +2529,15 @@
         self,
         *,
         DataSource: DataSourceTypeDef,
         Role: str,
         NumberOfWorkers: int = ...,
         Timeout: int = ...,
         CreatedRulesetName: str = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> StartDataQualityRuleRecommendationRunResponseTypeDef:
         """
         Starts a recommendation run that is used to generate rules when you don't know
         what rules to
         write.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.start_data_quality_rule_recommendation_run)
@@ -2551,15 +2550,15 @@
         DataSource: DataSourceTypeDef,
         Role: str,
         RulesetNames: Sequence[str],
         NumberOfWorkers: int = ...,
         Timeout: int = ...,
         ClientToken: str = ...,
         AdditionalRunOptions: DataQualityEvaluationRunAdditionalRunOptionsTypeDef = ...,
-        AdditionalDataSources: Mapping[str, DataSourceTypeDef] = ...
+        AdditionalDataSources: Mapping[str, DataSourceTypeDef] = ...,
     ) -> StartDataQualityRulesetEvaluationRunResponseTypeDef:
         """
         Once you have a ruleset definition (either recommended or your own), you call
         this operation to evaluate the ruleset against a data source (Glue
         table).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.start_data_quality_ruleset_evaluation_run)
@@ -2598,15 +2597,15 @@
         AllocatedCapacity: int = ...,
         Timeout: int = ...,
         MaxCapacity: float = ...,
         SecurityConfiguration: str = ...,
         NotificationProperty: NotificationPropertyTypeDef = ...,
         WorkerType: WorkerTypeType = ...,
         NumberOfWorkers: int = ...,
-        ExecutionClass: ExecutionClassType = ...
+        ExecutionClass: ExecutionClassType = ...,
     ) -> StartJobRunResponseTypeDef:
         """
         Starts a job run using a job definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.start_job_run)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#start_job_run)
         """
@@ -2737,15 +2736,15 @@
 
     async def update_classifier(
         self,
         *,
         GrokClassifier: UpdateGrokClassifierRequestTypeDef = ...,
         XMLClassifier: UpdateXMLClassifierRequestTypeDef = ...,
         JsonClassifier: UpdateJsonClassifierRequestTypeDef = ...,
-        CsvClassifier: UpdateCsvClassifierRequestTypeDef = ...
+        CsvClassifier: UpdateCsvClassifierRequestTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Modifies an existing classifier (a `GrokClassifier`, an `XMLClassifier`, a
         `JsonClassifier`, or a `CsvClassifier`, depending on which field is
         present).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.update_classifier)
@@ -2755,30 +2754,30 @@
     async def update_column_statistics_for_partition(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         PartitionValues: Sequence[str],
         ColumnStatisticsList: Sequence[ColumnStatisticsTypeDef],
-        CatalogId: str = ...
+        CatalogId: str = ...,
     ) -> UpdateColumnStatisticsForPartitionResponseTypeDef:
         """
         Creates or updates partition statistics of columns.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.update_column_statistics_for_partition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#update_column_statistics_for_partition)
         """
 
     async def update_column_statistics_for_table(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         ColumnStatisticsList: Sequence[ColumnStatisticsTypeDef],
-        CatalogId: str = ...
+        CatalogId: str = ...,
     ) -> UpdateColumnStatisticsForTableResponseTypeDef:
         """
         Creates or updates table statistics of columns.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.update_column_statistics_for_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#update_column_statistics_for_table)
         """
@@ -2805,15 +2804,15 @@
         Classifiers: Sequence[str] = ...,
         TablePrefix: str = ...,
         SchemaChangePolicy: SchemaChangePolicyTypeDef = ...,
         RecrawlPolicy: RecrawlPolicyTypeDef = ...,
         LineageConfiguration: LineageConfigurationTypeDef = ...,
         LakeFormationConfiguration: LakeFormationConfigurationTypeDef = ...,
         Configuration: str = ...,
-        CrawlerSecurityConfiguration: str = ...
+        CrawlerSecurityConfiguration: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates a crawler.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.update_crawler)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#update_crawler)
         """
@@ -2854,15 +2853,15 @@
         EndpointName: str,
         PublicKey: str = ...,
         AddPublicKeys: Sequence[str] = ...,
         DeletePublicKeys: Sequence[str] = ...,
         CustomLibraries: DevEndpointCustomLibrariesTypeDef = ...,
         UpdateEtlLibraries: bool = ...,
         DeleteArguments: Sequence[str] = ...,
-        AddArguments: Mapping[str, str] = ...
+        AddArguments: Mapping[str, str] = ...,
     ) -> Dict[str, Any]:
         """
         Updates a specified development endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.update_dev_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#update_dev_endpoint)
         """
@@ -2884,15 +2883,15 @@
         Provider: SourceControlProviderType = ...,
         RepositoryName: str = ...,
         RepositoryOwner: str = ...,
         BranchName: str = ...,
         Folder: str = ...,
         CommitId: str = ...,
         AuthStrategy: SourceControlAuthStrategyType = ...,
-        AuthToken: str = ...
+        AuthToken: str = ...,
     ) -> UpdateJobFromSourceControlResponseTypeDef:
         """
         Synchronizes a job from the source control repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.update_job_from_source_control)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#update_job_from_source_control)
         """
@@ -2906,15 +2905,15 @@
         Parameters: TransformParametersTypeDef = ...,
         Role: str = ...,
         GlueVersion: str = ...,
         MaxCapacity: float = ...,
         WorkerType: WorkerTypeType = ...,
         NumberOfWorkers: int = ...,
         Timeout: int = ...,
-        MaxRetries: int = ...
+        MaxRetries: int = ...,
     ) -> UpdateMLTransformResponseTypeDef:
         """
         Updates an existing machine learning transform.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.update_ml_transform)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#update_ml_transform)
         """
@@ -2922,15 +2921,15 @@
     async def update_partition(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         PartitionValueList: Sequence[str],
         PartitionInput: PartitionInputTypeDef,
-        CatalogId: str = ...
+        CatalogId: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates a partition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.update_partition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#update_partition)
         """
@@ -2947,15 +2946,15 @@
 
     async def update_schema(
         self,
         *,
         SchemaId: SchemaIdTypeDef,
         SchemaVersionNumber: SchemaVersionNumberTypeDef = ...,
         Compatibility: CompatibilityType = ...,
-        Description: str = ...
+        Description: str = ...,
     ) -> UpdateSchemaResponseTypeDef:
         """
         Updates the description, compatibility setting, or version checkpoint for a
         schema
         set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.update_schema)
@@ -2969,15 +2968,15 @@
         Provider: SourceControlProviderType = ...,
         RepositoryName: str = ...,
         RepositoryOwner: str = ...,
         BranchName: str = ...,
         Folder: str = ...,
         CommitId: str = ...,
         AuthStrategy: SourceControlAuthStrategyType = ...,
-        AuthToken: str = ...
+        AuthToken: str = ...,
     ) -> UpdateSourceControlFromJobResponseTypeDef:
         """
         Synchronizes a job to the source control repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.update_source_control_from_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#update_source_control_from_job)
         """
@@ -2986,15 +2985,15 @@
         self,
         *,
         DatabaseName: str,
         TableInput: TableInputTypeDef,
         CatalogId: str = ...,
         SkipArchive: bool = ...,
         TransactionId: str = ...,
-        VersionId: str = ...
+        VersionId: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates a metadata table in the Data Catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.update_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#update_table)
         """
@@ -3002,15 +3001,15 @@
     async def update_table_optimizer(
         self,
         *,
         CatalogId: str,
         DatabaseName: str,
         TableName: str,
         Type: Literal["compaction"],
-        TableOptimizerConfiguration: TableOptimizerConfigurationTypeDef
+        TableOptimizerConfiguration: TableOptimizerConfigurationTypeDef,
     ) -> Dict[str, Any]:
         """
         Updates the configuration for an existing table optimizer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.update_table_optimizer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#update_table_optimizer)
         """
@@ -3027,30 +3026,30 @@
 
     async def update_user_defined_function(
         self,
         *,
         DatabaseName: str,
         FunctionName: str,
         FunctionInput: UserDefinedFunctionInputTypeDef,
-        CatalogId: str = ...
+        CatalogId: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates an existing function definition in the Data Catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.update_user_defined_function)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#update_user_defined_function)
         """
 
     async def update_workflow(
         self,
         *,
         Name: str,
         Description: str = ...,
         DefaultRunProperties: Mapping[str, str] = ...,
-        MaxConcurrentRuns: int = ...
+        MaxConcurrentRuns: int = ...,
     ) -> UpdateWorkflowResponseTypeDef:
         """
         Updates an existing workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.update_workflow)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#update_workflow)
         """
```

### Comparing `types-aiobotocore-glue-2.9.0/types_aiobotocore_glue/client.pyi` & `types-aiobotocore-glue-2.9.1/types_aiobotocore_glue/client.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -364,15 +364,15 @@
 
     async def batch_create_partition(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         PartitionInputList: Sequence[PartitionInputTypeDef],
-        CatalogId: str = ...
+        CatalogId: str = ...,
     ) -> BatchCreatePartitionResponseTypeDef:
         """
         Creates one or more partitions in a batch operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.batch_create_partition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#batch_create_partition)
         """
@@ -389,30 +389,30 @@
 
     async def batch_delete_partition(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         PartitionsToDelete: Sequence[PartitionValueListTypeDef],
-        CatalogId: str = ...
+        CatalogId: str = ...,
     ) -> BatchDeletePartitionResponseTypeDef:
         """
         Deletes one or more partitions in a batch operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.batch_delete_partition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#batch_delete_partition)
         """
 
     async def batch_delete_table(
         self,
         *,
         DatabaseName: str,
         TablesToDelete: Sequence[str],
         CatalogId: str = ...,
-        TransactionId: str = ...
+        TransactionId: str = ...,
     ) -> BatchDeleteTableResponseTypeDef:
         """
         Deletes multiple tables at once.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.batch_delete_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#batch_delete_table)
         """
@@ -428,15 +428,15 @@
         """
 
     async def batch_get_blueprints(
         self,
         *,
         Names: Sequence[str],
         IncludeBlueprint: bool = ...,
-        IncludeParameterSpec: bool = ...
+        IncludeParameterSpec: bool = ...,
     ) -> BatchGetBlueprintsResponseTypeDef:
         """
         Retrieves information about a list of blueprints.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.batch_get_blueprints)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#batch_get_blueprints)
         """
@@ -492,15 +492,15 @@
 
     async def batch_get_partition(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         PartitionsToGet: Sequence[PartitionValueListTypeDef],
-        CatalogId: str = ...
+        CatalogId: str = ...,
     ) -> BatchGetPartitionResponseTypeDef:
         """
         Retrieves partitions in a batch request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.batch_get_partition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#batch_get_partition)
         """
@@ -547,15 +547,15 @@
 
     async def batch_update_partition(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         Entries: Sequence[BatchUpdatePartitionRequestEntryTypeDef],
-        CatalogId: str = ...
+        CatalogId: str = ...,
     ) -> BatchUpdatePartitionResponseTypeDef:
         """
         Updates one or more partitions in a batch operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.batch_update_partition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#batch_update_partition)
         """
@@ -624,44 +624,44 @@
 
     async def create_blueprint(
         self,
         *,
         Name: str,
         BlueprintLocation: str,
         Description: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateBlueprintResponseTypeDef:
         """
         Registers a blueprint with Glue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_blueprint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#create_blueprint)
         """
 
     async def create_classifier(
         self,
         *,
         GrokClassifier: CreateGrokClassifierRequestTypeDef = ...,
         XMLClassifier: CreateXMLClassifierRequestTypeDef = ...,
         JsonClassifier: CreateJsonClassifierRequestTypeDef = ...,
-        CsvClassifier: CreateCsvClassifierRequestTypeDef = ...
+        CsvClassifier: CreateCsvClassifierRequestTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Creates a classifier in the user's account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_classifier)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#create_classifier)
         """
 
     async def create_connection(
         self,
         *,
         ConnectionInput: ConnectionInputTypeDef,
         CatalogId: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> Dict[str, Any]:
         """
         Creates a connection definition in the Data Catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#create_connection)
         """
@@ -679,15 +679,15 @@
         TablePrefix: str = ...,
         SchemaChangePolicy: SchemaChangePolicyTypeDef = ...,
         RecrawlPolicy: RecrawlPolicyTypeDef = ...,
         LineageConfiguration: LineageConfigurationTypeDef = ...,
         LakeFormationConfiguration: LakeFormationConfigurationTypeDef = ...,
         Configuration: str = ...,
         CrawlerSecurityConfiguration: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> Dict[str, Any]:
         """
         Creates a new crawler with specified targets, role, configuration, and optional
         schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_crawler)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#create_crawler)
@@ -695,15 +695,15 @@
 
     async def create_custom_entity_type(
         self,
         *,
         Name: str,
         RegexString: str,
         ContextWords: Sequence[str] = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateCustomEntityTypeResponseTypeDef:
         """
         Creates a custom pattern that is used to detect sensitive data across the
         columns and rows of your structured
         data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_custom_entity_type)
@@ -714,30 +714,30 @@
         self,
         *,
         Name: str,
         Ruleset: str,
         Description: str = ...,
         Tags: Mapping[str, str] = ...,
         TargetTable: DataQualityTargetTableTypeDef = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreateDataQualityRulesetResponseTypeDef:
         """
         Creates a data quality ruleset with DQDL rules applied to a specified Glue
         table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_data_quality_ruleset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#create_data_quality_ruleset)
         """
 
     async def create_database(
         self,
         *,
         DatabaseInput: DatabaseInputTypeDef,
         CatalogId: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> Dict[str, Any]:
         """
         Creates a new database in a Data Catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_database)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#create_database)
         """
@@ -755,15 +755,15 @@
         WorkerType: WorkerTypeType = ...,
         GlueVersion: str = ...,
         NumberOfWorkers: int = ...,
         ExtraPythonLibsS3Path: str = ...,
         ExtraJarsS3Path: str = ...,
         SecurityConfiguration: str = ...,
         Tags: Mapping[str, str] = ...,
-        Arguments: Mapping[str, str] = ...
+        Arguments: Mapping[str, str] = ...,
     ) -> CreateDevEndpointResponseTypeDef:
         """
         Creates a new development endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_dev_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#create_dev_endpoint)
         """
@@ -788,15 +788,15 @@
         Tags: Mapping[str, str] = ...,
         NotificationProperty: NotificationPropertyTypeDef = ...,
         GlueVersion: str = ...,
         NumberOfWorkers: int = ...,
         WorkerType: WorkerTypeType = ...,
         CodeGenConfigurationNodes: Mapping[str, CodeGenConfigurationNodeTypeDef] = ...,
         ExecutionClass: ExecutionClassType = ...,
-        SourceControlDetails: SourceControlDetailsTypeDef = ...
+        SourceControlDetails: SourceControlDetailsTypeDef = ...,
     ) -> CreateJobResponseTypeDef:
         """
         Creates a new job definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#create_job)
         """
@@ -812,45 +812,45 @@
         GlueVersion: str = ...,
         MaxCapacity: float = ...,
         WorkerType: WorkerTypeType = ...,
         NumberOfWorkers: int = ...,
         Timeout: int = ...,
         MaxRetries: int = ...,
         Tags: Mapping[str, str] = ...,
-        TransformEncryption: TransformEncryptionTypeDef = ...
+        TransformEncryption: TransformEncryptionTypeDef = ...,
     ) -> CreateMLTransformResponseTypeDef:
         """
         Creates an Glue machine learning transform.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_ml_transform)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#create_ml_transform)
         """
 
     async def create_partition(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         PartitionInput: PartitionInputTypeDef,
-        CatalogId: str = ...
+        CatalogId: str = ...,
     ) -> Dict[str, Any]:
         """
         Creates a new partition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_partition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#create_partition)
         """
 
     async def create_partition_index(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         PartitionIndex: PartitionIndexTypeDef,
-        CatalogId: str = ...
+        CatalogId: str = ...,
     ) -> Dict[str, Any]:
         """
         Creates a specified partition index in an existing table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_partition_index)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#create_partition_index)
         """
@@ -870,29 +870,29 @@
         *,
         SchemaName: str,
         DataFormat: DataFormatType,
         RegistryId: RegistryIdTypeDef = ...,
         Compatibility: CompatibilityType = ...,
         Description: str = ...,
         Tags: Mapping[str, str] = ...,
-        SchemaDefinition: str = ...
+        SchemaDefinition: str = ...,
     ) -> CreateSchemaResponseTypeDef:
         """
         Creates a new schema set and registers the schema definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_schema)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#create_schema)
         """
 
     async def create_script(
         self,
         *,
         DagNodes: Sequence[CodeGenNodeTypeDef] = ...,
         DagEdges: Sequence[CodeGenEdgeTypeDef] = ...,
-        Language: LanguageType = ...
+        Language: LanguageType = ...,
     ) -> CreateScriptResponseTypeDef:
         """
         Transforms a directed acyclic graph (DAG) into code.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_script)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#create_script)
         """
@@ -920,15 +920,15 @@
         Connections: ConnectionsListTypeDef = ...,
         MaxCapacity: float = ...,
         NumberOfWorkers: int = ...,
         WorkerType: WorkerTypeType = ...,
         SecurityConfiguration: str = ...,
         GlueVersion: str = ...,
         Tags: Mapping[str, str] = ...,
-        RequestOrigin: str = ...
+        RequestOrigin: str = ...,
     ) -> CreateSessionResponseTypeDef:
         """
         Creates a new session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_session)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#create_session)
         """
@@ -937,15 +937,15 @@
         self,
         *,
         DatabaseName: str,
         TableInput: TableInputTypeDef,
         CatalogId: str = ...,
         PartitionIndexes: Sequence[PartitionIndexTypeDef] = ...,
         TransactionId: str = ...,
-        OpenTableFormatInput: OpenTableFormatInputTypeDef = ...
+        OpenTableFormatInput: OpenTableFormatInputTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Creates a new table definition in the Data Catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#create_table)
         """
@@ -953,15 +953,15 @@
     async def create_table_optimizer(
         self,
         *,
         CatalogId: str,
         DatabaseName: str,
         TableName: str,
         Type: Literal["compaction"],
-        TableOptimizerConfiguration: TableOptimizerConfigurationTypeDef
+        TableOptimizerConfiguration: TableOptimizerConfigurationTypeDef,
     ) -> Dict[str, Any]:
         """
         Creates a new table optimizer for a specific function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_table_optimizer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#create_table_optimizer)
         """
@@ -974,29 +974,29 @@
         Actions: Sequence[ActionTypeDef],
         WorkflowName: str = ...,
         Schedule: str = ...,
         Predicate: PredicateTypeDef = ...,
         Description: str = ...,
         StartOnCreation: bool = ...,
         Tags: Mapping[str, str] = ...,
-        EventBatchingCondition: EventBatchingConditionTypeDef = ...
+        EventBatchingCondition: EventBatchingConditionTypeDef = ...,
     ) -> CreateTriggerResponseTypeDef:
         """
         Creates a new trigger.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_trigger)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#create_trigger)
         """
 
     async def create_user_defined_function(
         self,
         *,
         DatabaseName: str,
         FunctionInput: UserDefinedFunctionInputTypeDef,
-        CatalogId: str = ...
+        CatalogId: str = ...,
     ) -> Dict[str, Any]:
         """
         Creates a new function definition in the Data Catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_user_defined_function)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#create_user_defined_function)
         """
@@ -1004,15 +1004,15 @@
     async def create_workflow(
         self,
         *,
         Name: str,
         Description: str = ...,
         DefaultRunProperties: Mapping[str, str] = ...,
         Tags: Mapping[str, str] = ...,
-        MaxConcurrentRuns: int = ...
+        MaxConcurrentRuns: int = ...,
     ) -> CreateWorkflowResponseTypeDef:
         """
         Creates a new workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_workflow)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#create_workflow)
         """
@@ -1036,15 +1036,15 @@
     async def delete_column_statistics_for_partition(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         PartitionValues: Sequence[str],
         ColumnName: str,
-        CatalogId: str = ...
+        CatalogId: str = ...,
     ) -> Dict[str, Any]:
         """
         Delete the partition column statistics of a column.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.delete_column_statistics_for_partition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#delete_column_statistics_for_partition)
         """
@@ -1131,15 +1131,15 @@
 
     async def delete_partition(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         PartitionValues: Sequence[str],
-        CatalogId: str = ...
+        CatalogId: str = ...,
     ) -> Dict[str, Any]:
         """
         Deletes a specified partition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.delete_partition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#delete_partition)
         """
@@ -1341,15 +1341,15 @@
     async def get_column_statistics_for_partition(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         PartitionValues: Sequence[str],
         ColumnNames: Sequence[str],
-        CatalogId: str = ...
+        CatalogId: str = ...,
     ) -> GetColumnStatisticsForPartitionResponseTypeDef:
         """
         Retrieves partition statistics of columns.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_column_statistics_for_partition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#get_column_statistics_for_partition)
         """
@@ -1397,15 +1397,15 @@
     async def get_connections(
         self,
         *,
         CatalogId: str = ...,
         Filter: GetConnectionsFilterTypeDef = ...,
         HidePassword: bool = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> GetConnectionsResponseTypeDef:
         """
         Retrieves a list of connection definitions from the Data Catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_connections)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#get_connections)
         """
@@ -1504,15 +1504,15 @@
 
     async def get_databases(
         self,
         *,
         CatalogId: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        ResourceShareType: ResourceShareTypeType = ...
+        ResourceShareType: ResourceShareTypeType = ...,
     ) -> GetDatabasesResponseTypeDef:
         """
         Retrieves all databases defined in a given Data Catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_databases)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#get_databases)
         """
@@ -1594,15 +1594,15 @@
         """
 
     async def get_mapping(
         self,
         *,
         Source: CatalogEntryTypeDef,
         Sinks: Sequence[CatalogEntryTypeDef] = ...,
-        Location: LocationTypeDef = ...
+        Location: LocationTypeDef = ...,
     ) -> GetMappingResponseTypeDef:
         """
         Creates mappings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_mapping)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#get_mapping)
         """
@@ -1620,15 +1620,15 @@
     async def get_ml_task_runs(
         self,
         *,
         TransformId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         Filter: TaskRunFilterCriteriaTypeDef = ...,
-        Sort: TaskRunSortCriteriaTypeDef = ...
+        Sort: TaskRunSortCriteriaTypeDef = ...,
     ) -> GetMLTaskRunsResponseTypeDef:
         """
         Gets a list of runs for a machine learning transform.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_ml_task_runs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#get_ml_task_runs)
         """
@@ -1644,30 +1644,30 @@
 
     async def get_ml_transforms(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         Filter: TransformFilterCriteriaTypeDef = ...,
-        Sort: TransformSortCriteriaTypeDef = ...
+        Sort: TransformSortCriteriaTypeDef = ...,
     ) -> GetMLTransformsResponseTypeDef:
         """
         Gets a sortable, filterable list of existing Glue machine learning transforms.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_ml_transforms)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#get_ml_transforms)
         """
 
     async def get_partition(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         PartitionValues: Sequence[str],
-        CatalogId: str = ...
+        CatalogId: str = ...,
     ) -> GetPartitionResponseTypeDef:
         """
         Retrieves information about a specified partition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_partition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#get_partition)
         """
@@ -1690,15 +1690,15 @@
         CatalogId: str = ...,
         Expression: str = ...,
         NextToken: str = ...,
         Segment: SegmentTypeDef = ...,
         MaxResults: int = ...,
         ExcludeColumnSchema: bool = ...,
         TransactionId: str = ...,
-        QueryAsOfTime: TimestampTypeDef = ...
+        QueryAsOfTime: TimestampTypeDef = ...,
     ) -> GetPartitionsResponseTypeDef:
         """
         Retrieves information about the partitions in a table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_partitions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#get_partitions)
         """
@@ -1707,15 +1707,15 @@
         self,
         *,
         Mapping: Sequence[MappingEntryTypeDef],
         Source: CatalogEntryTypeDef,
         Sinks: Sequence[CatalogEntryTypeDef] = ...,
         Location: LocationTypeDef = ...,
         Language: LanguageType = ...,
-        AdditionalPlanOptionsMap: Mapping[str, str] = ...
+        AdditionalPlanOptionsMap: Mapping[str, str] = ...,
     ) -> GetPlanResponseTypeDef:
         """
         Gets code to perform a specified mapping.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_plan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#get_plan)
         """
@@ -1769,15 +1769,15 @@
         """
 
     async def get_schema_version(
         self,
         *,
         SchemaId: SchemaIdTypeDef = ...,
         SchemaVersionId: str = ...,
-        SchemaVersionNumber: SchemaVersionNumberTypeDef = ...
+        SchemaVersionNumber: SchemaVersionNumberTypeDef = ...,
     ) -> GetSchemaVersionResponseTypeDef:
         """
         Get the specified schema by its unique ID assigned when a version of the schema
         is created or
         registered.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_schema_version)
@@ -1786,15 +1786,15 @@
 
     async def get_schema_versions_diff(
         self,
         *,
         SchemaId: SchemaIdTypeDef,
         FirstSchemaVersionNumber: SchemaVersionNumberTypeDef,
         SecondSchemaVersionNumber: SchemaVersionNumberTypeDef,
-        SchemaDiffType: Literal["SYNTAX_DIFF"]
+        SchemaDiffType: Literal["SYNTAX_DIFF"],
     ) -> GetSchemaVersionsDiffResponseTypeDef:
         """
         Fetches the schema version difference in the specified difference type between
         two stored schema versions in the Schema
         Registry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_schema_versions_diff)
@@ -1842,15 +1842,15 @@
     async def get_table(
         self,
         *,
         DatabaseName: str,
         Name: str,
         CatalogId: str = ...,
         TransactionId: str = ...,
-        QueryAsOfTime: TimestampTypeDef = ...
+        QueryAsOfTime: TimestampTypeDef = ...,
     ) -> GetTableResponseTypeDef:
         """
         Retrieves the `Table` definition in a Data Catalog for a specified table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#get_table)
         """
@@ -1878,15 +1878,15 @@
     async def get_table_versions(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         CatalogId: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> GetTableVersionsResponseTypeDef:
         """
         Retrieves a list of strings that identify available versions of a specified
         table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_table_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#get_table_versions)
@@ -1897,15 +1897,15 @@
         *,
         DatabaseName: str,
         CatalogId: str = ...,
         Expression: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         TransactionId: str = ...,
-        QueryAsOfTime: TimestampTypeDef = ...
+        QueryAsOfTime: TimestampTypeDef = ...,
     ) -> GetTablesResponseTypeDef:
         """
         Retrieves the definitions of some or all of the tables in a given `Database`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_tables)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#get_tables)
         """
@@ -1940,15 +1940,15 @@
         self,
         *,
         CatalogId: str,
         DatabaseName: str,
         TableName: str,
         PartitionValues: Sequence[str],
         SupportedPermissionTypes: Sequence[PermissionTypeType],
-        AuditContext: AuditContextTypeDef = ...
+        AuditContext: AuditContextTypeDef = ...,
     ) -> GetUnfilteredPartitionMetadataResponseTypeDef:
         """
         Retrieves partition metadata from the Data Catalog that contains unfiltered
         metadata.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_unfiltered_partition_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#get_unfiltered_partition_metadata)
@@ -1961,15 +1961,15 @@
         DatabaseName: str,
         TableName: str,
         SupportedPermissionTypes: Sequence[PermissionTypeType],
         Expression: str = ...,
         AuditContext: AuditContextTypeDef = ...,
         NextToken: str = ...,
         Segment: SegmentTypeDef = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> GetUnfilteredPartitionsMetadataResponseTypeDef:
         """
         Retrieves partition metadata from the Data Catalog that contains unfiltered
         metadata.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_unfiltered_partitions_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#get_unfiltered_partitions_metadata)
@@ -1978,15 +1978,15 @@
     async def get_unfiltered_table_metadata(
         self,
         *,
         CatalogId: str,
         DatabaseName: str,
         Name: str,
         SupportedPermissionTypes: Sequence[PermissionTypeType],
-        AuditContext: AuditContextTypeDef = ...
+        AuditContext: AuditContextTypeDef = ...,
     ) -> GetUnfilteredTableMetadataResponseTypeDef:
         """
         Retrieves table metadata from the Data Catalog that contains unfiltered
         metadata.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_unfiltered_table_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#get_unfiltered_table_metadata)
@@ -2005,15 +2005,15 @@
     async def get_user_defined_functions(
         self,
         *,
         Pattern: str,
         CatalogId: str = ...,
         DatabaseName: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> GetUserDefinedFunctionsResponseTypeDef:
         """
         Retrieves multiple function definitions from the Data Catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_user_defined_functions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#get_user_defined_functions)
         """
@@ -2100,15 +2100,15 @@
 
     async def list_crawls(
         self,
         *,
         CrawlerName: str,
         MaxResults: int = ...,
         Filters: Sequence[CrawlsFilterTypeDef] = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListCrawlsResponseTypeDef:
         """
         Returns all the crawls of a specified crawler.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.list_crawls)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#list_crawls)
         """
@@ -2124,43 +2124,43 @@
         """
 
     async def list_data_quality_results(
         self,
         *,
         Filter: DataQualityResultFilterCriteriaTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListDataQualityResultsResponseTypeDef:
         """
         Returns all data quality execution results for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.list_data_quality_results)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#list_data_quality_results)
         """
 
     async def list_data_quality_rule_recommendation_runs(
         self,
         *,
         Filter: DataQualityRuleRecommendationRunFilterTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListDataQualityRuleRecommendationRunsResponseTypeDef:
         """
         Lists the recommendation runs meeting the filter criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.list_data_quality_rule_recommendation_runs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#list_data_quality_rule_recommendation_runs)
         """
 
     async def list_data_quality_ruleset_evaluation_runs(
         self,
         *,
         Filter: DataQualityRulesetEvaluationRunFilterTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListDataQualityRulesetEvaluationRunsResponseTypeDef:
         """
         Lists all the runs meeting the filter criteria, where a ruleset is evaluated
         against a data
         source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.list_data_quality_ruleset_evaluation_runs)
@@ -2169,15 +2169,15 @@
 
     async def list_data_quality_rulesets(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         Filter: DataQualityRulesetFilterCriteriaTypeDef = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> ListDataQualityRulesetsResponseTypeDef:
         """
         Returns a paginated list of rulesets for the specified list of Glue tables.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.list_data_quality_rulesets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#list_data_quality_rulesets)
         """
@@ -2209,15 +2209,15 @@
     async def list_ml_transforms(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         Filter: TransformFilterCriteriaTypeDef = ...,
         Sort: TransformSortCriteriaTypeDef = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> ListMLTransformsResponseTypeDef:
         """
         Retrieves a sortable, filterable list of existing Glue machine learning
         transforms in this Amazon Web Services account, or the resources with the
         specified
         tag.
 
@@ -2259,15 +2259,15 @@
 
     async def list_sessions(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         Tags: Mapping[str, str] = ...,
-        RequestOrigin: str = ...
+        RequestOrigin: str = ...,
     ) -> ListSessionsResponseTypeDef:
         """
         Retrieve a list of sessions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.list_sessions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#list_sessions)
         """
@@ -2286,30 +2286,30 @@
         self,
         *,
         CatalogId: str,
         DatabaseName: str,
         TableName: str,
         Type: Literal["compaction"],
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListTableOptimizerRunsResponseTypeDef:
         """
         Lists the history of previous optimizer runs for a specific table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.list_table_optimizer_runs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#list_table_optimizer_runs)
         """
 
     async def list_triggers(
         self,
         *,
         NextToken: str = ...,
         DependentJobName: str = ...,
         MaxResults: int = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> ListTriggersResponseTypeDef:
         """
         Retrieves the names of all trigger resources in this Amazon Web Services
         account, or the resources with the specified
         tag.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.list_triggers)
@@ -2326,15 +2326,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#list_workflows)
         """
 
     async def put_data_catalog_encryption_settings(
         self,
         *,
         DataCatalogEncryptionSettings: DataCatalogEncryptionSettingsTypeDef,
-        CatalogId: str = ...
+        CatalogId: str = ...,
     ) -> Dict[str, Any]:
         """
         Sets the security configuration for a specified catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.put_data_catalog_encryption_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#put_data_catalog_encryption_settings)
         """
@@ -2342,30 +2342,30 @@
     async def put_resource_policy(
         self,
         *,
         PolicyInJson: str,
         ResourceArn: str = ...,
         PolicyHashCondition: str = ...,
         PolicyExistsCondition: ExistConditionType = ...,
-        EnableHybrid: EnableHybridValuesType = ...
+        EnableHybrid: EnableHybridValuesType = ...,
     ) -> PutResourcePolicyResponseTypeDef:
         """
         Sets the Data Catalog resource policy for access control.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.put_resource_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#put_resource_policy)
         """
 
     async def put_schema_version_metadata(
         self,
         *,
         MetadataKeyValue: MetadataKeyValuePairTypeDef,
         SchemaId: SchemaIdTypeDef = ...,
         SchemaVersionNumber: SchemaVersionNumberTypeDef = ...,
-        SchemaVersionId: str = ...
+        SchemaVersionId: str = ...,
     ) -> PutSchemaVersionMetadataResponseTypeDef:
         """
         Puts the metadata key value pair for a specified schema version ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.put_schema_version_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#put_schema_version_metadata)
         """
@@ -2384,15 +2384,15 @@
         self,
         *,
         SchemaId: SchemaIdTypeDef = ...,
         SchemaVersionNumber: SchemaVersionNumberTypeDef = ...,
         SchemaVersionId: str = ...,
         MetadataList: Sequence[MetadataKeyValuePairTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> QuerySchemaVersionMetadataResponseTypeDef:
         """
         Queries for the schema version metadata information.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.query_schema_version_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#query_schema_version_metadata)
         """
@@ -2409,15 +2409,15 @@
 
     async def remove_schema_version_metadata(
         self,
         *,
         MetadataKeyValue: MetadataKeyValuePairTypeDef,
         SchemaId: SchemaIdTypeDef = ...,
         SchemaVersionNumber: SchemaVersionNumberTypeDef = ...,
-        SchemaVersionId: str = ...
+        SchemaVersionId: str = ...,
     ) -> RemoveSchemaVersionMetadataResponseTypeDef:
         """
         Removes a key value pair from the schema version metadata for the specified
         schema version
         ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.remove_schema_version_metadata)
@@ -2461,15 +2461,15 @@
         *,
         CatalogId: str = ...,
         NextToken: str = ...,
         Filters: Sequence[PropertyPredicateTypeDef] = ...,
         SearchText: str = ...,
         SortCriteria: Sequence[SortCriterionTypeDef] = ...,
         MaxResults: int = ...,
-        ResourceShareType: ResourceShareTypeType = ...
+        ResourceShareType: ResourceShareTypeType = ...,
     ) -> SearchTablesResponseTypeDef:
         """
         Searches a set of tables based on properties in the table metadata as well as
         on the parent
         database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.search_tables)
@@ -2491,15 +2491,15 @@
         *,
         DatabaseName: str,
         TableName: str,
         Role: str,
         ColumnNameList: Sequence[str] = ...,
         SampleSize: float = ...,
         CatalogID: str = ...,
-        SecurityConfiguration: str = ...
+        SecurityConfiguration: str = ...,
     ) -> StartColumnStatisticsTaskRunResponseTypeDef:
         """
         Starts a column statistics task run, for a specified table and columns.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.start_column_statistics_task_run)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#start_column_statistics_task_run)
         """
@@ -2526,15 +2526,15 @@
         self,
         *,
         DataSource: DataSourceTypeDef,
         Role: str,
         NumberOfWorkers: int = ...,
         Timeout: int = ...,
         CreatedRulesetName: str = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> StartDataQualityRuleRecommendationRunResponseTypeDef:
         """
         Starts a recommendation run that is used to generate rules when you don't know
         what rules to
         write.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.start_data_quality_rule_recommendation_run)
@@ -2547,15 +2547,15 @@
         DataSource: DataSourceTypeDef,
         Role: str,
         RulesetNames: Sequence[str],
         NumberOfWorkers: int = ...,
         Timeout: int = ...,
         ClientToken: str = ...,
         AdditionalRunOptions: DataQualityEvaluationRunAdditionalRunOptionsTypeDef = ...,
-        AdditionalDataSources: Mapping[str, DataSourceTypeDef] = ...
+        AdditionalDataSources: Mapping[str, DataSourceTypeDef] = ...,
     ) -> StartDataQualityRulesetEvaluationRunResponseTypeDef:
         """
         Once you have a ruleset definition (either recommended or your own), you call
         this operation to evaluate the ruleset against a data source (Glue
         table).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.start_data_quality_ruleset_evaluation_run)
@@ -2594,15 +2594,15 @@
         AllocatedCapacity: int = ...,
         Timeout: int = ...,
         MaxCapacity: float = ...,
         SecurityConfiguration: str = ...,
         NotificationProperty: NotificationPropertyTypeDef = ...,
         WorkerType: WorkerTypeType = ...,
         NumberOfWorkers: int = ...,
-        ExecutionClass: ExecutionClassType = ...
+        ExecutionClass: ExecutionClassType = ...,
     ) -> StartJobRunResponseTypeDef:
         """
         Starts a job run using a job definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.start_job_run)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#start_job_run)
         """
@@ -2733,15 +2733,15 @@
 
     async def update_classifier(
         self,
         *,
         GrokClassifier: UpdateGrokClassifierRequestTypeDef = ...,
         XMLClassifier: UpdateXMLClassifierRequestTypeDef = ...,
         JsonClassifier: UpdateJsonClassifierRequestTypeDef = ...,
-        CsvClassifier: UpdateCsvClassifierRequestTypeDef = ...
+        CsvClassifier: UpdateCsvClassifierRequestTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Modifies an existing classifier (a `GrokClassifier`, an `XMLClassifier`, a
         `JsonClassifier`, or a `CsvClassifier`, depending on which field is
         present).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.update_classifier)
@@ -2751,30 +2751,30 @@
     async def update_column_statistics_for_partition(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         PartitionValues: Sequence[str],
         ColumnStatisticsList: Sequence[ColumnStatisticsTypeDef],
-        CatalogId: str = ...
+        CatalogId: str = ...,
     ) -> UpdateColumnStatisticsForPartitionResponseTypeDef:
         """
         Creates or updates partition statistics of columns.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.update_column_statistics_for_partition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#update_column_statistics_for_partition)
         """
 
     async def update_column_statistics_for_table(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         ColumnStatisticsList: Sequence[ColumnStatisticsTypeDef],
-        CatalogId: str = ...
+        CatalogId: str = ...,
     ) -> UpdateColumnStatisticsForTableResponseTypeDef:
         """
         Creates or updates table statistics of columns.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.update_column_statistics_for_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#update_column_statistics_for_table)
         """
@@ -2801,15 +2801,15 @@
         Classifiers: Sequence[str] = ...,
         TablePrefix: str = ...,
         SchemaChangePolicy: SchemaChangePolicyTypeDef = ...,
         RecrawlPolicy: RecrawlPolicyTypeDef = ...,
         LineageConfiguration: LineageConfigurationTypeDef = ...,
         LakeFormationConfiguration: LakeFormationConfigurationTypeDef = ...,
         Configuration: str = ...,
-        CrawlerSecurityConfiguration: str = ...
+        CrawlerSecurityConfiguration: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates a crawler.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.update_crawler)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#update_crawler)
         """
@@ -2850,15 +2850,15 @@
         EndpointName: str,
         PublicKey: str = ...,
         AddPublicKeys: Sequence[str] = ...,
         DeletePublicKeys: Sequence[str] = ...,
         CustomLibraries: DevEndpointCustomLibrariesTypeDef = ...,
         UpdateEtlLibraries: bool = ...,
         DeleteArguments: Sequence[str] = ...,
-        AddArguments: Mapping[str, str] = ...
+        AddArguments: Mapping[str, str] = ...,
     ) -> Dict[str, Any]:
         """
         Updates a specified development endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.update_dev_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#update_dev_endpoint)
         """
@@ -2880,15 +2880,15 @@
         Provider: SourceControlProviderType = ...,
         RepositoryName: str = ...,
         RepositoryOwner: str = ...,
         BranchName: str = ...,
         Folder: str = ...,
         CommitId: str = ...,
         AuthStrategy: SourceControlAuthStrategyType = ...,
-        AuthToken: str = ...
+        AuthToken: str = ...,
     ) -> UpdateJobFromSourceControlResponseTypeDef:
         """
         Synchronizes a job from the source control repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.update_job_from_source_control)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#update_job_from_source_control)
         """
@@ -2902,15 +2902,15 @@
         Parameters: TransformParametersTypeDef = ...,
         Role: str = ...,
         GlueVersion: str = ...,
         MaxCapacity: float = ...,
         WorkerType: WorkerTypeType = ...,
         NumberOfWorkers: int = ...,
         Timeout: int = ...,
-        MaxRetries: int = ...
+        MaxRetries: int = ...,
     ) -> UpdateMLTransformResponseTypeDef:
         """
         Updates an existing machine learning transform.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.update_ml_transform)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#update_ml_transform)
         """
@@ -2918,15 +2918,15 @@
     async def update_partition(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         PartitionValueList: Sequence[str],
         PartitionInput: PartitionInputTypeDef,
-        CatalogId: str = ...
+        CatalogId: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates a partition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.update_partition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#update_partition)
         """
@@ -2943,15 +2943,15 @@
 
     async def update_schema(
         self,
         *,
         SchemaId: SchemaIdTypeDef,
         SchemaVersionNumber: SchemaVersionNumberTypeDef = ...,
         Compatibility: CompatibilityType = ...,
-        Description: str = ...
+        Description: str = ...,
     ) -> UpdateSchemaResponseTypeDef:
         """
         Updates the description, compatibility setting, or version checkpoint for a
         schema
         set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.update_schema)
@@ -2965,15 +2965,15 @@
         Provider: SourceControlProviderType = ...,
         RepositoryName: str = ...,
         RepositoryOwner: str = ...,
         BranchName: str = ...,
         Folder: str = ...,
         CommitId: str = ...,
         AuthStrategy: SourceControlAuthStrategyType = ...,
-        AuthToken: str = ...
+        AuthToken: str = ...,
     ) -> UpdateSourceControlFromJobResponseTypeDef:
         """
         Synchronizes a job to the source control repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.update_source_control_from_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#update_source_control_from_job)
         """
@@ -2982,15 +2982,15 @@
         self,
         *,
         DatabaseName: str,
         TableInput: TableInputTypeDef,
         CatalogId: str = ...,
         SkipArchive: bool = ...,
         TransactionId: str = ...,
-        VersionId: str = ...
+        VersionId: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates a metadata table in the Data Catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.update_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#update_table)
         """
@@ -2998,15 +2998,15 @@
     async def update_table_optimizer(
         self,
         *,
         CatalogId: str,
         DatabaseName: str,
         TableName: str,
         Type: Literal["compaction"],
-        TableOptimizerConfiguration: TableOptimizerConfigurationTypeDef
+        TableOptimizerConfiguration: TableOptimizerConfigurationTypeDef,
     ) -> Dict[str, Any]:
         """
         Updates the configuration for an existing table optimizer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.update_table_optimizer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#update_table_optimizer)
         """
@@ -3023,30 +3023,30 @@
 
     async def update_user_defined_function(
         self,
         *,
         DatabaseName: str,
         FunctionName: str,
         FunctionInput: UserDefinedFunctionInputTypeDef,
-        CatalogId: str = ...
+        CatalogId: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates an existing function definition in the Data Catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.update_user_defined_function)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#update_user_defined_function)
         """
 
     async def update_workflow(
         self,
         *,
         Name: str,
         Description: str = ...,
         DefaultRunProperties: Mapping[str, str] = ...,
-        MaxConcurrentRuns: int = ...
+        MaxConcurrentRuns: int = ...,
     ) -> UpdateWorkflowResponseTypeDef:
         """
         Updates an existing workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.update_workflow)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#update_workflow)
         """
```

### Comparing `types-aiobotocore-glue-2.9.0/types_aiobotocore_glue/literals.py` & `types-aiobotocore-glue-2.9.1/types_aiobotocore_glue/literals.py`

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
     "AdditionalOptionKeysType",
     "AggFunctionType",
     "BackfillErrorCodeType",
     "BlueprintRunStateType",
     "BlueprintStatusType",
     "CatalogEncryptionModeType",
@@ -133,15 +132,14 @@
     "GlueServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AdditionalOptionKeysType = Literal["observations.scope", "performanceTuning.caching"]
 AggFunctionType = Literal[
     "avg",
     "count",
     "countDistinct",
     "first",
     "kurtosis",
```

### Comparing `types-aiobotocore-glue-2.9.0/types_aiobotocore_glue/literals.pyi` & `types-aiobotocore-glue-2.9.1/types_aiobotocore_glue/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glue-2.9.0/types_aiobotocore_glue/paginator.py` & `types-aiobotocore-glue-2.9.1/types_aiobotocore_glue/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,14 @@
     "GetTriggersPaginator",
     "GetUserDefinedFunctionsPaginator",
     "ListRegistriesPaginator",
     "ListSchemaVersionsPaginator",
     "ListSchemasPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -147,15 +146,15 @@
 
     def paginate(
         self,
         *,
         CatalogId: str = ...,
         Filter: GetConnectionsFilterTypeDef = ...,
         HidePassword: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetConnectionsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetConnections.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/paginators/#getconnectionspaginator)
         """
 
 
@@ -165,15 +164,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/paginators/#getcrawlermetricspaginator)
     """
 
     def paginate(
         self,
         *,
         CrawlerNameList: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetCrawlerMetricsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetCrawlerMetrics.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/paginators/#getcrawlermetricspaginator)
         """
 
 
@@ -199,15 +198,15 @@
     """
 
     def paginate(
         self,
         *,
         CatalogId: str = ...,
         ResourceShareType: ResourceShareTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetDatabasesResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetDatabases.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/paginators/#getdatabasespaginator)
         """
 
 
@@ -264,15 +263,15 @@
 
     def paginate(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         CatalogId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetPartitionIndexesResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetPartitionIndexes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/paginators/#getpartitionindexespaginator)
         """
 
 
@@ -289,15 +288,15 @@
         TableName: str,
         CatalogId: str = ...,
         Expression: str = ...,
         Segment: SegmentTypeDef = ...,
         ExcludeColumnSchema: bool = ...,
         TransactionId: str = ...,
         QueryAsOfTime: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetPartitionsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetPartitions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/paginators/#getpartitionspaginator)
         """
 
 
@@ -339,15 +338,15 @@
 
     def paginate(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         CatalogId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetTableVersionsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetTableVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/paginators/#gettableversionspaginator)
         """
 
 
@@ -361,15 +360,15 @@
         self,
         *,
         DatabaseName: str,
         CatalogId: str = ...,
         Expression: str = ...,
         TransactionId: str = ...,
         QueryAsOfTime: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetTablesResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetTables.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/paginators/#gettablespaginator)
         """
 
 
@@ -396,15 +395,15 @@
 
     def paginate(
         self,
         *,
         Pattern: str,
         CatalogId: str = ...,
         DatabaseName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetUserDefinedFunctionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetUserDefinedFunctions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/paginators/#getuserdefinedfunctionspaginator)
         """
```

### Comparing `types-aiobotocore-glue-2.9.0/types_aiobotocore_glue/paginator.pyi` & `types-aiobotocore-glue-2.9.1/types_aiobotocore_glue/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,15 @@
 
     def paginate(
         self,
         *,
         CatalogId: str = ...,
         Filter: GetConnectionsFilterTypeDef = ...,
         HidePassword: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetConnectionsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetConnections.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/paginators/#getconnectionspaginator)
         """
 
 class GetCrawlerMetricsPaginator(AioPaginator):
@@ -160,15 +160,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/paginators/#getcrawlermetricspaginator)
     """
 
     def paginate(
         self,
         *,
         CrawlerNameList: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetCrawlerMetricsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetCrawlerMetrics.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/paginators/#getcrawlermetricspaginator)
         """
 
 class GetCrawlersPaginator(AioPaginator):
@@ -192,15 +192,15 @@
     """
 
     def paginate(
         self,
         *,
         CatalogId: str = ...,
         ResourceShareType: ResourceShareTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetDatabasesResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetDatabases.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/paginators/#getdatabasespaginator)
         """
 
 class GetDevEndpointsPaginator(AioPaginator):
@@ -253,15 +253,15 @@
 
     def paginate(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         CatalogId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetPartitionIndexesResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetPartitionIndexes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/paginators/#getpartitionindexespaginator)
         """
 
 class GetPartitionsPaginator(AioPaginator):
@@ -277,15 +277,15 @@
         TableName: str,
         CatalogId: str = ...,
         Expression: str = ...,
         Segment: SegmentTypeDef = ...,
         ExcludeColumnSchema: bool = ...,
         TransactionId: str = ...,
         QueryAsOfTime: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetPartitionsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetPartitions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/paginators/#getpartitionspaginator)
         """
 
 class GetResourcePoliciesPaginator(AioPaginator):
@@ -324,15 +324,15 @@
 
     def paginate(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         CatalogId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetTableVersionsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetTableVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/paginators/#gettableversionspaginator)
         """
 
 class GetTablesPaginator(AioPaginator):
@@ -345,15 +345,15 @@
         self,
         *,
         DatabaseName: str,
         CatalogId: str = ...,
         Expression: str = ...,
         TransactionId: str = ...,
         QueryAsOfTime: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetTablesResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetTables.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/paginators/#gettablespaginator)
         """
 
 class GetTriggersPaginator(AioPaginator):
@@ -378,15 +378,15 @@
 
     def paginate(
         self,
         *,
         Pattern: str,
         CatalogId: str = ...,
         DatabaseName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetUserDefinedFunctionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetUserDefinedFunctions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/paginators/#getuserdefinedfunctionspaginator)
         """
 
 class ListRegistriesPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-glue-2.9.0/types_aiobotocore_glue/type_defs.py` & `types-aiobotocore-glue-2.9.1/types_aiobotocore_glue/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "NotificationPropertyTypeDef",
     "AggregateOperationTypeDef",
     "AmazonRedshiftAdvancedOptionTypeDef",
     "OptionTypeDef",
     "ApplyMappingTypeDef",
     "AuditContextTypeDef",
```

### Comparing `types-aiobotocore-glue-2.9.0/types_aiobotocore_glue/type_defs.pyi` & `types-aiobotocore-glue-2.9.1/types_aiobotocore_glue/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glue-2.9.0/types_aiobotocore_glue.egg-info/PKG-INFO` & `types-aiobotocore-glue-2.9.1/types_aiobotocore_glue.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-glue
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Glue 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Glue 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/
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
 
 <a id="types-aiobotocore-glue"></a>
 
 # types-aiobotocore-glue
 
 [![PyPI - types-aiobotocore-glue](https://img.shields.io/pypi/v/types-aiobotocore-glue.svg?color=blue)](https://pypi.org/project/types-aiobotocore-glue)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-glue.svg?color=blue)](https://pypi.org/project/types-aiobotocore-glue)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-glue)](https://pepy.tech/project/types-aiobotocore-glue)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Glue 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
+[aiobotocore.Glue 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
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
 [types-aiobotocore-glue docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-glue-2.9.0/types_aiobotocore_glue.egg-info/SOURCES.txt` & `types-aiobotocore-glue-2.9.1/types_aiobotocore_glue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

