# Comparing `tmp/types-aiobotocore-transfer-2.9.0.tar.gz` & `tmp/types-aiobotocore-transfer-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-transfer-2.9.0.tar", last modified: Wed Dec 13 20:00:42 2023, max compression
+gzip compressed data, was "types-aiobotocore-transfer-2.9.1.tar", last modified: Thu Jan 18 01:21:59 2024, max compression
```

## Comparing `types-aiobotocore-transfer-2.9.0.tar` & `types-aiobotocore-transfer-2.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:42.245037 types-aiobotocore-transfer-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:57:25.000000 types-aiobotocore-transfer-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15123 2023-12-13 20:00:42.245037 types-aiobotocore-transfer-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13556 2023-12-13 19:57:25.000000 types-aiobotocore-transfer-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:42.245037 types-aiobotocore-transfer-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2023-12-13 19:57:25.000000 types-aiobotocore-transfer-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:42.245037 types-aiobotocore-transfer-2.9.0/types_aiobotocore_transfer/
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2023-12-13 19:57:25.000000 types-aiobotocore-transfer-2.9.0/types_aiobotocore_transfer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2023-12-13 19:57:25.000000 types-aiobotocore-transfer-2.9.0/types_aiobotocore_transfer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      936 2023-12-13 19:57:25.000000 types-aiobotocore-transfer-2.9.0/types_aiobotocore_transfer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    50141 2023-12-13 19:57:25.000000 types-aiobotocore-transfer-2.9.0/types_aiobotocore_transfer/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    50137 2023-12-13 19:57:25.000000 types-aiobotocore-transfer-2.9.0/types_aiobotocore_transfer/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12954 2023-12-13 19:57:25.000000 types-aiobotocore-transfer-2.9.0/types_aiobotocore_transfer/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    12952 2023-12-13 19:57:25.000000 types-aiobotocore-transfer-2.9.0/types_aiobotocore_transfer/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12804 2023-12-13 19:57:25.000000 types-aiobotocore-transfer-2.9.0/types_aiobotocore_transfer/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12791 2023-12-13 19:57:25.000000 types-aiobotocore-transfer-2.9.0/types_aiobotocore_transfer/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:57:25.000000 types-aiobotocore-transfer-2.9.0/types_aiobotocore_transfer/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    51143 2023-12-13 19:57:29.000000 types-aiobotocore-transfer-2.9.0/types_aiobotocore_transfer/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    51142 2023-12-13 19:57:26.000000 types-aiobotocore-transfer-2.9.0/types_aiobotocore_transfer/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:57:25.000000 types-aiobotocore-transfer-2.9.0/types_aiobotocore_transfer/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2023-12-13 19:57:25.000000 types-aiobotocore-transfer-2.9.0/types_aiobotocore_transfer/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2023-12-13 19:57:25.000000 types-aiobotocore-transfer-2.9.0/types_aiobotocore_transfer/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:42.245037 types-aiobotocore-transfer-2.9.0/types_aiobotocore_transfer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15123 2023-12-13 20:00:42.000000 types-aiobotocore-transfer-2.9.0/types_aiobotocore_transfer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      907 2023-12-13 20:00:42.000000 types-aiobotocore-transfer-2.9.0/types_aiobotocore_transfer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:42.000000 types-aiobotocore-transfer-2.9.0/types_aiobotocore_transfer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:42.000000 types-aiobotocore-transfer-2.9.0/types_aiobotocore_transfer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:42.000000 types-aiobotocore-transfer-2.9.0/types_aiobotocore_transfer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-13 20:00:42.000000 types-aiobotocore-transfer-2.9.0/types_aiobotocore_transfer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:59.536986 types-aiobotocore-transfer-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:18:53.000000 types-aiobotocore-transfer-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15143 2024-01-18 01:21:59.536986 types-aiobotocore-transfer-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13556 2024-01-18 01:18:53.000000 types-aiobotocore-transfer-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:59.536986 types-aiobotocore-transfer-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-01-18 01:18:53.000000 types-aiobotocore-transfer-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:59.532986 types-aiobotocore-transfer-2.9.1/types_aiobotocore_transfer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-01-18 01:18:53.000000 types-aiobotocore-transfer-2.9.1/types_aiobotocore_transfer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-01-18 01:18:53.000000 types-aiobotocore-transfer-2.9.1/types_aiobotocore_transfer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-01-18 01:18:53.000000 types-aiobotocore-transfer-2.9.1/types_aiobotocore_transfer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50157 2024-01-18 01:18:54.000000 types-aiobotocore-transfer-2.9.1/types_aiobotocore_transfer/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50154 2024-01-18 01:18:53.000000 types-aiobotocore-transfer-2.9.1/types_aiobotocore_transfer/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12952 2024-01-18 01:18:54.000000 types-aiobotocore-transfer-2.9.1/types_aiobotocore_transfer/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12952 2024-01-18 01:18:54.000000 types-aiobotocore-transfer-2.9.1/types_aiobotocore_transfer/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12803 2024-01-18 01:18:54.000000 types-aiobotocore-transfer-2.9.1/types_aiobotocore_transfer/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12791 2024-01-18 01:18:54.000000 types-aiobotocore-transfer-2.9.1/types_aiobotocore_transfer/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:18:53.000000 types-aiobotocore-transfer-2.9.1/types_aiobotocore_transfer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    51142 2024-01-18 01:18:55.000000 types-aiobotocore-transfer-2.9.1/types_aiobotocore_transfer/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51142 2024-01-18 01:18:55.000000 types-aiobotocore-transfer-2.9.1/types_aiobotocore_transfer/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:18:53.000000 types-aiobotocore-transfer-2.9.1/types_aiobotocore_transfer/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-01-18 01:18:54.000000 types-aiobotocore-transfer-2.9.1/types_aiobotocore_transfer/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-01-18 01:18:54.000000 types-aiobotocore-transfer-2.9.1/types_aiobotocore_transfer/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:59.536986 types-aiobotocore-transfer-2.9.1/types_aiobotocore_transfer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15143 2024-01-18 01:21:59.000000 types-aiobotocore-transfer-2.9.1/types_aiobotocore_transfer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-01-18 01:21:59.000000 types-aiobotocore-transfer-2.9.1/types_aiobotocore_transfer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:59.000000 types-aiobotocore-transfer-2.9.1/types_aiobotocore_transfer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:59.000000 types-aiobotocore-transfer-2.9.1/types_aiobotocore_transfer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:59.000000 types-aiobotocore-transfer-2.9.1/types_aiobotocore_transfer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-18 01:21:59.000000 types-aiobotocore-transfer-2.9.1/types_aiobotocore_transfer.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-transfer-2.9.0/LICENSE` & `types-aiobotocore-transfer-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-transfer-2.9.0/PKG-INFO` & `types-aiobotocore-transfer-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-transfer
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Transfer 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Transfer 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/
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
 
 <a id="types-aiobotocore-transfer"></a>
 
 # types-aiobotocore-transfer
 
 [![PyPI - types-aiobotocore-transfer](https://img.shields.io/pypi/v/types-aiobotocore-transfer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-transfer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-transfer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-transfer)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-transfer)](https://pepy.tech/project/types-aiobotocore-transfer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Transfer 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
+[aiobotocore.Transfer 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
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
 [types-aiobotocore-transfer docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-transfer-2.9.0/README.md` & `types-aiobotocore-transfer-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-transfer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-transfer)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-transfer)](https://pepy.tech/project/types-aiobotocore-transfer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Transfer 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
+[aiobotocore.Transfer 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
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
 [types-aiobotocore-transfer docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-transfer-2.9.0/setup.py` & `types-aiobotocore-transfer-2.9.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-transfer",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_transfer"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Transfer 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.Transfer 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore transfer type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_transfer": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-transfer-2.9.0/types_aiobotocore_transfer/__init__.py` & `types-aiobotocore-transfer-2.9.1/types_aiobotocore_transfer/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,14 @@
     ListUsersPaginator,
     ListWorkflowsPaginator,
 )
 from .waiter import ServerOfflineWaiter, ServerOnlineWaiter
 
 Client = TransferClient
 
-
 __all__ = (
     "Client",
     "ListAccessesPaginator",
     "ListAgreementsPaginator",
     "ListCertificatesPaginator",
     "ListConnectorsPaginator",
     "ListExecutionsPaginator",
```

### Comparing `types-aiobotocore-transfer-2.9.0/types_aiobotocore_transfer/__init__.pyi` & `types-aiobotocore-transfer-2.9.1/types_aiobotocore_transfer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-transfer-2.9.0/types_aiobotocore_transfer/__main__.py` & `types-aiobotocore-transfer-2.9.1/types_aiobotocore_transfer/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Transfer 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Transfer 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer\nOther"
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

### Comparing `types-aiobotocore-transfer-2.9.0/types_aiobotocore_transfer/client.py` & `types-aiobotocore-transfer-2.9.1/types_aiobotocore_transfer/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,14 @@
 from .waiter import ServerOfflineWaiter, ServerOnlineWaiter
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("TransferClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -175,15 +174,15 @@
         Role: str,
         ServerId: str,
         ExternalId: str,
         HomeDirectory: str = ...,
         HomeDirectoryType: HomeDirectoryTypeType = ...,
         HomeDirectoryMappings: Sequence[HomeDirectoryMapEntryTypeDef] = ...,
         Policy: str = ...,
-        PosixProfile: PosixProfileTypeDef = ...
+        PosixProfile: PosixProfileTypeDef = ...,
     ) -> CreateAccessResponseTypeDef:
         """
         Used by administrators to choose which groups in the directory should have
         access to upload and download files over the enabled protocols using Transfer
         Family.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_access)
@@ -196,15 +195,15 @@
         ServerId: str,
         LocalProfileId: str,
         PartnerProfileId: str,
         BaseDirectory: str,
         AccessRole: str,
         Description: str = ...,
         Status: AgreementStatusTypeType = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateAgreementResponseTypeDef:
         """
         Creates an agreement.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_agreement)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/client/#create_agreement)
         """
@@ -213,15 +212,15 @@
         self,
         *,
         Url: str,
         AccessRole: str,
         As2Config: As2ConnectorConfigTypeDef = ...,
         LoggingRole: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        SftpConfig: SftpConnectorConfigTypeDef = ...
+        SftpConfig: SftpConnectorConfigTypeDef = ...,
     ) -> CreateConnectorResponseTypeDef:
         """
         Creates the connector, which captures the parameters for a connection for the
         AS2 or SFTP
         protocol.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_connector)
@@ -230,15 +229,15 @@
 
     async def create_profile(
         self,
         *,
         As2Id: str,
         ProfileType: ProfileTypeType,
         CertificateIds: Sequence[str] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateProfileResponseTypeDef:
         """
         Creates the local or partner profile to use for AS2 transfers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/client/#create_profile)
         """
@@ -258,15 +257,15 @@
         PreAuthenticationLoginBanner: str = ...,
         Protocols: Sequence[ProtocolType] = ...,
         ProtocolDetails: ProtocolDetailsTypeDef = ...,
         SecurityPolicyName: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         WorkflowDetails: WorkflowDetailsTypeDef = ...,
         StructuredLogDestinations: Sequence[str] = ...,
-        S3StorageOptions: S3StorageOptionsTypeDef = ...
+        S3StorageOptions: S3StorageOptionsTypeDef = ...,
     ) -> CreateServerResponseTypeDef:
         """
         Instantiates an auto-scaling virtual server based on the selected file transfer
         protocol in Amazon Web
         Services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_server)
@@ -281,15 +280,15 @@
         UserName: str,
         HomeDirectory: str = ...,
         HomeDirectoryType: HomeDirectoryTypeType = ...,
         HomeDirectoryMappings: Sequence[HomeDirectoryMapEntryTypeDef] = ...,
         Policy: str = ...,
         PosixProfile: PosixProfileTypeDef = ...,
         SshPublicKeyBody: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateUserResponseTypeDef:
         """
         Creates a user and associates them with an existing file transfer
         protocol-enabled
         server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_user)
@@ -298,15 +297,15 @@
 
     async def create_workflow(
         self,
         *,
         Steps: Sequence[WorkflowStepTypeDef],
         Description: str = ...,
         OnExceptionSteps: Sequence[WorkflowStepTypeDef] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateWorkflowResponseTypeDef:
         """
         Allows you to create a workflow with specified steps and step details the
         workflow invokes after file transfer
         completes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_workflow)
@@ -536,15 +535,15 @@
         Usage: CertificateUsageTypeType,
         Certificate: str,
         CertificateChain: str = ...,
         PrivateKey: str = ...,
         ActiveDate: TimestampTypeDef = ...,
         InactiveDate: TimestampTypeDef = ...,
         Description: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> ImportCertificateResponseTypeDef:
         """
         Imports the signing and encryption certificates that you need to create local
         (AS2) profiles and partner
         profiles.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.import_certificate)
@@ -553,15 +552,15 @@
 
     async def import_host_key(
         self,
         *,
         ServerId: str,
         HostKeyBody: str,
         Description: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> ImportHostKeyResponseTypeDef:
         """
         Adds a host key to the server that's specified by the `ServerId` parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.import_host_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/client/#import_host_key)
         """
@@ -726,15 +725,15 @@
     async def start_file_transfer(
         self,
         *,
         ConnectorId: str,
         SendFilePaths: Sequence[str] = ...,
         RetrieveFilePaths: Sequence[str] = ...,
         LocalDirectoryPath: str = ...,
-        RemoteDirectoryPath: str = ...
+        RemoteDirectoryPath: str = ...,
     ) -> StartFileTransferResponseTypeDef:
         """
         Begins a file transfer between local Amazon Web Services storage and a remote
         AS2 or SFTP
         server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.start_file_transfer)
@@ -782,15 +781,15 @@
     async def test_identity_provider(
         self,
         *,
         ServerId: str,
         UserName: str,
         ServerProtocol: ProtocolType = ...,
         SourceIp: str = ...,
-        UserPassword: str = ...
+        UserPassword: str = ...,
     ) -> TestIdentityProviderResponseTypeDef:
         """
         If the `IdentityProviderType` of a file transfer protocol-enabled server is
         `AWS_DIRECTORY_SERVICE` or `API_Gateway`, tests whether your identity provider
         is set up
         successfully.
 
@@ -816,15 +815,15 @@
         ServerId: str,
         ExternalId: str,
         HomeDirectory: str = ...,
         HomeDirectoryType: HomeDirectoryTypeType = ...,
         HomeDirectoryMappings: Sequence[HomeDirectoryMapEntryTypeDef] = ...,
         Policy: str = ...,
         PosixProfile: PosixProfileTypeDef = ...,
-        Role: str = ...
+        Role: str = ...,
     ) -> UpdateAccessResponseTypeDef:
         """
         Allows you to update parameters for the access specified in the `ServerID` and
         `ExternalID`
         parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_access)
@@ -837,30 +836,30 @@
         AgreementId: str,
         ServerId: str,
         Description: str = ...,
         Status: AgreementStatusTypeType = ...,
         LocalProfileId: str = ...,
         PartnerProfileId: str = ...,
         BaseDirectory: str = ...,
-        AccessRole: str = ...
+        AccessRole: str = ...,
     ) -> UpdateAgreementResponseTypeDef:
         """
         Updates some of the parameters for an existing agreement.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_agreement)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/client/#update_agreement)
         """
 
     async def update_certificate(
         self,
         *,
         CertificateId: str,
         ActiveDate: TimestampTypeDef = ...,
         InactiveDate: TimestampTypeDef = ...,
-        Description: str = ...
+        Description: str = ...,
     ) -> UpdateCertificateResponseTypeDef:
         """
         Updates the active and inactive dates for a certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_certificate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/client/#update_certificate)
         """
@@ -869,15 +868,15 @@
         self,
         *,
         ConnectorId: str,
         Url: str = ...,
         As2Config: As2ConnectorConfigTypeDef = ...,
         AccessRole: str = ...,
         LoggingRole: str = ...,
-        SftpConfig: SftpConnectorConfigTypeDef = ...
+        SftpConfig: SftpConnectorConfigTypeDef = ...,
     ) -> UpdateConnectorResponseTypeDef:
         """
         Updates some of the parameters for an existing connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_connector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/client/#update_connector)
         """
@@ -917,15 +916,15 @@
         LoggingRole: str = ...,
         PostAuthenticationLoginBanner: str = ...,
         PreAuthenticationLoginBanner: str = ...,
         Protocols: Sequence[ProtocolType] = ...,
         SecurityPolicyName: str = ...,
         WorkflowDetails: WorkflowDetailsTypeDef = ...,
         StructuredLogDestinations: Sequence[str] = ...,
-        S3StorageOptions: S3StorageOptionsTypeDef = ...
+        S3StorageOptions: S3StorageOptionsTypeDef = ...,
     ) -> UpdateServerResponseTypeDef:
         """
         Updates the file transfer protocol-enabled server's properties after that
         server has been
         created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_server)
