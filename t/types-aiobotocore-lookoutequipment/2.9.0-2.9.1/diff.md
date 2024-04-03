# Comparing `tmp/types-aiobotocore-lookoutequipment-2.9.0.tar.gz` & `tmp/types-aiobotocore-lookoutequipment-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-lookoutequipment-2.9.0.tar", last modified: Wed Dec 13 19:59:47 2023, max compression
+gzip compressed data, was "types-aiobotocore-lookoutequipment-2.9.1.tar", last modified: Thu Jan 18 01:21:09 2024, max compression
```

## Comparing `types-aiobotocore-lookoutequipment-2.9.0.tar` & `types-aiobotocore-lookoutequipment-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:47.473512 types-aiobotocore-lookoutequipment-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:49:27.000000 types-aiobotocore-lookoutequipment-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12722 2023-12-13 19:59:47.473512 types-aiobotocore-lookoutequipment-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11123 2023-12-13 19:49:27.000000 types-aiobotocore-lookoutequipment-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:47.473512 types-aiobotocore-lookoutequipment-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2023-12-13 19:49:27.000000 types-aiobotocore-lookoutequipment-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:47.469512 types-aiobotocore-lookoutequipment-2.9.0/types_aiobotocore_lookoutequipment/
--rw-r--r--   0 runner    (1001) docker     (127)      515 2023-12-13 19:49:27.000000 types-aiobotocore-lookoutequipment-2.9.0/types_aiobotocore_lookoutequipment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2023-12-13 19:49:27.000000 types-aiobotocore-lookoutequipment-2.9.0/types_aiobotocore_lookoutequipment/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      968 2023-12-13 19:49:27.000000 types-aiobotocore-lookoutequipment-2.9.0/types_aiobotocore_lookoutequipment/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38891 2023-12-13 19:49:28.000000 types-aiobotocore-lookoutequipment-2.9.0/types_aiobotocore_lookoutequipment/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    38888 2023-12-13 19:49:27.000000 types-aiobotocore-lookoutequipment-2.9.0/types_aiobotocore_lookoutequipment/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10266 2023-12-13 19:49:28.000000 types-aiobotocore-lookoutequipment-2.9.0/types_aiobotocore_lookoutequipment/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10264 2023-12-13 19:49:28.000000 types-aiobotocore-lookoutequipment-2.9.0/types_aiobotocore_lookoutequipment/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:49:27.000000 types-aiobotocore-lookoutequipment-2.9.0/types_aiobotocore_lookoutequipment/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    44209 2023-12-13 19:49:28.000000 types-aiobotocore-lookoutequipment-2.9.0/types_aiobotocore_lookoutequipment/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    44208 2023-12-13 19:49:28.000000 types-aiobotocore-lookoutequipment-2.9.0/types_aiobotocore_lookoutequipment/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:49:27.000000 types-aiobotocore-lookoutequipment-2.9.0/types_aiobotocore_lookoutequipment/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:47.473512 types-aiobotocore-lookoutequipment-2.9.0/types_aiobotocore_lookoutequipment.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12722 2023-12-13 19:59:47.000000 types-aiobotocore-lookoutequipment-2.9.0/types_aiobotocore_lookoutequipment.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      887 2023-12-13 19:59:47.000000 types-aiobotocore-lookoutequipment-2.9.0/types_aiobotocore_lookoutequipment.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:47.000000 types-aiobotocore-lookoutequipment-2.9.0/types_aiobotocore_lookoutequipment.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:47.000000 types-aiobotocore-lookoutequipment-2.9.0/types_aiobotocore_lookoutequipment.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:47.000000 types-aiobotocore-lookoutequipment-2.9.0/types_aiobotocore_lookoutequipment.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-13 19:59:47.000000 types-aiobotocore-lookoutequipment-2.9.0/types_aiobotocore_lookoutequipment.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:09.825210 types-aiobotocore-lookoutequipment-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:11:14.000000 types-aiobotocore-lookoutequipment-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12742 2024-01-18 01:21:09.825210 types-aiobotocore-lookoutequipment-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11123 2024-01-18 01:11:14.000000 types-aiobotocore-lookoutequipment-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:09.825210 types-aiobotocore-lookoutequipment-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-01-18 01:11:14.000000 types-aiobotocore-lookoutequipment-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:09.825210 types-aiobotocore-lookoutequipment-2.9.1/types_aiobotocore_lookoutequipment/
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-01-18 01:11:14.000000 types-aiobotocore-lookoutequipment-2.9.1/types_aiobotocore_lookoutequipment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-01-18 01:11:14.000000 types-aiobotocore-lookoutequipment-2.9.1/types_aiobotocore_lookoutequipment/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-01-18 01:11:14.000000 types-aiobotocore-lookoutequipment-2.9.1/types_aiobotocore_lookoutequipment/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38913 2024-01-18 01:11:14.000000 types-aiobotocore-lookoutequipment-2.9.1/types_aiobotocore_lookoutequipment/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38910 2024-01-18 01:11:14.000000 types-aiobotocore-lookoutequipment-2.9.1/types_aiobotocore_lookoutequipment/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10264 2024-01-18 01:11:14.000000 types-aiobotocore-lookoutequipment-2.9.1/types_aiobotocore_lookoutequipment/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10264 2024-01-18 01:11:14.000000 types-aiobotocore-lookoutequipment-2.9.1/types_aiobotocore_lookoutequipment/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:11:14.000000 types-aiobotocore-lookoutequipment-2.9.1/types_aiobotocore_lookoutequipment/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    44208 2024-01-18 01:11:15.000000 types-aiobotocore-lookoutequipment-2.9.1/types_aiobotocore_lookoutequipment/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44208 2024-01-18 01:11:15.000000 types-aiobotocore-lookoutequipment-2.9.1/types_aiobotocore_lookoutequipment/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:11:14.000000 types-aiobotocore-lookoutequipment-2.9.1/types_aiobotocore_lookoutequipment/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:09.825210 types-aiobotocore-lookoutequipment-2.9.1/types_aiobotocore_lookoutequipment.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12742 2024-01-18 01:21:09.000000 types-aiobotocore-lookoutequipment-2.9.1/types_aiobotocore_lookoutequipment.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-01-18 01:21:09.000000 types-aiobotocore-lookoutequipment-2.9.1/types_aiobotocore_lookoutequipment.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:09.000000 types-aiobotocore-lookoutequipment-2.9.1/types_aiobotocore_lookoutequipment.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:09.000000 types-aiobotocore-lookoutequipment-2.9.1/types_aiobotocore_lookoutequipment.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:09.000000 types-aiobotocore-lookoutequipment-2.9.1/types_aiobotocore_lookoutequipment.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-18 01:21:09.000000 types-aiobotocore-lookoutequipment-2.9.1/types_aiobotocore_lookoutequipment.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-lookoutequipment-2.9.0/LICENSE` & `types-aiobotocore-lookoutequipment-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-lookoutequipment-2.9.0/PKG-INFO` & `types-aiobotocore-lookoutequipment-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-lookoutequipment
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.LookoutEquipment 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.LookoutEquipment 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/
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
 
 <a id="types-aiobotocore-lookoutequipment"></a>
 
 # types-aiobotocore-lookoutequipment
 
 [![PyPI - types-aiobotocore-lookoutequipment](https://img.shields.io/pypi/v/types-aiobotocore-lookoutequipment.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lookoutequipment)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lookoutequipment.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lookoutequipment)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lookoutequipment)](https://pepy.tech/project/types-aiobotocore-lookoutequipment)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LookoutEquipment 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment)
+[aiobotocore.LookoutEquipment 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment)
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
 [types-aiobotocore-lookoutequipment docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-lookoutequipment-2.9.0/README.md` & `types-aiobotocore-lookoutequipment-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lookoutequipment.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lookoutequipment)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lookoutequipment)](https://pepy.tech/project/types-aiobotocore-lookoutequipment)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LookoutEquipment 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment)
+[aiobotocore.LookoutEquipment 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment)
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
 [types-aiobotocore-lookoutequipment docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-lookoutequipment-2.9.0/setup.py` & `types-aiobotocore-lookoutequipment-2.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-lookoutequipment",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_lookoutequipment"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.LookoutEquipment 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.LookoutEquipment 2.9.1 service generated with"
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
     keywords="aiobotocore lookoutequipment type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_lookoutequipment": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-lookoutequipment-2.9.0/types_aiobotocore_lookoutequipment/__init__.py` & `types-aiobotocore-lookoutequipment-2.9.1/types_aiobotocore_lookoutequipment/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,9 +18,8 @@
     ```
 """
 
 from .client import LookoutEquipmentClient
 
 Client = LookoutEquipmentClient
 
-
 __all__ = ("Client", "LookoutEquipmentClient")
```

### Comparing `types-aiobotocore-lookoutequipment-2.9.0/types_aiobotocore_lookoutequipment/__init__.pyi` & `types-aiobotocore-lookoutequipment-2.9.1/types_aiobotocore_lookoutequipment/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lookoutequipment-2.9.0/types_aiobotocore_lookoutequipment/__main__.py` & `types-aiobotocore-lookoutequipment-2.9.1/types_aiobotocore_lookoutequipment/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.LookoutEquipment 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.LookoutEquipment 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment\nOther"
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

### Comparing `types-aiobotocore-lookoutequipment-2.9.0/types_aiobotocore_lookoutequipment/client.py` & `types-aiobotocore-lookoutequipment-2.9.1/types_aiobotocore_lookoutequipment/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,15 +139,15 @@
     async def create_dataset(
         self,
         *,
         DatasetName: str,
         ClientToken: str,
         DatasetSchema: DatasetSchemaTypeDef = ...,
         ServerSideKmsKeyId: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDatasetResponseTypeDef:
         """
         Creates a container for a collection of data being ingested for analysis.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.create_dataset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#create_dataset)
         """
@@ -160,15 +160,15 @@
         DataUploadFrequency: DataUploadFrequencyType,
         DataInputConfiguration: InferenceInputConfigurationTypeDef,
         DataOutputConfiguration: InferenceOutputConfigurationTypeDef,
         RoleArn: str,
         ClientToken: str,
         DataDelayOffsetInMinutes: int = ...,
         ServerSideKmsKeyId: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateInferenceSchedulerResponseTypeDef:
         """
         Creates a scheduled inference.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.create_inference_scheduler)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#create_inference_scheduler)
         """
@@ -179,30 +179,30 @@
         LabelGroupName: str,
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
         Rating: LabelRatingType,
         ClientToken: str,
         FaultCode: str = ...,
         Notes: str = ...,
-        Equipment: str = ...
+        Equipment: str = ...,
     ) -> CreateLabelResponseTypeDef:
         """
         Creates a label for an event.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.create_label)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#create_label)
         """
 
     async def create_label_group(
         self,
         *,
         LabelGroupName: str,
         ClientToken: str,
         FaultCodes: Sequence[str] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateLabelGroupResponseTypeDef:
         """
         Creates a group of labels.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.create_label_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#create_label_group)
         """
@@ -219,15 +219,15 @@
         TrainingDataEndTime: TimestampTypeDef = ...,
         EvaluationDataStartTime: TimestampTypeDef = ...,
         EvaluationDataEndTime: TimestampTypeDef = ...,
         RoleArn: str = ...,
         DataPreProcessingConfiguration: DataPreProcessingConfigurationTypeDef = ...,
         ServerSideKmsKeyId: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        OffCondition: str = ...
+        OffCondition: str = ...,
     ) -> CreateModelResponseTypeDef:
         """
         Creates a machine learning model for data inference.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.create_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#create_model)
         """
@@ -236,15 +236,15 @@
         self,
         *,
         ModelName: str,
         RetrainingFrequency: str,
         LookbackWindow: str,
         ClientToken: str,
         RetrainingStartDate: TimestampTypeDef = ...,
-        PromoteMode: ModelPromoteModeType = ...
+        PromoteMode: ModelPromoteModeType = ...,
     ) -> CreateRetrainingSchedulerResponseTypeDef:
         """
         Creates a retraining scheduler on the specified model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.create_retraining_scheduler)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#create_retraining_scheduler)
         """
@@ -424,15 +424,15 @@
     async def import_dataset(
         self,
         *,
         SourceDatasetArn: str,
         ClientToken: str,
         DatasetName: str = ...,
         ServerSideKmsKeyId: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> ImportDatasetResponseTypeDef:
         """
         Imports a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.import_dataset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#import_dataset)
         """
@@ -444,30 +444,30 @@
         DatasetName: str,
         ClientToken: str,
         ModelName: str = ...,
         LabelsInputConfiguration: LabelsInputConfigurationTypeDef = ...,
         RoleArn: str = ...,
         ServerSideKmsKeyId: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        InferenceDataImportStrategy: InferenceDataImportStrategyType = ...
+        InferenceDataImportStrategy: InferenceDataImportStrategyType = ...,
     ) -> ImportModelVersionResponseTypeDef:
         """
         Imports a model that has been trained successfully.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.import_model_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#import_model_version)
         """
 
     async def list_data_ingestion_jobs(
         self,
         *,
         DatasetName: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        Status: IngestionJobStatusType = ...
+        Status: IngestionJobStatusType = ...,
     ) -> ListDataIngestionJobsResponseTypeDef:
         """
         Provides a list of all data ingestion jobs, including dataset name and ARN, S3
         location of the input data, status, and so
         on.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.list_data_ingestion_jobs)
@@ -489,15 +489,15 @@
     async def list_inference_events(
         self,
         *,
         InferenceSchedulerName: str,
         IntervalStartTime: TimestampTypeDef,
         IntervalEndTime: TimestampTypeDef,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListInferenceEventsResponseTypeDef:
         """
         Lists all inference events that have been found for the specified inference
         scheduler.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.list_inference_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#list_inference_events)
@@ -507,15 +507,15 @@
         self,
         *,
         InferenceSchedulerName: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         DataStartTimeAfter: TimestampTypeDef = ...,
         DataEndTimeBefore: TimestampTypeDef = ...,
-        Status: InferenceExecutionStatusType = ...
+        Status: InferenceExecutionStatusType = ...,
     ) -> ListInferenceExecutionsResponseTypeDef:
         """
         Lists all inference executions that have been performed by the specified
         inference
         scheduler.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.list_inference_executions)
@@ -525,15 +525,15 @@
     async def list_inference_schedulers(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         InferenceSchedulerNameBeginsWith: str = ...,
         ModelName: str = ...,
-        Status: InferenceSchedulerStatusType = ...
+        Status: InferenceSchedulerStatusType = ...,
     ) -> ListInferenceSchedulersResponseTypeDef:
         """
         Retrieves a list of all inference schedulers currently available for your
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.list_inference_schedulers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#list_inference_schedulers)
@@ -554,15 +554,15 @@
         *,
         LabelGroupName: str,
         IntervalStartTime: TimestampTypeDef = ...,
         IntervalEndTime: TimestampTypeDef = ...,
         FaultCode: str = ...,
         Equipment: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListLabelsResponseTypeDef:
         """
         Provides a list of labels.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.list_labels)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#list_labels)
         """
