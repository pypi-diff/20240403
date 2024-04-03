# Comparing `tmp/types-aiobotocore-bedrock-2.9.0.tar.gz` & `tmp/types-aiobotocore-bedrock-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-bedrock-2.9.0.tar", last modified: Wed Dec 13 19:58:42 2023, max compression
+gzip compressed data, was "types-aiobotocore-bedrock-2.9.1.tar", last modified: Thu Jan 18 01:20:09 2024, max compression
```

## Comparing `types-aiobotocore-bedrock-2.9.0.tar` & `types-aiobotocore-bedrock-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:42.470029 types-aiobotocore-bedrock-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:41:41.000000 types-aiobotocore-bedrock-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13377 2023-12-13 19:58:42.470029 types-aiobotocore-bedrock-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11814 2023-12-13 19:41:41.000000 types-aiobotocore-bedrock-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:42.470029 types-aiobotocore-bedrock-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2023-12-13 19:41:40.000000 types-aiobotocore-bedrock-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:42.470029 types-aiobotocore-bedrock-2.9.0/types_aiobotocore_bedrock/
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2023-12-13 19:41:41.000000 types-aiobotocore-bedrock-2.9.0/types_aiobotocore_bedrock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2023-12-13 19:41:41.000000 types-aiobotocore-bedrock-2.9.0/types_aiobotocore_bedrock/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      932 2023-12-13 19:41:41.000000 types-aiobotocore-bedrock-2.9.0/types_aiobotocore_bedrock/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19968 2023-12-13 19:41:41.000000 types-aiobotocore-bedrock-2.9.0/types_aiobotocore_bedrock/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    19964 2023-12-13 19:41:41.000000 types-aiobotocore-bedrock-2.9.0/types_aiobotocore_bedrock/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9978 2023-12-13 19:41:42.000000 types-aiobotocore-bedrock-2.9.0/types_aiobotocore_bedrock/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9976 2023-12-13 19:41:42.000000 types-aiobotocore-bedrock-2.9.0/types_aiobotocore_bedrock/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5677 2023-12-13 19:41:41.000000 types-aiobotocore-bedrock-2.9.0/types_aiobotocore_bedrock/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5671 2023-12-13 19:41:41.000000 types-aiobotocore-bedrock-2.9.0/types_aiobotocore_bedrock/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:41:41.000000 types-aiobotocore-bedrock-2.9.0/types_aiobotocore_bedrock/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    19939 2023-12-13 19:41:42.000000 types-aiobotocore-bedrock-2.9.0/types_aiobotocore_bedrock/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    19938 2023-12-13 19:41:42.000000 types-aiobotocore-bedrock-2.9.0/types_aiobotocore_bedrock/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:41:41.000000 types-aiobotocore-bedrock-2.9.0/types_aiobotocore_bedrock/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:42.470029 types-aiobotocore-bedrock-2.9.0/types_aiobotocore_bedrock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13377 2023-12-13 19:58:42.000000 types-aiobotocore-bedrock-2.9.0/types_aiobotocore_bedrock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      813 2023-12-13 19:58:42.000000 types-aiobotocore-bedrock-2.9.0/types_aiobotocore_bedrock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:42.000000 types-aiobotocore-bedrock-2.9.0/types_aiobotocore_bedrock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:42.000000 types-aiobotocore-bedrock-2.9.0/types_aiobotocore_bedrock.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:42.000000 types-aiobotocore-bedrock-2.9.0/types_aiobotocore_bedrock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-13 19:58:42.000000 types-aiobotocore-bedrock-2.9.0/types_aiobotocore_bedrock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:09.861490 types-aiobotocore-bedrock-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:03:39.000000 types-aiobotocore-bedrock-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13397 2024-01-18 01:20:09.861490 types-aiobotocore-bedrock-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11814 2024-01-18 01:03:39.000000 types-aiobotocore-bedrock-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:09.861490 types-aiobotocore-bedrock-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-01-18 01:03:39.000000 types-aiobotocore-bedrock-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:09.861490 types-aiobotocore-bedrock-2.9.1/types_aiobotocore_bedrock/
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-01-18 01:03:39.000000 types-aiobotocore-bedrock-2.9.1/types_aiobotocore_bedrock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-01-18 01:03:39.000000 types-aiobotocore-bedrock-2.9.1/types_aiobotocore_bedrock/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-01-18 01:03:39.000000 types-aiobotocore-bedrock-2.9.1/types_aiobotocore_bedrock/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19974 2024-01-18 01:03:39.000000 types-aiobotocore-bedrock-2.9.1/types_aiobotocore_bedrock/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19971 2024-01-18 01:03:39.000000 types-aiobotocore-bedrock-2.9.1/types_aiobotocore_bedrock/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9976 2024-01-18 01:03:39.000000 types-aiobotocore-bedrock-2.9.1/types_aiobotocore_bedrock/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9976 2024-01-18 01:03:39.000000 types-aiobotocore-bedrock-2.9.1/types_aiobotocore_bedrock/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5678 2024-01-18 01:03:39.000000 types-aiobotocore-bedrock-2.9.1/types_aiobotocore_bedrock/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5674 2024-01-18 01:03:39.000000 types-aiobotocore-bedrock-2.9.1/types_aiobotocore_bedrock/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:03:39.000000 types-aiobotocore-bedrock-2.9.1/types_aiobotocore_bedrock/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    19938 2024-01-18 01:03:40.000000 types-aiobotocore-bedrock-2.9.1/types_aiobotocore_bedrock/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19938 2024-01-18 01:03:40.000000 types-aiobotocore-bedrock-2.9.1/types_aiobotocore_bedrock/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:03:39.000000 types-aiobotocore-bedrock-2.9.1/types_aiobotocore_bedrock/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:09.861490 types-aiobotocore-bedrock-2.9.1/types_aiobotocore_bedrock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13397 2024-01-18 01:20:09.000000 types-aiobotocore-bedrock-2.9.1/types_aiobotocore_bedrock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-01-18 01:20:09.000000 types-aiobotocore-bedrock-2.9.1/types_aiobotocore_bedrock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:09.000000 types-aiobotocore-bedrock-2.9.1/types_aiobotocore_bedrock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:09.000000 types-aiobotocore-bedrock-2.9.1/types_aiobotocore_bedrock.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:09.000000 types-aiobotocore-bedrock-2.9.1/types_aiobotocore_bedrock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-01-18 01:20:09.000000 types-aiobotocore-bedrock-2.9.1/types_aiobotocore_bedrock.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-bedrock-2.9.0/LICENSE` & `types-aiobotocore-bedrock-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-bedrock-2.9.0/PKG-INFO` & `types-aiobotocore-bedrock-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-bedrock
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Bedrock 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Bedrock 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock/
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
 
 <a id="types-aiobotocore-bedrock"></a>
 
 # types-aiobotocore-bedrock
 
 [![PyPI - types-aiobotocore-bedrock](https://img.shields.io/pypi/v/types-aiobotocore-bedrock.svg?color=blue)](https://pypi.org/project/types-aiobotocore-bedrock)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-bedrock.svg?color=blue)](https://pypi.org/project/types-aiobotocore-bedrock)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-bedrock)](https://pepy.tech/project/types-aiobotocore-bedrock)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Bedrock 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock)
+[aiobotocore.Bedrock 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock)
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
 [types-aiobotocore-bedrock docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-bedrock-2.9.0/README.md` & `types-aiobotocore-bedrock-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-bedrock.svg?color=blue)](https://pypi.org/project/types-aiobotocore-bedrock)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-bedrock)](https://pepy.tech/project/types-aiobotocore-bedrock)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Bedrock 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock)
+[aiobotocore.Bedrock 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock)
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
 [types-aiobotocore-bedrock docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-bedrock-2.9.0/setup.py` & `types-aiobotocore-bedrock-2.9.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-bedrock",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_bedrock"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Bedrock 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.Bedrock 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore bedrock type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_bedrock": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-bedrock-2.9.0/types_aiobotocore_bedrock/__init__.py` & `types-aiobotocore-bedrock-2.9.1/types_aiobotocore_bedrock/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     ListCustomModelsPaginator,
     ListModelCustomizationJobsPaginator,
     ListProvisionedModelThroughputsPaginator,
 )
 
 Client = BedrockClient
 
-
 __all__ = (
     "BedrockClient",
     "Client",
     "ListCustomModelsPaginator",
     "ListModelCustomizationJobsPaginator",
     "ListProvisionedModelThroughputsPaginator",
 )
```

### Comparing `types-aiobotocore-bedrock-2.9.0/types_aiobotocore_bedrock/__init__.pyi` & `types-aiobotocore-bedrock-2.9.1/types_aiobotocore_bedrock/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-bedrock-2.9.0/types_aiobotocore_bedrock/__main__.py` & `types-aiobotocore-bedrock-2.9.1/types_aiobotocore_bedrock/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Bedrock 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Bedrock 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock\nOther"
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

### Comparing `types-aiobotocore-bedrock-2.9.0/types_aiobotocore_bedrock/client.py` & `types-aiobotocore-bedrock-2.9.1/types_aiobotocore_bedrock/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("BedrockClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -132,15 +131,15 @@
         hyperParameters: Mapping[str, str],
         clientRequestToken: str = ...,
         customizationType: CustomizationTypeType = ...,
         customModelKmsKeyId: str = ...,
         jobTags: Sequence[TagTypeDef] = ...,
         customModelTags: Sequence[TagTypeDef] = ...,
         validationDataConfig: ValidationDataConfigTypeDef = ...,
-        vpcConfig: VpcConfigTypeDef = ...
+        vpcConfig: VpcConfigTypeDef = ...,
     ) -> CreateModelCustomizationJobResponseTypeDef:
         """
         Creates a fine-tuning job to customize a base model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.create_model_customization_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock/client/#create_model_customization_job)
         """
@@ -149,15 +148,15 @@
         self,
         *,
         modelUnits: int,
         provisionedModelName: str,
         modelId: str,
         clientRequestToken: str = ...,
         commitmentDuration: CommitmentDurationType = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateProvisionedModelThroughputResponseTypeDef:
         """
         Creates a provisioned throughput with dedicated capacity for a foundation model
         or a fine-tuned
         model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.create_provisioned_model_throughput)
@@ -265,15 +264,15 @@
         creationTimeAfter: TimestampTypeDef = ...,
         nameContains: str = ...,
         baseModelArnEquals: str = ...,
         foundationModelArnEquals: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         sortBy: Literal["CreationTime"] = ...,
-        sortOrder: SortOrderType = ...
+        sortOrder: SortOrderType = ...,
     ) -> ListCustomModelsResponseTypeDef:
         """
         Returns a list of the custom models that you have created with the
         `CreateModelCustomizationJob`
         operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.list_custom_models)
