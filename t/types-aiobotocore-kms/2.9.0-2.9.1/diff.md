# Comparing `tmp/types-aiobotocore-kms-2.9.0.tar.gz` & `tmp/types-aiobotocore-kms-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-kms-2.9.0.tar", last modified: Wed Dec 13 19:59:42 2023, max compression
+gzip compressed data, was "types-aiobotocore-kms-2.9.1.tar", last modified: Thu Jan 18 01:21:04 2024, max compression
```

## Comparing `types-aiobotocore-kms-2.9.0.tar` & `types-aiobotocore-kms-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:42.205554 types-aiobotocore-kms-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:48:40.000000 types-aiobotocore-kms-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13547 2023-12-13 19:59:42.205554 types-aiobotocore-kms-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12000 2023-12-13 19:48:40.000000 types-aiobotocore-kms-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:42.205554 types-aiobotocore-kms-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2023-12-13 19:48:40.000000 types-aiobotocore-kms-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:42.201554 types-aiobotocore-kms-2.9.0/types_aiobotocore_kms/
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2023-12-13 19:48:40.000000 types-aiobotocore-kms-2.9.0/types_aiobotocore_kms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2023-12-13 19:48:40.000000 types-aiobotocore-kms-2.9.0/types_aiobotocore_kms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      905 2023-12-13 19:48:40.000000 types-aiobotocore-kms-2.9.0/types_aiobotocore_kms/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43270 2023-12-13 19:48:42.000000 types-aiobotocore-kms-2.9.0/types_aiobotocore_kms/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    43266 2023-12-13 19:48:41.000000 types-aiobotocore-kms-2.9.0/types_aiobotocore_kms/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13534 2023-12-13 19:48:43.000000 types-aiobotocore-kms-2.9.0/types_aiobotocore_kms/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    13532 2023-12-13 19:48:43.000000 types-aiobotocore-kms-2.9.0/types_aiobotocore_kms/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8446 2023-12-13 19:48:42.000000 types-aiobotocore-kms-2.9.0/types_aiobotocore_kms/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8437 2023-12-13 19:48:42.000000 types-aiobotocore-kms-2.9.0/types_aiobotocore_kms/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:48:40.000000 types-aiobotocore-kms-2.9.0/types_aiobotocore_kms/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    34371 2023-12-13 19:48:43.000000 types-aiobotocore-kms-2.9.0/types_aiobotocore_kms/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    34370 2023-12-13 19:48:43.000000 types-aiobotocore-kms-2.9.0/types_aiobotocore_kms/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:48:40.000000 types-aiobotocore-kms-2.9.0/types_aiobotocore_kms/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:42.205554 types-aiobotocore-kms-2.9.0/types_aiobotocore_kms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13547 2023-12-13 19:59:42.000000 types-aiobotocore-kms-2.9.0/types_aiobotocore_kms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      737 2023-12-13 19:59:42.000000 types-aiobotocore-kms-2.9.0/types_aiobotocore_kms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:42.000000 types-aiobotocore-kms-2.9.0/types_aiobotocore_kms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:42.000000 types-aiobotocore-kms-2.9.0/types_aiobotocore_kms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:42.000000 types-aiobotocore-kms-2.9.0/types_aiobotocore_kms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-13 19:59:42.000000 types-aiobotocore-kms-2.9.0/types_aiobotocore_kms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:04.901232 types-aiobotocore-kms-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:10:29.000000 types-aiobotocore-kms-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13567 2024-01-18 01:21:04.901232 types-aiobotocore-kms-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12000 2024-01-18 01:10:29.000000 types-aiobotocore-kms-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:04.901232 types-aiobotocore-kms-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-01-18 01:10:29.000000 types-aiobotocore-kms-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:04.901232 types-aiobotocore-kms-2.9.1/types_aiobotocore_kms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-01-18 01:10:29.000000 types-aiobotocore-kms-2.9.1/types_aiobotocore_kms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-01-18 01:10:29.000000 types-aiobotocore-kms-2.9.1/types_aiobotocore_kms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-01-18 01:10:29.000000 types-aiobotocore-kms-2.9.1/types_aiobotocore_kms/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43291 2024-01-18 01:10:29.000000 types-aiobotocore-kms-2.9.1/types_aiobotocore_kms/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43288 2024-01-18 01:10:29.000000 types-aiobotocore-kms-2.9.1/types_aiobotocore_kms/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13532 2024-01-18 01:10:29.000000 types-aiobotocore-kms-2.9.1/types_aiobotocore_kms/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13532 2024-01-18 01:10:29.000000 types-aiobotocore-kms-2.9.1/types_aiobotocore_kms/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8447 2024-01-18 01:10:29.000000 types-aiobotocore-kms-2.9.1/types_aiobotocore_kms/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8439 2024-01-18 01:10:29.000000 types-aiobotocore-kms-2.9.1/types_aiobotocore_kms/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:10:29.000000 types-aiobotocore-kms-2.9.1/types_aiobotocore_kms/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    34370 2024-01-18 01:10:30.000000 types-aiobotocore-kms-2.9.1/types_aiobotocore_kms/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34370 2024-01-18 01:10:30.000000 types-aiobotocore-kms-2.9.1/types_aiobotocore_kms/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:10:29.000000 types-aiobotocore-kms-2.9.1/types_aiobotocore_kms/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:04.901232 types-aiobotocore-kms-2.9.1/types_aiobotocore_kms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13567 2024-01-18 01:21:04.000000 types-aiobotocore-kms-2.9.1/types_aiobotocore_kms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-01-18 01:21:04.000000 types-aiobotocore-kms-2.9.1/types_aiobotocore_kms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:04.000000 types-aiobotocore-kms-2.9.1/types_aiobotocore_kms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:04.000000 types-aiobotocore-kms-2.9.1/types_aiobotocore_kms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:04.000000 types-aiobotocore-kms-2.9.1/types_aiobotocore_kms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-18 01:21:04.000000 types-aiobotocore-kms-2.9.1/types_aiobotocore_kms.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-kms-2.9.0/LICENSE` & `types-aiobotocore-kms-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-kms-2.9.0/PKG-INFO` & `types-aiobotocore-kms-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kms
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.KMS 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.KMS 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/
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
 
 <a id="types-aiobotocore-kms"></a>
 
 # types-aiobotocore-kms
 
 [![PyPI - types-aiobotocore-kms](https://img.shields.io/pypi/v/types-aiobotocore-kms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kms)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kms)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kms)](https://pepy.tech/project/types-aiobotocore-kms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.KMS 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
+[aiobotocore.KMS 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
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
 [types-aiobotocore-kms docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-kms-2.9.0/README.md` & `types-aiobotocore-kms-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kms)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kms)](https://pepy.tech/project/types-aiobotocore-kms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.KMS 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
+[aiobotocore.KMS 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
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
 [types-aiobotocore-kms docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-kms-2.9.0/setup.py` & `types-aiobotocore-kms-2.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-kms",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_kms"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.KMS 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.KMS 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore kms type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_kms": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-kms-2.9.0/types_aiobotocore_kms/__init__.py` & `types-aiobotocore-kms-2.9.1/types_aiobotocore_kms/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,14 @@
     ListKeysPaginator,
     ListResourceTagsPaginator,
     ListRetirableGrantsPaginator,
 )
 
 Client = KMSClient
 
-
 __all__ = (
     "Client",
     "DescribeCustomKeyStoresPaginator",
     "KMSClient",
     "ListAliasesPaginator",
     "ListGrantsPaginator",
     "ListKeyPoliciesPaginator",
```

### Comparing `types-aiobotocore-kms-2.9.0/types_aiobotocore_kms/__init__.pyi` & `types-aiobotocore-kms-2.9.1/types_aiobotocore_kms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kms-2.9.0/types_aiobotocore_kms/__main__.py` & `types-aiobotocore-kms-2.9.1/types_aiobotocore_kms/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.KMS 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.KMS 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS\nOther"
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

### Comparing `types-aiobotocore-kms-2.9.0/types_aiobotocore_kms/client.py` & `types-aiobotocore-kms-2.9.1/types_aiobotocore_kms/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -88,26 +88,23 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("KMSClient",)
 
-
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AlreadyExistsException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     CloudHsmClusterInUseException: Type[BotocoreClientError]
     CloudHsmClusterInvalidConfigurationException: Type[BotocoreClientError]
     CloudHsmClusterNotActiveException: Type[BotocoreClientError]
     CloudHsmClusterNotFoundException: Type[BotocoreClientError]
@@ -150,15 +147,14 @@
     XksProxyUriEndpointInUseException: Type[BotocoreClientError]
     XksProxyUriInUseException: Type[BotocoreClientError]
     XksProxyUriUnreachableException: Type[BotocoreClientError]
     XksProxyVpcEndpointServiceInUseException: Type[BotocoreClientError]
     XksProxyVpcEndpointServiceInvalidConfigurationException: Type[BotocoreClientError]
     XksProxyVpcEndpointServiceNotFoundException: Type[BotocoreClientError]
 
-
 class KMSClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/)
     """
 
     meta: ClientMeta
@@ -225,15 +221,15 @@
         TrustAnchorCertificate: str = ...,
         KeyStorePassword: str = ...,
         CustomKeyStoreType: CustomKeyStoreTypeType = ...,
         XksProxyUriEndpoint: str = ...,
         XksProxyUriPath: str = ...,
         XksProxyVpcEndpointServiceName: str = ...,
         XksProxyAuthenticationCredential: XksProxyAuthenticationCredentialTypeTypeDef = ...,
-        XksProxyConnectivity: XksProxyConnectivityTypeType = ...
+        XksProxyConnectivity: XksProxyConnectivityTypeType = ...,
     ) -> CreateCustomKeyStoreResponseTypeDef:
         """
         Creates a [custom key
         store](https://docs.aws.amazon.com/kms/latest/developerguide/custom-key-store-overview.html)
         backed by a key store that you own and
         manage.
 
@@ -247,15 +243,15 @@
         KeyId: str,
         GranteePrincipal: str,
         Operations: Sequence[GrantOperationType],
         RetiringPrincipal: str = ...,
         Constraints: GrantConstraintsTypeDef = ...,
         GrantTokens: Sequence[str] = ...,
         Name: str = ...,
-        DryRun: bool = ...
+        DryRun: bool = ...,
     ) -> CreateGrantResponseTypeDef:
         """
         Adds a grant to a KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.create_grant)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#create_grant)
         """
@@ -269,15 +265,15 @@
         CustomerMasterKeySpec: CustomerMasterKeySpecType = ...,
         KeySpec: KeySpecType = ...,
         Origin: OriginTypeType = ...,
         CustomKeyStoreId: str = ...,
         BypassPolicyLockoutSafetyCheck: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
         MultiRegion: bool = ...,
-        XksKeyId: str = ...
+        XksKeyId: str = ...,
     ) -> CreateKeyResponseTypeDef:
         """
         Creates a unique customer managed [KMS
         key](https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#kms-keys)
         in your Amazon Web Services account and
         Region.
 
@@ -290,15 +286,15 @@
         *,
         CiphertextBlob: BlobTypeDef,
         EncryptionContext: Mapping[str, str] = ...,
         GrantTokens: Sequence[str] = ...,
         KeyId: str = ...,
         EncryptionAlgorithm: EncryptionAlgorithmSpecType = ...,
         Recipient: RecipientInfoTypeDef = ...,
-        DryRun: bool = ...
+        DryRun: bool = ...,
     ) -> DecryptResponseTypeDef:
         """
         Decrypts ciphertext that was encrypted by a KMS key using any of the following
         operations: *  Encrypt *  GenerateDataKey *  GenerateDataKeyPair *
         GenerateDataKeyWithoutPlaintext *  GenerateDataKeyPairWithoutPlaintext You can
         use this operation to decrypt ciphertext that was
         enc...
@@ -334,15 +330,15 @@
 
     async def describe_custom_key_stores(
         self,
         *,
         CustomKeyStoreId: str = ...,
         CustomKeyStoreName: str = ...,
         Limit: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DescribeCustomKeyStoresResponseTypeDef:
         """
         Gets information about [custom key
         stores](https://docs.aws.amazon.com/kms/latest/developerguide/custom-key-store-overview.html)
         in the account and
         Region.
 
@@ -413,15 +409,15 @@
         self,
         *,
         KeyId: str,
         Plaintext: BlobTypeDef,
         EncryptionContext: Mapping[str, str] = ...,
         GrantTokens: Sequence[str] = ...,
         EncryptionAlgorithm: EncryptionAlgorithmSpecType = ...,
-        DryRun: bool = ...
+        DryRun: bool = ...,
     ) -> EncryptResponseTypeDef:
         """
         Encrypts plaintext of up to 4,096 bytes using a KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.encrypt)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#encrypt)
         """
@@ -431,15 +427,15 @@
         *,
         KeyId: str,
         EncryptionContext: Mapping[str, str] = ...,
         NumberOfBytes: int = ...,
         KeySpec: DataKeySpecType = ...,
         GrantTokens: Sequence[str] = ...,
         Recipient: RecipientInfoTypeDef = ...,
-        DryRun: bool = ...
+        DryRun: bool = ...,
     ) -> GenerateDataKeyResponseTypeDef:
         """
         Returns a unique symmetric data key for use outside of KMS.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.generate_data_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#generate_data_key)
         """
@@ -448,15 +444,15 @@
         self,
         *,
         KeyId: str,
         KeyPairSpec: DataKeyPairSpecType,
         EncryptionContext: Mapping[str, str] = ...,
         GrantTokens: Sequence[str] = ...,
         Recipient: RecipientInfoTypeDef = ...,
-        DryRun: bool = ...
+        DryRun: bool = ...,
     ) -> GenerateDataKeyPairResponseTypeDef:
         """
         Returns a unique asymmetric data key pair for use outside of KMS.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.generate_data_key_pair)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#generate_data_key_pair)
         """
@@ -464,15 +460,15 @@
     async def generate_data_key_pair_without_plaintext(
         self,
         *,
         KeyId: str,
         KeyPairSpec: DataKeyPairSpecType,
         EncryptionContext: Mapping[str, str] = ...,
         GrantTokens: Sequence[str] = ...,
-        DryRun: bool = ...
+        DryRun: bool = ...,
     ) -> GenerateDataKeyPairWithoutPlaintextResponseTypeDef:
         """
         Returns a unique asymmetric data key pair for use outside of KMS.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.generate_data_key_pair_without_plaintext)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#generate_data_key_pair_without_plaintext)
         """
@@ -481,15 +477,15 @@
         self,
         *,
         KeyId: str,
         EncryptionContext: Mapping[str, str] = ...,
         KeySpec: DataKeySpecType = ...,
         NumberOfBytes: int = ...,
         GrantTokens: Sequence[str] = ...,
-        DryRun: bool = ...
+        DryRun: bool = ...,
     ) -> GenerateDataKeyWithoutPlaintextResponseTypeDef:
         """
         Returns a unique symmetric data key for use outside of KMS.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.generate_data_key_without_plaintext)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#generate_data_key_without_plaintext)
         """
@@ -497,15 +493,15 @@
     async def generate_mac(
         self,
         *,
         Message: BlobTypeDef,
         KeyId: str,
         MacAlgorithm: MacAlgorithmSpecType,
         GrantTokens: Sequence[str] = ...,
-        DryRun: bool = ...
+        DryRun: bool = ...,
     ) -> GenerateMacResponseTypeDef:
         """
         Generates a hash-based message authentication code (HMAC) for a message using
         an HMAC KMS key and a MAC algorithm that the key
         supports.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.generate_mac)