@@ -574,15 +574,15 @@
         NextToken: str = ...,
         MaxResults: int = ...,
         Status: ModelVersionStatusType = ...,
         SourceType: ModelVersionSourceTypeType = ...,
         CreatedAtEndTime: TimestampTypeDef = ...,
         CreatedAtStartTime: TimestampTypeDef = ...,
         MaxModelVersion: int = ...,
-        MinModelVersion: int = ...
+        MinModelVersion: int = ...,
     ) -> ListModelVersionsResponseTypeDef:
         """
         Generates a list of all model versions for a given model, including the model
         version, model version ARN, and
         status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.list_model_versions)
@@ -592,15 +592,15 @@
     async def list_models(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         Status: ModelStatusType = ...,
         ModelNameBeginsWith: str = ...,
-        DatasetNameBeginsWith: str = ...
+        DatasetNameBeginsWith: str = ...,
     ) -> ListModelsResponseTypeDef:
         """
         Generates a list of all models in the account, including model name and ARN,
         dataset, and
         status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.list_models)
@@ -609,15 +609,15 @@
 
     async def list_retraining_schedulers(
         self,
         *,
         ModelNameBeginsWith: str = ...,
         Status: RetrainingSchedulerStatusType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListRetrainingSchedulersResponseTypeDef:
         """
         Lists all retraining schedulers in your account, filtering by model name prefix
         and
         status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.list_retraining_schedulers)
@@ -626,15 +626,15 @@
 
     async def list_sensor_statistics(
         self,
         *,
         DatasetName: str,
         IngestionJobId: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListSensorStatisticsResponseTypeDef:
         """
         Lists statistics about the data collected for each of the sensors that have
         been successfully ingested in the particular
         dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.list_sensor_statistics)
