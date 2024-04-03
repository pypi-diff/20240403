# Comparing `tmp/types-aiobotocore-connect-2.9.0.tar.gz` & `tmp/types-aiobotocore-connect-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-connect-2.9.0.tar", last modified: Wed Dec 13 19:59:00 2023, max compression
+gzip compressed data, was "types-aiobotocore-connect-2.9.1.tar", last modified: Thu Jan 18 01:20:25 2024, max compression
```

## Comparing `types-aiobotocore-connect-2.9.0.tar` & `types-aiobotocore-connect-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:00.081888 types-aiobotocore-connect-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:43:23.000000 types-aiobotocore-connect-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    20715 2023-12-13 19:59:00.081888 types-aiobotocore-connect-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19152 2023-12-13 19:43:23.000000 types-aiobotocore-connect-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:00.081888 types-aiobotocore-connect-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2023-12-13 19:43:23.000000 types-aiobotocore-connect-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:00.081888 types-aiobotocore-connect-2.9.0/types_aiobotocore_connect/
--rw-r--r--   0 runner    (1001) docker     (127)    11530 2023-12-13 19:43:23.000000 types-aiobotocore-connect-2.9.0/types_aiobotocore_connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11529 2023-12-13 19:43:23.000000 types-aiobotocore-connect-2.9.0/types_aiobotocore_connect/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      932 2023-12-13 19:43:23.000000 types-aiobotocore-connect-2.9.0/types_aiobotocore_connect/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)   182773 2023-12-13 19:43:25.000000 types-aiobotocore-connect-2.9.0/types_aiobotocore_connect/client.py
--rw-r--r--   0 runner    (1001) docker     (127)   182769 2023-12-13 19:43:25.000000 types-aiobotocore-connect-2.9.0/types_aiobotocore_connect/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    28938 2023-12-13 19:43:26.000000 types-aiobotocore-connect-2.9.0/types_aiobotocore_connect/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    28936 2023-12-13 19:43:26.000000 types-aiobotocore-connect-2.9.0/types_aiobotocore_connect/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    62653 2023-12-13 19:43:26.000000 types-aiobotocore-connect-2.9.0/types_aiobotocore_connect/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    62600 2023-12-13 19:43:26.000000 types-aiobotocore-connect-2.9.0/types_aiobotocore_connect/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:43:23.000000 types-aiobotocore-connect-2.9.0/types_aiobotocore_connect/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   204008 2023-12-13 19:43:32.000000 types-aiobotocore-connect-2.9.0/types_aiobotocore_connect/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   204007 2023-12-13 19:43:29.000000 types-aiobotocore-connect-2.9.0/types_aiobotocore_connect/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:43:23.000000 types-aiobotocore-connect-2.9.0/types_aiobotocore_connect/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:00.081888 types-aiobotocore-connect-2.9.0/types_aiobotocore_connect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20715 2023-12-13 19:59:00.000000 types-aiobotocore-connect-2.9.0/types_aiobotocore_connect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      813 2023-12-13 19:59:00.000000 types-aiobotocore-connect-2.9.0/types_aiobotocore_connect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:00.000000 types-aiobotocore-connect-2.9.0/types_aiobotocore_connect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:00.000000 types-aiobotocore-connect-2.9.0/types_aiobotocore_connect.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:00.000000 types-aiobotocore-connect-2.9.0/types_aiobotocore_connect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-13 19:59:00.000000 types-aiobotocore-connect-2.9.0/types_aiobotocore_connect.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:25.977417 types-aiobotocore-connect-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:05:20.000000 types-aiobotocore-connect-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    20735 2024-01-18 01:20:25.977417 types-aiobotocore-connect-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19152 2024-01-18 01:05:20.000000 types-aiobotocore-connect-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:25.977417 types-aiobotocore-connect-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-01-18 01:05:20.000000 types-aiobotocore-connect-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:25.977417 types-aiobotocore-connect-2.9.1/types_aiobotocore_connect/
+-rw-r--r--   0 runner    (1001) docker     (127)    11529 2024-01-18 01:05:20.000000 types-aiobotocore-connect-2.9.1/types_aiobotocore_connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11529 2024-01-18 01:05:20.000000 types-aiobotocore-connect-2.9.1/types_aiobotocore_connect/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-01-18 01:05:20.000000 types-aiobotocore-connect-2.9.1/types_aiobotocore_connect/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   182865 2024-01-18 01:05:22.000000 types-aiobotocore-connect-2.9.1/types_aiobotocore_connect/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   182862 2024-01-18 01:05:20.000000 types-aiobotocore-connect-2.9.1/types_aiobotocore_connect/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    28936 2024-01-18 01:05:23.000000 types-aiobotocore-connect-2.9.1/types_aiobotocore_connect/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28936 2024-01-18 01:05:23.000000 types-aiobotocore-connect-2.9.1/types_aiobotocore_connect/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    62683 2024-01-18 01:05:22.000000 types-aiobotocore-connect-2.9.1/types_aiobotocore_connect/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62632 2024-01-18 01:05:22.000000 types-aiobotocore-connect-2.9.1/types_aiobotocore_connect/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:05:20.000000 types-aiobotocore-connect-2.9.1/types_aiobotocore_connect/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   204007 2024-01-18 01:05:27.000000 types-aiobotocore-connect-2.9.1/types_aiobotocore_connect/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   204007 2024-01-18 01:05:26.000000 types-aiobotocore-connect-2.9.1/types_aiobotocore_connect/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:05:20.000000 types-aiobotocore-connect-2.9.1/types_aiobotocore_connect/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:25.977417 types-aiobotocore-connect-2.9.1/types_aiobotocore_connect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20735 2024-01-18 01:20:25.000000 types-aiobotocore-connect-2.9.1/types_aiobotocore_connect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-01-18 01:20:25.000000 types-aiobotocore-connect-2.9.1/types_aiobotocore_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:25.000000 types-aiobotocore-connect-2.9.1/types_aiobotocore_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:25.000000 types-aiobotocore-connect-2.9.1/types_aiobotocore_connect.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:25.000000 types-aiobotocore-connect-2.9.1/types_aiobotocore_connect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-01-18 01:20:25.000000 types-aiobotocore-connect-2.9.1/types_aiobotocore_connect.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-connect-2.9.0/LICENSE` & `types-aiobotocore-connect-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-connect-2.9.0/PKG-INFO` & `types-aiobotocore-connect-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-connect
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Connect 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Connect 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/
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
 
 <a id="types-aiobotocore-connect"></a>
 
 # types-aiobotocore-connect
 
 [![PyPI - types-aiobotocore-connect](https://img.shields.io/pypi/v/types-aiobotocore-connect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-connect)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-connect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-connect)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-connect)](https://pepy.tech/project/types-aiobotocore-connect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Connect 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
+[aiobotocore.Connect 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
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
 [types-aiobotocore-connect docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-connect-2.9.0/README.md` & `types-aiobotocore-connect-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-connect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-connect)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-connect)](https://pepy.tech/project/types-aiobotocore-connect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Connect 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
+[aiobotocore.Connect 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
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
 [types-aiobotocore-connect docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-connect-2.9.0/setup.py` & `types-aiobotocore-connect-2.9.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-connect",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_connect"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Connect 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.Connect 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore connect type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_connect": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-connect-2.9.0/types_aiobotocore_connect/__init__.py` & `types-aiobotocore-connect-2.9.1/types_aiobotocore_connect/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,15 +171,14 @@
     SearchSecurityProfilesPaginator,
     SearchUsersPaginator,
     SearchVocabulariesPaginator,
 )
 
 Client = ConnectClient
 
-
 __all__ = (
     "Client",
     "ConnectClient",
     "GetMetricDataPaginator",
     "ListAgentStatusesPaginator",
     "ListApprovedOriginsPaginator",
     "ListBotsPaginator",
```

### Comparing `types-aiobotocore-connect-2.9.0/types_aiobotocore_connect/__init__.pyi` & `types-aiobotocore-connect-2.9.1/types_aiobotocore_connect/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connect-2.9.0/types_aiobotocore_connect/__main__.py` & `types-aiobotocore-connect-2.9.1/types_aiobotocore_connect/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Connect 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Connect 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect\nOther"
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

### Comparing `types-aiobotocore-connect-2.9.0/types_aiobotocore_connect/client.py` & `types-aiobotocore-connect-2.9.1/types_aiobotocore_connect/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -314,15 +314,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ConnectClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -427,29 +426,29 @@
 
     async def associate_flow(
         self,
         *,
         InstanceId: str,
         ResourceId: str,
         FlowId: str,
-        ResourceType: Literal["SMS_PHONE_NUMBER"]
+        ResourceType: Literal["SMS_PHONE_NUMBER"],
     ) -> Dict[str, Any]:
         """
         Associates a connect resource to a flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.associate_flow)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#associate_flow)
         """
 
     async def associate_instance_storage_config(
         self,
         *,
         InstanceId: str,
         ResourceType: InstanceStorageResourceTypeType,
-        StorageConfig: InstanceStorageConfigTypeDef
+        StorageConfig: InstanceStorageConfigTypeDef,
     ) -> AssociateInstanceStorageConfigResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.associate_instance_storage_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#associate_instance_storage_config)
         """
@@ -495,15 +494,15 @@
         """
 
     async def associate_routing_profile_queues(
         self,
         *,
         InstanceId: str,
         RoutingProfileId: str,
-        QueueConfigs: Sequence[RoutingProfileQueueConfigTypeDef]
+        QueueConfigs: Sequence[RoutingProfileQueueConfigTypeDef],
     ) -> EmptyResponseMetadataTypeDef:
         """
         Associates a set of queues with a routing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.associate_routing_profile_queues)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#associate_routing_profile_queues)
         """
@@ -549,29 +548,29 @@
         """
 
     async def batch_get_flow_association(
         self,
         *,
         InstanceId: str,
         ResourceIds: Sequence[str],
-        ResourceType: Literal["VOICE_PHONE_NUMBER"] = ...
+        ResourceType: Literal["VOICE_PHONE_NUMBER"] = ...,
     ) -> BatchGetFlowAssociationResponseTypeDef:
         """
         Retrieve the flow associations for the given resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.batch_get_flow_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#batch_get_flow_association)
         """
 
     async def batch_put_contact(
         self,
         *,
         InstanceId: str,
         ContactDataRequestList: Sequence[ContactDataRequestTypeDef],
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> BatchPutContactResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.batch_put_contact)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#batch_put_contact)
         """
@@ -588,15 +587,15 @@
         self,
         *,
         PhoneNumber: str,
         TargetArn: str = ...,
         InstanceId: str = ...,
         PhoneNumberDescription: str = ...,
         Tags: Mapping[str, str] = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> ClaimPhoneNumberResponseTypeDef:
         """
         Claims an available phone number to your Amazon Connect instance or traffic
         distribution
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.claim_phone_number)
@@ -615,15 +614,15 @@
         self,
         *,
         InstanceId: str,
         Name: str,
         State: AgentStatusStateType,
         Description: str = ...,
         DisplayOrder: int = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateAgentStatusResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_agent_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#create_agent_status)
         """
@@ -632,15 +631,15 @@
         self,
         *,
         InstanceId: str,
         Name: str,
         Type: ContactFlowTypeType,
         Content: str,
         Description: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateContactFlowResponseTypeDef:
         """
         Creates a flow for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_contact_flow)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#create_contact_flow)
         """
@@ -649,15 +648,15 @@
         self,
         *,
         InstanceId: str,
         Name: str,
         Content: str,
         Description: str = ...,
         Tags: Mapping[str, str] = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreateContactFlowModuleResponseTypeDef:
         """
         Creates a flow module for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_contact_flow_module)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#create_contact_flow_module)
         """
@@ -666,15 +665,15 @@
         self,
         *,
         InstanceId: str,
         Title: str,
         Items: Sequence["EvaluationFormItemTypeDef"],
         Description: str = ...,
         ScoringStrategy: EvaluationFormScoringStrategyTypeDef = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreateEvaluationFormResponseTypeDef:
         """
         Creates an evaluation form in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_evaluation_form)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#create_evaluation_form)
         """
@@ -683,15 +682,15 @@
         self,
         *,
         InstanceId: str,
         Name: str,
         TimeZone: str,
         Config: Sequence[HoursOfOperationConfigTypeDef],
         Description: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateHoursOfOperationResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_hours_of_operation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#create_hours_of_operation)
         """
@@ -701,15 +700,15 @@
         *,
         IdentityManagementType: DirectoryTypeType,
         InboundCallsEnabled: bool,
         OutboundCallsEnabled: bool,
         ClientToken: str = ...,
         InstanceAlias: str = ...,
         DirectoryId: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateInstanceResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#create_instance)
         """
@@ -719,15 +718,15 @@
         *,
         InstanceId: str,
         IntegrationType: IntegrationTypeType,
         IntegrationArn: str,
         SourceApplicationUrl: str = ...,
         SourceApplicationName: str = ...,
         SourceType: SourceTypeType = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateIntegrationAssociationResponseTypeDef:
         """
         Creates an Amazon Web Services resource association with an Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_integration_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#create_integration_association)
@@ -735,15 +734,15 @@
 
     async def create_participant(
         self,
         *,
         InstanceId: str,
         ContactId: str,
         ParticipantDetails: ParticipantDetailsToAddTypeDef,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreateParticipantResponseTypeDef:
         """
         Adds a new participant into an on-going chat contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_participant)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#create_participant)
         """
@@ -751,15 +750,15 @@
     async def create_persistent_contact_association(
         self,
         *,
         InstanceId: str,
         InitialContactId: str,
         RehydrationType: RehydrationTypeType,
         SourceContactId: str,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreatePersistentContactAssociationResponseTypeDef:
         """
         Enables rehydration of chats for the lifespan of a contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_persistent_contact_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#create_persistent_contact_association)
         """
@@ -767,15 +766,15 @@
     async def create_prompt(
         self,
         *,
         InstanceId: str,
         Name: str,
         S3Uri: str,
         Description: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreatePromptResponseTypeDef:
         """
         Creates a prompt.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_prompt)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#create_prompt)
         """
@@ -786,15 +785,15 @@
         InstanceId: str,
         Name: str,
         HoursOfOperationId: str,
         Description: str = ...,
         OutboundCallerConfig: OutboundCallerConfigTypeDef = ...,
         MaxContacts: int = ...,
         QuickConnectIds: Sequence[str] = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateQueueResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_queue)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#create_queue)
         """
@@ -802,15 +801,15 @@
     async def create_quick_connect(
         self,
         *,
         InstanceId: str,
         Name: str,
         QuickConnectConfig: QuickConnectConfigTypeDef,
         Description: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateQuickConnectResponseTypeDef:
         """
         Creates a quick connect for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_quick_connect)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#create_quick_connect)
         """
@@ -821,15 +820,15 @@
         InstanceId: str,
         Name: str,
         Description: str,
         DefaultOutboundQueueId: str,
         MediaConcurrencies: Sequence[MediaConcurrencyTypeDef],
         QueueConfigs: Sequence[RoutingProfileQueueConfigTypeDef] = ...,
         Tags: Mapping[str, str] = ...,
-        AgentAvailabilityTimer: AgentAvailabilityTimerType = ...
+        AgentAvailabilityTimer: AgentAvailabilityTimerType = ...,
     ) -> CreateRoutingProfileResponseTypeDef:
         """
         Creates a new routing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_routing_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#create_routing_profile)
         """
@@ -839,15 +838,15 @@
         *,
         InstanceId: str,
         Name: str,
         TriggerEventSource: RuleTriggerEventSourceTypeDef,
         Function: str,
         Actions: Sequence[RuleActionTypeDef],
         PublishStatus: RulePublishStatusType,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreateRuleResponseTypeDef:
         """
         Creates a rule for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#create_rule)
         """
@@ -858,15 +857,15 @@
         SecurityProfileName: str,
         InstanceId: str,
         Description: str = ...,
         Permissions: Sequence[str] = ...,
         Tags: Mapping[str, str] = ...,
         AllowedAccessControlTags: Mapping[str, str] = ...,
         TagRestrictedResources: Sequence[str] = ...,
-        Applications: Sequence[ApplicationTypeDef] = ...
+        Applications: Sequence[ApplicationTypeDef] = ...,
     ) -> CreateSecurityProfileResponseTypeDef:
         """
         Creates a security profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_security_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#create_security_profile)
         """
@@ -878,15 +877,15 @@
         Name: str,
         Fields: Sequence[TaskTemplateFieldTypeDef],
         Description: str = ...,
         ContactFlowId: str = ...,
         Constraints: TaskTemplateConstraintsTypeDef = ...,
         Defaults: TaskTemplateDefaultsTypeDef = ...,
         Status: TaskTemplateStatusType = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreateTaskTemplateResponseTypeDef:
         """
         Creates a new task template in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_task_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#create_task_template)
         """
@@ -894,15 +893,15 @@
     async def create_traffic_distribution_group(
         self,
         *,
         Name: str,
         InstanceId: str,
         Description: str = ...,
         ClientToken: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateTrafficDistributionGroupResponseTypeDef:
         """
         Creates a traffic distribution group given an Amazon Connect instance that has
         been
         replicated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_traffic_distribution_group)
@@ -911,15 +910,15 @@
 
     async def create_use_case(
         self,
         *,
         InstanceId: str,
         IntegrationAssociationId: str,
         UseCaseType: UseCaseTypeType,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateUseCaseResponseTypeDef:
         """
         Creates a use case for an integration association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_use_case)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#create_use_case)
         """
@@ -932,15 +931,15 @@
         SecurityProfileIds: Sequence[str],
         RoutingProfileId: str,
         InstanceId: str,
         Password: str = ...,
         IdentityInfo: UserIdentityInfoTypeDef = ...,
         DirectoryUserId: str = ...,
         HierarchyGroupId: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateUserResponseTypeDef:
         """
         Creates a user account for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#create_user)
         """
@@ -960,30 +959,30 @@
         *,
         InstanceId: str,
         Status: ViewStatusType,
         Content: ViewInputContentTypeDef,
         Name: str,
         ClientToken: str = ...,
         Description: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateViewResponseTypeDef:
         """
         Creates a new view with the possible status of `SAVED` or `PUBLISHED`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_view)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#create_view)
         """
 
     async def create_view_version(
         self,
         *,
         InstanceId: str,
         ViewId: str,
         VersionDescription: str = ...,
-        ViewContentSha256: str = ...
+        ViewContentSha256: str = ...,
     ) -> CreateViewVersionResponseTypeDef:
         """
         Publishes a new version of the view identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_view_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#create_view_version)
         """
@@ -992,15 +991,15 @@
         self,
         *,
         InstanceId: str,
         VocabularyName: str,
         LanguageCode: VocabularyLanguageCodeType,
         Content: str,
         ClientToken: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateVocabularyResponseTypeDef:
         """
         Creates a custom vocabulary associated with your Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_vocabulary)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#create_vocabulary)
         """
@@ -1529,15 +1528,15 @@
         """
 
     async def disassociate_routing_profile_queues(
         self,
         *,
         InstanceId: str,
         RoutingProfileId: str,
-        QueueReferences: Sequence[RoutingProfileQueueReferenceTypeDef]
+        QueueReferences: Sequence[RoutingProfileQueueReferenceTypeDef],
     ) -> EmptyResponseMetadataTypeDef:
         """
         Disassociates a set of queues from a routing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.disassociate_routing_profile_queues)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#disassociate_routing_profile_queues)
         """