@@ -527,15 +523,15 @@
         """
 
     async def generate_random(
         self,
         *,
         NumberOfBytes: int = ...,
         CustomKeyStoreId: str = ...,
-        Recipient: RecipientInfoTypeDef = ...
+        Recipient: RecipientInfoTypeDef = ...,
     ) -> GenerateRandomResponseTypeDef:
         """
         Returns a random byte string that is cryptographically secure.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.generate_random)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#generate_random)
         """
@@ -560,15 +556,15 @@
         """
 
     async def get_parameters_for_import(
         self,
         *,
         KeyId: str,
         WrappingAlgorithm: AlgorithmSpecType,
-        WrappingKeySpec: WrappingKeySpecType
+        WrappingKeySpec: WrappingKeySpecType,
     ) -> GetParametersForImportResponseTypeDef:
         """
         Returns the public key and an import token you need to import or reimport key
         material for a KMS
         key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_parameters_for_import)
@@ -588,15 +584,15 @@
     async def import_key_material(
         self,
         *,
         KeyId: str,
         ImportToken: BlobTypeDef,
         EncryptedKeyMaterial: BlobTypeDef,
         ValidTo: TimestampTypeDef = ...,
-        ExpirationModel: ExpirationModelTypeType = ...
+        ExpirationModel: ExpirationModelTypeType = ...,
     ) -> Dict[str, Any]:
         """
         Imports or reimports key material into an existing KMS key that was created
         without key
         material.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.import_key_material)