@@ -938,15 +937,15 @@
         ServerId: str,
         UserName: str,
         HomeDirectory: str = ...,
         HomeDirectoryType: HomeDirectoryTypeType = ...,
         HomeDirectoryMappings: Sequence[HomeDirectoryMapEntryTypeDef] = ...,
         Policy: str = ...,
         PosixProfile: PosixProfileTypeDef = ...,
-        Role: str = ...
+        Role: str = ...,
     ) -> UpdateUserResponseTypeDef:
         """
         Assigns new properties to a user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/client/#update_user)
         """
```

### Comparing `types-aiobotocore-transfer-2.9.0/types_aiobotocore_transfer/client.pyi` & `types-aiobotocore-transfer-2.9.1/types_aiobotocore_transfer/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -171,15 +171,15 @@
         Role: str,
         ServerId: str,
         ExternalId: str,
         HomeDirectory: str = ...,
         HomeDirectoryType: HomeDirectoryTypeType = ...,
         HomeDirectoryMappings: Sequence[HomeDirectoryMapEntryTypeDef] = ...,
         Policy: str = ...,
-        PosixProfile: PosixProfileTypeDef = ...
+        PosixProfile: PosixProfileTypeDef = ...,
     ) -> CreateAccessResponseTypeDef:
         """
         Used by administrators to choose which groups in the directory should have
         access to upload and download files over the enabled protocols using Transfer
         Family.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_access)
@@ -192,15 +192,15 @@
         ServerId: str,
         LocalProfileId: str,
         PartnerProfileId: str,
         BaseDirectory: str,
         AccessRole: str,
         Description: str = ...,
         Status: AgreementStatusTypeType = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateAgreementResponseTypeDef:
         """
         Creates an agreement.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_agreement)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/client/#create_agreement)
         """
@@ -209,15 +209,15 @@
         self,
         *,
         Url: str,
         AccessRole: str,
         As2Config: As2ConnectorConfigTypeDef = ...,
         LoggingRole: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        SftpConfig: SftpConnectorConfigTypeDef = ...
+        SftpConfig: SftpConnectorConfigTypeDef = ...,
     ) -> CreateConnectorResponseTypeDef:
         """
         Creates the connector, which captures the parameters for a connection for the
         AS2 or SFTP
         protocol.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_connector)