@@ -282,15 +281,15 @@
 
     async def list_foundation_models(
         self,
         *,
         byProvider: str = ...,
         byCustomizationType: ModelCustomizationType = ...,
         byOutputModality: ModelModalityType = ...,
-        byInferenceType: InferenceTypeType = ...
+        byInferenceType: InferenceTypeType = ...,
     ) -> ListFoundationModelsResponseTypeDef:
         """
         List of Amazon Bedrock foundation models that you can use.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.list_foundation_models)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock/client/#list_foundation_models)
         """
@@ -301,15 +300,15 @@
         creationTimeAfter: TimestampTypeDef = ...,
         creationTimeBefore: TimestampTypeDef = ...,
         statusEquals: FineTuningJobStatusType = ...,
         nameContains: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         sortBy: Literal["CreationTime"] = ...,
-        sortOrder: SortOrderType = ...
+        sortOrder: SortOrderType = ...,
     ) -> ListModelCustomizationJobsResponseTypeDef:
         """
         Returns a list of model customization jobs that you have submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.list_model_customization_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock/client/#list_model_customization_jobs)
         """
@@ -321,15 +320,15 @@
         creationTimeBefore: TimestampTypeDef = ...,
         statusEquals: ProvisionedModelStatusType = ...,
         modelArnEquals: str = ...,
         nameContains: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         sortBy: Literal["CreationTime"] = ...,
