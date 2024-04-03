# Comparing `tmp/types-aiobotocore-imagebuilder-2.9.0.tar.gz` & `tmp/types-aiobotocore-imagebuilder-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-imagebuilder-2.9.0.tar", last modified: Wed Dec 13 19:59:27 2023, max compression
+gzip compressed data, was "types-aiobotocore-imagebuilder-2.9.1.tar", last modified: Thu Jan 18 01:20:51 2024, max compression
```

## Comparing `types-aiobotocore-imagebuilder-2.9.0.tar` & `types-aiobotocore-imagebuilder-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:27.697692 types-aiobotocore-imagebuilder-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:47:24.000000 types-aiobotocore-imagebuilder-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12484 2023-12-13 19:59:27.697692 types-aiobotocore-imagebuilder-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10901 2023-12-13 19:47:24.000000 types-aiobotocore-imagebuilder-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:27.697692 types-aiobotocore-imagebuilder-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2023-12-13 19:47:24.000000 types-aiobotocore-imagebuilder-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:27.697692 types-aiobotocore-imagebuilder-2.9.0/types_aiobotocore_imagebuilder/
--rw-r--r--   0 runner    (1001) docker     (127)      483 2023-12-13 19:47:24.000000 types-aiobotocore-imagebuilder-2.9.0/types_aiobotocore_imagebuilder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2023-12-13 19:47:24.000000 types-aiobotocore-imagebuilder-2.9.0/types_aiobotocore_imagebuilder/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      952 2023-12-13 19:47:24.000000 types-aiobotocore-imagebuilder-2.9.0/types_aiobotocore_imagebuilder/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    57188 2023-12-13 19:47:25.000000 types-aiobotocore-imagebuilder-2.9.0/types_aiobotocore_imagebuilder/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    57184 2023-12-13 19:47:24.000000 types-aiobotocore-imagebuilder-2.9.0/types_aiobotocore_imagebuilder/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11625 2023-12-13 19:47:25.000000 types-aiobotocore-imagebuilder-2.9.0/types_aiobotocore_imagebuilder/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11623 2023-12-13 19:47:25.000000 types-aiobotocore-imagebuilder-2.9.0/types_aiobotocore_imagebuilder/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:47:24.000000 types-aiobotocore-imagebuilder-2.9.0/types_aiobotocore_imagebuilder/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    84487 2023-12-13 19:47:26.000000 types-aiobotocore-imagebuilder-2.9.0/types_aiobotocore_imagebuilder/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    84486 2023-12-13 19:47:26.000000 types-aiobotocore-imagebuilder-2.9.0/types_aiobotocore_imagebuilder/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:47:24.000000 types-aiobotocore-imagebuilder-2.9.0/types_aiobotocore_imagebuilder/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:27.697692 types-aiobotocore-imagebuilder-2.9.0/types_aiobotocore_imagebuilder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12484 2023-12-13 19:59:27.000000 types-aiobotocore-imagebuilder-2.9.0/types_aiobotocore_imagebuilder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      819 2023-12-13 19:59:27.000000 types-aiobotocore-imagebuilder-2.9.0/types_aiobotocore_imagebuilder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:27.000000 types-aiobotocore-imagebuilder-2.9.0/types_aiobotocore_imagebuilder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:27.000000 types-aiobotocore-imagebuilder-2.9.0/types_aiobotocore_imagebuilder.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:27.000000 types-aiobotocore-imagebuilder-2.9.0/types_aiobotocore_imagebuilder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-13 19:59:27.000000 types-aiobotocore-imagebuilder-2.9.0/types_aiobotocore_imagebuilder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:51.541292 types-aiobotocore-imagebuilder-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:09:15.000000 types-aiobotocore-imagebuilder-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12504 2024-01-18 01:20:51.541292 types-aiobotocore-imagebuilder-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10901 2024-01-18 01:09:15.000000 types-aiobotocore-imagebuilder-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:51.541292 types-aiobotocore-imagebuilder-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-01-18 01:09:15.000000 types-aiobotocore-imagebuilder-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:51.541292 types-aiobotocore-imagebuilder-2.9.1/types_aiobotocore_imagebuilder/
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-01-18 01:09:15.000000 types-aiobotocore-imagebuilder-2.9.1/types_aiobotocore_imagebuilder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-01-18 01:09:15.000000 types-aiobotocore-imagebuilder-2.9.1/types_aiobotocore_imagebuilder/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-01-18 01:09:15.000000 types-aiobotocore-imagebuilder-2.9.1/types_aiobotocore_imagebuilder/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57213 2024-01-18 01:09:15.000000 types-aiobotocore-imagebuilder-2.9.1/types_aiobotocore_imagebuilder/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57210 2024-01-18 01:09:15.000000 types-aiobotocore-imagebuilder-2.9.1/types_aiobotocore_imagebuilder/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11623 2024-01-18 01:09:16.000000 types-aiobotocore-imagebuilder-2.9.1/types_aiobotocore_imagebuilder/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11623 2024-01-18 01:09:16.000000 types-aiobotocore-imagebuilder-2.9.1/types_aiobotocore_imagebuilder/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:09:15.000000 types-aiobotocore-imagebuilder-2.9.1/types_aiobotocore_imagebuilder/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    84486 2024-01-18 01:09:19.000000 types-aiobotocore-imagebuilder-2.9.1/types_aiobotocore_imagebuilder/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84486 2024-01-18 01:09:17.000000 types-aiobotocore-imagebuilder-2.9.1/types_aiobotocore_imagebuilder/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:09:15.000000 types-aiobotocore-imagebuilder-2.9.1/types_aiobotocore_imagebuilder/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:51.541292 types-aiobotocore-imagebuilder-2.9.1/types_aiobotocore_imagebuilder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12504 2024-01-18 01:20:51.000000 types-aiobotocore-imagebuilder-2.9.1/types_aiobotocore_imagebuilder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-01-18 01:20:51.000000 types-aiobotocore-imagebuilder-2.9.1/types_aiobotocore_imagebuilder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:51.000000 types-aiobotocore-imagebuilder-2.9.1/types_aiobotocore_imagebuilder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:51.000000 types-aiobotocore-imagebuilder-2.9.1/types_aiobotocore_imagebuilder.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:51.000000 types-aiobotocore-imagebuilder-2.9.1/types_aiobotocore_imagebuilder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-01-18 01:20:51.000000 types-aiobotocore-imagebuilder-2.9.1/types_aiobotocore_imagebuilder.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-imagebuilder-2.9.0/LICENSE` & `types-aiobotocore-imagebuilder-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-imagebuilder-2.9.0/PKG-INFO` & `types-aiobotocore-imagebuilder-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-imagebuilder
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.imagebuilder 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.imagebuilder 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/
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
 
 <a id="types-aiobotocore-imagebuilder"></a>
 
 # types-aiobotocore-imagebuilder
 
 [![PyPI - types-aiobotocore-imagebuilder](https://img.shields.io/pypi/v/types-aiobotocore-imagebuilder.svg?color=blue)](https://pypi.org/project/types-aiobotocore-imagebuilder)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-imagebuilder.svg?color=blue)](https://pypi.org/project/types-aiobotocore-imagebuilder)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-imagebuilder)](https://pepy.tech/project/types-aiobotocore-imagebuilder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.imagebuilder 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder)
+[aiobotocore.imagebuilder 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder)
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
 [types-aiobotocore-imagebuilder docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-imagebuilder-2.9.0/README.md` & `types-aiobotocore-imagebuilder-2.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-imagebuilder.svg?color=blue)](https://pypi.org/project/types-aiobotocore-imagebuilder)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-imagebuilder)](https://pepy.tech/project/types-aiobotocore-imagebuilder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.imagebuilder 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder)
+[aiobotocore.imagebuilder 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder)
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
 [types-aiobotocore-imagebuilder docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-imagebuilder-2.9.0/setup.py` & `types-aiobotocore-imagebuilder-2.9.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-imagebuilder",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_imagebuilder"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.imagebuilder 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.imagebuilder 2.9.1 service generated with"
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
     keywords="aiobotocore imagebuilder type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_imagebuilder": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-imagebuilder-2.9.0/types_aiobotocore_imagebuilder/__main__.py` & `types-aiobotocore-imagebuilder-2.9.1/types_aiobotocore_imagebuilder/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.imagebuilder 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.imagebuilder 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder\nOther"
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

### Comparing `types-aiobotocore-imagebuilder-2.9.0/types_aiobotocore_imagebuilder/client.py` & `types-aiobotocore-imagebuilder-2.9.1/types_aiobotocore_imagebuilder/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("imagebuilderClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -225,15 +224,15 @@
         clientToken: str,
         description: str = ...,
         changeDescription: str = ...,
         supportedOsVersions: Sequence[str] = ...,
         data: str = ...,
         uri: str = ...,
         kmsKeyId: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateComponentResponseTypeDef:
         """
         Creates a new component that can be used to build, validate, test, and assess
         your
         image.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.create_component)
@@ -254,15 +253,15 @@
         instanceConfiguration: InstanceConfigurationTypeDef = ...,
         dockerfileTemplateData: str = ...,
         dockerfileTemplateUri: str = ...,
         platformOverride: PlatformType = ...,
         imageOsVersionOverride: str = ...,
         tags: Mapping[str, str] = ...,
         workingDirectory: str = ...,
-        kmsKeyId: str = ...
+        kmsKeyId: str = ...,
     ) -> CreateContainerRecipeResponseTypeDef:
         """
         Creates a new container recipe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.create_container_recipe)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#create_container_recipe)
         """
@@ -270,15 +269,15 @@
     async def create_distribution_configuration(
         self,
         *,
         name: str,
         distributions: Sequence[DistributionTypeDef],
         clientToken: str,
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateDistributionConfigurationResponseTypeDef:
         """
         Creates a new distribution configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.create_distribution_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#create_distribution_configuration)
         """
@@ -292,15 +291,15 @@
         containerRecipeArn: str = ...,
         distributionConfigurationArn: str = ...,
         imageTestsConfiguration: ImageTestsConfigurationTypeDef = ...,
         enhancedImageMetadataEnabled: bool = ...,
         tags: Mapping[str, str] = ...,
         imageScanningConfiguration: ImageScanningConfigurationTypeDef = ...,
         workflows: Sequence[WorkflowConfigurationTypeDef] = ...,
-        executionRole: str = ...
+        executionRole: str = ...,
     ) -> CreateImageResponseTypeDef:
         """
         Creates a new image.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.create_image)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#create_image)
         """
@@ -318,15 +317,15 @@
         imageTestsConfiguration: ImageTestsConfigurationTypeDef = ...,
         enhancedImageMetadataEnabled: bool = ...,
         schedule: ScheduleTypeDef = ...,
         status: PipelineStatusType = ...,
         tags: Mapping[str, str] = ...,
         imageScanningConfiguration: ImageScanningConfigurationTypeDef = ...,
         workflows: Sequence[WorkflowConfigurationTypeDef] = ...,
-        executionRole: str = ...
+        executionRole: str = ...,
     ) -> CreateImagePipelineResponseTypeDef:
         """
         Creates a new image pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.create_image_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#create_image_pipeline)
         """
@@ -339,15 +338,15 @@
         components: Sequence[ComponentConfigurationTypeDef],
         parentImage: str,
         clientToken: str,
         description: str = ...,
         blockDeviceMappings: Sequence[InstanceBlockDeviceMappingTypeDef] = ...,
         tags: Mapping[str, str] = ...,
         workingDirectory: str = ...,
-        additionalInstanceConfiguration: AdditionalInstanceConfigurationTypeDef = ...
+        additionalInstanceConfiguration: AdditionalInstanceConfigurationTypeDef = ...,
     ) -> CreateImageRecipeResponseTypeDef:
         """
         Creates a new image recipe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.create_image_recipe)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#create_image_recipe)
         """
@@ -364,15 +363,15 @@
         subnetId: str = ...,
         logging: LoggingTypeDef = ...,
         keyPair: str = ...,
         terminateInstanceOnFailure: bool = ...,
         snsTopicArn: str = ...,
         resourceTags: Mapping[str, str] = ...,
         instanceMetadataOptions: InstanceMetadataOptionsTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateInfrastructureConfigurationResponseTypeDef:
         """
         Creates a new infrastructure configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.create_infrastructure_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#create_infrastructure_configuration)
         """
@@ -384,15 +383,15 @@
         executionRole: str,
         resourceType: LifecyclePolicyResourceTypeType,
         policyDetails: Sequence[LifecyclePolicyDetailTypeDef],
         resourceSelection: LifecyclePolicyResourceSelectionTypeDef,
         clientToken: str,
         description: str = ...,
         status: LifecyclePolicyStatusType = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateLifecyclePolicyResponseTypeDef:
         """
         Create a lifecycle policy resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.create_lifecycle_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#create_lifecycle_policy)
         """
@@ -405,15 +404,15 @@
         clientToken: str,
         type: WorkflowTypeType,
         description: str = ...,
         changeDescription: str = ...,
         data: str = ...,
         uri: str = ...,
         kmsKeyId: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateWorkflowResponseTypeDef:
         """
         Create a new workflow or a new version of an existing workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.create_workflow)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#create_workflow)
         """
@@ -680,15 +679,15 @@
         platform: PlatformType,
         clientToken: str,
         description: str = ...,
         changeDescription: str = ...,
         data: str = ...,
         uri: str = ...,
         kmsKeyId: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> ImportComponentResponseTypeDef:
         """
         Imports a component and transforms its data into a component document.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.import_component)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#import_component)
         """
@@ -699,15 +698,15 @@
         name: str,
         semanticVersion: str,
         platform: PlatformType,
         vmImportTaskId: str,
         clientToken: str,
         description: str = ...,
         osVersion: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> ImportVmImageResponseTypeDef:
         """
         When you export your virtual machine (VM) from its virtualization environment,
         that process creates a set of one or more disk container files that act as
         snapshots of your VM’s environment, settings, and
         data.
 