@@ -1603,30 +1602,30 @@
         *,
         InstanceId: str,
         Filters: FiltersTypeDef,
         CurrentMetrics: Sequence[CurrentMetricTypeDef],
         Groupings: Sequence[GroupingType] = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        SortCriteria: Sequence[CurrentMetricSortCriteriaTypeDef] = ...
+        SortCriteria: Sequence[CurrentMetricSortCriteriaTypeDef] = ...,
     ) -> GetCurrentMetricDataResponseTypeDef:
         """
         Gets the real-time metric data from the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_current_metric_data)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#get_current_metric_data)
         """
 
     async def get_current_user_data(
         self,
         *,
         InstanceId: str,
         Filters: UserDataFiltersTypeDef,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> GetCurrentUserDataResponseTypeDef:
         """
         Gets the real-time active user data from the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_current_user_data)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#get_current_user_data)
         """
@@ -1655,15 +1654,15 @@
         InstanceId: str,
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
         Filters: FiltersTypeDef,
         HistoricalMetrics: Sequence[HistoricalMetricTypeDef],
         Groupings: Sequence[GroupingType] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> GetMetricDataResponseTypeDef:
         """
         Gets historical metric data from the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_metric_data)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#get_metric_data)
         """
@@ -1675,15 +1674,15 @@
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
         Filters: Sequence[FilterV2TypeDef],
         Metrics: Sequence[MetricV2TypeDef],
         Interval: IntervalDetailsTypeDef = ...,
         Groupings: Sequence[str] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> GetMetricDataV2ResponseTypeDef:
         """
         Gets metric data from the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_metric_data_v2)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#get_metric_data_v2)
         """
@@ -1721,15 +1720,15 @@
     async def import_phone_number(
         self,
         *,
         InstanceId: str,
         SourcePhoneNumberArn: str,
         PhoneNumberDescription: str = ...,
         Tags: Mapping[str, str] = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> ImportPhoneNumberResponseTypeDef:
         """
         Imports a claimed phone number from an external service, such as Amazon
         Pinpoint, into an Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.import_phone_number)
@@ -1738,15 +1737,15 @@
 
     async def list_agent_statuses(
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
-        AgentStatusTypes: Sequence[AgentStatusTypeType] = ...
+        AgentStatusTypes: Sequence[AgentStatusTypeType] = ...,
     ) -> ListAgentStatusResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_agent_statuses)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#list_agent_statuses)
         """
@@ -1773,15 +1772,15 @@
 
     async def list_bots(
         self,
         *,
         InstanceId: str,
         LexVersion: LexVersionType,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListBotsResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_bots)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#list_bots)
         """
@@ -1798,15 +1797,15 @@
 
     async def list_contact_flow_modules(
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
-        ContactFlowModuleState: ContactFlowModuleStateType = ...
+        ContactFlowModuleState: ContactFlowModuleStateType = ...,
     ) -> ListContactFlowModulesResponseTypeDef:
         """
         Provides information about the flow modules for the specified Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_contact_flow_modules)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#list_contact_flow_modules)
@@ -1814,45 +1813,45 @@
 
     async def list_contact_flows(
         self,
         *,
         InstanceId: str,
         ContactFlowTypes: Sequence[ContactFlowTypeType] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListContactFlowsResponseTypeDef:
         """
         Provides information about the flows for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_contact_flows)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#list_contact_flows)
         """
 
     async def list_contact_references(
         self,
         *,
         InstanceId: str,
         ContactId: str,
         ReferenceTypes: Sequence[ReferenceTypeType],
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListContactReferencesResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_contact_references)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#list_contact_references)
         """
 
     async def list_default_vocabularies(
         self,
         *,
         InstanceId: str,
         LanguageCode: VocabularyLanguageCodeType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListDefaultVocabulariesResponseTypeDef:
         """
         Lists the default vocabularies for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_default_vocabularies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#list_default_vocabularies)
         """
@@ -1879,15 +1878,15 @@
 
     async def list_flow_associations(
         self,
         *,
         InstanceId: str,
         ResourceType: Literal["VOICE_PHONE_NUMBER"] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListFlowAssociationsResponseTypeDef:
         """
         List the flow association based on the filters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_flow_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#list_flow_associations)
         """
@@ -1916,15 +1915,15 @@
 
     async def list_instance_storage_configs(
         self,
         *,
         InstanceId: str,
         ResourceType: InstanceStorageResourceTypeType,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListInstanceStorageConfigsResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_instance_storage_configs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#list_instance_storage_configs)
         """
@@ -1942,15 +1941,15 @@
     async def list_integration_associations(
         self,
         *,
         InstanceId: str,
         IntegrationType: IntegrationTypeType = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        IntegrationArn: str = ...
+        IntegrationArn: str = ...,
     ) -> ListIntegrationAssociationsResponseTypeDef:
         """
         Provides summary information about the Amazon Web Services resource
         associations for the specified Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_integration_associations)
@@ -1980,15 +1979,15 @@
     async def list_phone_numbers(
         self,
         *,
         InstanceId: str,
         PhoneNumberTypes: Sequence[PhoneNumberTypeType] = ...,
         PhoneNumberCountryCodes: Sequence[PhoneNumberCountryCodeType] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListPhoneNumbersResponseTypeDef:
         """
         Provides information about the phone numbers for the specified Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_phone_numbers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#list_phone_numbers)
@@ -1999,15 +1998,15 @@
         *,
         TargetArn: str = ...,
         InstanceId: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         PhoneNumberCountryCodes: Sequence[PhoneNumberCountryCodeType] = ...,
         PhoneNumberTypes: Sequence[PhoneNumberTypeType] = ...,
-        PhoneNumberPrefix: str = ...
+        PhoneNumberPrefix: str = ...,
     ) -> ListPhoneNumbersV2ResponseTypeDef:
         """
         Lists phone numbers claimed to your Amazon Connect instance or traffic
         distribution
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_phone_numbers_v2)
@@ -2037,30 +2036,30 @@
 
     async def list_queues(
         self,
         *,
         InstanceId: str,
         QueueTypes: Sequence[QueueTypeType] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListQueuesResponseTypeDef:
         """
         Provides information about the queues for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_queues)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#list_queues)
         """
 
     async def list_quick_connects(
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
-        QuickConnectTypes: Sequence[QuickConnectTypeType] = ...
+        QuickConnectTypes: Sequence[QuickConnectTypeType] = ...,
     ) -> ListQuickConnectsResponseTypeDef:
         """
         Provides information about the quick connects for the specified Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_quick_connects)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#list_quick_connects)
@@ -2070,15 +2069,15 @@
         self,
         *,
         InstanceId: str,
         ContactId: str,
         OutputType: RealTimeContactAnalysisOutputTypeType,
         SegmentTypes: Sequence[RealTimeContactAnalysisSegmentTypeType],
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListRealtimeContactAnalysisSegmentsV2ResponseTypeDef:
         """
         Provides a list of analysis segments for a real-time analysis session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_realtime_contact_analysis_segments_v2)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#list_realtime_contact_analysis_segments_v2)
         """