@@ -653,30 +653,30 @@
 
     async def put_resource_policy(
         self,
         *,
         ResourceArn: str,
         ResourcePolicy: str,
         ClientToken: str,
-        PolicyRevisionId: str = ...
+        PolicyRevisionId: str = ...,
     ) -> PutResourcePolicyResponseTypeDef:
         """
         Creates a resource control policy for a given resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.put_resource_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#put_resource_policy)
         """
 
     async def start_data_ingestion_job(
         self,
         *,
         DatasetName: str,
         IngestionInputConfiguration: IngestionInputConfigurationTypeDef,
         RoleArn: str,
-        ClientToken: str
+        ClientToken: str,
     ) -> StartDataIngestionJobResponseTypeDef:
         """
         Starts a data ingestion job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.start_data_ingestion_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#start_data_ingestion_job)
         """
@@ -751,15 +751,15 @@
         self,
         *,
         InferenceSchedulerName: str,
         DataDelayOffsetInMinutes: int = ...,
         DataUploadFrequency: DataUploadFrequencyType = ...,
         DataInputConfiguration: InferenceInputConfigurationTypeDef = ...,
         DataOutputConfiguration: InferenceOutputConfigurationTypeDef = ...,
-        RoleArn: str = ...
+        RoleArn: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates an inference scheduler.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.update_inference_scheduler)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#update_inference_scheduler)
         """
@@ -775,15 +775,15 @@
         """
 
     async def update_model(
         self,
         *,
         ModelName: str,
         LabelsInputConfiguration: LabelsInputConfigurationTypeDef = ...,
-        RoleArn: str = ...
+        RoleArn: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a model in the account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.update_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#update_model)
         """
@@ -791,15 +791,15 @@
     async def update_retraining_scheduler(
         self,
         *,
         ModelName: str,
         RetrainingStartDate: TimestampTypeDef = ...,
         RetrainingFrequency: str = ...,
         LookbackWindow: str = ...,
-        PromoteMode: ModelPromoteModeType = ...
+        PromoteMode: ModelPromoteModeType = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a retraining scheduler.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.update_retraining_scheduler)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#update_retraining_scheduler)
         """
```

### Comparing `types-aiobotocore-lookoutequipment-2.9.0/types_aiobotocore_lookoutequipment/client.pyi` & `types-aiobotocore-lookoutequipment-2.9.1/types_aiobotocore_lookoutequipment/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,15 @@
     async def create_dataset(
         self,
         *,
         DatasetName: str,
         ClientToken: str,
         DatasetSchema: DatasetSchemaTypeDef = ...,
         ServerSideKmsKeyId: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDatasetResponseTypeDef:
         """
         Creates a container for a collection of data being ingested for analysis.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.create_dataset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#create_dataset)
         """
@@ -157,15 +157,15 @@
         DataUploadFrequency: DataUploadFrequencyType,
         DataInputConfiguration: InferenceInputConfigurationTypeDef,
         DataOutputConfiguration: InferenceOutputConfigurationTypeDef,
         RoleArn: str,
         ClientToken: str,
         DataDelayOffsetInMinutes: int = ...,
         ServerSideKmsKeyId: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateInferenceSchedulerResponseTypeDef:
         """
         Creates a scheduled inference.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.create_inference_scheduler)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#create_inference_scheduler)
         """
@@ -176,30 +176,30 @@
         LabelGroupName: str,
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
         Rating: LabelRatingType,
         ClientToken: str,
         FaultCode: str = ...,
         Notes: str = ...,
-        Equipment: str = ...
+        Equipment: str = ...,
     ) -> CreateLabelResponseTypeDef:
         """
         Creates a label for an event.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.create_label)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#create_label)
         """
 
     async def create_label_group(
         self,
         *,
         LabelGroupName: str,
         ClientToken: str,
         FaultCodes: Sequence[str] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateLabelGroupResponseTypeDef:
         """
         Creates a group of labels.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.create_label_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#create_label_group)
         """
@@ -216,15 +216,15 @@
         TrainingDataEndTime: TimestampTypeDef = ...,
         EvaluationDataStartTime: TimestampTypeDef = ...,
         EvaluationDataEndTime: TimestampTypeDef = ...,
         RoleArn: str = ...,
         DataPreProcessingConfiguration: DataPreProcessingConfigurationTypeDef = ...,
         ServerSideKmsKeyId: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        OffCondition: str = ...
+        OffCondition: str = ...,
     ) -> CreateModelResponseTypeDef:
         """
         Creates a machine learning model for data inference.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.create_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#create_model)
         """
@@ -233,15 +233,15 @@
         self,
         *,
         ModelName: str,
         RetrainingFrequency: str,
         LookbackWindow: str,
         ClientToken: str,
         RetrainingStartDate: TimestampTypeDef = ...,
-        PromoteMode: ModelPromoteModeType = ...
+        PromoteMode: ModelPromoteModeType = ...,
     ) -> CreateRetrainingSchedulerResponseTypeDef:
         """
         Creates a retraining scheduler on the specified model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.create_retraining_scheduler)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#create_retraining_scheduler)
         """