@@ -728,15 +727,15 @@
     async def list_components(
         self,
         *,
         owner: OwnershipType = ...,
         filters: Sequence[FilterTypeDef] = ...,
         byName: bool = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListComponentsResponseTypeDef:
         """
         Returns the list of components that can be filtered by name, or by using the
         listed `filters` to streamline
         results.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.list_components)
@@ -745,15 +744,15 @@
 
     async def list_container_recipes(
         self,
         *,
         owner: OwnershipType = ...,
         filters: Sequence[FilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListContainerRecipesResponseTypeDef:
         """
         Returns a list of container recipes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.list_container_recipes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#list_container_recipes)
         """
@@ -770,15 +769,15 @@
 
     async def list_image_build_versions(
         self,
         *,
         imageVersionArn: str,
         filters: Sequence[FilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListImageBuildVersionsResponseTypeDef:
         """
         Returns a list of image build versions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.list_image_build_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#list_image_build_versions)
         """
@@ -797,15 +796,15 @@
 
     async def list_image_pipeline_images(
         self,
         *,
         imagePipelineArn: str,
         filters: Sequence[FilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListImagePipelineImagesResponseTypeDef:
         """
         Returns a list of images created by the specified pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.list_image_pipeline_images)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#list_image_pipeline_images)
         """
@@ -822,15 +821,15 @@
 
     async def list_image_recipes(
         self,
         *,
         owner: OwnershipType = ...,
         filters: Sequence[FilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListImageRecipesResponseTypeDef:
         """
         Returns a list of image recipes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.list_image_recipes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#list_image_recipes)
         """
@@ -846,15 +845,15 @@
         """
 
     async def list_image_scan_findings(
         self,
         *,
         filters: Sequence[ImageScanFindingsFilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListImageScanFindingsResponseTypeDef:
         """
         Returns a list of image scan findings for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.list_image_scan_findings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#list_image_scan_findings)
         """
@@ -863,15 +862,15 @@
         self,
         *,
         owner: OwnershipType = ...,
         filters: Sequence[FilterTypeDef] = ...,
         byName: bool = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        includeDeprecated: bool = ...
+        includeDeprecated: bool = ...,
     ) -> ListImagesResponseTypeDef:
         """
         Returns the list of images that you have access to.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.list_images)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#list_images)
         """
@@ -888,15 +887,15 @@
 
     async def list_lifecycle_execution_resources(
         self,
         *,
         lifecycleExecutionId: str,
         parentResourceId: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListLifecycleExecutionResourcesResponseTypeDef:
         """
         List resources that the runtime instance of the image lifecycle identified for
         lifecycle
         actions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.list_lifecycle_execution_resources)
@@ -982,15 +981,15 @@
     async def list_workflows(
         self,
         *,
         owner: OwnershipType = ...,
         filters: Sequence[FilterTypeDef] = ...,
         byName: bool = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListWorkflowsResponseTypeDef:
         """
         Lists workflow build versions based on filtering parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.list_workflows)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#list_workflows)
         """
@@ -1038,15 +1037,15 @@
     async def send_workflow_step_action(
         self,
         *,
         stepExecutionId: str,
         imageBuildVersionArn: str,
         action: WorkflowStepActionTypeType,
         clientToken: str,
-        reason: str = ...
+        reason: str = ...,
     ) -> SendWorkflowStepActionResponseTypeDef:
         """
         Pauses or resumes image creation when the associated workflow runs a
         `WaitForAction`
         step.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.send_workflow_step_action)