@@ -226,15 +226,15 @@
 
     async def create_profile(
         self,
         *,
         As2Id: str,
         ProfileType: ProfileTypeType,
         CertificateIds: Sequence[str] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateProfileResponseTypeDef:
         """
         Creates the local or partner profile to use for AS2 transfers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/client/#create_profile)
         """
@@ -254,15 +254,15 @@
         PreAuthenticationLoginBanner: str = ...,
         Protocols: Sequence[ProtocolType] = ...,
         ProtocolDetails: ProtocolDetailsTypeDef = ...,
         SecurityPolicyName: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         WorkflowDetails: WorkflowDetailsTypeDef = ...,
         StructuredLogDestinations: Sequence[str] = ...,
-        S3StorageOptions: S3StorageOptionsTypeDef = ...
+        S3StorageOptions: S3StorageOptionsTypeDef = ...,
     ) -> CreateServerResponseTypeDef:
         """
         Instantiates an auto-scaling virtual server based on the selected file transfer
         protocol in Amazon Web
         Services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_server)
@@ -277,15 +277,15 @@
         UserName: str,
         HomeDirectory: str = ...,
         HomeDirectoryType: HomeDirectoryTypeType = ...,
         HomeDirectoryMappings: Sequence[HomeDirectoryMapEntryTypeDef] = ...,
         Policy: str = ...,
         PosixProfile: PosixProfileTypeDef = ...,
         SshPublicKeyBody: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateUserResponseTypeDef:
         """
         Creates a user and associates them with an existing file transfer
         protocol-enabled
         server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_user)