@@ -421,15 +421,15 @@
     async def import_dataset(
         self,
         *,
         SourceDatasetArn: str,
         ClientToken: str,
         DatasetName: str = ...,
         ServerSideKmsKeyId: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> ImportDatasetResponseTypeDef:
         """
         Imports a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.import_dataset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#import_dataset)
         """
@@ -441,30 +441,30 @@
         DatasetName: str,
         ClientToken: str,
         ModelName: str = ...,
         LabelsInputConfiguration: LabelsInputConfigurationTypeDef = ...,
         RoleArn: str = ...,
         ServerSideKmsKeyId: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        InferenceDataImportStrategy: InferenceDataImportStrategyType = ...
+        InferenceDataImportStrategy: InferenceDataImportStrategyType = ...,
     ) -> ImportModelVersionResponseTypeDef:
         """
         Imports a model that has been trained successfully.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.import_model_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#import_model_version)
         """
 
     async def list_data_ingestion_jobs(
         self,
         *,
         DatasetName: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        Status: IngestionJobStatusType = ...
+        Status: IngestionJobStatusType = ...,
     ) -> ListDataIngestionJobsResponseTypeDef:
         """
         Provides a list of all data ingestion jobs, including dataset name and ARN, S3
         location of the input data, status, and so
         on.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.list_data_ingestion_jobs)
@@ -486,15 +486,15 @@
     async def list_inference_events(
         self,
         *,
         InferenceSchedulerName: str,
         IntervalStartTime: TimestampTypeDef,
         IntervalEndTime: TimestampTypeDef,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListInferenceEventsResponseTypeDef:
         """
         Lists all inference events that have been found for the specified inference
         scheduler.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.list_inference_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#list_inference_events)