@@ -2108,15 +2107,15 @@
     async def list_rules(
         self,
         *,
         InstanceId: str,
         PublishStatus: RulePublishStatusType = ...,
         EventSourceName: EventSourceNameType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListRulesResponseTypeDef:
         """
         List all rules for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_rules)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#list_rules)
         """
@@ -2133,30 +2132,30 @@
 
     async def list_security_profile_applications(
         self,
         *,
         SecurityProfileId: str,
         InstanceId: str,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListSecurityProfileApplicationsResponseTypeDef:
         """
         Returns a list of third-party applications in a specific security profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_security_profile_applications)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#list_security_profile_applications)
         """
 
     async def list_security_profile_permissions(
         self,
         *,
         SecurityProfileId: str,
         InstanceId: str,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListSecurityProfilePermissionsResponseTypeDef:
         """
         Lists the permissions granted to a security profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_security_profile_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#list_security_profile_permissions)
         """
@@ -2186,15 +2185,15 @@
     async def list_task_templates(
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         Status: TaskTemplateStatusType = ...,
-        Name: str = ...
+        Name: str = ...,
     ) -> ListTaskTemplatesResponseTypeDef:
         """
         Lists task templates for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_task_templates)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#list_task_templates)
         """
@@ -2221,15 +2220,15 @@
 
     async def list_use_cases(
         self,
         *,
         InstanceId: str,
         IntegrationAssociationId: str,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListUseCasesResponseTypeDef:
         """
         Lists the use cases for the integration association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_use_cases)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#list_use_cases)
         """
@@ -2271,15 +2270,15 @@
 
     async def list_views(
         self,
         *,
         InstanceId: str,
         Type: ViewTypeType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListViewsResponseTypeDef:
         """
         Returns views in the given instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_views)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#list_views)
         """
@@ -2287,15 +2286,15 @@
     async def monitor_contact(
         self,
         *,
         InstanceId: str,
         ContactId: str,
         UserId: str,
         AllowedMonitorCapabilities: Sequence[MonitorCapabilityType] = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> MonitorContactResponseTypeDef:
         """
         Initiates silent monitoring of a contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.monitor_contact)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#monitor_contact)
         """
@@ -2353,15 +2352,15 @@
         *,
         PhoneNumberCountryCode: PhoneNumberCountryCodeType,
         PhoneNumberType: PhoneNumberTypeType,
         TargetArn: str = ...,
         InstanceId: str = ...,
         PhoneNumberPrefix: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> SearchAvailablePhoneNumbersResponseTypeDef:
         """
         Searches for available phone numbers that you can claim to your Amazon Connect
         instance or traffic distribution
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_available_phone_numbers)
@@ -2371,15 +2370,15 @@
     async def search_hours_of_operations(
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchFilter: HoursOfOperationSearchFilterTypeDef = ...,
-        SearchCriteria: "HoursOfOperationSearchCriteriaTypeDef" = ...
+        SearchCriteria: "HoursOfOperationSearchCriteriaTypeDef" = ...,
     ) -> SearchHoursOfOperationsResponseTypeDef:
         """
         Searches the hours of operation in an Amazon Connect instance, with optional
         filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_hours_of_operations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#search_hours_of_operations)
@@ -2388,15 +2387,15 @@
     async def search_prompts(
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchFilter: PromptSearchFilterTypeDef = ...,
-        SearchCriteria: "PromptSearchCriteriaTypeDef" = ...
+        SearchCriteria: "PromptSearchCriteriaTypeDef" = ...,
     ) -> SearchPromptsResponseTypeDef:
         """
         Searches prompts in an Amazon Connect instance, with optional filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_prompts)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#search_prompts)
         """
@@ -2404,15 +2403,15 @@
     async def search_queues(
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchFilter: QueueSearchFilterTypeDef = ...,
-        SearchCriteria: "QueueSearchCriteriaTypeDef" = ...
+        SearchCriteria: "QueueSearchCriteriaTypeDef" = ...,
     ) -> SearchQueuesResponseTypeDef:
         """
         Searches queues in an Amazon Connect instance, with optional filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_queues)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#search_queues)
         """
@@ -2420,15 +2419,15 @@
     async def search_quick_connects(
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchFilter: QuickConnectSearchFilterTypeDef = ...,
-        SearchCriteria: "QuickConnectSearchCriteriaTypeDef" = ...
+        SearchCriteria: "QuickConnectSearchCriteriaTypeDef" = ...,
     ) -> SearchQuickConnectsResponseTypeDef:
         """
         Searches quick connects in an Amazon Connect instance, with optional filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_quick_connects)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#search_quick_connects)
         """
@@ -2436,15 +2435,15 @@
     async def search_resource_tags(
         self,
         *,
         InstanceId: str,
         ResourceTypes: Sequence[str] = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        SearchCriteria: ResourceTagsSearchCriteriaTypeDef = ...
+        SearchCriteria: ResourceTagsSearchCriteriaTypeDef = ...,
     ) -> SearchResourceTagsResponseTypeDef:
         """
         Searches tags used in an Amazon Connect instance using optional search criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_resource_tags)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#search_resource_tags)
         """
@@ -2452,15 +2451,15 @@
     async def search_routing_profiles(
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchFilter: RoutingProfileSearchFilterTypeDef = ...,
-        SearchCriteria: "RoutingProfileSearchCriteriaTypeDef" = ...
+        SearchCriteria: "RoutingProfileSearchCriteriaTypeDef" = ...,
     ) -> SearchRoutingProfilesResponseTypeDef:
         """
         Searches routing profiles in an Amazon Connect instance, with optional
         filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_routing_profiles)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#search_routing_profiles)
@@ -2469,15 +2468,15 @@
     async def search_security_profiles(
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchCriteria: "SecurityProfileSearchCriteriaTypeDef" = ...,
-        SearchFilter: SecurityProfilesSearchFilterTypeDef = ...
+        SearchFilter: SecurityProfilesSearchFilterTypeDef = ...,
     ) -> SearchSecurityProfilesResponseTypeDef:
         """
         Searches security profiles in an Amazon Connect instance, with optional
         filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_security_profiles)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#search_security_profiles)
@@ -2486,15 +2485,15 @@
     async def search_users(
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchFilter: UserSearchFilterTypeDef = ...,
-        SearchCriteria: "UserSearchCriteriaTypeDef" = ...
+        SearchCriteria: "UserSearchCriteriaTypeDef" = ...,
     ) -> SearchUsersResponseTypeDef:
         """
         Searches users in an Amazon Connect instance, with optional filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_users)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#search_users)
         """
@@ -2503,15 +2502,15 @@
         self,
         *,
         InstanceId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
         State: VocabularyStateType = ...,
         NameStartsWith: str = ...,
-        LanguageCode: VocabularyLanguageCodeType = ...
+        LanguageCode: VocabularyLanguageCodeType = ...,
     ) -> SearchVocabulariesResponseTypeDef:
         """
         Searches for vocabularies within a specific Amazon Connect instance using
         `State`, `NameStartsWith`, and
         `LanguageCode`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_vocabularies)
@@ -2521,15 +2520,15 @@
     async def send_chat_integration_event(
         self,
         *,
         SourceId: str,
         DestinationId: str,
         Event: ChatEventTypeDef,
         Subtype: str = ...,
-        NewSessionDetails: NewSessionDetailsTypeDef = ...
+        NewSessionDetails: NewSessionDetailsTypeDef = ...,
     ) -> SendChatIntegrationEventResponseTypeDef:
         """
         Processes chat integration events from Amazon Web Services or external
         integrations to Amazon
         Connect.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.send_chat_integration_event)
@@ -2545,15 +2544,15 @@
         Attributes: Mapping[str, str] = ...,
         InitialMessage: ChatMessageTypeDef = ...,
         ClientToken: str = ...,
         ChatDurationInMinutes: int = ...,
         SupportedMessagingContentTypes: Sequence[str] = ...,
         PersistentChat: PersistentChatTypeDef = ...,
         RelatedContactId: str = ...,
-        SegmentAttributes: Mapping[str, SegmentAttributeValueTypeDef] = ...
+        SegmentAttributes: Mapping[str, SegmentAttributeValueTypeDef] = ...,
     ) -> StartChatContactResponseTypeDef:
         """
         Initiates a flow to start a new chat for the customer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.start_chat_contact)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#start_chat_contact)
         """
@@ -2572,15 +2571,15 @@
 
     async def start_contact_recording(
         self,
         *,
         InstanceId: str,
         ContactId: str,
         InitialContactId: str,
-        VoiceRecordingConfiguration: VoiceRecordingConfigurationTypeDef
+        VoiceRecordingConfiguration: VoiceRecordingConfigurationTypeDef,
     ) -> Dict[str, Any]:
         """
         Starts recording the contact: * If the API is called *before* the agent joins
         the call, recording starts when the agent joins the
         call.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.start_contact_recording)
@@ -2589,15 +2588,15 @@
 
     async def start_contact_streaming(
         self,
         *,
         InstanceId: str,
         ContactId: str,
         ChatStreamingConfiguration: ChatStreamingConfigurationTypeDef,
-        ClientToken: str
+        ClientToken: str,
     ) -> StartContactStreamingResponseTypeDef:
         """
         Initiates real-time message streaming for a new chat contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.start_contact_streaming)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#start_contact_streaming)
         """
@@ -2610,15 +2609,15 @@
         InstanceId: str,
         ClientToken: str = ...,
         SourcePhoneNumber: str = ...,
         QueueId: str = ...,
         Attributes: Mapping[str, str] = ...,
         AnswerMachineDetectionConfig: AnswerMachineDetectionConfigTypeDef = ...,
         CampaignId: str = ...,
-        TrafficType: TrafficTypeType = ...
+        TrafficType: TrafficTypeType = ...,
     ) -> StartOutboundVoiceContactResponseTypeDef:
         """
         Places an outbound call to a contact, and then initiates the flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.start_outbound_voice_contact)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#start_outbound_voice_contact)
         """
@@ -2633,15 +2632,15 @@
         Attributes: Mapping[str, str] = ...,
         References: Mapping[str, ReferenceTypeDef] = ...,
         Description: str = ...,
         ClientToken: str = ...,
         ScheduledTime: TimestampTypeDef = ...,
         TaskTemplateId: str = ...,
         QuickConnectId: str = ...,
-        RelatedContactId: str = ...
+        RelatedContactId: str = ...,
     ) -> StartTaskContactResponseTypeDef:
         """
         Initiates a flow to start a new task contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.start_task_contact)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#start_task_contact)
         """
@@ -2653,15 +2652,15 @@
         InstanceId: str,
         ParticipantDetails: ParticipantDetailsTypeDef,
         Attributes: Mapping[str, str] = ...,
         ClientToken: str = ...,
         AllowedCapabilities: AllowedCapabilitiesTypeDef = ...,
         RelatedContactId: str = ...,
         References: Mapping[str, ReferenceTypeDef] = ...,
-        Description: str = ...
+        Description: str = ...,
     ) -> StartWebRTCContactResponseTypeDef:
         """
         Places an inbound in-app, web, or video call to a contact, and then initiates
         the
         flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.start_web_rtc_contact)
@@ -2700,15 +2699,15 @@
 
     async def submit_contact_evaluation(
         self,
         *,
         InstanceId: str,
         EvaluationId: str,
         Answers: Mapping[str, EvaluationAnswerInputTypeDef] = ...,
-        Notes: Mapping[str, EvaluationNoteTypeDef] = ...
+        Notes: Mapping[str, EvaluationNoteTypeDef] = ...,
     ) -> SubmitContactEvaluationResponseTypeDef:
         """
         Submits a contact evaluation in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.submit_contact_evaluation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#submit_contact_evaluation)
         """
@@ -2739,15 +2738,15 @@
         self,
         *,
         InstanceId: str,
         ContactId: str,
         ContactFlowId: str,
         QueueId: str = ...,
         UserId: str = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> TransferContactResponseTypeDef:
         """
         Transfers contacts from one agent or queue to another agent or queue at any
         point after a contact is
         created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.transfer_contact)
@@ -2769,15 +2768,15 @@
         *,
         InstanceId: str,
         AgentStatusId: str,
         Name: str = ...,
         Description: str = ...,
         State: AgentStatusStateType = ...,
         DisplayOrder: int = ...,
-        ResetOrderNumber: bool = ...
+        ResetOrderNumber: bool = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_agent_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#update_agent_status)
         """