-        sortOrder: SortOrderType = ...
+        sortOrder: SortOrderType = ...,
     ) -> ListProvisionedModelThroughputsResponseTypeDef:
         """
         List the provisioned capacities.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.list_provisioned_model_throughputs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock/client/#list_provisioned_model_throughputs)
         """
@@ -379,15 +378,15 @@
         """
 
     async def update_provisioned_model_throughput(
         self,
         *,
         provisionedModelId: str,
         desiredProvisionedModelName: str = ...,
-        desiredModelId: str = ...
+        desiredModelId: str = ...,
     ) -> Dict[str, Any]:
         """
         Update a provisioned throughput.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.update_provisioned_model_throughput)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock/client/#update_provisioned_model_throughput)
         """
```

### Comparing `types-aiobotocore-bedrock-2.9.0/types_aiobotocore_bedrock/client.pyi` & `types-aiobotocore-bedrock-2.9.1/types_aiobotocore_bedrock/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -128,15 +128,15 @@
         hyperParameters: Mapping[str, str],
         clientRequestToken: str = ...,
         customizationType: CustomizationTypeType = ...,
         customModelKmsKeyId: str = ...,
         jobTags: Sequence[TagTypeDef] = ...,
         customModelTags: Sequence[TagTypeDef] = ...,
         validationDataConfig: ValidationDataConfigTypeDef = ...,
-        vpcConfig: VpcConfigTypeDef = ...
+        vpcConfig: VpcConfigTypeDef = ...,
     ) -> CreateModelCustomizationJobResponseTypeDef:
         """
         Creates a fine-tuning job to customize a base model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.create_model_customization_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock/client/#create_model_customization_job)
         """
@@ -145,15 +145,15 @@
         self,
         *,
         modelUnits: int,
         provisionedModelName: str,
         modelId: str,
         clientRequestToken: str = ...,
         commitmentDuration: CommitmentDurationType = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateProvisionedModelThroughputResponseTypeDef:
         """
         Creates a provisioned throughput with dedicated capacity for a foundation model
         or a fine-tuned
         model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.create_provisioned_model_throughput)
