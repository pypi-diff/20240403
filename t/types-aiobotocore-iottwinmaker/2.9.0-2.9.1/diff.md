# Comparing `tmp/types-aiobotocore-iottwinmaker-2.9.0.tar.gz` & `tmp/types-aiobotocore-iottwinmaker-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iottwinmaker-2.9.0.tar", last modified: Wed Dec 13 19:59:35 2023, max compression
+gzip compressed data, was "types-aiobotocore-iottwinmaker-2.9.1.tar", last modified: Thu Jan 18 01:20:58 2024, max compression
```

## Comparing `types-aiobotocore-iottwinmaker-2.9.0.tar` & `types-aiobotocore-iottwinmaker-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:35.501609 types-aiobotocore-iottwinmaker-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:48:09.000000 types-aiobotocore-iottwinmaker-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12490 2023-12-13 19:59:35.501609 types-aiobotocore-iottwinmaker-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10907 2023-12-13 19:48:09.000000 types-aiobotocore-iottwinmaker-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:35.501609 types-aiobotocore-iottwinmaker-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2023-12-13 19:48:09.000000 types-aiobotocore-iottwinmaker-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:35.497609 types-aiobotocore-iottwinmaker-2.9.0/types_aiobotocore_iottwinmaker/
--rw-r--r--   0 runner    (1001) docker     (127)      483 2023-12-13 19:48:09.000000 types-aiobotocore-iottwinmaker-2.9.0/types_aiobotocore_iottwinmaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2023-12-13 19:48:09.000000 types-aiobotocore-iottwinmaker-2.9.0/types_aiobotocore_iottwinmaker/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      952 2023-12-13 19:48:09.000000 types-aiobotocore-iottwinmaker-2.9.0/types_aiobotocore_iottwinmaker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31488 2023-12-13 19:48:09.000000 types-aiobotocore-iottwinmaker-2.9.0/types_aiobotocore_iottwinmaker/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    31485 2023-12-13 19:48:09.000000 types-aiobotocore-iottwinmaker-2.9.0/types_aiobotocore_iottwinmaker/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10650 2023-12-13 19:48:09.000000 types-aiobotocore-iottwinmaker-2.9.0/types_aiobotocore_iottwinmaker/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10648 2023-12-13 19:48:09.000000 types-aiobotocore-iottwinmaker-2.9.0/types_aiobotocore_iottwinmaker/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:48:09.000000 types-aiobotocore-iottwinmaker-2.9.0/types_aiobotocore_iottwinmaker/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    47422 2023-12-13 19:48:12.000000 types-aiobotocore-iottwinmaker-2.9.0/types_aiobotocore_iottwinmaker/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    47421 2023-12-13 19:48:10.000000 types-aiobotocore-iottwinmaker-2.9.0/types_aiobotocore_iottwinmaker/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:48:09.000000 types-aiobotocore-iottwinmaker-2.9.0/types_aiobotocore_iottwinmaker/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:35.497609 types-aiobotocore-iottwinmaker-2.9.0/types_aiobotocore_iottwinmaker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12490 2023-12-13 19:59:35.000000 types-aiobotocore-iottwinmaker-2.9.0/types_aiobotocore_iottwinmaker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      819 2023-12-13 19:59:35.000000 types-aiobotocore-iottwinmaker-2.9.0/types_aiobotocore_iottwinmaker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:35.000000 types-aiobotocore-iottwinmaker-2.9.0/types_aiobotocore_iottwinmaker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:35.000000 types-aiobotocore-iottwinmaker-2.9.0/types_aiobotocore_iottwinmaker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:35.000000 types-aiobotocore-iottwinmaker-2.9.0/types_aiobotocore_iottwinmaker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-13 19:59:35.000000 types-aiobotocore-iottwinmaker-2.9.0/types_aiobotocore_iottwinmaker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:58.785259 types-aiobotocore-iottwinmaker-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:09:58.000000 types-aiobotocore-iottwinmaker-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12510 2024-01-18 01:20:58.785259 types-aiobotocore-iottwinmaker-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10907 2024-01-18 01:09:58.000000 types-aiobotocore-iottwinmaker-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:58.785259 types-aiobotocore-iottwinmaker-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-01-18 01:09:58.000000 types-aiobotocore-iottwinmaker-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:58.781259 types-aiobotocore-iottwinmaker-2.9.1/types_aiobotocore_iottwinmaker/
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-01-18 01:09:58.000000 types-aiobotocore-iottwinmaker-2.9.1/types_aiobotocore_iottwinmaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-01-18 01:09:58.000000 types-aiobotocore-iottwinmaker-2.9.1/types_aiobotocore_iottwinmaker/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-01-18 01:09:58.000000 types-aiobotocore-iottwinmaker-2.9.1/types_aiobotocore_iottwinmaker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31504 2024-01-18 01:09:59.000000 types-aiobotocore-iottwinmaker-2.9.1/types_aiobotocore_iottwinmaker/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31501 2024-01-18 01:09:58.000000 types-aiobotocore-iottwinmaker-2.9.1/types_aiobotocore_iottwinmaker/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10648 2024-01-18 01:09:59.000000 types-aiobotocore-iottwinmaker-2.9.1/types_aiobotocore_iottwinmaker/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10648 2024-01-18 01:09:59.000000 types-aiobotocore-iottwinmaker-2.9.1/types_aiobotocore_iottwinmaker/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:09:58.000000 types-aiobotocore-iottwinmaker-2.9.1/types_aiobotocore_iottwinmaker/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    47421 2024-01-18 01:10:00.000000 types-aiobotocore-iottwinmaker-2.9.1/types_aiobotocore_iottwinmaker/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47421 2024-01-18 01:09:59.000000 types-aiobotocore-iottwinmaker-2.9.1/types_aiobotocore_iottwinmaker/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:09:58.000000 types-aiobotocore-iottwinmaker-2.9.1/types_aiobotocore_iottwinmaker/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:58.785259 types-aiobotocore-iottwinmaker-2.9.1/types_aiobotocore_iottwinmaker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12510 2024-01-18 01:20:58.000000 types-aiobotocore-iottwinmaker-2.9.1/types_aiobotocore_iottwinmaker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-01-18 01:20:58.000000 types-aiobotocore-iottwinmaker-2.9.1/types_aiobotocore_iottwinmaker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:58.000000 types-aiobotocore-iottwinmaker-2.9.1/types_aiobotocore_iottwinmaker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:58.000000 types-aiobotocore-iottwinmaker-2.9.1/types_aiobotocore_iottwinmaker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:58.000000 types-aiobotocore-iottwinmaker-2.9.1/types_aiobotocore_iottwinmaker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-01-18 01:20:58.000000 types-aiobotocore-iottwinmaker-2.9.1/types_aiobotocore_iottwinmaker.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iottwinmaker-2.9.0/LICENSE` & `types-aiobotocore-iottwinmaker-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-iottwinmaker-2.9.0/PKG-INFO` & `types-aiobotocore-iottwinmaker-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iottwinmaker
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.IoTTwinMaker 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.IoTTwinMaker 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/
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
 
 <a id="types-aiobotocore-iottwinmaker"></a>
 
 # types-aiobotocore-iottwinmaker
 
 [![PyPI - types-aiobotocore-iottwinmaker](https://img.shields.io/pypi/v/types-aiobotocore-iottwinmaker.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iottwinmaker)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iottwinmaker.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iottwinmaker)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iottwinmaker)](https://pepy.tech/project/types-aiobotocore-iottwinmaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTTwinMaker 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker)
+[aiobotocore.IoTTwinMaker 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker)
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
 [types-aiobotocore-iottwinmaker docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-iottwinmaker-2.9.0/README.md` & `types-aiobotocore-iottwinmaker-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iottwinmaker.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iottwinmaker)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iottwinmaker)](https://pepy.tech/project/types-aiobotocore-iottwinmaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTTwinMaker 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker)
+[aiobotocore.IoTTwinMaker 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker)
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
 [types-aiobotocore-iottwinmaker docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-iottwinmaker-2.9.0/setup.py` & `types-aiobotocore-iottwinmaker-2.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iottwinmaker",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_iottwinmaker"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.IoTTwinMaker 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.IoTTwinMaker 2.9.1 service generated with"
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
     keywords="aiobotocore iottwinmaker type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_iottwinmaker": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-iottwinmaker-2.9.0/types_aiobotocore_iottwinmaker/__main__.py` & `types-aiobotocore-iottwinmaker-2.9.1/types_aiobotocore_iottwinmaker/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IoTTwinMaker 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.IoTTwinMaker 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker\nOther"
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

### Comparing `types-aiobotocore-iottwinmaker-2.9.0/types_aiobotocore_iottwinmaker/client.py` & `types-aiobotocore-iottwinmaker-2.9.1/types_aiobotocore_iottwinmaker/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,15 +169,15 @@
         description: str = ...,
         propertyDefinitions: Mapping[str, PropertyDefinitionRequestTypeDef] = ...,
         extendsFrom: Sequence[str] = ...,
         functions: Mapping[str, FunctionRequestTypeDef] = ...,
         tags: Mapping[str, str] = ...,
         propertyGroups: Mapping[str, PropertyGroupRequestTypeDef] = ...,
         componentTypeName: str = ...,
-        compositeComponentTypes: Mapping[str, CompositeComponentTypeRequestTypeDef] = ...
+        compositeComponentTypes: Mapping[str, CompositeComponentTypeRequestTypeDef] = ...,
     ) -> CreateComponentTypeResponseTypeDef:
         """
         Creates a component type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.create_component_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#create_component_type)
         """
@@ -188,30 +188,30 @@
         workspaceId: str,
         entityName: str,
         entityId: str = ...,
         description: str = ...,
         components: Mapping[str, ComponentRequestTypeDef] = ...,
         compositeComponents: Mapping[str, CompositeComponentRequestTypeDef] = ...,
         parentEntityId: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateEntityResponseTypeDef:
         """
         Creates an entity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.create_entity)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#create_entity)
         """
 
     async def create_metadata_transfer_job(
         self,
         *,
         sources: Sequence[SourceConfigurationTypeDef],
         destination: DestinationConfigurationTypeDef,
         metadataTransferJobId: str = ...,
-        description: str = ...
+        description: str = ...,
     ) -> CreateMetadataTransferJobResponseTypeDef:
         """
         Creates a new metadata transfer job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.create_metadata_transfer_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#create_metadata_transfer_job)
         """
@@ -221,15 +221,15 @@
         *,
         workspaceId: str,
         sceneId: str,
         contentLocation: str,
         description: str = ...,
         capabilities: Sequence[str] = ...,
         tags: Mapping[str, str] = ...,
-        sceneMetadata: Mapping[str, str] = ...
+        sceneMetadata: Mapping[str, str] = ...,
     ) -> CreateSceneResponseTypeDef:
         """
         Creates a scene.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.create_scene)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#create_scene)
         """