@@ -616,15 +612,15 @@
     async def list_grants(
         self,
         *,
         KeyId: str,
         Limit: int = ...,
         Marker: str = ...,
         GrantId: str = ...,
-        GranteePrincipal: str = ...
+        GranteePrincipal: str = ...,
     ) -> ListGrantsResponseTypeDef:
         """
         Gets a list of all grants for the specified KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.list_grants)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#list_grants)
         """
@@ -672,15 +668,15 @@
 
     async def put_key_policy(
         self,
         *,
         KeyId: str,
         PolicyName: str,
         Policy: str,
-        BypassPolicyLockoutSafetyCheck: bool = ...
+        BypassPolicyLockoutSafetyCheck: bool = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Attaches a key policy to the specified KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.put_key_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#put_key_policy)
         """
@@ -692,15 +688,15 @@
         DestinationKeyId: str,
         SourceEncryptionContext: Mapping[str, str] = ...,
         SourceKeyId: str = ...,
         DestinationEncryptionContext: Mapping[str, str] = ...,
         SourceEncryptionAlgorithm: EncryptionAlgorithmSpecType = ...,
         DestinationEncryptionAlgorithm: EncryptionAlgorithmSpecType = ...,
         GrantTokens: Sequence[str] = ...,
-        DryRun: bool = ...
+        DryRun: bool = ...,
     ) -> ReEncryptResponseTypeDef:
         """
         Decrypts ciphertext and then reencrypts it entirely within KMS.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.re_encrypt)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#re_encrypt)
         """
@@ -709,15 +705,15 @@
         self,
         *,
         KeyId: str,
         ReplicaRegion: str,
         Policy: str = ...,
         BypassPolicyLockoutSafetyCheck: bool = ...,
         Description: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> ReplicateKeyResponseTypeDef:
         """
         Replicates a multi-Region key into the specified Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.replicate_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#replicate_key)
         """
@@ -756,15 +752,15 @@
         self,
         *,
         KeyId: str,
         Message: BlobTypeDef,
         SigningAlgorithm: SigningAlgorithmSpecType,
         MessageType: MessageTypeType = ...,
         GrantTokens: Sequence[str] = ...,
-        DryRun: bool = ...
+        DryRun: bool = ...,
     ) -> SignResponseTypeDef:
         """
         Creates a [digital signature](https://en.wikipedia.org/wiki/Digital_signature)
         for a message or message digest by using the private key in an asymmetric
         signing KMS
         key.
 
@@ -811,15 +807,15 @@
         NewCustomKeyStoreName: str = ...,
         KeyStorePassword: str = ...,
         CloudHsmClusterId: str = ...,
         XksProxyUriEndpoint: str = ...,
         XksProxyUriPath: str = ...,
         XksProxyVpcEndpointServiceName: str = ...,
         XksProxyAuthenticationCredential: XksProxyAuthenticationCredentialTypeTypeDef = ...,
-        XksProxyConnectivity: XksProxyConnectivityTypeType = ...
+        XksProxyConnectivity: XksProxyConnectivityTypeType = ...,
     ) -> Dict[str, Any]:
         """
         Changes the properties of a custom key store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.update_custom_key_store)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#update_custom_key_store)
         """