@@ -2785,15 +2784,15 @@
     async def update_contact(
         self,
         *,
         InstanceId: str,
         ContactId: str,
         Name: str = ...,
         Description: str = ...,
-        References: Mapping[str, ReferenceTypeDef] = ...
+        References: Mapping[str, ReferenceTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_contact)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#update_contact)
         """
@@ -2812,15 +2811,15 @@
 
     async def update_contact_evaluation(
         self,
         *,
         InstanceId: str,
         EvaluationId: str,
         Answers: Mapping[str, EvaluationAnswerInputTypeDef] = ...,
-        Notes: Mapping[str, EvaluationNoteTypeDef] = ...
+        Notes: Mapping[str, EvaluationNoteTypeDef] = ...,
     ) -> UpdateContactEvaluationResponseTypeDef:
         """
         Updates details about a contact evaluation in the specified Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_contact_evaluation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#update_contact_evaluation)
@@ -2839,15 +2838,15 @@
     async def update_contact_flow_metadata(
         self,
         *,
         InstanceId: str,
         ContactFlowId: str,
         Name: str = ...,
         Description: str = ...,
-        ContactFlowState: ContactFlowStateType = ...
+        ContactFlowState: ContactFlowStateType = ...,
     ) -> Dict[str, Any]:
         """
         Updates metadata about specified flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_contact_flow_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#update_contact_flow_metadata)
         """
@@ -2865,15 +2864,15 @@
     async def update_contact_flow_module_metadata(
         self,
         *,
         InstanceId: str,
         ContactFlowModuleId: str,
         Name: str = ...,
         Description: str = ...,
-        State: ContactFlowModuleStateType = ...
+        State: ContactFlowModuleStateType = ...,
     ) -> Dict[str, Any]:
         """
         Updates metadata about specified flow module.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_contact_flow_module_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#update_contact_flow_module_metadata)
         """
@@ -2905,15 +2904,15 @@
         EvaluationFormId: str,
         EvaluationFormVersion: int,
         Title: str,
         Items: Sequence["EvaluationFormItemTypeDef"],
         CreateNewVersion: bool = ...,
         Description: str = ...,
         ScoringStrategy: EvaluationFormScoringStrategyTypeDef = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> UpdateEvaluationFormResponseTypeDef:
         """
         Updates details about a specific evaluation form version in the specified
         Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_evaluation_form)
@@ -2924,15 +2923,15 @@
         self,
         *,
         InstanceId: str,
         HoursOfOperationId: str,
         Name: str = ...,
         Description: str = ...,
         TimeZone: str = ...,
-        Config: Sequence[HoursOfOperationConfigTypeDef] = ...
+        Config: Sequence[HoursOfOperationConfigTypeDef] = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_hours_of_operation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#update_hours_of_operation)
         """
@@ -2949,29 +2948,29 @@
 
     async def update_instance_storage_config(
         self,
         *,
         InstanceId: str,
         AssociationId: str,
         ResourceType: InstanceStorageResourceTypeType,
-        StorageConfig: InstanceStorageConfigTypeDef
+        StorageConfig: InstanceStorageConfigTypeDef,
     ) -> EmptyResponseMetadataTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_instance_storage_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#update_instance_storage_config)
         """
 
     async def update_participant_role_config(
         self,
         *,
         InstanceId: str,
         ContactId: str,
-        ChannelConfiguration: UpdateParticipantRoleConfigChannelInfoTypeDef
+        ChannelConfiguration: UpdateParticipantRoleConfigChannelInfoTypeDef,
     ) -> Dict[str, Any]:
         """
         Updates timeouts for when human chat participants are to be considered idle,
         and when agents are automatically disconnected from a chat due to
         idleness.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_participant_role_config)
@@ -2980,15 +2979,15 @@
 
     async def update_phone_number(
         self,
         *,
         PhoneNumberId: str,
         TargetArn: str = ...,
         InstanceId: str = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> UpdatePhoneNumberResponseTypeDef:
         """
         Updates your claimed phone number from its current Amazon Connect instance or
         traffic distribution group to another Amazon Connect instance or traffic
         distribution group in the same Amazon Web Services
         Region.
 
@@ -3009,15 +3008,15 @@
     async def update_prompt(
         self,
         *,
         InstanceId: str,
         PromptId: str,
         Name: str = ...,
         Description: str = ...,
-        S3Uri: str = ...
+        S3Uri: str = ...,
     ) -> UpdatePromptResponseTypeDef:
         """
         Updates a prompt.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_prompt)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#update_prompt)
         """
@@ -3093,15 +3092,15 @@
         """
 
     async def update_routing_profile_agent_availability_timer(
         self,
         *,
         InstanceId: str,
         RoutingProfileId: str,
-        AgentAvailabilityTimer: AgentAvailabilityTimerType
+        AgentAvailabilityTimer: AgentAvailabilityTimerType,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Whether agents with this routing profile will have their routing order
         calculated based on *time since their last inbound contact* or *longest idle
         time*.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_routing_profile_agent_availability_timer)
@@ -3109,15 +3108,15 @@
         """
 
     async def update_routing_profile_concurrency(
         self,
         *,
         InstanceId: str,
         RoutingProfileId: str,
-        MediaConcurrencies: Sequence[MediaConcurrencyTypeDef]
+        MediaConcurrencies: Sequence[MediaConcurrencyTypeDef],
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates the channels that agents can handle in the Contact Control Panel (CCP)
         for a routing
         profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_routing_profile_concurrency)
@@ -3145,15 +3144,15 @@
         """
 
     async def update_routing_profile_queues(
         self,
         *,
         InstanceId: str,
         RoutingProfileId: str,
-        QueueConfigs: Sequence[RoutingProfileQueueConfigTypeDef]
+        QueueConfigs: Sequence[RoutingProfileQueueConfigTypeDef],
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates the properties associated with a set of queues for a routing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_routing_profile_queues)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#update_routing_profile_queues)
         """
@@ -3162,15 +3161,15 @@
         self,
         *,
         RuleId: str,
         InstanceId: str,
         Name: str,
         Function: str,
         Actions: Sequence[RuleActionTypeDef],
-        PublishStatus: RulePublishStatusType
+        PublishStatus: RulePublishStatusType,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a rule for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#update_rule)
         """
@@ -3180,15 +3179,15 @@
         *,
         SecurityProfileId: str,
         InstanceId: str,
         Description: str = ...,
         Permissions: Sequence[str] = ...,
         AllowedAccessControlTags: Mapping[str, str] = ...,
         TagRestrictedResources: Sequence[str] = ...,
-        Applications: Sequence[ApplicationTypeDef] = ...
+        Applications: Sequence[ApplicationTypeDef] = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a security profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_security_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#update_security_profile)
         """
@@ -3200,15 +3199,15 @@
         InstanceId: str,
         Name: str = ...,
         Description: str = ...,
         ContactFlowId: str = ...,
         Constraints: TaskTemplateConstraintsTypeDef = ...,
         Defaults: TaskTemplateDefaultsTypeDef = ...,
         Status: TaskTemplateStatusType = ...,
-        Fields: Sequence[TaskTemplateFieldTypeDef] = ...
+        Fields: Sequence[TaskTemplateFieldTypeDef] = ...,
     ) -> UpdateTaskTemplateResponseTypeDef:
         """
         Updates details about a specific task template in the specified Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_task_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#update_task_template)
@@ -3216,15 +3215,15 @@
 
     async def update_traffic_distribution(
         self,
         *,
         Id: str,
         TelephonyConfig: TelephonyConfigTypeDef = ...,
         SignInConfig: SignInConfigTypeDef = ...,
-        AgentConfig: AgentConfigTypeDef = ...
+        AgentConfig: AgentConfigTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates the traffic distribution for a given traffic distribution group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_traffic_distribution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#update_traffic_distribution)
         """
@@ -3302,15 +3301,15 @@
 
     async def update_view_content(
         self,
         *,
         InstanceId: str,
         ViewId: str,
         Status: ViewStatusType,
-        Content: ViewInputContentTypeDef
+        Content: ViewInputContentTypeDef,
     ) -> UpdateViewContentResponseTypeDef:
         """
         Updates the view content of the given view identifier in the specified Amazon
         Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_view_content)
```

### Comparing `types-aiobotocore-connect-2.9.0/types_aiobotocore_connect/client.pyi` & `types-aiobotocore-connect-2.9.1/types_aiobotocore_connect/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -423,29 +423,29 @@
 
     async def associate_flow(
         self,
         *,
         InstanceId: str,
         ResourceId: str,
         FlowId: str,
-        ResourceType: Literal["SMS_PHONE_NUMBER"]
+        ResourceType: Literal["SMS_PHONE_NUMBER"],
     ) -> Dict[str, Any]:
         """
         Associates a connect resource to a flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.associate_flow)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#associate_flow)
         """
 
     async def associate_instance_storage_config(
         self,
         *,
         InstanceId: str,
         ResourceType: InstanceStorageResourceTypeType,
-        StorageConfig: InstanceStorageConfigTypeDef
+        StorageConfig: InstanceStorageConfigTypeDef,
     ) -> AssociateInstanceStorageConfigResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.associate_instance_storage_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#associate_instance_storage_config)
         """
@@ -491,15 +491,15 @@
         """
 
     async def associate_routing_profile_queues(
         self,
         *,
         InstanceId: str,
         RoutingProfileId: str,
-        QueueConfigs: Sequence[RoutingProfileQueueConfigTypeDef]
+        QueueConfigs: Sequence[RoutingProfileQueueConfigTypeDef],
     ) -> EmptyResponseMetadataTypeDef:
         """
         Associates a set of queues with a routing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.associate_routing_profile_queues)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#associate_routing_profile_queues)
         """
@@ -545,29 +545,29 @@
         """
 
     async def batch_get_flow_association(
         self,
         *,
         InstanceId: str,
         ResourceIds: Sequence[str],
-        ResourceType: Literal["VOICE_PHONE_NUMBER"] = ...
+        ResourceType: Literal["VOICE_PHONE_NUMBER"] = ...,
     ) -> BatchGetFlowAssociationResponseTypeDef:
         """
         Retrieve the flow associations for the given resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.batch_get_flow_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#batch_get_flow_association)
         """
 
     async def batch_put_contact(
         self,
         *,
         InstanceId: str,
         ContactDataRequestList: Sequence[ContactDataRequestTypeDef],
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> BatchPutContactResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.batch_put_contact)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#batch_put_contact)
         """
@@ -584,15 +584,15 @@
         self,
         *,
         PhoneNumber: str,
         TargetArn: str = ...,
         InstanceId: str = ...,
         PhoneNumberDescription: str = ...,
         Tags: Mapping[str, str] = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> ClaimPhoneNumberResponseTypeDef:
         """
         Claims an available phone number to your Amazon Connect instance or traffic
         distribution
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.claim_phone_number)
@@ -611,15 +611,15 @@
         self,
         *,
         InstanceId: str,
         Name: str,
         State: AgentStatusStateType,
         Description: str = ...,
         DisplayOrder: int = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateAgentStatusResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_agent_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#create_agent_status)
         """
@@ -628,15 +628,15 @@
         self,
         *,
         InstanceId: str,
         Name: str,
         Type: ContactFlowTypeType,
         Content: str,
         Description: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateContactFlowResponseTypeDef:
         """
         Creates a flow for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_contact_flow)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#create_contact_flow)
         """
@@ -645,15 +645,15 @@
         self,
         *,
         InstanceId: str,
         Name: str,
         Content: str,
         Description: str = ...,
         Tags: Mapping[str, str] = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreateContactFlowModuleResponseTypeDef:
         """
         Creates a flow module for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_contact_flow_module)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#create_contact_flow_module)
         """
@@ -662,15 +662,15 @@
         self,
         *,
         InstanceId: str,
         Title: str,
         Items: Sequence["EvaluationFormItemTypeDef"],
         Description: str = ...,
         ScoringStrategy: EvaluationFormScoringStrategyTypeDef = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreateEvaluationFormResponseTypeDef:
         """
         Creates an evaluation form in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_evaluation_form)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#create_evaluation_form)
         """
@@ -679,15 +679,15 @@
         self,
         *,
         InstanceId: str,
         Name: str,
         TimeZone: str,
         Config: Sequence[HoursOfOperationConfigTypeDef],
         Description: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateHoursOfOperationResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_hours_of_operation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#create_hours_of_operation)
         """
@@ -697,15 +697,15 @@
         *,
         IdentityManagementType: DirectoryTypeType,
         InboundCallsEnabled: bool,
         OutboundCallsEnabled: bool,
         ClientToken: str = ...,
         InstanceAlias: str = ...,
         DirectoryId: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateInstanceResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#create_instance)
         """
@@ -715,15 +715,15 @@
         *,
         InstanceId: str,
         IntegrationType: IntegrationTypeType,
         IntegrationArn: str,
         SourceApplicationUrl: str = ...,
         SourceApplicationName: str = ...,
         SourceType: SourceTypeType = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateIntegrationAssociationResponseTypeDef:
         """
         Creates an Amazon Web Services resource association with an Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_integration_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#create_integration_association)
@@ -731,15 +731,15 @@
 
     async def create_participant(
         self,
         *,
         InstanceId: str,
         ContactId: str,
         ParticipantDetails: ParticipantDetailsToAddTypeDef,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreateParticipantResponseTypeDef:
         """
         Adds a new participant into an on-going chat contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_participant)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#create_participant)
         """
@@ -747,15 +747,15 @@
     async def create_persistent_contact_association(
         self,
         *,
         InstanceId: str,
         InitialContactId: str,
         RehydrationType: RehydrationTypeType,
         SourceContactId: str,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreatePersistentContactAssociationResponseTypeDef:
         """
         Enables rehydration of chats for the lifespan of a contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_persistent_contact_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#create_persistent_contact_association)
         """
@@ -763,15 +763,15 @@
     async def create_prompt(
         self,
         *,
         InstanceId: str,
         Name: str,
         S3Uri: str,
         Description: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreatePromptResponseTypeDef:
         """
         Creates a prompt.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_prompt)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#create_prompt)
         """
@@ -782,15 +782,15 @@
         InstanceId: str,
         Name: str,
         HoursOfOperationId: str,
         Description: str = ...,
         OutboundCallerConfig: OutboundCallerConfigTypeDef = ...,
         MaxContacts: int = ...,
         QuickConnectIds: Sequence[str] = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateQueueResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_queue)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#create_queue)
         """
@@ -798,15 +798,15 @@
     async def create_quick_connect(
         self,
         *,
         InstanceId: str,
         Name: str,
         QuickConnectConfig: QuickConnectConfigTypeDef,
         Description: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateQuickConnectResponseTypeDef:
         """
         Creates a quick connect for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_quick_connect)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#create_quick_connect)
         """
@@ -817,15 +817,15 @@
         InstanceId: str,
         Name: str,
         Description: str,
         DefaultOutboundQueueId: str,
         MediaConcurrencies: Sequence[MediaConcurrencyTypeDef],
         QueueConfigs: Sequence[RoutingProfileQueueConfigTypeDef] = ...,
         Tags: Mapping[str, str] = ...,
-        AgentAvailabilityTimer: AgentAvailabilityTimerType = ...
+        AgentAvailabilityTimer: AgentAvailabilityTimerType = ...,
     ) -> CreateRoutingProfileResponseTypeDef:
         """
         Creates a new routing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_routing_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#create_routing_profile)
         """