@@ -1068,15 +1067,15 @@
         *,
         resourceArn: str,
         state: ResourceStateTypeDef,
         clientToken: str,
         executionRole: str = ...,
         includeResources: ResourceStateUpdateIncludeResourcesTypeDef = ...,
         exclusionRules: ResourceStateUpdateExclusionRulesTypeDef = ...,
-        updateAt: TimestampTypeDef = ...
+        updateAt: TimestampTypeDef = ...,
     ) -> StartResourceStateUpdateResponseTypeDef:
         """
         Begin asynchronous resource state update for lifecycle changes to the specified
         image
         resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.start_resource_state_update)
@@ -1101,15 +1100,15 @@
 
     async def update_distribution_configuration(
         self,
         *,
         distributionConfigurationArn: str,
         distributions: Sequence[DistributionTypeDef],
         clientToken: str,
-        description: str = ...
+        description: str = ...,
     ) -> UpdateDistributionConfigurationResponseTypeDef:
         """
         Updates a new distribution configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.update_distribution_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#update_distribution_configuration)
         """
@@ -1126,15 +1125,15 @@
         distributionConfigurationArn: str = ...,
         imageTestsConfiguration: ImageTestsConfigurationTypeDef = ...,
         enhancedImageMetadataEnabled: bool = ...,
         schedule: ScheduleTypeDef = ...,
         status: PipelineStatusType = ...,
         imageScanningConfiguration: ImageScanningConfigurationTypeDef = ...,
         workflows: Sequence[WorkflowConfigurationTypeDef] = ...,
-        executionRole: str = ...
+        executionRole: str = ...,
     ) -> UpdateImagePipelineResponseTypeDef:
         """
         Updates an image pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.update_image_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#update_image_pipeline)
         """
@@ -1150,15 +1149,15 @@
         securityGroupIds: Sequence[str] = ...,
         subnetId: str = ...,
         logging: LoggingTypeDef = ...,
         keyPair: str = ...,
         terminateInstanceOnFailure: bool = ...,
         snsTopicArn: str = ...,
         resourceTags: Mapping[str, str] = ...,
-        instanceMetadataOptions: InstanceMetadataOptionsTypeDef = ...
+        instanceMetadataOptions: InstanceMetadataOptionsTypeDef = ...,
     ) -> UpdateInfrastructureConfigurationResponseTypeDef:
         """
         Updates a new infrastructure configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.update_infrastructure_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#update_infrastructure_configuration)
         """
@@ -1169,15 +1168,15 @@
         lifecyclePolicyArn: str,
         executionRole: str,
         resourceType: LifecyclePolicyResourceTypeType,
         policyDetails: Sequence[LifecyclePolicyDetailTypeDef],
         resourceSelection: LifecyclePolicyResourceSelectionTypeDef,
         clientToken: str,
         description: str = ...,
-        status: LifecyclePolicyStatusType = ...
+        status: LifecyclePolicyStatusType = ...,
     ) -> UpdateLifecyclePolicyResponseTypeDef:
         """
         Update the specified lifecycle policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.update_lifecycle_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#update_lifecycle_policy)
         """
```

### Comparing `types-aiobotocore-imagebuilder-2.9.0/types_aiobotocore_imagebuilder/client.pyi` & `types-aiobotocore-imagebuilder-2.9.1/types_aiobotocore_imagebuilder/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -221,15 +221,15 @@
         clientToken: str,
         description: str = ...,
         changeDescription: str = ...,
         supportedOsVersions: Sequence[str] = ...,
         data: str = ...,
         uri: str = ...,
         kmsKeyId: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateComponentResponseTypeDef:
         """
         Creates a new component that can be used to build, validate, test, and assess
         your
         image.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.create_component)