@@ -849,15 +845,15 @@
         *,
         KeyId: str,
         Message: BlobTypeDef,
         Signature: BlobTypeDef,
         SigningAlgorithm: SigningAlgorithmSpecType,
         MessageType: MessageTypeType = ...,
         GrantTokens: Sequence[str] = ...,
-        DryRun: bool = ...
+        DryRun: bool = ...,
     ) -> VerifyResponseTypeDef:
         """
         Verifies a digital signature that was generated by the  Sign operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.verify)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#verify)
         """
@@ -866,15 +862,15 @@
         self,
         *,
         Message: BlobTypeDef,
         KeyId: str,
         MacAlgorithm: MacAlgorithmSpecType,
         Mac: BlobTypeDef,
         GrantTokens: Sequence[str] = ...,
-        DryRun: bool = ...
+        DryRun: bool = ...,
     ) -> VerifyMacResponseTypeDef:
         """
         Verifies the hash-based message authentication code (HMAC) for a specified
         message, HMAC KMS key, and MAC
         algorithm.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.verify_mac)
```

### Comparing `types-aiobotocore-kms-2.9.0/types_aiobotocore_kms/client.pyi` & `types-aiobotocore-kms-2.9.1/types_aiobotocore_kms/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,21 +90,23 @@
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = ("KMSClient",)
 
+
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AlreadyExistsException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     CloudHsmClusterInUseException: Type[BotocoreClientError]
     CloudHsmClusterInvalidConfigurationException: Type[BotocoreClientError]
     CloudHsmClusterNotActiveException: Type[BotocoreClientError]
     CloudHsmClusterNotFoundException: Type[BotocoreClientError]
@@ -147,14 +149,15 @@
     XksProxyUriEndpointInUseException: Type[BotocoreClientError]
     XksProxyUriInUseException: Type[BotocoreClientError]
     XksProxyUriUnreachableException: Type[BotocoreClientError]
     XksProxyVpcEndpointServiceInUseException: Type[BotocoreClientError]
     XksProxyVpcEndpointServiceInvalidConfigurationException: Type[BotocoreClientError]
     XksProxyVpcEndpointServiceNotFoundException: Type[BotocoreClientError]
 
+
 class KMSClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/)
     """
 
     meta: ClientMeta