@@ -835,15 +835,15 @@
         *,
         InstanceId: str,
         Name: str,
         TriggerEventSource: RuleTriggerEventSourceTypeDef,
         Function: str,
         Actions: Sequence[RuleActionTypeDef],
         PublishStatus: RulePublishStatusType,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreateRuleResponseTypeDef:
         """
         Creates a rule for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#create_rule)
         """
@@ -854,15 +854,15 @@
         SecurityProfileName: str,
         InstanceId: str,
         Description: str = ...,
         Permissions: Sequence[str] = ...,
         Tags: Mapping[str, str] = ...,
         AllowedAccessControlTags: Mapping[str, str] = ...,
         TagRestrictedResources: Sequence[str] = ...,
-        Applications: Sequence[ApplicationTypeDef] = ...
+        Applications: Sequence[ApplicationTypeDef] = ...,
     ) -> CreateSecurityProfileResponseTypeDef:
         """
         Creates a security profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_security_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#create_security_profile)
         """
@@ -874,15 +874,15 @@
         Name: str,
         Fields: Sequence[TaskTemplateFieldTypeDef],
         Description: str = ...,
         ContactFlowId: str = ...,
         Constraints: TaskTemplateConstraintsTypeDef = ...,
         Defaults: TaskTemplateDefaultsTypeDef = ...,
         Status: TaskTemplateStatusType = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreateTaskTemplateResponseTypeDef:
         """
         Creates a new task template in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_task_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#create_task_template)
         """
@@ -890,15 +890,15 @@
     async def create_traffic_distribution_group(
         self,
         *,
         Name: str,
         InstanceId: str,
         Description: str = ...,
         ClientToken: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateTrafficDistributionGroupResponseTypeDef:
         """
         Creates a traffic distribution group given an Amazon Connect instance that has
         been
         replicated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_traffic_distribution_group)
@@ -907,15 +907,15 @@
 
     async def create_use_case(
         self,
         *,
         InstanceId: str,
         IntegrationAssociationId: str,
         UseCaseType: UseCaseTypeType,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateUseCaseResponseTypeDef:
         """
         Creates a use case for an integration association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_use_case)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#create_use_case)
         """
@@ -928,15 +928,15 @@
         SecurityProfileIds: Sequence[str],
         RoutingProfileId: str,
         InstanceId: str,
         Password: str = ...,
         IdentityInfo: UserIdentityInfoTypeDef = ...,
         DirectoryUserId: str = ...,
         HierarchyGroupId: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateUserResponseTypeDef:
         """
         Creates a user account for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#create_user)
         """
@@ -956,30 +956,30 @@
         *,
         InstanceId: str,
         Status: ViewStatusType,
         Content: ViewInputContentTypeDef,
         Name: str,
         ClientToken: str = ...,
         Description: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateViewResponseTypeDef:
         """
         Creates a new view with the possible status of `SAVED` or `PUBLISHED`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_view)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#create_view)
         """
 
     async def create_view_version(
         self,
         *,
         InstanceId: str,
         ViewId: str,
         VersionDescription: str = ...,
-        ViewContentSha256: str = ...
+        ViewContentSha256: str = ...,
     ) -> CreateViewVersionResponseTypeDef:
         """
         Publishes a new version of the view identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_view_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#create_view_version)
         """
@@ -988,15 +988,15 @@
         self,
         *,
         InstanceId: str,
         VocabularyName: str,
         LanguageCode: VocabularyLanguageCodeType,
         Content: str,
         ClientToken: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateVocabularyResponseTypeDef:
         """
         Creates a custom vocabulary associated with your Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_vocabulary)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#create_vocabulary)
         """
@@ -1525,15 +1525,15 @@
         """
 
     async def disassociate_routing_profile_queues(
         self,
         *,
         InstanceId: str,
         RoutingProfileId: str,
-        QueueReferences: Sequence[RoutingProfileQueueReferenceTypeDef]
+        QueueReferences: Sequence[RoutingProfileQueueReferenceTypeDef],
     ) -> EmptyResponseMetadataTypeDef:
         """
         Disassociates a set of queues from a routing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.disassociate_routing_profile_queues)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#disassociate_routing_profile_queues)
         """
@@ -1599,30 +1599,30 @@
         *,
         InstanceId: str,
         Filters: FiltersTypeDef,
         CurrentMetrics: Sequence[CurrentMetricTypeDef],
         Groupings: Sequence[GroupingType] = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        SortCriteria: Sequence[CurrentMetricSortCriteriaTypeDef] = ...
+        SortCriteria: Sequence[CurrentMetricSortCriteriaTypeDef] = ...,
     ) -> GetCurrentMetricDataResponseTypeDef:
         """
         Gets the real-time metric data from the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_current_metric_data)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#get_current_metric_data)
         """
 
     async def get_current_user_data(
         self,
         *,
         InstanceId: str,
         Filters: UserDataFiltersTypeDef,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> GetCurrentUserDataResponseTypeDef:
         """
         Gets the real-time active user data from the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_current_user_data)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#get_current_user_data)
         """
@@ -1651,15 +1651,15 @@
         InstanceId: str,
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
         Filters: FiltersTypeDef,
         HistoricalMetrics: Sequence[HistoricalMetricTypeDef],
         Groupings: Sequence[GroupingType] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> GetMetricDataResponseTypeDef:
         """
         Gets historical metric data from the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_metric_data)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#get_metric_data)
         """
@@ -1671,15 +1671,15 @@
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
         Filters: Sequence[FilterV2TypeDef],
         Metrics: Sequence[MetricV2TypeDef],
         Interval: IntervalDetailsTypeDef = ...,
         Groupings: Sequence[str] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> GetMetricDataV2ResponseTypeDef:
         """
         Gets metric data from the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_metric_data_v2)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#get_metric_data_v2)
         """
@@ -1717,15 +1717,15 @@
     async def import_phone_number(
         self,
         *,
         InstanceId: str,
         SourcePhoneNumberArn: str,
         PhoneNumberDescription: str = ...,
         Tags: Mapping[str, str] = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> ImportPhoneNumberResponseTypeDef:
         """
         Imports a claimed phone number from an external service, such as Amazon
         Pinpoint, into an Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.import_phone_number)
@@ -1734,15 +1734,15 @@
 
     async def list_agent_statuses(
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
-        AgentStatusTypes: Sequence[AgentStatusTypeType] = ...
+        AgentStatusTypes: Sequence[AgentStatusTypeType] = ...,
     ) -> ListAgentStatusResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_agent_statuses)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#list_agent_statuses)
         """
@@ -1769,15 +1769,15 @@
 
     async def list_bots(
         self,
         *,
         InstanceId: str,
         LexVersion: LexVersionType,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListBotsResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_bots)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#list_bots)
         """
@@ -1794,15 +1794,15 @@
 
     async def list_contact_flow_modules(
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
-        ContactFlowModuleState: ContactFlowModuleStateType = ...
+        ContactFlowModuleState: ContactFlowModuleStateType = ...,
     ) -> ListContactFlowModulesResponseTypeDef:
         """
         Provides information about the flow modules for the specified Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_contact_flow_modules)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#list_contact_flow_modules)
@@ -1810,45 +1810,45 @@
 
     async def list_contact_flows(
         self,
         *,
         InstanceId: str,
         ContactFlowTypes: Sequence[ContactFlowTypeType] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListContactFlowsResponseTypeDef:
         """
         Provides information about the flows for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_contact_flows)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#list_contact_flows)
         """
 
     async def list_contact_references(
         self,
         *,
         InstanceId: str,
         ContactId: str,
         ReferenceTypes: Sequence[ReferenceTypeType],
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListContactReferencesResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_contact_references)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#list_contact_references)
         """
 
     async def list_default_vocabularies(
         self,
         *,
         InstanceId: str,
         LanguageCode: VocabularyLanguageCodeType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListDefaultVocabulariesResponseTypeDef:
         """
         Lists the default vocabularies for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_default_vocabularies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#list_default_vocabularies)
         """
@@ -1875,15 +1875,15 @@
 
     async def list_flow_associations(
         self,
         *,
         InstanceId: str,
         ResourceType: Literal["VOICE_PHONE_NUMBER"] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListFlowAssociationsResponseTypeDef:
         """
         List the flow association based on the filters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_flow_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#list_flow_associations)
         """
@@ -1912,15 +1912,15 @@
 
     async def list_instance_storage_configs(
         self,
         *,
         InstanceId: str,
         ResourceType: InstanceStorageResourceTypeType,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListInstanceStorageConfigsResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_instance_storage_configs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#list_instance_storage_configs)
         """
@@ -1938,15 +1938,15 @@
     async def list_integration_associations(
         self,
         *,
         InstanceId: str,
         IntegrationType: IntegrationTypeType = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        IntegrationArn: str = ...
+        IntegrationArn: str = ...,
     ) -> ListIntegrationAssociationsResponseTypeDef:
         """
         Provides summary information about the Amazon Web Services resource
         associations for the specified Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_integration_associations)
@@ -1976,15 +1976,15 @@
     async def list_phone_numbers(
         self,
         *,
         InstanceId: str,
         PhoneNumberTypes: Sequence[PhoneNumberTypeType] = ...,
         PhoneNumberCountryCodes: Sequence[PhoneNumberCountryCodeType] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListPhoneNumbersResponseTypeDef:
         """
         Provides information about the phone numbers for the specified Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_phone_numbers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#list_phone_numbers)
@@ -1995,15 +1995,15 @@
         *,
         TargetArn: str = ...,
         InstanceId: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         PhoneNumberCountryCodes: Sequence[PhoneNumberCountryCodeType] = ...,
         PhoneNumberTypes: Sequence[PhoneNumberTypeType] = ...,
-        PhoneNumberPrefix: str = ...
+        PhoneNumberPrefix: str = ...,
     ) -> ListPhoneNumbersV2ResponseTypeDef:
         """
         Lists phone numbers claimed to your Amazon Connect instance or traffic
         distribution
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_phone_numbers_v2)
@@ -2033,30 +2033,30 @@
 
     async def list_queues(
         self,
         *,
         InstanceId: str,
         QueueTypes: Sequence[QueueTypeType] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListQueuesResponseTypeDef:
         """
         Provides information about the queues for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_queues)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#list_queues)
         """
 
     async def list_quick_connects(
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
-        QuickConnectTypes: Sequence[QuickConnectTypeType] = ...
+        QuickConnectTypes: Sequence[QuickConnectTypeType] = ...,
     ) -> ListQuickConnectsResponseTypeDef:
         """
         Provides information about the quick connects for the specified Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_quick_connects)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#list_quick_connects)
@@ -2066,15 +2066,15 @@
         self,
         *,
         InstanceId: str,
         ContactId: str,
         OutputType: RealTimeContactAnalysisOutputTypeType,
         SegmentTypes: Sequence[RealTimeContactAnalysisSegmentTypeType],
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListRealtimeContactAnalysisSegmentsV2ResponseTypeDef:
         """
         Provides a list of analysis segments for a real-time analysis session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_realtime_contact_analysis_segments_v2)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#list_realtime_contact_analysis_segments_v2)
         """