@@ -504,15 +504,15 @@
         self,
         *,
         InferenceSchedulerName: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         DataStartTimeAfter: TimestampTypeDef = ...,
         DataEndTimeBefore: TimestampTypeDef = ...,
-        Status: InferenceExecutionStatusType = ...
+        Status: InferenceExecutionStatusType = ...,
     ) -> ListInferenceExecutionsResponseTypeDef:
         """
         Lists all inference executions that have been performed by the specified
         inference
         scheduler.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.list_inference_executions)
@@ -522,15 +522,15 @@
     async def list_inference_schedulers(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         InferenceSchedulerNameBeginsWith: str = ...,
         ModelName: str = ...,
-        Status: InferenceSchedulerStatusType = ...
+        Status: InferenceSchedulerStatusType = ...,
     ) -> ListInferenceSchedulersResponseTypeDef:
         """
         Retrieves a list of all inference schedulers currently available for your
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.list_inference_schedulers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#list_inference_schedulers)
@@ -551,15 +551,15 @@
         *,
         LabelGroupName: str,
         IntervalStartTime: TimestampTypeDef = ...,
         IntervalEndTime: TimestampTypeDef = ...,
         FaultCode: str = ...,
         Equipment: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListLabelsResponseTypeDef:
         """
         Provides a list of labels.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.list_labels)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#list_labels)
         """