@@ -221,15 +224,15 @@
         TrustAnchorCertificate: str = ...,
         KeyStorePassword: str = ...,
         CustomKeyStoreType: CustomKeyStoreTypeType = ...,
         XksProxyUriEndpoint: str = ...,
         XksProxyUriPath: str = ...,
         XksProxyVpcEndpointServiceName: str = ...,
         XksProxyAuthenticationCredential: XksProxyAuthenticationCredentialTypeTypeDef = ...,
-        XksProxyConnectivity: XksProxyConnectivityTypeType = ...
+        XksProxyConnectivity: XksProxyConnectivityTypeType = ...,
     ) -> CreateCustomKeyStoreResponseTypeDef:
         """
         Creates a [custom key
         store](https://docs.aws.amazon.com/kms/latest/developerguide/custom-key-store-overview.html)
         backed by a key store that you own and
         manage.
 
@@ -243,15 +246,15 @@
         KeyId: str,
         GranteePrincipal: str,
         Operations: Sequence[GrantOperationType],
         RetiringPrincipal: str = ...,
         Constraints: GrantConstraintsTypeDef = ...,
         GrantTokens: Sequence[str] = ...,
         Name: str = ...,
-        DryRun: bool = ...
+        DryRun: bool = ...,
     ) -> CreateGrantResponseTypeDef:
         """
         Adds a grant to a KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.create_grant)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#create_grant)
         """
@@ -265,15 +268,15 @@
         CustomerMasterKeySpec: CustomerMasterKeySpecType = ...,
         KeySpec: KeySpecType = ...,
         Origin: OriginTypeType = ...,
         CustomKeyStoreId: str = ...,
         BypassPolicyLockoutSafetyCheck: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
         MultiRegion: bool = ...,
-        XksKeyId: str = ...
+        XksKeyId: str = ...,
     ) -> CreateKeyResponseTypeDef:
         """
         Creates a unique customer managed [KMS
         key](https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#kms-keys)
         in your Amazon Web Services account and
         Region.
 
@@ -286,15 +289,15 @@
         *,
         CiphertextBlob: BlobTypeDef,
         EncryptionContext: Mapping[str, str] = ...,
         GrantTokens: Sequence[str] = ...,
         KeyId: str = ...,
         EncryptionAlgorithm: EncryptionAlgorithmSpecType = ...,
         Recipient: RecipientInfoTypeDef = ...,
-        DryRun: bool = ...
+        DryRun: bool = ...,
     ) -> DecryptResponseTypeDef:
         """
         Decrypts ciphertext that was encrypted by a KMS key using any of the following
         operations: *  Encrypt *  GenerateDataKey *  GenerateDataKeyPair *
         GenerateDataKeyWithoutPlaintext *  GenerateDataKeyPairWithoutPlaintext You can
         use this operation to decrypt ciphertext that was
         enc...
@@ -330,15 +333,15 @@
 
     async def describe_custom_key_stores(
         self,
         *,
         CustomKeyStoreId: str = ...,
         CustomKeyStoreName: str = ...,
         Limit: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DescribeCustomKeyStoresResponseTypeDef:
         """
         Gets information about [custom key
         stores](https://docs.aws.amazon.com/kms/latest/developerguide/custom-key-store-overview.html)
         in the account and
         Region.
 
@@ -409,15 +412,15 @@
         self,
         *,
         KeyId: str,
         Plaintext: BlobTypeDef,
         EncryptionContext: Mapping[str, str] = ...,
         GrantTokens: Sequence[str] = ...,
         EncryptionAlgorithm: EncryptionAlgorithmSpecType = ...,
-        DryRun: bool = ...
+        DryRun: bool = ...,
     ) -> EncryptResponseTypeDef:
         """
         Encrypts plaintext of up to 4,096 bytes using a KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.encrypt)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#encrypt)
         """