@@ -2104,15 +2104,15 @@
     async def list_rules(
         self,
         *,
         InstanceId: str,
         PublishStatus: RulePublishStatusType = ...,
         EventSourceName: EventSourceNameType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListRulesResponseTypeDef:
         """
         List all rules for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_rules)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#list_rules)
         """
@@ -2129,30 +2129,30 @@
 
     async def list_security_profile_applications(
         self,
         *,
         SecurityProfileId: str,
         InstanceId: str,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListSecurityProfileApplicationsResponseTypeDef:
         """
         Returns a list of third-party applications in a specific security profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_security_profile_applications)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#list_security_profile_applications)
         """
 
     async def list_security_profile_permissions(
         self,
         *,
         SecurityProfileId: str,
         InstanceId: str,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListSecurityProfilePermissionsResponseTypeDef:
         """
         Lists the permissions granted to a security profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_security_profile_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#list_security_profile_permissions)
         """
@@ -2182,15 +2182,15 @@
     async def list_task_templates(
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         Status: TaskTemplateStatusType = ...,
-        Name: str = ...
+        Name: str = ...,
     ) -> ListTaskTemplatesResponseTypeDef:
         """
         Lists task templates for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_task_templates)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#list_task_templates)
         """
@@ -2217,15 +2217,15 @@
 
     async def list_use_cases(
         self,
         *,
         InstanceId: str,
         IntegrationAssociationId: str,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListUseCasesResponseTypeDef:
         """
         Lists the use cases for the integration association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_use_cases)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#list_use_cases)
         """
@@ -2267,15 +2267,15 @@
 
     async def list_views(
         self,
         *,
         InstanceId: str,
         Type: ViewTypeType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListViewsResponseTypeDef:
         """
         Returns views in the given instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_views)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#list_views)
         """
@@ -2283,15 +2283,15 @@
     async def monitor_contact(
         self,
         *,
         InstanceId: str,
         ContactId: str,
         UserId: str,
         AllowedMonitorCapabilities: Sequence[MonitorCapabilityType] = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> MonitorContactResponseTypeDef:
         """
         Initiates silent monitoring of a contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.monitor_contact)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#monitor_contact)
         """
@@ -2349,15 +2349,15 @@
         *,
         PhoneNumberCountryCode: PhoneNumberCountryCodeType,
         PhoneNumberType: PhoneNumberTypeType,
         TargetArn: str = ...,
         InstanceId: str = ...,
         PhoneNumberPrefix: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> SearchAvailablePhoneNumbersResponseTypeDef:
         """
         Searches for available phone numbers that you can claim to your Amazon Connect
         instance or traffic distribution
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_available_phone_numbers)
@@ -2367,15 +2367,15 @@
     async def search_hours_of_operations(
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchFilter: HoursOfOperationSearchFilterTypeDef = ...,
-        SearchCriteria: "HoursOfOperationSearchCriteriaTypeDef" = ...
+        SearchCriteria: "HoursOfOperationSearchCriteriaTypeDef" = ...,
     ) -> SearchHoursOfOperationsResponseTypeDef:
         """
         Searches the hours of operation in an Amazon Connect instance, with optional
         filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_hours_of_operations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#search_hours_of_operations)
@@ -2384,15 +2384,15 @@
     async def search_prompts(
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchFilter: PromptSearchFilterTypeDef = ...,
-        SearchCriteria: "PromptSearchCriteriaTypeDef" = ...
+        SearchCriteria: "PromptSearchCriteriaTypeDef" = ...,
     ) -> SearchPromptsResponseTypeDef:
         """
         Searches prompts in an Amazon Connect instance, with optional filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_prompts)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#search_prompts)
         """
@@ -2400,15 +2400,15 @@
     async def search_queues(
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchFilter: QueueSearchFilterTypeDef = ...,
-        SearchCriteria: "QueueSearchCriteriaTypeDef" = ...
+        SearchCriteria: "QueueSearchCriteriaTypeDef" = ...,
     ) -> SearchQueuesResponseTypeDef:
         """
         Searches queues in an Amazon Connect instance, with optional filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_queues)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#search_queues)
         """
@@ -2416,15 +2416,15 @@
     async def search_quick_connects(
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchFilter: QuickConnectSearchFilterTypeDef = ...,
-        SearchCriteria: "QuickConnectSearchCriteriaTypeDef" = ...
+        SearchCriteria: "QuickConnectSearchCriteriaTypeDef" = ...,
     ) -> SearchQuickConnectsResponseTypeDef:
         """
         Searches quick connects in an Amazon Connect instance, with optional filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_quick_connects)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#search_quick_connects)
         """
@@ -2432,15 +2432,15 @@
     async def search_resource_tags(
         self,
         *,
         InstanceId: str,
         ResourceTypes: Sequence[str] = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        SearchCriteria: ResourceTagsSearchCriteriaTypeDef = ...
+        SearchCriteria: ResourceTagsSearchCriteriaTypeDef = ...,
     ) -> SearchResourceTagsResponseTypeDef:
         """
         Searches tags used in an Amazon Connect instance using optional search criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_resource_tags)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#search_resource_tags)
         """
@@ -2448,15 +2448,15 @@
     async def search_routing_profiles(
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchFilter: RoutingProfileSearchFilterTypeDef = ...,
-        SearchCriteria: "RoutingProfileSearchCriteriaTypeDef" = ...
+        SearchCriteria: "RoutingProfileSearchCriteriaTypeDef" = ...,
     ) -> SearchRoutingProfilesResponseTypeDef:
         """
         Searches routing profiles in an Amazon Connect instance, with optional
         filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_routing_profiles)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#search_routing_profiles)
@@ -2465,15 +2465,15 @@
     async def search_security_profiles(
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchCriteria: "SecurityProfileSearchCriteriaTypeDef" = ...,
-        SearchFilter: SecurityProfilesSearchFilterTypeDef = ...
+        SearchFilter: SecurityProfilesSearchFilterTypeDef = ...,
     ) -> SearchSecurityProfilesResponseTypeDef:
         """
         Searches security profiles in an Amazon Connect instance, with optional
         filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_security_profiles)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#search_security_profiles)
@@ -2482,15 +2482,15 @@
     async def search_users(
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchFilter: UserSearchFilterTypeDef = ...,
-        SearchCriteria: "UserSearchCriteriaTypeDef" = ...
+        SearchCriteria: "UserSearchCriteriaTypeDef" = ...,
     ) -> SearchUsersResponseTypeDef:
         """
         Searches users in an Amazon Connect instance, with optional filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_users)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#search_users)
         """
@@ -2499,15 +2499,15 @@
         self,
         *,
         InstanceId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
         State: VocabularyStateType = ...,
         NameStartsWith: str = ...,
-        LanguageCode: VocabularyLanguageCodeType = ...
+        LanguageCode: VocabularyLanguageCodeType = ...,
     ) -> SearchVocabulariesResponseTypeDef:
         """
         Searches for vocabularies within a specific Amazon Connect instance using
         `State`, `NameStartsWith`, and
         `LanguageCode`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_vocabularies)
@@ -2517,15 +2517,15 @@
     async def send_chat_integration_event(
         self,
         *,
         SourceId: str,
         DestinationId: str,
         Event: ChatEventTypeDef,
         Subtype: str = ...,
-        NewSessionDetails: NewSessionDetailsTypeDef = ...
+        NewSessionDetails: NewSessionDetailsTypeDef = ...,
     ) -> SendChatIntegrationEventResponseTypeDef:
         """
         Processes chat integration events from Amazon Web Services or external
         integrations to Amazon
         Connect.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.send_chat_integration_event)
@@ -2541,15 +2541,15 @@
         Attributes: Mapping[str, str] = ...,
         InitialMessage: ChatMessageTypeDef = ...,
         ClientToken: str = ...,
         ChatDurationInMinutes: int = ...,
         SupportedMessagingContentTypes: Sequence[str] = ...,
         PersistentChat: PersistentChatTypeDef = ...,
         RelatedContactId: str = ...,
-        SegmentAttributes: Mapping[str, SegmentAttributeValueTypeDef] = ...
+        SegmentAttributes: Mapping[str, SegmentAttributeValueTypeDef] = ...,
     ) -> StartChatContactResponseTypeDef:
         """
         Initiates a flow to start a new chat for the customer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.start_chat_contact)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#start_chat_contact)
         """
@@ -2568,15 +2568,15 @@
 
     async def start_contact_recording(
         self,
         *,
         InstanceId: str,
         ContactId: str,
         InitialContactId: str,
-        VoiceRecordingConfiguration: VoiceRecordingConfigurationTypeDef
+        VoiceRecordingConfiguration: VoiceRecordingConfigurationTypeDef,
     ) -> Dict[str, Any]:
         """
         Starts recording the contact: * If the API is called *before* the agent joins
         the call, recording starts when the agent joins the
         call.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.start_contact_recording)
@@ -2585,15 +2585,15 @@
 
     async def start_contact_streaming(
         self,
         *,
         InstanceId: str,
         ContactId: str,
         ChatStreamingConfiguration: ChatStreamingConfigurationTypeDef,
-        ClientToken: str
+        ClientToken: str,
     ) -> StartContactStreamingResponseTypeDef:
         """
         Initiates real-time message streaming for a new chat contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.start_contact_streaming)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#start_contact_streaming)
         """
@@ -2606,15 +2606,15 @@
         InstanceId: str,
         ClientToken: str = ...,
         SourcePhoneNumber: str = ...,
         QueueId: str = ...,
         Attributes: Mapping[str, str] = ...,
         AnswerMachineDetectionConfig: AnswerMachineDetectionConfigTypeDef = ...,
         CampaignId: str = ...,
-        TrafficType: TrafficTypeType = ...
+        TrafficType: TrafficTypeType = ...,
     ) -> StartOutboundVoiceContactResponseTypeDef:
         """
         Places an outbound call to a contact, and then initiates the flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.start_outbound_voice_contact)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#start_outbound_voice_contact)
         """
@@ -2629,15 +2629,15 @@
         Attributes: Mapping[str, str] = ...,
         References: Mapping[str, ReferenceTypeDef] = ...,
         Description: str = ...,
         ClientToken: str = ...,
         ScheduledTime: TimestampTypeDef = ...,
         TaskTemplateId: str = ...,
         QuickConnectId: str = ...,
-        RelatedContactId: str = ...
+        RelatedContactId: str = ...,
     ) -> StartTaskContactResponseTypeDef:
         """
         Initiates a flow to start a new task contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.start_task_contact)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#start_task_contact)
         """
@@ -2649,15 +2649,15 @@
         InstanceId: str,
         ParticipantDetails: ParticipantDetailsTypeDef,
         Attributes: Mapping[str, str] = ...,
         ClientToken: str = ...,
         AllowedCapabilities: AllowedCapabilitiesTypeDef = ...,
         RelatedContactId: str = ...,
         References: Mapping[str, ReferenceTypeDef] = ...,
-        Description: str = ...
+        Description: str = ...,
     ) -> StartWebRTCContactResponseTypeDef:
         """
         Places an inbound in-app, web, or video call to a contact, and then initiates
         the
         flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.start_web_rtc_contact)
@@ -2696,15 +2696,15 @@
 
     async def submit_contact_evaluation(
         self,
         *,
         InstanceId: str,
         EvaluationId: str,
         Answers: Mapping[str, EvaluationAnswerInputTypeDef] = ...,
-        Notes: Mapping[str, EvaluationNoteTypeDef] = ...
+        Notes: Mapping[str, EvaluationNoteTypeDef] = ...,
     ) -> SubmitContactEvaluationResponseTypeDef:
         """
         Submits a contact evaluation in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.submit_contact_evaluation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#submit_contact_evaluation)
         """
@@ -2735,15 +2735,15 @@
         self,
         *,
         InstanceId: str,
         ContactId: str,
         ContactFlowId: str,
         QueueId: str = ...,
         UserId: str = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> TransferContactResponseTypeDef:
         """
         Transfers contacts from one agent or queue to another agent or queue at any
         point after a contact is
         created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.transfer_contact)
@@ -2765,15 +2765,15 @@
         *,
         InstanceId: str,
         AgentStatusId: str,
         Name: str = ...,
         Description: str = ...,
         State: AgentStatusStateType = ...,
         DisplayOrder: int = ...,
-        ResetOrderNumber: bool = ...
+        ResetOrderNumber: bool = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_agent_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#update_agent_status)
         """
@@ -2781,15 +2781,15 @@
     async def update_contact(
         self,
         *,
         InstanceId: str,
         ContactId: str,
         Name: str = ...,
         Description: str = ...,
-        References: Mapping[str, ReferenceTypeDef] = ...
+        References: Mapping[str, ReferenceTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_contact)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#update_contact)
         """
@@ -2808,15 +2808,15 @@
 
     async def update_contact_evaluation(
         self,
         *,
         InstanceId: str,
         EvaluationId: str,
         Answers: Mapping[str, EvaluationAnswerInputTypeDef] = ...,
-        Notes: Mapping[str, EvaluationNoteTypeDef] = ...
+        Notes: Mapping[str, EvaluationNoteTypeDef] = ...,
     ) -> UpdateContactEvaluationResponseTypeDef:
         """
         Updates details about a contact evaluation in the specified Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_contact_evaluation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#update_contact_evaluation)
@@ -2835,15 +2835,15 @@
     async def update_contact_flow_metadata(
         self,
         *,
         InstanceId: str,
         ContactFlowId: str,
         Name: str = ...,
         Description: str = ...,
-        ContactFlowState: ContactFlowStateType = ...
+        ContactFlowState: ContactFlowStateType = ...,
     ) -> Dict[str, Any]:
         """
         Updates metadata about specified flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_contact_flow_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#update_contact_flow_metadata)
         """
@@ -2861,15 +2861,15 @@
     async def update_contact_flow_module_metadata(
         self,
         *,
         InstanceId: str,
         ContactFlowModuleId: str,
         Name: str = ...,
         Description: str = ...,
-        State: ContactFlowModuleStateType = ...
+        State: ContactFlowModuleStateType = ...,
     ) -> Dict[str, Any]:
         """
         Updates metadata about specified flow module.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_contact_flow_module_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#update_contact_flow_module_metadata)
         """
@@ -2901,15 +2901,15 @@
         EvaluationFormId: str,
         EvaluationFormVersion: int,
         Title: str,
         Items: Sequence["EvaluationFormItemTypeDef"],
         CreateNewVersion: bool = ...,
         Description: str = ...,
         ScoringStrategy: EvaluationFormScoringStrategyTypeDef = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> UpdateEvaluationFormResponseTypeDef:
         """
         Updates details about a specific evaluation form version in the specified
         Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_evaluation_form)
@@ -2920,15 +2920,15 @@
         self,
         *,
         InstanceId: str,
         HoursOfOperationId: str,
         Name: str = ...,
         Description: str = ...,
         TimeZone: str = ...,
-        Config: Sequence[HoursOfOperationConfigTypeDef] = ...
+        Config: Sequence[HoursOfOperationConfigTypeDef] = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_hours_of_operation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#update_hours_of_operation)
         """
@@ -2945,29 +2945,29 @@
 
     async def update_instance_storage_config(
         self,
         *,
         InstanceId: str,
         AssociationId: str,
         ResourceType: InstanceStorageResourceTypeType,
-        StorageConfig: InstanceStorageConfigTypeDef
+        StorageConfig: InstanceStorageConfigTypeDef,
     ) -> EmptyResponseMetadataTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_instance_storage_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#update_instance_storage_config)
         """
 
     async def update_participant_role_config(
         self,
         *,
         InstanceId: str,
         ContactId: str,
-        ChannelConfiguration: UpdateParticipantRoleConfigChannelInfoTypeDef
+        ChannelConfiguration: UpdateParticipantRoleConfigChannelInfoTypeDef,
     ) -> Dict[str, Any]:
         """
         Updates timeouts for when human chat participants are to be considered idle,
         and when agents are automatically disconnected from a chat due to
         idleness.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_participant_role_config)