@@ -571,15 +571,15 @@
         NextToken: str = ...,
         MaxResults: int = ...,
         Status: ModelVersionStatusType = ...,
         SourceType: ModelVersionSourceTypeType = ...,
         CreatedAtEndTime: TimestampTypeDef = ...,
         CreatedAtStartTime: TimestampTypeDef = ...,
         MaxModelVersion: int = ...,
-        MinModelVersion: int = ...
+        MinModelVersion: int = ...,
     ) -> ListModelVersionsResponseTypeDef:
         """
         Generates a list of all model versions for a given model, including the model
         version, model version ARN, and
         status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.list_model_versions)
@@ -589,15 +589,15 @@
     async def list_models(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         Status: ModelStatusType = ...,
         ModelNameBeginsWith: str = ...,
-        DatasetNameBeginsWith: str = ...
+        DatasetNameBeginsWith: str = ...,
     ) -> ListModelsResponseTypeDef:
         """
         Generates a list of all models in the account, including model name and ARN,
         dataset, and
         status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.list_models)
@@ -606,15 +606,15 @@
 
     async def list_retraining_schedulers(
         self,
         *,
         ModelNameBeginsWith: str = ...,
         Status: RetrainingSchedulerStatusType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListRetrainingSchedulersResponseTypeDef:
         """
         Lists all retraining schedulers in your account, filtering by model name prefix
         and
         status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.list_retraining_schedulers)
@@ -623,15 +623,15 @@
 
     async def list_sensor_statistics(
         self,
         *,
         DatasetName: str,
         IngestionJobId: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListSensorStatisticsResponseTypeDef:
         """
         Lists statistics about the data collected for each of the sensors that have
         been successfully ingested in the particular
         dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.list_sensor_statistics)