@@ -427,15 +430,15 @@
         *,
         KeyId: str,
         EncryptionContext: Mapping[str, str] = ...,
         NumberOfBytes: int = ...,
         KeySpec: DataKeySpecType = ...,
         GrantTokens: Sequence[str] = ...,
         Recipient: RecipientInfoTypeDef = ...,
-        DryRun: bool = ...
+        DryRun: bool = ...,
     ) -> GenerateDataKeyResponseTypeDef:
         """
         Returns a unique symmetric data key for use outside of KMS.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.generate_data_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#generate_data_key)
         """
@@ -444,15 +447,15 @@
         self,
         *,
         KeyId: str,
         KeyPairSpec: DataKeyPairSpecType,
         EncryptionContext: Mapping[str, str] = ...,
         GrantTokens: Sequence[str] = ...,
         Recipient: RecipientInfoTypeDef = ...,
-        DryRun: bool = ...
+        DryRun: bool = ...,
     ) -> GenerateDataKeyPairResponseTypeDef:
         """
         Returns a unique asymmetric data key pair for use outside of KMS.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.generate_data_key_pair)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#generate_data_key_pair)
         """
@@ -460,15 +463,15 @@
     async def generate_data_key_pair_without_plaintext(
         self,
         *,
         KeyId: str,
         KeyPairSpec: DataKeyPairSpecType,
         EncryptionContext: Mapping[str, str] = ...,
         GrantTokens: Sequence[str] = ...,
-        DryRun: bool = ...
+        DryRun: bool = ...,
     ) -> GenerateDataKeyPairWithoutPlaintextResponseTypeDef:
         """
         Returns a unique asymmetric data key pair for use outside of KMS.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.generate_data_key_pair_without_plaintext)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#generate_data_key_pair_without_plaintext)
         """
@@ -477,15 +480,15 @@
         self,
         *,
         KeyId: str,
         EncryptionContext: Mapping[str, str] = ...,
         KeySpec: DataKeySpecType = ...,
         NumberOfBytes: int = ...,
         GrantTokens: Sequence[str] = ...,
-        DryRun: bool = ...
+        DryRun: bool = ...,
     ) -> GenerateDataKeyWithoutPlaintextResponseTypeDef:
         """
         Returns a unique symmetric data key for use outside of KMS.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.generate_data_key_without_plaintext)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#generate_data_key_without_plaintext)
         """