@@ -294,15 +294,15 @@
 
     async def create_workflow(
         self,
         *,
         Steps: Sequence[WorkflowStepTypeDef],
         Description: str = ...,
         OnExceptionSteps: Sequence[WorkflowStepTypeDef] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateWorkflowResponseTypeDef:
         """
         Allows you to create a workflow with specified steps and step details the
         workflow invokes after file transfer
         completes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_workflow)
@@ -532,15 +532,15 @@
         Usage: CertificateUsageTypeType,
         Certificate: str,
         CertificateChain: str = ...,
         PrivateKey: str = ...,
         ActiveDate: TimestampTypeDef = ...,
         InactiveDate: TimestampTypeDef = ...,
         Description: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> ImportCertificateResponseTypeDef:
         """
         Imports the signing and encryption certificates that you need to create local
         (AS2) profiles and partner
         profiles.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.import_certificate)
@@ -549,15 +549,15 @@
 
     async def import_host_key(
         self,
         *,
         ServerId: str,
         HostKeyBody: str,
         Description: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> ImportHostKeyResponseTypeDef:
         """
         Adds a host key to the server that's specified by the `ServerId` parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.import_host_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/client/#import_host_key)
         """
@@ -722,15 +722,15 @@
     async def start_file_transfer(
         self,
         *,
         ConnectorId: str,
         SendFilePaths: Sequence[str] = ...,
         RetrieveFilePaths: Sequence[str] = ...,
         LocalDirectoryPath: str = ...,
-        RemoteDirectoryPath: str = ...
+        RemoteDirectoryPath: str = ...,
     ) -> StartFileTransferResponseTypeDef:
         """
         Begins a file transfer between local Amazon Web Services storage and a remote
         AS2 or SFTP
         server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.start_file_transfer)
@@ -778,15 +778,15 @@
     async def test_identity_provider(
         self,
         *,
         ServerId: str,
         UserName: str,
         ServerProtocol: ProtocolType = ...,
         SourceIp: str = ...,
-        UserPassword: str = ...
+        UserPassword: str = ...,
     ) -> TestIdentityProviderResponseTypeDef:
         """
         If the `IdentityProviderType` of a file transfer protocol-enabled server is
         `AWS_DIRECTORY_SERVICE` or `API_Gateway`, tests whether your identity provider
         is set up
         successfully.
 
@@ -812,15 +812,15 @@
         ServerId: str,
         ExternalId: str,
         HomeDirectory: str = ...,
         HomeDirectoryType: HomeDirectoryTypeType = ...,
         HomeDirectoryMappings: Sequence[HomeDirectoryMapEntryTypeDef] = ...,
         Policy: str = ...,
         PosixProfile: PosixProfileTypeDef = ...,
-        Role: str = ...
+        Role: str = ...,
     ) -> UpdateAccessResponseTypeDef:
         """
         Allows you to update parameters for the access specified in the `ServerID` and
         `ExternalID`
         parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_access)
@@ -833,30 +833,30 @@
         AgreementId: str,
         ServerId: str,
         Description: str = ...,
         Status: AgreementStatusTypeType = ...,
         LocalProfileId: str = ...,
         PartnerProfileId: str = ...,
         BaseDirectory: str = ...,
-        AccessRole: str = ...
+        AccessRole: str = ...,
     ) -> UpdateAgreementResponseTypeDef:
         """
         Updates some of the parameters for an existing agreement.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_agreement)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/client/#update_agreement)
         """
 
     async def update_certificate(
         self,
         *,
         CertificateId: str,
         ActiveDate: TimestampTypeDef = ...,
         InactiveDate: TimestampTypeDef = ...,
-        Description: str = ...
+        Description: str = ...,
     ) -> UpdateCertificateResponseTypeDef:
         """
         Updates the active and inactive dates for a certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_certificate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/client/#update_certificate)
         """
@@ -865,15 +865,15 @@
         self,
         *,
         ConnectorId: str,
         Url: str = ...,
         As2Config: As2ConnectorConfigTypeDef = ...,
         AccessRole: str = ...,
         LoggingRole: str = ...,
-        SftpConfig: SftpConnectorConfigTypeDef = ...
+        SftpConfig: SftpConnectorConfigTypeDef = ...,
     ) -> UpdateConnectorResponseTypeDef:
         """
         Updates some of the parameters for an existing connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_connector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/client/#update_connector)
         """
@@ -913,15 +913,15 @@
         LoggingRole: str = ...,
         PostAuthenticationLoginBanner: str = ...,
         PreAuthenticationLoginBanner: str = ...,
         Protocols: Sequence[ProtocolType] = ...,
         SecurityPolicyName: str = ...,
         WorkflowDetails: WorkflowDetailsTypeDef = ...,
         StructuredLogDestinations: Sequence[str] = ...,
-        S3StorageOptions: S3StorageOptionsTypeDef = ...
+        S3StorageOptions: S3StorageOptionsTypeDef = ...,
     ) -> UpdateServerResponseTypeDef:
         """
         Updates the file transfer protocol-enabled server's properties after that
         server has been
         created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_server)