@@ -250,15 +250,15 @@
         instanceConfiguration: InstanceConfigurationTypeDef = ...,
         dockerfileTemplateData: str = ...,
         dockerfileTemplateUri: str = ...,
         platformOverride: PlatformType = ...,
         imageOsVersionOverride: str = ...,
         tags: Mapping[str, str] = ...,
         workingDirectory: str = ...,
-        kmsKeyId: str = ...
+        kmsKeyId: str = ...,
     ) -> CreateContainerRecipeResponseTypeDef:
         """
         Creates a new container recipe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.create_container_recipe)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#create_container_recipe)
         """
@@ -266,15 +266,15 @@
     async def create_distribution_configuration(
         self,
         *,
         name: str,
         distributions: Sequence[DistributionTypeDef],
         clientToken: str,
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateDistributionConfigurationResponseTypeDef:
         """
         Creates a new distribution configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.create_distribution_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#create_distribution_configuration)
         """
@@ -288,15 +288,15 @@
         containerRecipeArn: str = ...,
         distributionConfigurationArn: str = ...,
         imageTestsConfiguration: ImageTestsConfigurationTypeDef = ...,
         enhancedImageMetadataEnabled: bool = ...,
         tags: Mapping[str, str] = ...,
         imageScanningConfiguration: ImageScanningConfigurationTypeDef = ...,
         workflows: Sequence[WorkflowConfigurationTypeDef] = ...,
-        executionRole: str = ...
+        executionRole: str = ...,
     ) -> CreateImageResponseTypeDef:
         """
         Creates a new image.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.create_image)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#create_image)
         """