@@ -2976,15 +2976,15 @@
 
     async def update_phone_number(
         self,
         *,
         PhoneNumberId: str,
         TargetArn: str = ...,
         InstanceId: str = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> UpdatePhoneNumberResponseTypeDef:
         """
         Updates your claimed phone number from its current Amazon Connect instance or
         traffic distribution group to another Amazon Connect instance or traffic
         distribution group in the same Amazon Web Services
         Region.
 
@@ -3005,15 +3005,15 @@
     async def update_prompt(
         self,
         *,
         InstanceId: str,
         PromptId: str,
         Name: str = ...,
         Description: str = ...,
-        S3Uri: str = ...
+        S3Uri: str = ...,
     ) -> UpdatePromptResponseTypeDef:
         """
         Updates a prompt.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_prompt)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#update_prompt)
         """
@@ -3089,15 +3089,15 @@
         """
 
     async def update_routing_profile_agent_availability_timer(
         self,
         *,
         InstanceId: str,
         RoutingProfileId: str,
-        AgentAvailabilityTimer: AgentAvailabilityTimerType
+        AgentAvailabilityTimer: AgentAvailabilityTimerType,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Whether agents with this routing profile will have their routing order
         calculated based on *time since their last inbound contact* or *longest idle
         time*.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_routing_profile_agent_availability_timer)
@@ -3105,15 +3105,15 @@
         """
 
     async def update_routing_profile_concurrency(
         self,
         *,
         InstanceId: str,
         RoutingProfileId: str,
-        MediaConcurrencies: Sequence[MediaConcurrencyTypeDef]
+        MediaConcurrencies: Sequence[MediaConcurrencyTypeDef],
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates the channels that agents can handle in the Contact Control Panel (CCP)
         for a routing
         profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_routing_profile_concurrency)
@@ -3141,15 +3141,15 @@
         """
 
     async def update_routing_profile_queues(
         self,
         *,
         InstanceId: str,
         RoutingProfileId: str,
-        QueueConfigs: Sequence[RoutingProfileQueueConfigTypeDef]
+        QueueConfigs: Sequence[RoutingProfileQueueConfigTypeDef],
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates the properties associated with a set of queues for a routing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_routing_profile_queues)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#update_routing_profile_queues)
         """
@@ -3158,15 +3158,15 @@
         self,
         *,
         RuleId: str,
         InstanceId: str,
         Name: str,
         Function: str,
         Actions: Sequence[RuleActionTypeDef],
-        PublishStatus: RulePublishStatusType
+        PublishStatus: RulePublishStatusType,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a rule for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#update_rule)
         """
@@ -3176,15 +3176,15 @@
         *,
         SecurityProfileId: str,
         InstanceId: str,
         Description: str = ...,
         Permissions: Sequence[str] = ...,
         AllowedAccessControlTags: Mapping[str, str] = ...,
         TagRestrictedResources: Sequence[str] = ...,
-        Applications: Sequence[ApplicationTypeDef] = ...
+        Applications: Sequence[ApplicationTypeDef] = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a security profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_security_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#update_security_profile)
         """
@@ -3196,15 +3196,15 @@
         InstanceId: str,
         Name: str = ...,
         Description: str = ...,
         ContactFlowId: str = ...,
         Constraints: TaskTemplateConstraintsTypeDef = ...,
         Defaults: TaskTemplateDefaultsTypeDef = ...,
         Status: TaskTemplateStatusType = ...,
-        Fields: Sequence[TaskTemplateFieldTypeDef] = ...
+        Fields: Sequence[TaskTemplateFieldTypeDef] = ...,
     ) -> UpdateTaskTemplateResponseTypeDef:
         """
         Updates details about a specific task template in the specified Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_task_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#update_task_template)
@@ -3212,15 +3212,15 @@
 
     async def update_traffic_distribution(
         self,
         *,
         Id: str,
         TelephonyConfig: TelephonyConfigTypeDef = ...,
         SignInConfig: SignInConfigTypeDef = ...,
-        AgentConfig: AgentConfigTypeDef = ...
+        AgentConfig: AgentConfigTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates the traffic distribution for a given traffic distribution group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_traffic_distribution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#update_traffic_distribution)
         """
@@ -3298,15 +3298,15 @@
 
     async def update_view_content(
         self,
         *,
         InstanceId: str,
         ViewId: str,
         Status: ViewStatusType,
-        Content: ViewInputContentTypeDef
+        Content: ViewInputContentTypeDef,
     ) -> UpdateViewContentResponseTypeDef:
         """
         Updates the view content of the given view identifier in the specified Amazon
         Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_view_content)
```

### Comparing `types-aiobotocore-connect-2.9.0/types_aiobotocore_connect/literals.py` & `types-aiobotocore-connect-2.9.1/types_aiobotocore_connect/literals.py`

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
     "ActionTypeType",
     "AgentAvailabilityTimerType",
     "AgentStatusStateType",
     "AgentStatusTypeType",
     "ArtifactStatusType",
     "BehaviorTypeType",
@@ -157,15 +156,14 @@
     "ConnectServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ActionTypeType = Literal[
     "ASSIGN_CONTACT_CATEGORY", "CREATE_TASK", "GENERATE_EVENTBRIDGE_EVENT", "SEND_NOTIFICATION"
 ]
 AgentAvailabilityTimerType = Literal["TIME_SINCE_LAST_ACTIVITY", "TIME_SINCE_LAST_INBOUND"]
 AgentStatusStateType = Literal["DISABLED", "ENABLED"]
 AgentStatusTypeType = Literal["CUSTOM", "OFFLINE", "ROUTABLE"]
 ArtifactStatusType = Literal["APPROVED", "IN_PROGRESS", "REJECTED"]
```

### Comparing `types-aiobotocore-connect-2.9.0/types_aiobotocore_connect/literals.pyi` & `types-aiobotocore-connect-2.9.1/types_aiobotocore_connect/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connect-2.9.0/types_aiobotocore_connect/paginator.py` & `types-aiobotocore-connect-2.9.1/types_aiobotocore_connect/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,15 +218,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "GetMetricDataPaginator",
     "ListAgentStatusesPaginator",
     "ListApprovedOriginsPaginator",
     "ListBotsPaginator",
     "ListContactEvaluationsPaginator",
     "ListContactFlowModulesPaginator",