@@ -934,15 +934,15 @@
         ServerId: str,
         UserName: str,
         HomeDirectory: str = ...,
         HomeDirectoryType: HomeDirectoryTypeType = ...,
         HomeDirectoryMappings: Sequence[HomeDirectoryMapEntryTypeDef] = ...,
         Policy: str = ...,
         PosixProfile: PosixProfileTypeDef = ...,
-        Role: str = ...
+        Role: str = ...,
     ) -> UpdateUserResponseTypeDef:
         """
         Assigns new properties to a user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/client/#update_user)
         """
```

### Comparing `types-aiobotocore-transfer-2.9.0/types_aiobotocore_transfer/literals.py` & `types-aiobotocore-transfer-2.9.1/types_aiobotocore_transfer/literals.py`

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
     "AgreementStatusTypeType",
     "As2TransportType",
     "CertificateStatusTypeType",
     "CertificateTypeType",
     "CertificateUsageTypeType",
     "CompressionEnumType",
@@ -66,15 +65,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 AgreementStatusTypeType = Literal["ACTIVE", "INACTIVE"]
 As2TransportType = Literal["HTTP"]
 CertificateStatusTypeType = Literal["ACTIVE", "INACTIVE", "PENDING_ROTATION"]
 CertificateTypeType = Literal["CERTIFICATE", "CERTIFICATE_WITH_PRIVATE_KEY"]
 CertificateUsageTypeType = Literal["ENCRYPTION", "SIGNING"]
 CompressionEnumType = Literal["DISABLED", "ZLIB"]
 CustomStepStatusType = Literal["FAILURE", "SUCCESS"]
```