@@ -493,15 +496,15 @@
     async def generate_mac(
         self,
         *,
         Message: BlobTypeDef,
         KeyId: str,
         MacAlgorithm: MacAlgorithmSpecType,
         GrantTokens: Sequence[str] = ...,
-        DryRun: bool = ...
+        DryRun: bool = ...,
     ) -> GenerateMacResponseTypeDef:
         """
         Generates a hash-based message authentication code (HMAC) for a message using
         an HMAC KMS key and a MAC algorithm that the key
         supports.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.generate_mac)
@@ -523,15 +526,15 @@
         """
 
     async def generate_random(
         self,
         *,
         NumberOfBytes: int = ...,
         CustomKeyStoreId: str = ...,
-        Recipient: RecipientInfoTypeDef = ...
+        Recipient: RecipientInfoTypeDef = ...,
     ) -> GenerateRandomResponseTypeDef:
         """
         Returns a random byte string that is cryptographically secure.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.generate_random)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#generate_random)
         """
@@ -556,15 +559,15 @@
         """
 
     async def get_parameters_for_import(
         self,
         *,
         KeyId: str,
         WrappingAlgorithm: AlgorithmSpecType,
-        WrappingKeySpec: WrappingKeySpecType
+        WrappingKeySpec: WrappingKeySpecType,
     ) -> GetParametersForImportResponseTypeDef:
         """
         Returns the public key and an import token you need to import or reimport key
         material for a KMS
         key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_parameters_for_import)
@@ -584,15 +587,15 @@
     async def import_key_material(
         self,
         *,
         KeyId: str,
         ImportToken: BlobTypeDef,
         EncryptedKeyMaterial: BlobTypeDef,
         ValidTo: TimestampTypeDef = ...,
-        ExpirationModel: ExpirationModelTypeType = ...
+        ExpirationModel: ExpirationModelTypeType = ...,
     ) -> Dict[str, Any]:
         """
         Imports or reimports key material into an existing KMS key that was created
         without key
         material.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.import_key_material)
@@ -612,15 +615,15 @@
     async def list_grants(
         self,
         *,
         KeyId: str,
         Limit: int = ...,
         Marker: str = ...,
         GrantId: str = ...,
-        GranteePrincipal: str = ...
+        GranteePrincipal: str = ...,
     ) -> ListGrantsResponseTypeDef:
         """
         Gets a list of all grants for the specified KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.list_grants)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#list_grants)
         """
@@ -668,15 +671,15 @@
 
     async def put_key_policy(
         self,
         *,
         KeyId: str,
         PolicyName: str,
         Policy: str,
-        BypassPolicyLockoutSafetyCheck: bool = ...
+        BypassPolicyLockoutSafetyCheck: bool = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Attaches a key policy to the specified KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.put_key_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#put_key_policy)
         """
@@ -688,15 +691,15 @@
         DestinationKeyId: str,
         SourceEncryptionContext: Mapping[str, str] = ...,
         SourceKeyId: str = ...,
         DestinationEncryptionContext: Mapping[str, str] = ...,
         SourceEncryptionAlgorithm: EncryptionAlgorithmSpecType = ...,
         DestinationEncryptionAlgorithm: EncryptionAlgorithmSpecType = ...,
         GrantTokens: Sequence[str] = ...,
-        DryRun: bool = ...
+        DryRun: bool = ...,
     ) -> ReEncryptResponseTypeDef:
         """
         Decrypts ciphertext and then reencrypts it entirely within KMS.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.re_encrypt)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#re_encrypt)
         """
@@ -705,15 +708,15 @@
         self,
         *,
         KeyId: str,
         ReplicaRegion: str,
         Policy: str = ...,
         BypassPolicyLockoutSafetyCheck: bool = ...,
         Description: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> ReplicateKeyResponseTypeDef:
         """
         Replicates a multi-Region key into the specified Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.replicate_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#replicate_key)
         """
@@ -752,15 +755,15 @@
         self,
         *,
         KeyId: str,
         Message: BlobTypeDef,
         SigningAlgorithm: SigningAlgorithmSpecType,
         MessageType: MessageTypeType = ...,
         GrantTokens: Sequence[str] = ...,
-        DryRun: bool = ...
+        DryRun: bool = ...,
     ) -> SignResponseTypeDef:
         """
         Creates a [digital signature](https://en.wikipedia.org/wiki/Digital_signature)
         for a message or message digest by using the private key in an asymmetric
         signing KMS
         key.
 
@@ -807,15 +810,15 @@
         NewCustomKeyStoreName: str = ...,
         KeyStorePassword: str = ...,
         CloudHsmClusterId: str = ...,
         XksProxyUriEndpoint: str = ...,
         XksProxyUriPath: str = ...,
         XksProxyVpcEndpointServiceName: str = ...,
         XksProxyAuthenticationCredential: XksProxyAuthenticationCredentialTypeTypeDef = ...,
-        XksProxyConnectivity: XksProxyConnectivityTypeType = ...
+        XksProxyConnectivity: XksProxyConnectivityTypeType = ...,
     ) -> Dict[str, Any]:
         """
         Changes the properties of a custom key store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.update_custom_key_store)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#update_custom_key_store)
         """
@@ -845,15 +848,15 @@
         *,
         KeyId: str,
         Message: BlobTypeDef,
         Signature: BlobTypeDef,
         SigningAlgorithm: SigningAlgorithmSpecType,
         MessageType: MessageTypeType = ...,
         GrantTokens: Sequence[str] = ...,
-        DryRun: bool = ...
+        DryRun: bool = ...,
     ) -> VerifyResponseTypeDef:
         """
         Verifies a digital signature that was generated by the  Sign operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.verify)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#verify)
         """
@@ -862,15 +865,15 @@
         self,
         *,
         Message: BlobTypeDef,
         KeyId: str,
         MacAlgorithm: MacAlgorithmSpecType,
         Mac: BlobTypeDef,
         GrantTokens: Sequence[str] = ...,
-        DryRun: bool = ...
+        DryRun: bool = ...,
     ) -> VerifyMacResponseTypeDef:
         """
         Verifies the hash-based message authentication code (HMAC) for a specified
         message, HMAC KMS key, and MAC
         algorithm.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.verify_mac)