@@ -247,15 +247,15 @@
     async def create_workspace(
         self,
         *,
         workspaceId: str,
         description: str = ...,
         s3Location: str = ...,
         role: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateWorkspaceResponseTypeDef:
         """
         Creates a workplace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.create_workspace)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#create_workspace)
         """
@@ -376,15 +376,15 @@
         componentName: str = ...,
         componentPath: str = ...,
         componentTypeId: str = ...,
         entityId: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         propertyGroupName: str = ...,
-        tabularConditions: TabularConditionsTypeDef = ...
+        tabularConditions: TabularConditionsTypeDef = ...,
     ) -> GetPropertyValueResponseTypeDef:
         """
         Gets the property values for a component, component type, entity, or workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.get_property_value)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#get_property_value)
         """
@@ -402,15 +402,15 @@
         startDateTime: TimestampTypeDef = ...,
         endDateTime: TimestampTypeDef = ...,
         interpolation: InterpolationParametersTypeDef = ...,
         nextToken: str = ...,
         maxResults: int = ...,
         orderByTime: OrderByTimeType = ...,
         startTime: str = ...,
-        endTime: str = ...
+        endTime: str = ...,
     ) -> GetPropertyValueHistoryResponseTypeDef:
         """
         Retrieves information about the history of a time series property value for a
         component, component type, entity, or
         workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.get_property_value_history)
@@ -445,15 +445,15 @@
 
     async def list_component_types(
         self,
         *,
         workspaceId: str,
         filters: Sequence[ListComponentTypesFilterTypeDef] = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListComponentTypesResponseTypeDef:
         """
         Lists all component types in a workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.list_component_types)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#list_component_types)
         """
@@ -461,30 +461,30 @@
     async def list_components(
         self,
         *,
         workspaceId: str,
         entityId: str,
         componentPath: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListComponentsResponseTypeDef:
         """
         This API lists the components of an entity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.list_components)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#list_components)
         """
 
     async def list_entities(
         self,
         *,
         workspaceId: str,
         filters: Sequence[ListEntitiesFilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListEntitiesResponseTypeDef:
         """
         Lists all entities in a workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.list_entities)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#list_entities)
         """
@@ -492,15 +492,15 @@
     async def list_metadata_transfer_jobs(
         self,
         *,
         sourceType: SourceTypeType,
         destinationType: DestinationTypeType,
         filters: Sequence[ListMetadataTransferJobsFilterTypeDef] = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListMetadataTransferJobsResponseTypeDef:
         """
         Lists the metadata transfer jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.list_metadata_transfer_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#list_metadata_transfer_jobs)
         """
@@ -509,15 +509,15 @@
         self,
         *,
         workspaceId: str,
         entityId: str,
         componentName: str = ...,
         componentPath: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListPropertiesResponseTypeDef:
         """
         This API lists the properties of a component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.list_properties)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#list_properties)
         """
@@ -545,15 +545,15 @@
     async def list_sync_resources(
         self,
         *,
         workspaceId: str,
         syncSource: str,
         filters: Sequence[SyncResourceFilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListSyncResourcesResponseTypeDef:
         """
         Lists the sync resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.list_sync_resources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#list_sync_resources)
         """
@@ -602,15 +602,15 @@
         isSingleton: bool = ...,
         description: str = ...,
         propertyDefinitions: Mapping[str, PropertyDefinitionRequestTypeDef] = ...,
         extendsFrom: Sequence[str] = ...,
         functions: Mapping[str, FunctionRequestTypeDef] = ...,
         propertyGroups: Mapping[str, PropertyGroupRequestTypeDef] = ...,
         componentTypeName: str = ...,
-        compositeComponentTypes: Mapping[str, CompositeComponentTypeRequestTypeDef] = ...
+        compositeComponentTypes: Mapping[str, CompositeComponentTypeRequestTypeDef] = ...,
     ) -> UpdateComponentTypeResponseTypeDef:
         """
         Updates information in a component type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.update_component_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#update_component_type)
         """
@@ -620,15 +620,15 @@
         *,
         workspaceId: str,
         entityId: str,
         entityName: str = ...,
         description: str = ...,
         componentUpdates: Mapping[str, ComponentUpdateRequestTypeDef] = ...,
         compositeComponentUpdates: Mapping[str, CompositeComponentUpdateRequestTypeDef] = ...,
-        parentEntityUpdate: ParentEntityUpdateRequestTypeDef = ...
+        parentEntityUpdate: ParentEntityUpdateRequestTypeDef = ...,
     ) -> UpdateEntityResponseTypeDef:
         """
         Updates an entity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.update_entity)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#update_entity)
         """
@@ -647,15 +647,15 @@
         self,
         *,
         workspaceId: str,
         sceneId: str,
         contentLocation: str = ...,
         description: str = ...,
         capabilities: Sequence[str] = ...,
-        sceneMetadata: Mapping[str, str] = ...
+        sceneMetadata: Mapping[str, str] = ...,
     ) -> UpdateSceneResponseTypeDef:
         """
         Updates a scene.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.update_scene)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#update_scene)
         """
```

### Comparing `types-aiobotocore-iottwinmaker-2.9.0/types_aiobotocore_iottwinmaker/client.pyi` & `types-aiobotocore-iottwinmaker-2.9.1/types_aiobotocore_iottwinmaker/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -166,15 +166,15 @@
         description: str = ...,
         propertyDefinitions: Mapping[str, PropertyDefinitionRequestTypeDef] = ...,
         extendsFrom: Sequence[str] = ...,
         functions: Mapping[str, FunctionRequestTypeDef] = ...,
         tags: Mapping[str, str] = ...,
         propertyGroups: Mapping[str, PropertyGroupRequestTypeDef] = ...,
         componentTypeName: str = ...,
-        compositeComponentTypes: Mapping[str, CompositeComponentTypeRequestTypeDef] = ...
+        compositeComponentTypes: Mapping[str, CompositeComponentTypeRequestTypeDef] = ...,
     ) -> CreateComponentTypeResponseTypeDef:
         """
         Creates a component type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.create_component_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#create_component_type)
         """
@@ -185,30 +185,30 @@
         workspaceId: str,
         entityName: str,
         entityId: str = ...,
         description: str = ...,
         components: Mapping[str, ComponentRequestTypeDef] = ...,
         compositeComponents: Mapping[str, CompositeComponentRequestTypeDef] = ...,
         parentEntityId: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateEntityResponseTypeDef:
         """
         Creates an entity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.create_entity)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#create_entity)
         """
 
     async def create_metadata_transfer_job(
         self,
         *,
         sources: Sequence[SourceConfigurationTypeDef],
         destination: DestinationConfigurationTypeDef,
         metadataTransferJobId: str = ...,
-        description: str = ...
+        description: str = ...,
     ) -> CreateMetadataTransferJobResponseTypeDef:
         """
         Creates a new metadata transfer job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.create_metadata_transfer_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#create_metadata_transfer_job)
         """
@@ -218,15 +218,15 @@
         *,
         workspaceId: str,
         sceneId: str,
         contentLocation: str,
         description: str = ...,
         capabilities: Sequence[str] = ...,
         tags: Mapping[str, str] = ...,
-        sceneMetadata: Mapping[str, str] = ...
+        sceneMetadata: Mapping[str, str] = ...,
     ) -> CreateSceneResponseTypeDef:
         """
         Creates a scene.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.create_scene)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#create_scene)
         """
@@ -244,15 +244,15 @@
     async def create_workspace(
         self,
         *,
         workspaceId: str,
         description: str = ...,
         s3Location: str = ...,
         role: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateWorkspaceResponseTypeDef:
         """
         Creates a workplace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.create_workspace)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#create_workspace)
         """
@@ -373,15 +373,15 @@
         componentName: str = ...,
         componentPath: str = ...,
         componentTypeId: str = ...,
         entityId: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         propertyGroupName: str = ...,
-        tabularConditions: TabularConditionsTypeDef = ...
+        tabularConditions: TabularConditionsTypeDef = ...,
     ) -> GetPropertyValueResponseTypeDef:
         """
         Gets the property values for a component, component type, entity, or workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.get_property_value)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#get_property_value)
         """
@@ -399,15 +399,15 @@
         startDateTime: TimestampTypeDef = ...,
         endDateTime: TimestampTypeDef = ...,
         interpolation: InterpolationParametersTypeDef = ...,
         nextToken: str = ...,
         maxResults: int = ...,
         orderByTime: OrderByTimeType = ...,
         startTime: str = ...,
-        endTime: str = ...
+        endTime: str = ...,
     ) -> GetPropertyValueHistoryResponseTypeDef:
         """
         Retrieves information about the history of a time series property value for a
         component, component type, entity, or
         workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.get_property_value_history)