@@ -261,15 +261,15 @@
         creationTimeAfter: TimestampTypeDef = ...,
         nameContains: str = ...,
         baseModelArnEquals: str = ...,
         foundationModelArnEquals: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         sortBy: Literal["CreationTime"] = ...,
-        sortOrder: SortOrderType = ...
+        sortOrder: SortOrderType = ...,
     ) -> ListCustomModelsResponseTypeDef:
         """
         Returns a list of the custom models that you have created with the
         `CreateModelCustomizationJob`
         operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.list_custom_models)
@@ -278,15 +278,15 @@
 
     async def list_foundation_models(
         self,
         *,
         byProvider: str = ...,
         byCustomizationType: ModelCustomizationType = ...,
         byOutputModality: ModelModalityType = ...,
-        byInferenceType: InferenceTypeType = ...
+        byInferenceType: InferenceTypeType = ...,
     ) -> ListFoundationModelsResponseTypeDef:
         """
         List of Amazon Bedrock foundation models that you can use.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.list_foundation_models)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock/client/#list_foundation_models)
         """
@@ -297,15 +297,15 @@
         creationTimeAfter: TimestampTypeDef = ...,
         creationTimeBefore: TimestampTypeDef = ...,
         statusEquals: FineTuningJobStatusType = ...,
         nameContains: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         sortBy: Literal["CreationTime"] = ...,
-        sortOrder: SortOrderType = ...
+        sortOrder: SortOrderType = ...,
     ) -> ListModelCustomizationJobsResponseTypeDef:
         """
         Returns a list of model customization jobs that you have submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.list_model_customization_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock/client/#list_model_customization_jobs)
         """
@@ -317,15 +317,15 @@
         creationTimeBefore: TimestampTypeDef = ...,
         statusEquals: ProvisionedModelStatusType = ...,
         modelArnEquals: str = ...,
         nameContains: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         sortBy: Literal["CreationTime"] = ...,
-        sortOrder: SortOrderType = ...
+        sortOrder: SortOrderType = ...,
     ) -> ListProvisionedModelThroughputsResponseTypeDef:
         """
         List the provisioned capacities.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.list_provisioned_model_throughputs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock/client/#list_provisioned_model_throughputs)
         """
@@ -375,15 +375,15 @@
         """
 
     async def update_provisioned_model_throughput(
         self,
         *,
         provisionedModelId: str,
         desiredProvisionedModelName: str = ...,
-        desiredModelId: str = ...
+        desiredModelId: str = ...,
     ) -> Dict[str, Any]:
         """
         Update a provisioned throughput.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.update_provisioned_model_throughput)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock/client/#update_provisioned_model_throughput)
         """