@@ -314,15 +314,15 @@
         imageTestsConfiguration: ImageTestsConfigurationTypeDef = ...,
         enhancedImageMetadataEnabled: bool = ...,
         schedule: ScheduleTypeDef = ...,
         status: PipelineStatusType = ...,
         tags: Mapping[str, str] = ...,
         imageScanningConfiguration: ImageScanningConfigurationTypeDef = ...,
         workflows: Sequence[WorkflowConfigurationTypeDef] = ...,
-        executionRole: str = ...
+        executionRole: str = ...,
     ) -> CreateImagePipelineResponseTypeDef:
         """
         Creates a new image pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.create_image_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#create_image_pipeline)
         """
@@ -335,15 +335,15 @@
         components: Sequence[ComponentConfigurationTypeDef],
         parentImage: str,
         clientToken: str,
         description: str = ...,
         blockDeviceMappings: Sequence[InstanceBlockDeviceMappingTypeDef] = ...,
         tags: Mapping[str, str] = ...,
         workingDirectory: str = ...,
-        additionalInstanceConfiguration: AdditionalInstanceConfigurationTypeDef = ...
+        additionalInstanceConfiguration: AdditionalInstanceConfigurationTypeDef = ...,
     ) -> CreateImageRecipeResponseTypeDef:
         """
         Creates a new image recipe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.create_image_recipe)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#create_image_recipe)
         """