```

### Comparing `types-aiobotocore-kms-2.9.0/types_aiobotocore_kms/literals.py` & `types-aiobotocore-kms-2.9.1/types_aiobotocore_kms/literals.py`

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
     "AlgorithmSpecType",
     "ConnectionErrorCodeTypeType",
     "ConnectionStateTypeType",
     "CustomKeyStoreTypeType",
     "CustomerMasterKeySpecType",
     "DataKeyPairSpecType",
@@ -53,15 +52,14 @@
     "KMSServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AlgorithmSpecType = Literal[
     "RSAES_OAEP_SHA_1",
     "RSAES_OAEP_SHA_256",
     "RSAES_PKCS1_V1_5",
     "RSA_AES_KEY_WRAP_SHA_1",
     "RSA_AES_KEY_WRAP_SHA_256",
 ]
```

### Comparing `types-aiobotocore-kms-2.9.0/types_aiobotocore_kms/literals.pyi` & `types-aiobotocore-kms-2.9.1/types_aiobotocore_kms/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kms-2.9.0/types_aiobotocore_kms/paginator.py` & `types-aiobotocore-kms-2.9.1/types_aiobotocore_kms/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,14 @@
     "ListGrantsPaginator",
     "ListKeyPoliciesPaginator",
     "ListKeysPaginator",
     "ListResourceTagsPaginator",
     "ListRetirableGrantsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -76,15 +75,15 @@
     """
 
     def paginate(
         self,
         *,
         CustomKeyStoreId: str = ...,
         CustomKeyStoreName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeCustomKeyStoresResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.DescribeCustomKeyStores.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/paginators/#describecustomkeystorespaginator)
         """
 
 
@@ -111,15 +110,15 @@
 
     def paginate(
         self,
         *,
         KeyId: str,
         GrantId: str = ...,
         GranteePrincipal: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListGrantsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListGrants.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/paginators/#listgrantspaginator)
         """
```

### Comparing `types-aiobotocore-kms-2.9.0/types_aiobotocore_kms/paginator.pyi` & `types-aiobotocore-kms-2.9.1/types_aiobotocore_kms/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     """
 
     def paginate(
         self,
         *,
         CustomKeyStoreId: str = ...,
         CustomKeyStoreName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeCustomKeyStoresResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.DescribeCustomKeyStores.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/paginators/#describecustomkeystorespaginator)
         """
 
 class ListAliasesPaginator(AioPaginator):
@@ -106,15 +106,15 @@
 
     def paginate(
         self,
         *,
         KeyId: str,
         GrantId: str = ...,
         GranteePrincipal: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListGrantsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListGrants.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/paginators/#listgrantspaginator)
         """
 
 class ListKeyPoliciesPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-kms-2.9.0/types_aiobotocore_kms/type_defs.py` & `types-aiobotocore-kms-2.9.1/types_aiobotocore_kms/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AliasListEntryTypeDef",
     "BlobTypeDef",
     "CancelKeyDeletionRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "ConnectCustomKeyStoreRequestRequestTypeDef",
     "CreateAliasRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-kms-2.9.0/types_aiobotocore_kms/type_defs.pyi` & `types-aiobotocore-kms-2.9.1/types_aiobotocore_kms/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kms-2.9.0/types_aiobotocore_kms.egg-info/PKG-INFO` & `types-aiobotocore-kms-2.9.1/types_aiobotocore_kms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kms
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.KMS 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.KMS 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/
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
 
 <a id="types-aiobotocore-kms"></a>
 
 # types-aiobotocore-kms
 
 [![PyPI - types-aiobotocore-kms](https://img.shields.io/pypi/v/types-aiobotocore-kms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kms)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kms)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kms)](https://pepy.tech/project/types-aiobotocore-kms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.KMS 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
+[aiobotocore.KMS 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
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
 [types-aiobotocore-kms docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-kms-2.9.0/types_aiobotocore_kms.egg-info/SOURCES.txt` & `types-aiobotocore-kms-2.9.1/types_aiobotocore_kms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