@@ -442,15 +442,15 @@
 
     async def list_component_types(
         self,
         *,
         workspaceId: str,
         filters: Sequence[ListComponentTypesFilterTypeDef] = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListComponentTypesResponseTypeDef:
         """
         Lists all component types in a workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.list_component_types)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#list_component_types)
         """
@@ -458,30 +458,30 @@
     async def list_components(
         self,
         *,
         workspaceId: str,
         entityId: str,
         componentPath: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListComponentsResponseTypeDef:
         """
         This API lists the components of an entity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.list_components)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#list_components)
         """
 
     async def list_entities(
         self,
         *,
         workspaceId: str,
         filters: Sequence[ListEntitiesFilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListEntitiesResponseTypeDef:
         """
         Lists all entities in a workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.list_entities)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#list_entities)
         """
@@ -489,15 +489,15 @@
     async def list_metadata_transfer_jobs(
         self,
         *,
         sourceType: SourceTypeType,
         destinationType: DestinationTypeType,
         filters: Sequence[ListMetadataTransferJobsFilterTypeDef] = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListMetadataTransferJobsResponseTypeDef:
         """
         Lists the metadata transfer jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.list_metadata_transfer_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#list_metadata_transfer_jobs)
         """
@@ -506,15 +506,15 @@
         self,
         *,
         workspaceId: str,
         entityId: str,
         componentName: str = ...,
         componentPath: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListPropertiesResponseTypeDef:
         """
         This API lists the properties of a component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.list_properties)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#list_properties)
         """
@@ -542,15 +542,15 @@
     async def list_sync_resources(
         self,
         *,
         workspaceId: str,
         syncSource: str,
         filters: Sequence[SyncResourceFilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListSyncResourcesResponseTypeDef:
         """
         Lists the sync resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.list_sync_resources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#list_sync_resources)
         """
@@ -599,15 +599,15 @@
         isSingleton: bool = ...,
         description: str = ...,
         propertyDefinitions: Mapping[str, PropertyDefinitionRequestTypeDef] = ...,
         extendsFrom: Sequence[str] = ...,
         functions: Mapping[str, FunctionRequestTypeDef] = ...,
         propertyGroups: Mapping[str, PropertyGroupRequestTypeDef] = ...,
         componentTypeName: str = ...,
-        compositeComponentTypes: Mapping[str, CompositeComponentTypeRequestTypeDef] = ...
+        compositeComponentTypes: Mapping[str, CompositeComponentTypeRequestTypeDef] = ...,
     ) -> UpdateComponentTypeResponseTypeDef:
         """
         Updates information in a component type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.update_component_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#update_component_type)
         """
@@ -617,15 +617,15 @@
         *,
         workspaceId: str,
         entityId: str,
         entityName: str = ...,
         description: str = ...,
         componentUpdates: Mapping[str, ComponentUpdateRequestTypeDef] = ...,
         compositeComponentUpdates: Mapping[str, CompositeComponentUpdateRequestTypeDef] = ...,
-        parentEntityUpdate: ParentEntityUpdateRequestTypeDef = ...
+        parentEntityUpdate: ParentEntityUpdateRequestTypeDef = ...,
     ) -> UpdateEntityResponseTypeDef:
         """
         Updates an entity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.update_entity)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#update_entity)
         """
@@ -644,15 +644,15 @@
         self,
         *,
         workspaceId: str,
         sceneId: str,
         contentLocation: str = ...,
         description: str = ...,
         capabilities: Sequence[str] = ...,
-        sceneMetadata: Mapping[str, str] = ...
+        sceneMetadata: Mapping[str, str] = ...,
     ) -> UpdateSceneResponseTypeDef:
         """
         Updates a scene.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.update_scene)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#update_scene)
         """
```

### Comparing `types-aiobotocore-iottwinmaker-2.9.0/types_aiobotocore_iottwinmaker/literals.py` & `types-aiobotocore-iottwinmaker-2.9.1/types_aiobotocore_iottwinmaker/literals.py`

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
     "ColumnTypeType",
     "ComponentUpdateTypeType",
     "DestinationTypeType",
     "ErrorCodeType",
     "GroupTypeType",
     "InterpolationTypeType",
@@ -46,15 +45,14 @@
     "UpdateReasonType",
     "IoTTwinMakerServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 ColumnTypeType = Literal["EDGE", "NODE", "VALUE"]
 ComponentUpdateTypeType = Literal["CREATE", "DELETE", "UPDATE"]
 DestinationTypeType = Literal["iotsitewise", "iottwinmaker", "s3"]
 ErrorCodeType = Literal[
     "COMPOSITE_COMPONENT_FAILURE",
     "INTERNAL_FAILURE",
     "PROCESSING_ERROR",
```

### Comparing `types-aiobotocore-iottwinmaker-2.9.0/types_aiobotocore_iottwinmaker/literals.pyi` & `types-aiobotocore-iottwinmaker-2.9.1/types_aiobotocore_iottwinmaker/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iottwinmaker-2.9.0/types_aiobotocore_iottwinmaker/type_defs.py` & `types-aiobotocore-iottwinmaker-2.9.1/types_aiobotocore_iottwinmaker/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ResponseMetadataTypeDef",
     "BundleInformationTypeDef",
     "CancelMetadataTransferJobRequestRequestTypeDef",
     "MetadataTransferJobProgressTypeDef",
     "ColumnDescriptionTypeDef",
     "ComponentPropertyGroupRequestTypeDef",
```

### Comparing `types-aiobotocore-iottwinmaker-2.9.0/types_aiobotocore_iottwinmaker/type_defs.pyi` & `types-aiobotocore-iottwinmaker-2.9.1/types_aiobotocore_iottwinmaker/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iottwinmaker-2.9.0/types_aiobotocore_iottwinmaker.egg-info/PKG-INFO` & `types-aiobotocore-iottwinmaker-2.9.1/types_aiobotocore_iottwinmaker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iottwinmaker
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.IoTTwinMaker 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.IoTTwinMaker 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/
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
 
 <a id="types-aiobotocore-iottwinmaker"></a>
 
 # types-aiobotocore-iottwinmaker
 
 [![PyPI - types-aiobotocore-iottwinmaker](https://img.shields.io/pypi/v/types-aiobotocore-iottwinmaker.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iottwinmaker)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iottwinmaker.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iottwinmaker)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iottwinmaker)](https://pepy.tech/project/types-aiobotocore-iottwinmaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTTwinMaker 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker)
+[aiobotocore.IoTTwinMaker 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker)
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
 [types-aiobotocore-iottwinmaker docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-iottwinmaker-2.9.0/types_aiobotocore_iottwinmaker.egg-info/SOURCES.txt` & `types-aiobotocore-iottwinmaker-2.9.1/types_aiobotocore_iottwinmaker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