### Comparing `types-aiobotocore-transfer-2.9.0/types_aiobotocore_transfer/literals.pyi` & `types-aiobotocore-transfer-2.9.1/types_aiobotocore_transfer/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-transfer-2.9.0/types_aiobotocore_transfer/paginator.py` & `types-aiobotocore-transfer-2.9.1/types_aiobotocore_transfer/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,14 @@
     "ListSecurityPoliciesPaginator",
     "ListServersPaginator",
     "ListTagsForResourcePaginator",
     "ListUsersPaginator",
     "ListWorkflowsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
```

### Comparing `types-aiobotocore-transfer-2.9.0/types_aiobotocore_transfer/paginator.pyi` & `types-aiobotocore-transfer-2.9.1/types_aiobotocore_transfer/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-transfer-2.9.0/types_aiobotocore_transfer/type_defs.py` & `types-aiobotocore-transfer-2.9.1/types_aiobotocore_transfer/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "As2ConnectorConfigTypeDef",
     "HomeDirectoryMapEntryTypeDef",
     "PosixProfileTypeDef",
     "ResponseMetadataTypeDef",
     "TagTypeDef",
     "SftpConnectorConfigTypeDef",
```

### Comparing `types-aiobotocore-transfer-2.9.0/types_aiobotocore_transfer/type_defs.pyi` & `types-aiobotocore-transfer-2.9.1/types_aiobotocore_transfer/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-transfer-2.9.0/types_aiobotocore_transfer/waiter.py` & `types-aiobotocore-transfer-2.9.1/types_aiobotocore_transfer/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-transfer-2.9.0/types_aiobotocore_transfer/waiter.pyi` & `types-aiobotocore-transfer-2.9.1/types_aiobotocore_transfer/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-transfer-2.9.0/types_aiobotocore_transfer.egg-info/PKG-INFO` & `types-aiobotocore-transfer-2.9.1/types_aiobotocore_transfer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-transfer
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Transfer 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Transfer 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/
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
 
 <a id="types-aiobotocore-transfer"></a>
 
 # types-aiobotocore-transfer
 
 [![PyPI - types-aiobotocore-transfer](https://img.shields.io/pypi/v/types-aiobotocore-transfer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-transfer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-transfer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-transfer)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-transfer)](https://pepy.tech/project/types-aiobotocore-transfer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Transfer 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
+[aiobotocore.Transfer 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
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
 [types-aiobotocore-transfer docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-transfer-2.9.0/types_aiobotocore_transfer.egg-info/SOURCES.txt` & `types-aiobotocore-transfer-2.9.1/types_aiobotocore_transfer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