```

### Comparing `types-aiobotocore-bedrock-2.9.0/types_aiobotocore_bedrock/literals.py` & `types-aiobotocore-bedrock-2.9.1/types_aiobotocore_bedrock/literals.py`

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
     "CommitmentDurationType",
     "CustomizationTypeType",
     "FineTuningJobStatusType",
     "FoundationModelLifecycleStatusType",
     "InferenceTypeType",
     "ListCustomModelsPaginatorName",
@@ -40,15 +39,14 @@
     "BedrockServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 CommitmentDurationType = Literal["OneMonth", "SixMonths"]
 CustomizationTypeType = Literal["CONTINUED_PRE_TRAINING", "FINE_TUNING"]
 FineTuningJobStatusType = Literal["Completed", "Failed", "InProgress", "Stopped", "Stopping"]
 FoundationModelLifecycleStatusType = Literal["ACTIVE", "LEGACY"]
 InferenceTypeType = Literal["ON_DEMAND", "PROVISIONED"]
 ListCustomModelsPaginatorName = Literal["list_custom_models"]
 ListModelCustomizationJobsPaginatorName = Literal["list_model_customization_jobs"]
```

### Comparing `types-aiobotocore-bedrock-2.9.0/types_aiobotocore_bedrock/literals.pyi` & `types-aiobotocore-bedrock-2.9.1/types_aiobotocore_bedrock/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-bedrock-2.9.0/types_aiobotocore_bedrock/paginator.py` & `types-aiobotocore-bedrock-2.9.1/types_aiobotocore_bedrock/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,22 +41,20 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ListCustomModelsPaginator",
     "ListModelCustomizationJobsPaginator",
     "ListProvisionedModelThroughputsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -75,15 +73,15 @@
         creationTimeBefore: TimestampTypeDef = ...,
         creationTimeAfter: TimestampTypeDef = ...,
         nameContains: str = ...,
         baseModelArnEquals: str = ...,
         foundationModelArnEquals: str = ...,
         sortBy: Literal["CreationTime"] = ...,
         sortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCustomModelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Paginator.ListCustomModels.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock/paginators/#listcustommodelspaginator)
         """
 
 
@@ -98,15 +96,15 @@
         *,
         creationTimeAfter: TimestampTypeDef = ...,
         creationTimeBefore: TimestampTypeDef = ...,
         statusEquals: FineTuningJobStatusType = ...,
         nameContains: str = ...,
         sortBy: Literal["CreationTime"] = ...,
         sortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListModelCustomizationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Paginator.ListModelCustomizationJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock/paginators/#listmodelcustomizationjobspaginator)
         """
 
 