@@ -272,15 +271,14 @@
     "SearchResourceTagsPaginator",
     "SearchRoutingProfilesPaginator",
     "SearchSecurityProfilesPaginator",
     "SearchUsersPaginator",
     "SearchVocabulariesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -298,15 +296,15 @@
         *,
         InstanceId: str,
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
         Filters: FiltersTypeDef,
         HistoricalMetrics: Sequence[HistoricalMetricTypeDef],
         Groupings: Sequence[GroupingType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetMetricDataResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.GetMetricData.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#getmetricdatapaginator)
         """
 
 
@@ -317,15 +315,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         AgentStatusTypes: Sequence[AgentStatusTypeType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAgentStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListAgentStatuses.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#listagentstatusespaginator)
         """
 
 
@@ -351,15 +349,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         LexVersion: LexVersionType,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListBotsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListBots.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#listbotspaginator)
         """
 
 
@@ -385,15 +383,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         ContactFlowModuleState: ContactFlowModuleStateType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListContactFlowModulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListContactFlowModules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#listcontactflowmodulespaginator)
         """
 
 
@@ -404,15 +402,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         ContactFlowTypes: Sequence[ContactFlowTypeType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListContactFlowsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListContactFlows.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#listcontactflowspaginator)
         """
 
 
@@ -424,15 +422,15 @@
 
     def paginate(
         self,
         *,
         InstanceId: str,
         ContactId: str,
         ReferenceTypes: Sequence[ReferenceTypeType],
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListContactReferencesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListContactReferences.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#listcontactreferencespaginator)
         """
 
 
@@ -443,15 +441,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         LanguageCode: VocabularyLanguageCodeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDefaultVocabulariesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListDefaultVocabularies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#listdefaultvocabulariespaginator)
         """
 
 
@@ -462,15 +460,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         EvaluationFormId: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEvaluationFormVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListEvaluationFormVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#listevaluationformversionspaginator)
         """
 
 
@@ -496,15 +494,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         ResourceType: Literal["VOICE_PHONE_NUMBER"] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListFlowAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListFlowAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#listflowassociationspaginator)
         """
 
 
@@ -545,15 +543,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         ResourceType: InstanceStorageResourceTypeType,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListInstanceStorageConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListInstanceStorageConfigs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#listinstancestorageconfigspaginator)
         """
 
 
@@ -580,15 +578,15 @@
 
     def paginate(
         self,
         *,
         InstanceId: str,
         IntegrationType: IntegrationTypeType = ...,
         IntegrationArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListIntegrationAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListIntegrationAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#listintegrationassociationspaginator)
         """
 
 
@@ -630,15 +628,15 @@
 
     def paginate(
         self,
         *,
         InstanceId: str,
         PhoneNumberTypes: Sequence[PhoneNumberTypeType] = ...,
         PhoneNumberCountryCodes: Sequence[PhoneNumberCountryCodeType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPhoneNumbersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListPhoneNumbers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#listphonenumberspaginator)
         """
 
 
@@ -652,15 +650,15 @@
         self,
         *,
         TargetArn: str = ...,
         InstanceId: str = ...,
         PhoneNumberCountryCodes: Sequence[PhoneNumberCountryCodeType] = ...,
         PhoneNumberTypes: Sequence[PhoneNumberTypeType] = ...,
         PhoneNumberPrefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPhoneNumbersV2ResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListPhoneNumbersV2.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#listphonenumbersv2paginator)
         """
 
 
@@ -701,15 +699,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         QueueTypes: Sequence[QueueTypeType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListQueuesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListQueues.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#listqueuespaginator)
         """
 
 
@@ -720,15 +718,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         QuickConnectTypes: Sequence[QuickConnectTypeType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListQuickConnectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListQuickConnects.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#listquickconnectspaginator)
         """
 
 
@@ -739,15 +737,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         RoutingProfileId: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRoutingProfileQueuesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListRoutingProfileQueues.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#listroutingprofilequeuespaginator)
         """
 
 
@@ -774,15 +772,15 @@
 
     def paginate(
         self,
         *,
         InstanceId: str,
         PublishStatus: RulePublishStatusType = ...,
         EventSourceName: EventSourceNameType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#listrulespaginator)
         """
 
 
@@ -808,15 +806,15 @@
     """
 
     def paginate(
         self,
         *,
         SecurityProfileId: str,
         InstanceId: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSecurityProfileApplicationsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListSecurityProfileApplications.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#listsecurityprofileapplicationspaginator)
         """
 
 
@@ -827,15 +825,15 @@
     """
 
     def paginate(
         self,
         *,
         SecurityProfileId: str,
         InstanceId: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSecurityProfilePermissionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListSecurityProfilePermissions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#listsecurityprofilepermissionspaginator)
         """
 
 
@@ -862,15 +860,15 @@
 
     def paginate(
         self,
         *,
         InstanceId: str,
         Status: TaskTemplateStatusType = ...,
         Name: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTaskTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListTaskTemplates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#listtasktemplatespaginator)
         """
 
 
@@ -911,15 +909,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         IntegrationAssociationId: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListUseCasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListUseCases.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#listusecasespaginator)
         """
 
 
@@ -975,15 +973,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         Type: ViewTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListViewsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListViews.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#listviewspaginator)
         """
 
 
@@ -997,15 +995,15 @@
         self,
         *,
         PhoneNumberCountryCode: PhoneNumberCountryCodeType,
         PhoneNumberType: PhoneNumberTypeType,
         TargetArn: str = ...,
         InstanceId: str = ...,
         PhoneNumberPrefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchAvailablePhoneNumbersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchAvailablePhoneNumbers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#searchavailablephonenumberspaginator)
         """
 
 
@@ -1017,15 +1015,15 @@
 
     def paginate(
         self,
         *,
         InstanceId: str,
         SearchFilter: HoursOfOperationSearchFilterTypeDef = ...,
         SearchCriteria: HoursOfOperationSearchCriteriaTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchHoursOfOperationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchHoursOfOperations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#searchhoursofoperationspaginator)
         """
 
 
@@ -1037,15 +1035,15 @@
 
     def paginate(
         self,
         *,
         InstanceId: str,
         SearchFilter: PromptSearchFilterTypeDef = ...,
         SearchCriteria: PromptSearchCriteriaTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchPromptsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchPrompts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#searchpromptspaginator)
         """
 
 
@@ -1057,15 +1055,15 @@
 
     def paginate(
         self,
         *,
         InstanceId: str,
         SearchFilter: QueueSearchFilterTypeDef = ...,
         SearchCriteria: QueueSearchCriteriaTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchQueuesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchQueues.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#searchqueuespaginator)
         """
 
 
@@ -1077,15 +1075,15 @@
 
     def paginate(
         self,
         *,
         InstanceId: str,
         SearchFilter: QuickConnectSearchFilterTypeDef = ...,
         SearchCriteria: QuickConnectSearchCriteriaTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchQuickConnectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchQuickConnects.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#searchquickconnectspaginator)
         """
 
 
@@ -1097,15 +1095,15 @@
 
     def paginate(
         self,
         *,
         InstanceId: str,
         ResourceTypes: Sequence[str] = ...,
         SearchCriteria: ResourceTagsSearchCriteriaTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchResourceTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchResourceTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#searchresourcetagspaginator)
         """
 
 
@@ -1117,15 +1115,15 @@
 
     def paginate(
         self,
         *,
         InstanceId: str,
         SearchFilter: RoutingProfileSearchFilterTypeDef = ...,
         SearchCriteria: RoutingProfileSearchCriteriaTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchRoutingProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchRoutingProfiles.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#searchroutingprofilespaginator)
         """
 
 
@@ -1137,15 +1135,15 @@
 
     def paginate(
         self,
         *,
         InstanceId: str,
         SearchCriteria: SecurityProfileSearchCriteriaTypeDef = ...,
         SearchFilter: SecurityProfilesSearchFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchSecurityProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchSecurityProfiles.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#searchsecurityprofilespaginator)
         """
 
 
@@ -1157,15 +1155,15 @@
 
     def paginate(
         self,
         *,
         InstanceId: str,
         SearchFilter: UserSearchFilterTypeDef = ...,
         SearchCriteria: UserSearchCriteriaTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchUsers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#searchuserspaginator)
         """
 
 
@@ -1178,13 +1176,13 @@
     def paginate(
         self,
         *,
         InstanceId: str,
         State: VocabularyStateType = ...,
         NameStartsWith: str = ...,
         LanguageCode: VocabularyLanguageCodeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchVocabulariesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchVocabularies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#searchvocabulariespaginator)
         """
```

### Comparing `types-aiobotocore-connect-2.9.0/types_aiobotocore_connect/paginator.pyi` & `types-aiobotocore-connect-2.9.1/types_aiobotocore_connect/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -294,15 +294,15 @@
         *,
         InstanceId: str,
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
         Filters: FiltersTypeDef,
         HistoricalMetrics: Sequence[HistoricalMetricTypeDef],
         Groupings: Sequence[GroupingType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetMetricDataResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.GetMetricData.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#getmetricdatapaginator)
         """
 
 class ListAgentStatusesPaginator(AioPaginator):
@@ -312,15 +312,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         AgentStatusTypes: Sequence[AgentStatusTypeType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAgentStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListAgentStatuses.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#listagentstatusespaginator)
         """
 
 class ListApprovedOriginsPaginator(AioPaginator):
@@ -344,15 +344,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         LexVersion: LexVersionType,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListBotsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListBots.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#listbotspaginator)
         """
 
 class ListContactEvaluationsPaginator(AioPaginator):
@@ -376,15 +376,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         ContactFlowModuleState: ContactFlowModuleStateType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListContactFlowModulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListContactFlowModules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#listcontactflowmodulespaginator)
         """
 
 class ListContactFlowsPaginator(AioPaginator):
@@ -394,15 +394,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         ContactFlowTypes: Sequence[ContactFlowTypeType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListContactFlowsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListContactFlows.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#listcontactflowspaginator)
         """
 
 class ListContactReferencesPaginator(AioPaginator):
@@ -413,15 +413,15 @@
 
     def paginate(
         self,
         *,
         InstanceId: str,
         ContactId: str,
         ReferenceTypes: Sequence[ReferenceTypeType],
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListContactReferencesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListContactReferences.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#listcontactreferencespaginator)
         """
 
 class ListDefaultVocabulariesPaginator(AioPaginator):
@@ -431,15 +431,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         LanguageCode: VocabularyLanguageCodeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDefaultVocabulariesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListDefaultVocabularies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#listdefaultvocabulariespaginator)
         """
 
 class ListEvaluationFormVersionsPaginator(AioPaginator):
@@ -449,15 +449,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         EvaluationFormId: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEvaluationFormVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListEvaluationFormVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#listevaluationformversionspaginator)
         """
 
 class ListEvaluationFormsPaginator(AioPaginator):
@@ -481,15 +481,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         ResourceType: Literal["VOICE_PHONE_NUMBER"] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListFlowAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListFlowAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#listflowassociationspaginator)
         """
 
 class ListHoursOfOperationsPaginator(AioPaginator):
@@ -527,15 +527,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         ResourceType: InstanceStorageResourceTypeType,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListInstanceStorageConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListInstanceStorageConfigs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#listinstancestorageconfigspaginator)
         """
 
 class ListInstancesPaginator(AioPaginator):
@@ -560,15 +560,15 @@
 
     def paginate(
         self,
         *,
         InstanceId: str,
         IntegrationType: IntegrationTypeType = ...,
         IntegrationArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListIntegrationAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListIntegrationAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#listintegrationassociationspaginator)
         """
 
 class ListLambdaFunctionsPaginator(AioPaginator):
@@ -607,15 +607,15 @@
 
     def paginate(
         self,
         *,
         InstanceId: str,
         PhoneNumberTypes: Sequence[PhoneNumberTypeType] = ...,
         PhoneNumberCountryCodes: Sequence[PhoneNumberCountryCodeType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPhoneNumbersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListPhoneNumbers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#listphonenumberspaginator)
         """
 
 class ListPhoneNumbersV2Paginator(AioPaginator):
@@ -628,15 +628,15 @@
         self,
         *,
         TargetArn: str = ...,
         InstanceId: str = ...,
         PhoneNumberCountryCodes: Sequence[PhoneNumberCountryCodeType] = ...,
         PhoneNumberTypes: Sequence[PhoneNumberTypeType] = ...,
         PhoneNumberPrefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPhoneNumbersV2ResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListPhoneNumbersV2.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#listphonenumbersv2paginator)
         """
 
 class ListPromptsPaginator(AioPaginator):
@@ -674,15 +674,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         QueueTypes: Sequence[QueueTypeType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListQueuesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListQueues.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#listqueuespaginator)
         """
 
 class ListQuickConnectsPaginator(AioPaginator):
@@ -692,15 +692,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         QuickConnectTypes: Sequence[QuickConnectTypeType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListQuickConnectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListQuickConnects.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#listquickconnectspaginator)
         """
 
 class ListRoutingProfileQueuesPaginator(AioPaginator):
@@ -710,15 +710,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         RoutingProfileId: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRoutingProfileQueuesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListRoutingProfileQueues.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#listroutingprofilequeuespaginator)
         """
 
 class ListRoutingProfilesPaginator(AioPaginator):
@@ -743,15 +743,15 @@
 
     def paginate(
         self,
         *,
         InstanceId: str,
         PublishStatus: RulePublishStatusType = ...,
         EventSourceName: EventSourceNameType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#listrulespaginator)
         """
 
 class ListSecurityKeysPaginator(AioPaginator):
@@ -775,15 +775,15 @@
     """
 
     def paginate(
         self,
         *,
         SecurityProfileId: str,
         InstanceId: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSecurityProfileApplicationsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListSecurityProfileApplications.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#listsecurityprofileapplicationspaginator)
         """
 
 class ListSecurityProfilePermissionsPaginator(AioPaginator):
@@ -793,15 +793,15 @@
     """
 
     def paginate(
         self,
         *,
         SecurityProfileId: str,
         InstanceId: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSecurityProfilePermissionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListSecurityProfilePermissions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#listsecurityprofilepermissionspaginator)
         """
 
 class ListSecurityProfilesPaginator(AioPaginator):
@@ -826,15 +826,15 @@
 
     def paginate(
         self,
         *,
         InstanceId: str,
         Status: TaskTemplateStatusType = ...,
         Name: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTaskTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListTaskTemplates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#listtasktemplatespaginator)
         """
 
 class ListTrafficDistributionGroupUsersPaginator(AioPaginator):
@@ -872,15 +872,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         IntegrationAssociationId: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListUseCasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListUseCases.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#listusecasespaginator)
         """
 
 class ListUserHierarchyGroupsPaginator(AioPaginator):
@@ -932,15 +932,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         Type: ViewTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListViewsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListViews.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#listviewspaginator)
         """
 
 class SearchAvailablePhoneNumbersPaginator(AioPaginator):
@@ -953,15 +953,15 @@
         self,
         *,
         PhoneNumberCountryCode: PhoneNumberCountryCodeType,
         PhoneNumberType: PhoneNumberTypeType,
         TargetArn: str = ...,
         InstanceId: str = ...,
         PhoneNumberPrefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchAvailablePhoneNumbersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchAvailablePhoneNumbers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#searchavailablephonenumberspaginator)
         """
 
 class SearchHoursOfOperationsPaginator(AioPaginator):
@@ -972,15 +972,15 @@
 
     def paginate(
         self,
         *,
         InstanceId: str,
         SearchFilter: HoursOfOperationSearchFilterTypeDef = ...,
         SearchCriteria: HoursOfOperationSearchCriteriaTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchHoursOfOperationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchHoursOfOperations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#searchhoursofoperationspaginator)
         """
 
 class SearchPromptsPaginator(AioPaginator):
@@ -991,15 +991,15 @@
 
     def paginate(
         self,
         *,
         InstanceId: str,
         SearchFilter: PromptSearchFilterTypeDef = ...,
         SearchCriteria: PromptSearchCriteriaTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchPromptsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchPrompts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#searchpromptspaginator)
         """
 
 class SearchQueuesPaginator(AioPaginator):
@@ -1010,15 +1010,15 @@
 
     def paginate(
         self,
         *,
         InstanceId: str,
         SearchFilter: QueueSearchFilterTypeDef = ...,
         SearchCriteria: QueueSearchCriteriaTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchQueuesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchQueues.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#searchqueuespaginator)
         """
 
 class SearchQuickConnectsPaginator(AioPaginator):
@@ -1029,15 +1029,15 @@
 
     def paginate(
         self,
         *,
         InstanceId: str,
         SearchFilter: QuickConnectSearchFilterTypeDef = ...,
         SearchCriteria: QuickConnectSearchCriteriaTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchQuickConnectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchQuickConnects.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#searchquickconnectspaginator)
         """
 
 class SearchResourceTagsPaginator(AioPaginator):
@@ -1048,15 +1048,15 @@
 
     def paginate(
         self,
         *,
         InstanceId: str,
         ResourceTypes: Sequence[str] = ...,
         SearchCriteria: ResourceTagsSearchCriteriaTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchResourceTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchResourceTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#searchresourcetagspaginator)
         """
 
 class SearchRoutingProfilesPaginator(AioPaginator):
@@ -1067,15 +1067,15 @@
 
     def paginate(
         self,
         *,
         InstanceId: str,
         SearchFilter: RoutingProfileSearchFilterTypeDef = ...,
         SearchCriteria: RoutingProfileSearchCriteriaTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchRoutingProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchRoutingProfiles.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#searchroutingprofilespaginator)
         """
 
 class SearchSecurityProfilesPaginator(AioPaginator):
@@ -1086,15 +1086,15 @@
 
     def paginate(
         self,
         *,
         InstanceId: str,
         SearchCriteria: SecurityProfileSearchCriteriaTypeDef = ...,
         SearchFilter: SecurityProfilesSearchFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchSecurityProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchSecurityProfiles.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#searchsecurityprofilespaginator)
         """
 
 class SearchUsersPaginator(AioPaginator):
@@ -1105,15 +1105,15 @@
 
     def paginate(
         self,
         *,
         InstanceId: str,
         SearchFilter: UserSearchFilterTypeDef = ...,
         SearchCriteria: UserSearchCriteriaTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchUsers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#searchuserspaginator)
         """
 
 class SearchVocabulariesPaginator(AioPaginator):
@@ -1125,13 +1125,13 @@
     def paginate(
         self,
         *,
         InstanceId: str,
         State: VocabularyStateType = ...,
         NameStartsWith: str = ...,
         LanguageCode: VocabularyLanguageCodeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchVocabulariesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchVocabularies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/paginators/#searchvocabulariespaginator)
         """
```

### Comparing `types-aiobotocore-connect-2.9.0/types_aiobotocore_connect/type_defs.py` & `types-aiobotocore-connect-2.9.1/types_aiobotocore_connect/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ActionSummaryTypeDef",
     "ActivateEvaluationFormRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "DistributionTypeDef",
     "QueueReferenceTypeDef",
     "AgentInfoTypeDef",
```

### Comparing `types-aiobotocore-connect-2.9.0/types_aiobotocore_connect/type_defs.pyi` & `types-aiobotocore-connect-2.9.1/types_aiobotocore_connect/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connect-2.9.0/types_aiobotocore_connect.egg-info/PKG-INFO` & `types-aiobotocore-connect-2.9.1/types_aiobotocore_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-connect
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Connect 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Connect 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/
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
 
 <a id="types-aiobotocore-connect"></a>
 
 # types-aiobotocore-connect
 
 [![PyPI - types-aiobotocore-connect](https://img.shields.io/pypi/v/types-aiobotocore-connect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-connect)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-connect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-connect)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-connect)](https://pepy.tech/project/types-aiobotocore-connect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Connect 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
+[aiobotocore.Connect 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
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
 [types-aiobotocore-connect docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-connect-2.9.0/types_aiobotocore_connect.egg-info/SOURCES.txt` & `types-aiobotocore-connect-2.9.1/types_aiobotocore_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