@@ -650,30 +650,30 @@
 
     async def put_resource_policy(
         self,
         *,
         ResourceArn: str,
         ResourcePolicy: str,
         ClientToken: str,
-        PolicyRevisionId: str = ...
+        PolicyRevisionId: str = ...,
     ) -> PutResourcePolicyResponseTypeDef:
         """
         Creates a resource control policy for a given resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.put_resource_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#put_resource_policy)
         """
 
     async def start_data_ingestion_job(
         self,
         *,
         DatasetName: str,
         IngestionInputConfiguration: IngestionInputConfigurationTypeDef,
         RoleArn: str,
-        ClientToken: str
+        ClientToken: str,
     ) -> StartDataIngestionJobResponseTypeDef:
         """
         Starts a data ingestion job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.start_data_ingestion_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#start_data_ingestion_job)
         """
@@ -748,15 +748,15 @@
         self,
         *,
         InferenceSchedulerName: str,
         DataDelayOffsetInMinutes: int = ...,
         DataUploadFrequency: DataUploadFrequencyType = ...,
         DataInputConfiguration: InferenceInputConfigurationTypeDef = ...,
         DataOutputConfiguration: InferenceOutputConfigurationTypeDef = ...,
-        RoleArn: str = ...
+        RoleArn: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates an inference scheduler.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.update_inference_scheduler)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#update_inference_scheduler)
         """
@@ -772,15 +772,15 @@
         """
 
     async def update_model(
         self,
         *,
         ModelName: str,
         LabelsInputConfiguration: LabelsInputConfigurationTypeDef = ...,
-        RoleArn: str = ...
+        RoleArn: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a model in the account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.update_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#update_model)
         """
@@ -788,15 +788,15 @@
     async def update_retraining_scheduler(
         self,
         *,
         ModelName: str,
         RetrainingStartDate: TimestampTypeDef = ...,
         RetrainingFrequency: str = ...,
         LookbackWindow: str = ...,
-        PromoteMode: ModelPromoteModeType = ...
+        PromoteMode: ModelPromoteModeType = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a retraining scheduler.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.update_retraining_scheduler)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#update_retraining_scheduler)
         """
```

### Comparing `types-aiobotocore-lookoutequipment-2.9.0/types_aiobotocore_lookoutequipment/literals.py` & `types-aiobotocore-lookoutequipment-2.9.1/types_aiobotocore_lookoutequipment/literals.py`

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
     "AutoPromotionResultType",
     "DataUploadFrequencyType",
     "DatasetStatusType",
     "InferenceDataImportStrategyType",
     "InferenceExecutionStatusType",
     "InferenceSchedulerStatusType",
@@ -40,15 +39,14 @@
     "TargetSamplingRateType",
     "LookoutEquipmentServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 AutoPromotionResultType = Literal[
     "MODEL_NOT_PROMOTED",
     "MODEL_PROMOTED",
     "RETRAINING_CANCELLED",
     "RETRAINING_CUSTOMER_ERROR",
     "RETRAINING_INTERNAL_ERROR",
 ]
```

### Comparing `types-aiobotocore-lookoutequipment-2.9.0/types_aiobotocore_lookoutequipment/literals.pyi` & `types-aiobotocore-lookoutequipment-2.9.1/types_aiobotocore_lookoutequipment/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lookoutequipment-2.9.0/types_aiobotocore_lookoutequipment/type_defs.py` & `types-aiobotocore-lookoutequipment-2.9.1/types_aiobotocore_lookoutequipment/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CategoricalValuesTypeDef",
     "CountPercentTypeDef",
     "DatasetSchemaTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "TimestampTypeDef",
```

### Comparing `types-aiobotocore-lookoutequipment-2.9.0/types_aiobotocore_lookoutequipment/type_defs.pyi` & `types-aiobotocore-lookoutequipment-2.9.1/types_aiobotocore_lookoutequipment/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lookoutequipment-2.9.0/types_aiobotocore_lookoutequipment.egg-info/PKG-INFO` & `types-aiobotocore-lookoutequipment-2.9.1/types_aiobotocore_lookoutequipment.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-lookoutequipment
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.LookoutEquipment 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.LookoutEquipment 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/
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
 
 <a id="types-aiobotocore-lookoutequipment"></a>
 
 # types-aiobotocore-lookoutequipment
 
 [![PyPI - types-aiobotocore-lookoutequipment](https://img.shields.io/pypi/v/types-aiobotocore-lookoutequipment.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lookoutequipment)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lookoutequipment.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lookoutequipment)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lookoutequipment)](https://pepy.tech/project/types-aiobotocore-lookoutequipment)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LookoutEquipment 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment)
+[aiobotocore.LookoutEquipment 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment)
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
 [types-aiobotocore-lookoutequipment docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-lookoutequipment-2.9.0/types_aiobotocore_lookoutequipment.egg-info/SOURCES.txt` & `types-aiobotocore-lookoutequipment-2.9.1/types_aiobotocore_lookoutequipment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