@@ -122,13 +120,13 @@
         creationTimeAfter: TimestampTypeDef = ...,
         creationTimeBefore: TimestampTypeDef = ...,
         statusEquals: ProvisionedModelStatusType = ...,
         modelArnEquals: str = ...,
         nameContains: str = ...,
         sortBy: Literal["CreationTime"] = ...,
         sortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListProvisionedModelThroughputsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Paginator.ListProvisionedModelThroughputs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock/paginators/#listprovisionedmodelthroughputspaginator)
         """
```

### Comparing `types-aiobotocore-bedrock-2.9.0/types_aiobotocore_bedrock/paginator.pyi` & `types-aiobotocore-bedrock-2.9.1/types_aiobotocore_bedrock/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         creationTimeBefore: TimestampTypeDef = ...,
         creationTimeAfter: TimestampTypeDef = ...,
         nameContains: str = ...,
         baseModelArnEquals: str = ...,
         foundationModelArnEquals: str = ...,
         sortBy: Literal["CreationTime"] = ...,
         sortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCustomModelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Paginator.ListCustomModels.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock/paginators/#listcustommodelspaginator)
         """
 
 class ListModelCustomizationJobsPaginator(AioPaginator):
@@ -93,15 +93,15 @@
         *,
         creationTimeAfter: TimestampTypeDef = ...,
         creationTimeBefore: TimestampTypeDef = ...,
         statusEquals: FineTuningJobStatusType = ...,
         nameContains: str = ...,
         sortBy: Literal["CreationTime"] = ...,
         sortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListModelCustomizationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Paginator.ListModelCustomizationJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock/paginators/#listmodelcustomizationjobspaginator)
         """
 
 class ListProvisionedModelThroughputsPaginator(AioPaginator):
@@ -116,13 +116,13 @@
         creationTimeAfter: TimestampTypeDef = ...,
         creationTimeBefore: TimestampTypeDef = ...,
         statusEquals: ProvisionedModelStatusType = ...,
         modelArnEquals: str = ...,
         nameContains: str = ...,
         sortBy: Literal["CreationTime"] = ...,
         sortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListProvisionedModelThroughputsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Paginator.ListProvisionedModelThroughputs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock/paginators/#listprovisionedmodelthroughputspaginator)
         """
```

### Comparing `types-aiobotocore-bedrock-2.9.0/types_aiobotocore_bedrock/type_defs.py` & `types-aiobotocore-bedrock-2.9.1/types_aiobotocore_bedrock/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "S3ConfigTypeDef",
     "OutputDataConfigTypeDef",
     "TagTypeDef",
     "TrainingDataConfigTypeDef",
     "VpcConfigTypeDef",
     "ResponseMetadataTypeDef",
```

### Comparing `types-aiobotocore-bedrock-2.9.0/types_aiobotocore_bedrock/type_defs.pyi` & `types-aiobotocore-bedrock-2.9.1/types_aiobotocore_bedrock/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-bedrock-2.9.0/types_aiobotocore_bedrock.egg-info/PKG-INFO` & `types-aiobotocore-bedrock-2.9.1/types_aiobotocore_bedrock.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-bedrock
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Bedrock 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Bedrock 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock/
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
 
 <a id="types-aiobotocore-bedrock"></a>
 
 # types-aiobotocore-bedrock
 
 [![PyPI - types-aiobotocore-bedrock](https://img.shields.io/pypi/v/types-aiobotocore-bedrock.svg?color=blue)](https://pypi.org/project/types-aiobotocore-bedrock)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-bedrock.svg?color=blue)](https://pypi.org/project/types-aiobotocore-bedrock)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-bedrock)](https://pepy.tech/project/types-aiobotocore-bedrock)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Bedrock 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock)
+[aiobotocore.Bedrock 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock)
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
 [types-aiobotocore-bedrock docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_bedrock/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-bedrock-2.9.0/types_aiobotocore_bedrock.egg-info/SOURCES.txt` & `types-aiobotocore-bedrock-2.9.1/types_aiobotocore_bedrock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