@@ -360,15 +360,15 @@
         subnetId: str = ...,
         logging: LoggingTypeDef = ...,
         keyPair: str = ...,
         terminateInstanceOnFailure: bool = ...,
         snsTopicArn: str = ...,
         resourceTags: Mapping[str, str] = ...,
         instanceMetadataOptions: InstanceMetadataOptionsTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateInfrastructureConfigurationResponseTypeDef:
         """
         Creates a new infrastructure configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.create_infrastructure_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#create_infrastructure_configuration)
         """
@@ -380,15 +380,15 @@
         executionRole: str,
         resourceType: LifecyclePolicyResourceTypeType,
         policyDetails: Sequence[LifecyclePolicyDetailTypeDef],
         resourceSelection: LifecyclePolicyResourceSelectionTypeDef,
         clientToken: str,
         description: str = ...,
         status: LifecyclePolicyStatusType = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateLifecyclePolicyResponseTypeDef:
         """
         Create a lifecycle policy resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.create_lifecycle_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#create_lifecycle_policy)
         """
@@ -401,15 +401,15 @@
         clientToken: str,
         type: WorkflowTypeType,
         description: str = ...,
         changeDescription: str = ...,
         data: str = ...,
         uri: str = ...,
         kmsKeyId: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateWorkflowResponseTypeDef:
         """
         Create a new workflow or a new version of an existing workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.create_workflow)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#create_workflow)
         """
@@ -676,15 +676,15 @@
         platform: PlatformType,
         clientToken: str,
         description: str = ...,
         changeDescription: str = ...,
         data: str = ...,
         uri: str = ...,
         kmsKeyId: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> ImportComponentResponseTypeDef:
         """
         Imports a component and transforms its data into a component document.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.import_component)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#import_component)
         """
@@ -695,15 +695,15 @@
         name: str,
         semanticVersion: str,
         platform: PlatformType,
         vmImportTaskId: str,
         clientToken: str,
         description: str = ...,
         osVersion: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> ImportVmImageResponseTypeDef:
         """
         When you export your virtual machine (VM) from its virtualization environment,
         that process creates a set of one or more disk container files that act as
         snapshots of your VM’s environment, settings, and
         data.
 
@@ -724,15 +724,15 @@
     async def list_components(
         self,
         *,
         owner: OwnershipType = ...,
         filters: Sequence[FilterTypeDef] = ...,
         byName: bool = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListComponentsResponseTypeDef:
         """
         Returns the list of components that can be filtered by name, or by using the
         listed `filters` to streamline
         results.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.list_components)
@@ -741,15 +741,15 @@
 
     async def list_container_recipes(
         self,
         *,
         owner: OwnershipType = ...,
         filters: Sequence[FilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListContainerRecipesResponseTypeDef:
         """
         Returns a list of container recipes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.list_container_recipes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#list_container_recipes)
         """
@@ -766,15 +766,15 @@
 
     async def list_image_build_versions(
         self,
         *,
         imageVersionArn: str,
         filters: Sequence[FilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListImageBuildVersionsResponseTypeDef:
         """
         Returns a list of image build versions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.list_image_build_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#list_image_build_versions)
         """
@@ -793,15 +793,15 @@
 
     async def list_image_pipeline_images(
         self,
         *,
         imagePipelineArn: str,
         filters: Sequence[FilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListImagePipelineImagesResponseTypeDef:
         """
         Returns a list of images created by the specified pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.list_image_pipeline_images)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#list_image_pipeline_images)
         """
@@ -818,15 +818,15 @@
 
     async def list_image_recipes(
         self,
         *,
         owner: OwnershipType = ...,
         filters: Sequence[FilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListImageRecipesResponseTypeDef:
         """
         Returns a list of image recipes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.list_image_recipes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#list_image_recipes)
         """
@@ -842,15 +842,15 @@
         """
 
     async def list_image_scan_findings(
         self,
         *,
         filters: Sequence[ImageScanFindingsFilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListImageScanFindingsResponseTypeDef:
         """
         Returns a list of image scan findings for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.list_image_scan_findings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#list_image_scan_findings)
         """
@@ -859,15 +859,15 @@
         self,
         *,
         owner: OwnershipType = ...,
         filters: Sequence[FilterTypeDef] = ...,
         byName: bool = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        includeDeprecated: bool = ...
+        includeDeprecated: bool = ...,
     ) -> ListImagesResponseTypeDef:
         """
         Returns the list of images that you have access to.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.list_images)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#list_images)
         """
@@ -884,15 +884,15 @@
 
     async def list_lifecycle_execution_resources(
         self,
         *,
         lifecycleExecutionId: str,
         parentResourceId: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListLifecycleExecutionResourcesResponseTypeDef:
         """
         List resources that the runtime instance of the image lifecycle identified for
         lifecycle
         actions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.list_lifecycle_execution_resources)
@@ -978,15 +978,15 @@
     async def list_workflows(
         self,
         *,
         owner: OwnershipType = ...,
         filters: Sequence[FilterTypeDef] = ...,
         byName: bool = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListWorkflowsResponseTypeDef:
         """
         Lists workflow build versions based on filtering parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.list_workflows)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#list_workflows)
         """
@@ -1034,15 +1034,15 @@
     async def send_workflow_step_action(
         self,
         *,
         stepExecutionId: str,
         imageBuildVersionArn: str,
         action: WorkflowStepActionTypeType,
         clientToken: str,
-        reason: str = ...
+        reason: str = ...,
     ) -> SendWorkflowStepActionResponseTypeDef:
         """
         Pauses or resumes image creation when the associated workflow runs a
         `WaitForAction`
         step.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.send_workflow_step_action)
@@ -1064,15 +1064,15 @@
         *,
         resourceArn: str,
         state: ResourceStateTypeDef,
         clientToken: str,
         executionRole: str = ...,
         includeResources: ResourceStateUpdateIncludeResourcesTypeDef = ...,
         exclusionRules: ResourceStateUpdateExclusionRulesTypeDef = ...,
-        updateAt: TimestampTypeDef = ...
+        updateAt: TimestampTypeDef = ...,
     ) -> StartResourceStateUpdateResponseTypeDef:
         """
         Begin asynchronous resource state update for lifecycle changes to the specified
         image
         resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.start_resource_state_update)
@@ -1097,15 +1097,15 @@
 
     async def update_distribution_configuration(
         self,
         *,
         distributionConfigurationArn: str,
         distributions: Sequence[DistributionTypeDef],
         clientToken: str,
-        description: str = ...
+        description: str = ...,
     ) -> UpdateDistributionConfigurationResponseTypeDef:
         """
         Updates a new distribution configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.update_distribution_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#update_distribution_configuration)
         """
@@ -1122,15 +1122,15 @@
         distributionConfigurationArn: str = ...,
         imageTestsConfiguration: ImageTestsConfigurationTypeDef = ...,
         enhancedImageMetadataEnabled: bool = ...,
         schedule: ScheduleTypeDef = ...,
         status: PipelineStatusType = ...,
         imageScanningConfiguration: ImageScanningConfigurationTypeDef = ...,
         workflows: Sequence[WorkflowConfigurationTypeDef] = ...,
-        executionRole: str = ...
+        executionRole: str = ...,
     ) -> UpdateImagePipelineResponseTypeDef:
         """
         Updates an image pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.update_image_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#update_image_pipeline)
         """
@@ -1146,15 +1146,15 @@
         securityGroupIds: Sequence[str] = ...,
         subnetId: str = ...,
         logging: LoggingTypeDef = ...,
         keyPair: str = ...,
         terminateInstanceOnFailure: bool = ...,
         snsTopicArn: str = ...,
         resourceTags: Mapping[str, str] = ...,
-        instanceMetadataOptions: InstanceMetadataOptionsTypeDef = ...
+        instanceMetadataOptions: InstanceMetadataOptionsTypeDef = ...,
     ) -> UpdateInfrastructureConfigurationResponseTypeDef:
         """
         Updates a new infrastructure configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.update_infrastructure_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#update_infrastructure_configuration)
         """
@@ -1165,15 +1165,15 @@
         lifecyclePolicyArn: str,
         executionRole: str,
         resourceType: LifecyclePolicyResourceTypeType,
         policyDetails: Sequence[LifecyclePolicyDetailTypeDef],
         resourceSelection: LifecyclePolicyResourceSelectionTypeDef,
         clientToken: str,
         description: str = ...,
-        status: LifecyclePolicyStatusType = ...
+        status: LifecyclePolicyStatusType = ...,
     ) -> UpdateLifecyclePolicyResponseTypeDef:
         """
         Update the specified lifecycle policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.update_lifecycle_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#update_lifecycle_policy)
         """
```

### Comparing `types-aiobotocore-imagebuilder-2.9.0/types_aiobotocore_imagebuilder/literals.py` & `types-aiobotocore-imagebuilder-2.9.1/types_aiobotocore_imagebuilder/literals.py`

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
     "BuildTypeType",
     "ComponentFormatType",
     "ComponentStatusType",
     "ComponentTypeType",
     "ContainerRepositoryServiceType",
     "ContainerTypeType",
@@ -54,15 +53,14 @@
     "WorkflowStepExecutionStatusType",
     "WorkflowTypeType",
     "imagebuilderServiceName",
     "ServiceName",
     "ResourceServiceName",
 )
 
-
 BuildTypeType = Literal["IMPORT", "SCHEDULED", "USER_INITIATED"]
 ComponentFormatType = Literal["SHELL"]
 ComponentStatusType = Literal["DEPRECATED"]
 ComponentTypeType = Literal["BUILD", "TEST"]
 ContainerRepositoryServiceType = Literal["ECR"]
 ContainerTypeType = Literal["DOCKER"]
 DiskImageFormatType = Literal["RAW", "VHD", "VMDK"]
```

### Comparing `types-aiobotocore-imagebuilder-2.9.0/types_aiobotocore_imagebuilder/literals.pyi` & `types-aiobotocore-imagebuilder-2.9.1/types_aiobotocore_imagebuilder/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-imagebuilder-2.9.0/types_aiobotocore_imagebuilder/type_defs.py` & `types-aiobotocore-imagebuilder-2.9.1/types_aiobotocore_imagebuilder/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "SeverityCountsTypeDef",
     "SystemsManagerAgentTypeDef",
     "LaunchPermissionConfigurationTypeDef",
     "ImageStateTypeDef",
     "CancelImageCreationRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
```

### Comparing `types-aiobotocore-imagebuilder-2.9.0/types_aiobotocore_imagebuilder/type_defs.pyi` & `types-aiobotocore-imagebuilder-2.9.1/types_aiobotocore_imagebuilder/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-imagebuilder-2.9.0/types_aiobotocore_imagebuilder.egg-info/PKG-INFO` & `types-aiobotocore-imagebuilder-2.9.1/types_aiobotocore_imagebuilder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-imagebuilder
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.imagebuilder 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.imagebuilder 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/
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
 
 <a id="types-aiobotocore-imagebuilder"></a>
 
 # types-aiobotocore-imagebuilder
 
 [![PyPI - types-aiobotocore-imagebuilder](https://img.shields.io/pypi/v/types-aiobotocore-imagebuilder.svg?color=blue)](https://pypi.org/project/types-aiobotocore-imagebuilder)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-imagebuilder.svg?color=blue)](https://pypi.org/project/types-aiobotocore-imagebuilder)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-imagebuilder)](https://pepy.tech/project/types-aiobotocore-imagebuilder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.imagebuilder 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder)
+[aiobotocore.imagebuilder 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder)
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
 [types-aiobotocore-imagebuilder docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-imagebuilder-2.9.0/types_aiobotocore_imagebuilder.egg-info/SOURCES.txt` & `types-aiobotocore-imagebuilder-2.9.1/types_aiobotocore_imagebuilder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

