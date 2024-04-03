# Comparing `tmp/types-aiobotocore-networkmanager-2.9.0.tar.gz` & `tmp/types-aiobotocore-networkmanager-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-networkmanager-2.9.0.tar", last modified: Wed Dec 13 20:00:01 2023, max compression
+gzip compressed data, was "types-aiobotocore-networkmanager-2.9.1.tar", last modified: Thu Jan 18 01:21:22 2024, max compression
```

## Comparing `types-aiobotocore-networkmanager-2.9.0.tar` & `types-aiobotocore-networkmanager-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:01.729387 types-aiobotocore-networkmanager-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:50:55.000000 types-aiobotocore-networkmanager-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16732 2023-12-13 20:00:01.729387 types-aiobotocore-networkmanager-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15141 2023-12-13 19:50:55.000000 types-aiobotocore-networkmanager-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:01.729387 types-aiobotocore-networkmanager-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2023-12-13 19:50:55.000000 types-aiobotocore-networkmanager-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:01.725387 types-aiobotocore-networkmanager-2.9.0/types_aiobotocore_networkmanager/
--rw-r--r--   0 runner    (1001) docker     (127)     5444 2023-12-13 19:50:55.000000 types-aiobotocore-networkmanager-2.9.0/types_aiobotocore_networkmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5443 2023-12-13 19:50:55.000000 types-aiobotocore-networkmanager-2.9.0/types_aiobotocore_networkmanager/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      960 2023-12-13 19:50:55.000000 types-aiobotocore-networkmanager-2.9.0/types_aiobotocore_networkmanager/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    73564 2023-12-13 19:50:55.000000 types-aiobotocore-networkmanager-2.9.0/types_aiobotocore_networkmanager/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    73560 2023-12-13 19:50:55.000000 types-aiobotocore-networkmanager-2.9.0/types_aiobotocore_networkmanager/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    15213 2023-12-13 19:50:56.000000 types-aiobotocore-networkmanager-2.9.0/types_aiobotocore_networkmanager/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    15211 2023-12-13 19:50:56.000000 types-aiobotocore-networkmanager-2.9.0/types_aiobotocore_networkmanager/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    28539 2023-12-13 19:50:56.000000 types-aiobotocore-networkmanager-2.9.0/types_aiobotocore_networkmanager/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    28515 2023-12-13 19:50:55.000000 types-aiobotocore-networkmanager-2.9.0/types_aiobotocore_networkmanager/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:50:55.000000 types-aiobotocore-networkmanager-2.9.0/types_aiobotocore_networkmanager/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    79219 2023-12-13 19:50:57.000000 types-aiobotocore-networkmanager-2.9.0/types_aiobotocore_networkmanager/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    79218 2023-12-13 19:50:56.000000 types-aiobotocore-networkmanager-2.9.0/types_aiobotocore_networkmanager/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:50:55.000000 types-aiobotocore-networkmanager-2.9.0/types_aiobotocore_networkmanager/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:01.729387 types-aiobotocore-networkmanager-2.9.0/types_aiobotocore_networkmanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16732 2023-12-13 20:00:01.000000 types-aiobotocore-networkmanager-2.9.0/types_aiobotocore_networkmanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      946 2023-12-13 20:00:01.000000 types-aiobotocore-networkmanager-2.9.0/types_aiobotocore_networkmanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:01.000000 types-aiobotocore-networkmanager-2.9.0/types_aiobotocore_networkmanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:01.000000 types-aiobotocore-networkmanager-2.9.0/types_aiobotocore_networkmanager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:01.000000 types-aiobotocore-networkmanager-2.9.0/types_aiobotocore_networkmanager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-13 20:00:01.000000 types-aiobotocore-networkmanager-2.9.0/types_aiobotocore_networkmanager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:22.877151 types-aiobotocore-networkmanager-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:12:35.000000 types-aiobotocore-networkmanager-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16752 2024-01-18 01:21:22.877151 types-aiobotocore-networkmanager-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15141 2024-01-18 01:12:35.000000 types-aiobotocore-networkmanager-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:22.877151 types-aiobotocore-networkmanager-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-01-18 01:12:35.000000 types-aiobotocore-networkmanager-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:22.877151 types-aiobotocore-networkmanager-2.9.1/types_aiobotocore_networkmanager/
+-rw-r--r--   0 runner    (1001) docker     (127)     5443 2024-01-18 01:12:35.000000 types-aiobotocore-networkmanager-2.9.1/types_aiobotocore_networkmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5443 2024-01-18 01:12:35.000000 types-aiobotocore-networkmanager-2.9.1/types_aiobotocore_networkmanager/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-01-18 01:12:36.000000 types-aiobotocore-networkmanager-2.9.1/types_aiobotocore_networkmanager/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73602 2024-01-18 01:12:36.000000 types-aiobotocore-networkmanager-2.9.1/types_aiobotocore_networkmanager/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73599 2024-01-18 01:12:36.000000 types-aiobotocore-networkmanager-2.9.1/types_aiobotocore_networkmanager/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    15211 2024-01-18 01:12:36.000000 types-aiobotocore-networkmanager-2.9.1/types_aiobotocore_networkmanager/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15211 2024-01-18 01:12:36.000000 types-aiobotocore-networkmanager-2.9.1/types_aiobotocore_networkmanager/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    28556 2024-01-18 01:12:36.000000 types-aiobotocore-networkmanager-2.9.1/types_aiobotocore_networkmanager/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28534 2024-01-18 01:12:36.000000 types-aiobotocore-networkmanager-2.9.1/types_aiobotocore_networkmanager/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:12:36.000000 types-aiobotocore-networkmanager-2.9.1/types_aiobotocore_networkmanager/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    79218 2024-01-18 01:12:38.000000 types-aiobotocore-networkmanager-2.9.1/types_aiobotocore_networkmanager/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79218 2024-01-18 01:12:37.000000 types-aiobotocore-networkmanager-2.9.1/types_aiobotocore_networkmanager/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:12:35.000000 types-aiobotocore-networkmanager-2.9.1/types_aiobotocore_networkmanager/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:22.877151 types-aiobotocore-networkmanager-2.9.1/types_aiobotocore_networkmanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16752 2024-01-18 01:21:22.000000 types-aiobotocore-networkmanager-2.9.1/types_aiobotocore_networkmanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-01-18 01:21:22.000000 types-aiobotocore-networkmanager-2.9.1/types_aiobotocore_networkmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:22.000000 types-aiobotocore-networkmanager-2.9.1/types_aiobotocore_networkmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:22.000000 types-aiobotocore-networkmanager-2.9.1/types_aiobotocore_networkmanager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:22.000000 types-aiobotocore-networkmanager-2.9.1/types_aiobotocore_networkmanager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-18 01:21:22.000000 types-aiobotocore-networkmanager-2.9.1/types_aiobotocore_networkmanager.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-networkmanager-2.9.0/LICENSE` & `types-aiobotocore-networkmanager-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-networkmanager-2.9.0/PKG-INFO` & `types-aiobotocore-networkmanager-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-networkmanager
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.NetworkManager 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.NetworkManager 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/
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
 
 <a id="types-aiobotocore-networkmanager"></a>
 
 # types-aiobotocore-networkmanager
 
 [![PyPI - types-aiobotocore-networkmanager](https://img.shields.io/pypi/v/types-aiobotocore-networkmanager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-networkmanager)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-networkmanager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-networkmanager)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-networkmanager)](https://pepy.tech/project/types-aiobotocore-networkmanager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.NetworkManager 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager)
+[aiobotocore.NetworkManager 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager)
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
 [types-aiobotocore-networkmanager docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-networkmanager-2.9.0/README.md` & `types-aiobotocore-networkmanager-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-networkmanager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-networkmanager)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-networkmanager)](https://pepy.tech/project/types-aiobotocore-networkmanager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.NetworkManager 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager)
+[aiobotocore.NetworkManager 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager)
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
 [types-aiobotocore-networkmanager docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-networkmanager-2.9.0/setup.py` & `types-aiobotocore-networkmanager-2.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-networkmanager",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_networkmanager"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.NetworkManager 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.NetworkManager 2.9.1 service generated with"
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
     keywords="aiobotocore networkmanager type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_networkmanager": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-networkmanager-2.9.0/types_aiobotocore_networkmanager/__init__.py` & `types-aiobotocore-networkmanager-2.9.1/types_aiobotocore_networkmanager/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,14 @@
     ListCoreNetworkPolicyVersionsPaginator,
     ListCoreNetworksPaginator,
     ListPeeringsPaginator,
 )
 
 Client = NetworkManagerClient
 
-
 __all__ = (
     "Client",
     "DescribeGlobalNetworksPaginator",
     "GetConnectPeerAssociationsPaginator",
     "GetConnectionsPaginator",
     "GetCoreNetworkChangeEventsPaginator",
     "GetCoreNetworkChangeSetPaginator",
```

### Comparing `types-aiobotocore-networkmanager-2.9.0/types_aiobotocore_networkmanager/__init__.pyi` & `types-aiobotocore-networkmanager-2.9.1/types_aiobotocore_networkmanager/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-networkmanager-2.9.0/types_aiobotocore_networkmanager/__main__.py` & `types-aiobotocore-networkmanager-2.9.1/types_aiobotocore_networkmanager/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.NetworkManager 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.NetworkManager 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager\nOther"
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

### Comparing `types-aiobotocore-networkmanager-2.9.0/types_aiobotocore_networkmanager/client.py` & `types-aiobotocore-networkmanager-2.9.1/types_aiobotocore_networkmanager/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("NetworkManagerClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -231,15 +230,15 @@
 
     async def associate_transit_gateway_connect_peer(
         self,
         *,
         GlobalNetworkId: str,
         TransitGatewayConnectPeerArn: str,
         DeviceId: str,
-        LinkId: str = ...
+        LinkId: str = ...,
     ) -> AssociateTransitGatewayConnectPeerResponseTypeDef:
         """
         Associates a transit gateway Connect peer with a device, and optionally, with a
         link.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.associate_transit_gateway_connect_peer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#associate_transit_gateway_connect_peer)
@@ -265,15 +264,15 @@
         self,
         *,
         CoreNetworkId: str,
         EdgeLocation: str,
         TransportAttachmentId: str,
         Options: ConnectAttachmentOptionsTypeDef,
         Tags: Sequence[TagTypeDef] = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreateConnectAttachmentResponseTypeDef:
         """
         Creates a core network Connect attachment from a specified core network
         attachment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.create_connect_attachment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#create_connect_attachment)
@@ -285,15 +284,15 @@
         ConnectAttachmentId: str,
         PeerAddress: str,
         CoreNetworkAddress: str = ...,
         BgpOptions: BgpOptionsTypeDef = ...,
         InsideCidrBlocks: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientToken: str = ...,
-        SubnetArn: str = ...
+        SubnetArn: str = ...,
     ) -> CreateConnectPeerResponseTypeDef:
         """
         Creates a core network Connect peer for a specified core network connect
         attachment between a core network and an
         appliance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.create_connect_peer)
@@ -305,15 +304,15 @@
         *,
         GlobalNetworkId: str,
         DeviceId: str,
         ConnectedDeviceId: str,
         LinkId: str = ...,
         ConnectedLinkId: str = ...,
         Description: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateConnectionResponseTypeDef:
         """
         Creates a connection between two devices.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.create_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#create_connection)
         """
@@ -321,15 +320,15 @@
     async def create_core_network(
         self,
         *,
         GlobalNetworkId: str,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         PolicyDocument: str = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreateCoreNetworkResponseTypeDef:
         """
         Creates a core network as part of your global network, and optionally, with a
         core network
         policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.create_core_network)
@@ -344,15 +343,15 @@
         Description: str = ...,
         Type: str = ...,
         Vendor: str = ...,
         Model: str = ...,
         SerialNumber: str = ...,
         Location: LocationTypeDef = ...,
         SiteId: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDeviceResponseTypeDef:
         """
         Creates a new device in a global network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.create_device)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#create_device)
         """
@@ -372,45 +371,45 @@
         *,
         GlobalNetworkId: str,
         Bandwidth: BandwidthTypeDef,
         SiteId: str,
         Description: str = ...,
         Type: str = ...,
         Provider: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateLinkResponseTypeDef:
         """
         Creates a new link for a specified site.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.create_link)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#create_link)
         """
 
     async def create_site(
         self,
         *,
         GlobalNetworkId: str,
         Description: str = ...,
         Location: LocationTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateSiteResponseTypeDef:
         """
         Creates a new site in a global network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.create_site)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#create_site)
         """
 
     async def create_site_to_site_vpn_attachment(
         self,
         *,
         CoreNetworkId: str,
         VpnConnectionArn: str,
         Tags: Sequence[TagTypeDef] = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreateSiteToSiteVpnAttachmentResponseTypeDef:
         """
         Creates an Amazon Web Services site-to-site VPN attachment on an edge location
         of a core
         network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.create_site_to_site_vpn_attachment)
@@ -419,30 +418,30 @@
 
     async def create_transit_gateway_peering(
         self,
         *,
         CoreNetworkId: str,
         TransitGatewayArn: str,
         Tags: Sequence[TagTypeDef] = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreateTransitGatewayPeeringResponseTypeDef:
         """
         Creates a transit gateway peering connection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.create_transit_gateway_peering)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#create_transit_gateway_peering)
         """
 
     async def create_transit_gateway_route_table_attachment(
         self,
         *,
         PeeringId: str,
         TransitGatewayRouteTableArn: str,
         Tags: Sequence[TagTypeDef] = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreateTransitGatewayRouteTableAttachmentResponseTypeDef:
         """
         Creates a transit gateway route table attachment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.create_transit_gateway_route_table_attachment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#create_transit_gateway_route_table_attachment)
         """
@@ -451,15 +450,15 @@
         self,
         *,
         CoreNetworkId: str,
         VpcArn: str,
         SubnetArns: Sequence[str],
         Options: VpcOptionsTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreateVpcAttachmentResponseTypeDef:
         """
         Creates a VPC attachment on an edge location of a core network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.create_vpc_attachment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#create_vpc_attachment)
         """
@@ -664,15 +663,15 @@
 
     async def get_connect_peer_associations(
         self,
         *,
         GlobalNetworkId: str,
         ConnectPeerIds: Sequence[str] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetConnectPeerAssociationsResponseTypeDef:
         """
         Returns information about a core network Connect peer associations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.get_connect_peer_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#get_connect_peer_associations)
         """
@@ -680,15 +679,15 @@
     async def get_connections(
         self,
         *,
         GlobalNetworkId: str,
         ConnectionIds: Sequence[str] = ...,
         DeviceId: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetConnectionsResponseTypeDef:
         """
         Gets information about one or more of your connections in a global network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.get_connections)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#get_connections)
         """
@@ -703,60 +702,60 @@
 
     async def get_core_network_change_events(
         self,
         *,
         CoreNetworkId: str,
         PolicyVersionId: int,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetCoreNetworkChangeEventsResponseTypeDef:
         """
         Returns information about a core network change event.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.get_core_network_change_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#get_core_network_change_events)
         """
 
     async def get_core_network_change_set(
         self,
         *,
         CoreNetworkId: str,
         PolicyVersionId: int,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetCoreNetworkChangeSetResponseTypeDef:
         """
         Returns a change set between the LIVE core network policy and a submitted
         policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.get_core_network_change_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#get_core_network_change_set)
         """
 
     async def get_core_network_policy(
         self,
         *,
         CoreNetworkId: str,
         PolicyVersionId: int = ...,
-        Alias: CoreNetworkPolicyAliasType = ...
+        Alias: CoreNetworkPolicyAliasType = ...,
     ) -> GetCoreNetworkPolicyResponseTypeDef:
         """
         Returns details about a core network policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.get_core_network_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#get_core_network_policy)
         """
 
     async def get_customer_gateway_associations(
         self,
         *,
         GlobalNetworkId: str,
         CustomerGatewayArns: Sequence[str] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetCustomerGatewayAssociationsResponseTypeDef:
         """
         Gets the association information for customer gateways that are associated with
         devices and links in your global
         network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.get_customer_gateway_associations)
@@ -766,15 +765,15 @@
     async def get_devices(
         self,
         *,
         GlobalNetworkId: str,
         DeviceIds: Sequence[str] = ...,
         SiteId: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetDevicesResponseTypeDef:
         """
         Gets information about one or more of your devices in a global network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.get_devices)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#get_devices)
         """
@@ -782,15 +781,15 @@
     async def get_link_associations(
         self,
         *,
         GlobalNetworkId: str,
         DeviceId: str = ...,
         LinkId: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetLinkAssociationsResponseTypeDef:
         """
         Gets the link associations for a device or a link.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.get_link_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#get_link_associations)
         """
@@ -800,30 +799,30 @@
         *,
         GlobalNetworkId: str,
         LinkIds: Sequence[str] = ...,
         SiteId: str = ...,
         Type: str = ...,
         Provider: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetLinksResponseTypeDef:
         """
         Gets information about one or more links in a specified global network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.get_links)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#get_links)
         """
 
     async def get_network_resource_counts(
         self,
         *,
         GlobalNetworkId: str,
         ResourceType: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetNetworkResourceCountsResponseTypeDef:
         """
         Gets the count of network resources, by resource type, for the specified global
         network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.get_network_resource_counts)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#get_network_resource_counts)
@@ -836,15 +835,15 @@
         CoreNetworkId: str = ...,
         RegisteredGatewayArn: str = ...,
         AwsRegion: str = ...,
         AccountId: str = ...,
         ResourceType: str = ...,
         ResourceArn: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetNetworkResourceRelationshipsResponseTypeDef:
         """
         Gets the network resource relationships for the specified global network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.get_network_resource_relationships)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#get_network_resource_relationships)
         """
@@ -856,15 +855,15 @@
         CoreNetworkId: str = ...,
         RegisteredGatewayArn: str = ...,
         AwsRegion: str = ...,
         AccountId: str = ...,
         ResourceType: str = ...,
         ResourceArn: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetNetworkResourcesResponseTypeDef:
         """
         Describes the network resources for the specified global network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.get_network_resources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#get_network_resources)
         """
@@ -877,15 +876,15 @@
         ExactCidrMatches: Sequence[str] = ...,
         LongestPrefixMatches: Sequence[str] = ...,
         SubnetOfMatches: Sequence[str] = ...,
         SupernetOfMatches: Sequence[str] = ...,
         PrefixListIds: Sequence[str] = ...,
         States: Sequence[RouteStateType] = ...,
         Types: Sequence[RouteTypeType] = ...,
-        DestinationFilters: Mapping[str, Sequence[str]] = ...
+        DestinationFilters: Mapping[str, Sequence[str]] = ...,
     ) -> GetNetworkRoutesResponseTypeDef:
         """
         Gets the network routes of the specified global network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.get_network_routes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#get_network_routes)
         """
@@ -897,15 +896,15 @@
         CoreNetworkId: str = ...,
         RegisteredGatewayArn: str = ...,
         AwsRegion: str = ...,
         AccountId: str = ...,
         ResourceType: str = ...,
         ResourceArn: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetNetworkTelemetryResponseTypeDef:
         """
         Gets the network telemetry of the specified global network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.get_network_telemetry)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#get_network_telemetry)
         """
@@ -940,30 +939,30 @@
 
     async def get_sites(
         self,
         *,
         GlobalNetworkId: str,
         SiteIds: Sequence[str] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetSitesResponseTypeDef:
         """
         Gets information about one or more of your sites in a global network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.get_sites)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#get_sites)
         """
 
     async def get_transit_gateway_connect_peer_associations(
         self,
         *,
         GlobalNetworkId: str,
         TransitGatewayConnectPeerArns: Sequence[str] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetTransitGatewayConnectPeerAssociationsResponseTypeDef:
         """
         Gets information about one or more of your transit gateway Connect peer
         associations in a global
         network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.get_transit_gateway_connect_peer_associations)
@@ -982,15 +981,15 @@
 
     async def get_transit_gateway_registrations(
         self,
         *,
         GlobalNetworkId: str,
         TransitGatewayArns: Sequence[str] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetTransitGatewayRegistrationsResponseTypeDef:
         """
         Gets information about the transit gateway registrations in a specified global
         network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.get_transit_gateway_registrations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#get_transit_gateway_registrations)
@@ -1018,30 +1017,30 @@
         self,
         *,
         CoreNetworkId: str = ...,
         AttachmentType: AttachmentTypeType = ...,
         EdgeLocation: str = ...,
         State: AttachmentStateType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListAttachmentsResponseTypeDef:
         """
         Returns a list of core network attachments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.list_attachments)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#list_attachments)
         """
 
     async def list_connect_peers(
         self,
         *,
         CoreNetworkId: str = ...,
         ConnectAttachmentId: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListConnectPeersResponseTypeDef:
         """
         Returns a list of core network Connect peers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.list_connect_peers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#list_connect_peers)
         """
@@ -1082,15 +1081,15 @@
         self,
         *,
         CoreNetworkId: str = ...,
         PeeringType: Literal["TRANSIT_GATEWAY"] = ...,
         EdgeLocation: str = ...,
         State: PeeringStateType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListPeeringsResponseTypeDef:
         """
         Lists the peerings for a core network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.list_peerings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#list_peerings)
         """
@@ -1108,15 +1107,15 @@
     async def put_core_network_policy(
         self,
         *,
         CoreNetworkId: str,
         PolicyDocument: str,
         Description: str = ...,
         LatestVersionId: int = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> PutCoreNetworkPolicyResponseTypeDef:
         """
         Creates a new, immutable version of a core network policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.put_core_network_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#put_core_network_policy)
         """
@@ -1172,15 +1171,15 @@
     async def start_route_analysis(
         self,
         *,
         GlobalNetworkId: str,
         Source: RouteAnalysisEndpointOptionsSpecificationTypeDef,
         Destination: RouteAnalysisEndpointOptionsSpecificationTypeDef,
         IncludeReturnPath: bool = ...,
-        UseMiddleboxes: bool = ...
+        UseMiddleboxes: bool = ...,
     ) -> StartRouteAnalysisResponseTypeDef:
         """
         Starts analyzing the routing path between the specified source and destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.start_route_analysis)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#start_route_analysis)
         """
@@ -1204,15 +1203,15 @@
     async def update_connection(
         self,
         *,
         GlobalNetworkId: str,
         ConnectionId: str,
         LinkId: str = ...,
         ConnectedLinkId: str = ...,
-        Description: str = ...
+        Description: str = ...,
     ) -> UpdateConnectionResponseTypeDef:
         """
         Updates the information for an existing connection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.update_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#update_connection)
         """
@@ -1235,15 +1234,15 @@
         AWSLocation: AWSLocationTypeDef = ...,
         Description: str = ...,
         Type: str = ...,
         Vendor: str = ...,
         Model: str = ...,
         SerialNumber: str = ...,
         Location: LocationTypeDef = ...,
-        SiteId: str = ...
+        SiteId: str = ...,
     ) -> UpdateDeviceResponseTypeDef:
         """
         Updates the details for an existing device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.update_device)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#update_device)
         """
@@ -1262,15 +1261,15 @@
         self,
         *,
         GlobalNetworkId: str,
         LinkId: str,
         Description: str = ...,
         Type: str = ...,
         Bandwidth: BandwidthTypeDef = ...,
-        Provider: str = ...
+        Provider: str = ...,
     ) -> UpdateLinkResponseTypeDef:
         """
         Updates the details for an existing link.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.update_link)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#update_link)
         """
@@ -1287,30 +1286,30 @@
 
     async def update_site(
         self,
         *,
         GlobalNetworkId: str,
         SiteId: str,
         Description: str = ...,
-        Location: LocationTypeDef = ...
+        Location: LocationTypeDef = ...,
     ) -> UpdateSiteResponseTypeDef:
         """
         Updates the information for an existing site.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.update_site)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#update_site)
         """
 
     async def update_vpc_attachment(
         self,
         *,
         AttachmentId: str,
         AddSubnetArns: Sequence[str] = ...,
         RemoveSubnetArns: Sequence[str] = ...,
-        Options: VpcOptionsTypeDef = ...
+        Options: VpcOptionsTypeDef = ...,
     ) -> UpdateVpcAttachmentResponseTypeDef:
         """
         Updates a VPC attachment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.update_vpc_attachment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#update_vpc_attachment)
         """
```

### Comparing `types-aiobotocore-networkmanager-2.9.0/types_aiobotocore_networkmanager/client.pyi` & `types-aiobotocore-networkmanager-2.9.1/types_aiobotocore_networkmanager/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -227,15 +227,15 @@
 
     async def associate_transit_gateway_connect_peer(
         self,
         *,
         GlobalNetworkId: str,
         TransitGatewayConnectPeerArn: str,
         DeviceId: str,
-        LinkId: str = ...
+        LinkId: str = ...,
     ) -> AssociateTransitGatewayConnectPeerResponseTypeDef:
         """
         Associates a transit gateway Connect peer with a device, and optionally, with a
         link.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.associate_transit_gateway_connect_peer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#associate_transit_gateway_connect_peer)
@@ -261,15 +261,15 @@
         self,
         *,
         CoreNetworkId: str,
         EdgeLocation: str,
         TransportAttachmentId: str,
         Options: ConnectAttachmentOptionsTypeDef,
         Tags: Sequence[TagTypeDef] = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreateConnectAttachmentResponseTypeDef:
         """
         Creates a core network Connect attachment from a specified core network
         attachment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.create_connect_attachment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#create_connect_attachment)
@@ -281,15 +281,15 @@
         ConnectAttachmentId: str,
         PeerAddress: str,
         CoreNetworkAddress: str = ...,
         BgpOptions: BgpOptionsTypeDef = ...,
         InsideCidrBlocks: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientToken: str = ...,
-        SubnetArn: str = ...
+        SubnetArn: str = ...,
     ) -> CreateConnectPeerResponseTypeDef:
         """
         Creates a core network Connect peer for a specified core network connect
         attachment between a core network and an
         appliance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.create_connect_peer)
@@ -301,15 +301,15 @@
         *,
         GlobalNetworkId: str,
         DeviceId: str,
         ConnectedDeviceId: str,
         LinkId: str = ...,
         ConnectedLinkId: str = ...,
         Description: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateConnectionResponseTypeDef:
         """
         Creates a connection between two devices.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.create_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#create_connection)
         """
@@ -317,15 +317,15 @@
     async def create_core_network(
         self,
         *,
         GlobalNetworkId: str,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         PolicyDocument: str = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreateCoreNetworkResponseTypeDef:
         """
         Creates a core network as part of your global network, and optionally, with a
         core network
         policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.create_core_network)
@@ -340,15 +340,15 @@
         Description: str = ...,
         Type: str = ...,
         Vendor: str = ...,
         Model: str = ...,
         SerialNumber: str = ...,
         Location: LocationTypeDef = ...,
         SiteId: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDeviceResponseTypeDef:
         """
         Creates a new device in a global network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.create_device)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#create_device)
         """
@@ -368,45 +368,45 @@
         *,
         GlobalNetworkId: str,
         Bandwidth: BandwidthTypeDef,
         SiteId: str,
         Description: str = ...,
         Type: str = ...,
         Provider: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateLinkResponseTypeDef:
         """
         Creates a new link for a specified site.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.create_link)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#create_link)
         """
 
     async def create_site(
         self,
         *,
         GlobalNetworkId: str,
         Description: str = ...,
         Location: LocationTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateSiteResponseTypeDef:
         """
         Creates a new site in a global network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.create_site)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#create_site)
         """
 
     async def create_site_to_site_vpn_attachment(
         self,
         *,
         CoreNetworkId: str,
         VpnConnectionArn: str,
         Tags: Sequence[TagTypeDef] = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreateSiteToSiteVpnAttachmentResponseTypeDef:
         """
         Creates an Amazon Web Services site-to-site VPN attachment on an edge location
         of a core
         network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.create_site_to_site_vpn_attachment)
@@ -415,30 +415,30 @@
 
     async def create_transit_gateway_peering(
         self,
         *,
         CoreNetworkId: str,
         TransitGatewayArn: str,
         Tags: Sequence[TagTypeDef] = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreateTransitGatewayPeeringResponseTypeDef:
         """
         Creates a transit gateway peering connection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.create_transit_gateway_peering)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#create_transit_gateway_peering)
         """
 
     async def create_transit_gateway_route_table_attachment(
         self,
         *,
         PeeringId: str,
         TransitGatewayRouteTableArn: str,
         Tags: Sequence[TagTypeDef] = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreateTransitGatewayRouteTableAttachmentResponseTypeDef:
         """
         Creates a transit gateway route table attachment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.create_transit_gateway_route_table_attachment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#create_transit_gateway_route_table_attachment)
         """
@@ -447,15 +447,15 @@
         self,
         *,
         CoreNetworkId: str,
         VpcArn: str,
         SubnetArns: Sequence[str],
         Options: VpcOptionsTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreateVpcAttachmentResponseTypeDef:
         """
         Creates a VPC attachment on an edge location of a core network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.create_vpc_attachment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#create_vpc_attachment)
         """
@@ -660,15 +660,15 @@
 
     async def get_connect_peer_associations(
         self,
         *,
         GlobalNetworkId: str,
         ConnectPeerIds: Sequence[str] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetConnectPeerAssociationsResponseTypeDef:
         """
         Returns information about a core network Connect peer associations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.get_connect_peer_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#get_connect_peer_associations)
         """
@@ -676,15 +676,15 @@
     async def get_connections(
         self,
         *,
         GlobalNetworkId: str,
         ConnectionIds: Sequence[str] = ...,
         DeviceId: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetConnectionsResponseTypeDef:
         """
         Gets information about one or more of your connections in a global network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.get_connections)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#get_connections)
         """
@@ -699,60 +699,60 @@
 
     async def get_core_network_change_events(
         self,
         *,
         CoreNetworkId: str,
         PolicyVersionId: int,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetCoreNetworkChangeEventsResponseTypeDef:
         """
         Returns information about a core network change event.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.get_core_network_change_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#get_core_network_change_events)
         """
 
     async def get_core_network_change_set(
         self,
         *,
         CoreNetworkId: str,
         PolicyVersionId: int,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetCoreNetworkChangeSetResponseTypeDef:
         """
         Returns a change set between the LIVE core network policy and a submitted
         policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.get_core_network_change_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#get_core_network_change_set)
         """
 
     async def get_core_network_policy(
         self,
         *,
         CoreNetworkId: str,
         PolicyVersionId: int = ...,
-        Alias: CoreNetworkPolicyAliasType = ...
+        Alias: CoreNetworkPolicyAliasType = ...,
     ) -> GetCoreNetworkPolicyResponseTypeDef:
         """
         Returns details about a core network policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.get_core_network_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#get_core_network_policy)
         """
 
     async def get_customer_gateway_associations(
         self,
         *,
         GlobalNetworkId: str,
         CustomerGatewayArns: Sequence[str] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetCustomerGatewayAssociationsResponseTypeDef:
         """
         Gets the association information for customer gateways that are associated with
         devices and links in your global
         network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.get_customer_gateway_associations)
@@ -762,15 +762,15 @@
     async def get_devices(
         self,
         *,
         GlobalNetworkId: str,
         DeviceIds: Sequence[str] = ...,
         SiteId: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetDevicesResponseTypeDef:
         """
         Gets information about one or more of your devices in a global network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.get_devices)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#get_devices)
         """
@@ -778,15 +778,15 @@
     async def get_link_associations(
         self,
         *,
         GlobalNetworkId: str,
         DeviceId: str = ...,
         LinkId: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetLinkAssociationsResponseTypeDef:
         """
         Gets the link associations for a device or a link.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.get_link_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#get_link_associations)
         """
@@ -796,30 +796,30 @@
         *,
         GlobalNetworkId: str,
         LinkIds: Sequence[str] = ...,
         SiteId: str = ...,
         Type: str = ...,
         Provider: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetLinksResponseTypeDef:
         """
         Gets information about one or more links in a specified global network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.get_links)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#get_links)
         """
 
     async def get_network_resource_counts(
         self,
         *,
         GlobalNetworkId: str,
         ResourceType: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetNetworkResourceCountsResponseTypeDef:
         """
         Gets the count of network resources, by resource type, for the specified global
         network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.get_network_resource_counts)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#get_network_resource_counts)
@@ -832,15 +832,15 @@
         CoreNetworkId: str = ...,
         RegisteredGatewayArn: str = ...,
         AwsRegion: str = ...,
         AccountId: str = ...,
         ResourceType: str = ...,
         ResourceArn: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetNetworkResourceRelationshipsResponseTypeDef:
         """
         Gets the network resource relationships for the specified global network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.get_network_resource_relationships)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#get_network_resource_relationships)
         """
@@ -852,15 +852,15 @@
         CoreNetworkId: str = ...,
         RegisteredGatewayArn: str = ...,
         AwsRegion: str = ...,
         AccountId: str = ...,
         ResourceType: str = ...,
         ResourceArn: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetNetworkResourcesResponseTypeDef:
         """
         Describes the network resources for the specified global network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.get_network_resources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#get_network_resources)
         """
@@ -873,15 +873,15 @@
         ExactCidrMatches: Sequence[str] = ...,
         LongestPrefixMatches: Sequence[str] = ...,
         SubnetOfMatches: Sequence[str] = ...,
         SupernetOfMatches: Sequence[str] = ...,
         PrefixListIds: Sequence[str] = ...,
         States: Sequence[RouteStateType] = ...,
         Types: Sequence[RouteTypeType] = ...,
-        DestinationFilters: Mapping[str, Sequence[str]] = ...
+        DestinationFilters: Mapping[str, Sequence[str]] = ...,
     ) -> GetNetworkRoutesResponseTypeDef:
         """
         Gets the network routes of the specified global network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.get_network_routes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#get_network_routes)
         """
@@ -893,15 +893,15 @@
         CoreNetworkId: str = ...,
         RegisteredGatewayArn: str = ...,
         AwsRegion: str = ...,
         AccountId: str = ...,
         ResourceType: str = ...,
         ResourceArn: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetNetworkTelemetryResponseTypeDef:
         """
         Gets the network telemetry of the specified global network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.get_network_telemetry)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#get_network_telemetry)
         """
@@ -936,30 +936,30 @@
 
     async def get_sites(
         self,
         *,
         GlobalNetworkId: str,
         SiteIds: Sequence[str] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetSitesResponseTypeDef:
         """
         Gets information about one or more of your sites in a global network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.get_sites)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#get_sites)
         """
 
     async def get_transit_gateway_connect_peer_associations(
         self,
         *,
         GlobalNetworkId: str,
         TransitGatewayConnectPeerArns: Sequence[str] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetTransitGatewayConnectPeerAssociationsResponseTypeDef:
         """
         Gets information about one or more of your transit gateway Connect peer
         associations in a global
         network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.get_transit_gateway_connect_peer_associations)
@@ -978,15 +978,15 @@
 
     async def get_transit_gateway_registrations(
         self,
         *,
         GlobalNetworkId: str,
         TransitGatewayArns: Sequence[str] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetTransitGatewayRegistrationsResponseTypeDef:
         """
         Gets information about the transit gateway registrations in a specified global
         network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.get_transit_gateway_registrations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#get_transit_gateway_registrations)
@@ -1014,30 +1014,30 @@
         self,
         *,
         CoreNetworkId: str = ...,
         AttachmentType: AttachmentTypeType = ...,
         EdgeLocation: str = ...,
         State: AttachmentStateType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListAttachmentsResponseTypeDef:
         """
         Returns a list of core network attachments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.list_attachments)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#list_attachments)
         """
 
     async def list_connect_peers(
         self,
         *,
         CoreNetworkId: str = ...,
         ConnectAttachmentId: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListConnectPeersResponseTypeDef:
         """
         Returns a list of core network Connect peers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.list_connect_peers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#list_connect_peers)
         """
@@ -1078,15 +1078,15 @@
         self,
         *,
         CoreNetworkId: str = ...,
         PeeringType: Literal["TRANSIT_GATEWAY"] = ...,
         EdgeLocation: str = ...,
         State: PeeringStateType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListPeeringsResponseTypeDef:
         """
         Lists the peerings for a core network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.list_peerings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#list_peerings)
         """
@@ -1104,15 +1104,15 @@
     async def put_core_network_policy(
         self,
         *,
         CoreNetworkId: str,
         PolicyDocument: str,
         Description: str = ...,
         LatestVersionId: int = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> PutCoreNetworkPolicyResponseTypeDef:
         """
         Creates a new, immutable version of a core network policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.put_core_network_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#put_core_network_policy)
         """
@@ -1168,15 +1168,15 @@
     async def start_route_analysis(
         self,
         *,
         GlobalNetworkId: str,
         Source: RouteAnalysisEndpointOptionsSpecificationTypeDef,
         Destination: RouteAnalysisEndpointOptionsSpecificationTypeDef,
         IncludeReturnPath: bool = ...,
-        UseMiddleboxes: bool = ...
+        UseMiddleboxes: bool = ...,
     ) -> StartRouteAnalysisResponseTypeDef:
         """
         Starts analyzing the routing path between the specified source and destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.start_route_analysis)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#start_route_analysis)
         """
@@ -1200,15 +1200,15 @@
     async def update_connection(
         self,
         *,
         GlobalNetworkId: str,
         ConnectionId: str,
         LinkId: str = ...,
         ConnectedLinkId: str = ...,
-        Description: str = ...
+        Description: str = ...,
     ) -> UpdateConnectionResponseTypeDef:
         """
         Updates the information for an existing connection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.update_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#update_connection)
         """
@@ -1231,15 +1231,15 @@
         AWSLocation: AWSLocationTypeDef = ...,
         Description: str = ...,
         Type: str = ...,
         Vendor: str = ...,
         Model: str = ...,
         SerialNumber: str = ...,
         Location: LocationTypeDef = ...,
-        SiteId: str = ...
+        SiteId: str = ...,
     ) -> UpdateDeviceResponseTypeDef:
         """
         Updates the details for an existing device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.update_device)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#update_device)
         """
@@ -1258,15 +1258,15 @@
         self,
         *,
         GlobalNetworkId: str,
         LinkId: str,
         Description: str = ...,
         Type: str = ...,
         Bandwidth: BandwidthTypeDef = ...,
-        Provider: str = ...
+        Provider: str = ...,
     ) -> UpdateLinkResponseTypeDef:
         """
         Updates the details for an existing link.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.update_link)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#update_link)
         """
@@ -1283,30 +1283,30 @@
 
     async def update_site(
         self,
         *,
         GlobalNetworkId: str,
         SiteId: str,
         Description: str = ...,
-        Location: LocationTypeDef = ...
+        Location: LocationTypeDef = ...,
     ) -> UpdateSiteResponseTypeDef:
         """
         Updates the information for an existing site.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.update_site)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#update_site)
         """
 
     async def update_vpc_attachment(
         self,
         *,
         AttachmentId: str,
         AddSubnetArns: Sequence[str] = ...,
         RemoveSubnetArns: Sequence[str] = ...,
-        Options: VpcOptionsTypeDef = ...
+        Options: VpcOptionsTypeDef = ...,
     ) -> UpdateVpcAttachmentResponseTypeDef:
         """
         Updates a VPC attachment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Client.update_vpc_attachment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/client/#update_vpc_attachment)
         """
```

### Comparing `types-aiobotocore-networkmanager-2.9.0/types_aiobotocore_networkmanager/literals.py` & `types-aiobotocore-networkmanager-2.9.1/types_aiobotocore_networkmanager/literals.py`

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
     "AttachmentStateType",
     "AttachmentTypeType",
     "ChangeActionType",
     "ChangeSetStateType",
     "ChangeStatusType",
     "ChangeTypeType",
@@ -74,15 +73,14 @@
     "TunnelProtocolType",
     "NetworkManagerServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 AttachmentStateType = Literal[
     "AVAILABLE",
     "CREATING",
     "DELETING",
     "FAILED",
     "PENDING_ATTACHMENT_ACCEPTANCE",
     "PENDING_NETWORK_UPDATE",
```

### Comparing `types-aiobotocore-networkmanager-2.9.0/types_aiobotocore_networkmanager/literals.pyi` & `types-aiobotocore-networkmanager-2.9.1/types_aiobotocore_networkmanager/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-networkmanager-2.9.0/types_aiobotocore_networkmanager/paginator.py` & `types-aiobotocore-networkmanager-2.9.1/types_aiobotocore_networkmanager/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "DescribeGlobalNetworksPaginator",
     "GetConnectPeerAssociationsPaginator",
     "GetConnectionsPaginator",
     "GetCoreNetworkChangeEventsPaginator",
     "GetCoreNetworkChangeSetPaginator",
     "GetCustomerGatewayAssociationsPaginator",
@@ -119,15 +118,14 @@
     "ListAttachmentsPaginator",
     "ListConnectPeersPaginator",
     "ListCoreNetworkPolicyVersionsPaginator",
     "ListCoreNetworksPaginator",
     "ListPeeringsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -140,15 +138,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#describeglobalnetworkspaginator)
     """
 
     def paginate(
         self,
         *,
         GlobalNetworkIds: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeGlobalNetworksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.DescribeGlobalNetworks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#describeglobalnetworkspaginator)
         """
 
 
@@ -159,15 +157,15 @@
     """
 
     def paginate(
         self,
         *,
         GlobalNetworkId: str,
         ConnectPeerIds: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetConnectPeerAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetConnectPeerAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#getconnectpeerassociationspaginator)
         """
 
 
@@ -179,15 +177,15 @@
 
     def paginate(
         self,
         *,
         GlobalNetworkId: str,
         ConnectionIds: Sequence[str] = ...,
         DeviceId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetConnectionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetConnections.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#getconnectionspaginator)
         """
 
 
@@ -198,15 +196,15 @@
     """
 
     def paginate(
         self,
         *,
         CoreNetworkId: str,
         PolicyVersionId: int,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetCoreNetworkChangeEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetCoreNetworkChangeEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#getcorenetworkchangeeventspaginator)
         """
 
 
@@ -217,15 +215,15 @@
     """
 
     def paginate(
         self,
         *,
         CoreNetworkId: str,
         PolicyVersionId: int,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetCoreNetworkChangeSetResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetCoreNetworkChangeSet.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#getcorenetworkchangesetpaginator)
         """
 
 
@@ -236,15 +234,15 @@
     """
 
     def paginate(
         self,
         *,
         GlobalNetworkId: str,
         CustomerGatewayArns: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetCustomerGatewayAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetCustomerGatewayAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#getcustomergatewayassociationspaginator)
         """
 
 
@@ -256,15 +254,15 @@
 
     def paginate(
         self,
         *,
         GlobalNetworkId: str,
         DeviceIds: Sequence[str] = ...,
         SiteId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetDevicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetDevices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#getdevicespaginator)
         """
 
 
@@ -276,15 +274,15 @@
 
     def paginate(
         self,
         *,
         GlobalNetworkId: str,
         DeviceId: str = ...,
         LinkId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetLinkAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetLinkAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#getlinkassociationspaginator)
         """
 
 
@@ -298,15 +296,15 @@
         self,
         *,
         GlobalNetworkId: str,
         LinkIds: Sequence[str] = ...,
         SiteId: str = ...,
         Type: str = ...,
         Provider: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetLinksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetLinks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#getlinkspaginator)
         """
 
 
@@ -317,15 +315,15 @@
     """
 
     def paginate(
         self,
         *,
         GlobalNetworkId: str,
         ResourceType: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetNetworkResourceCountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetNetworkResourceCounts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#getnetworkresourcecountspaginator)
         """
 
 
@@ -341,15 +339,15 @@
         GlobalNetworkId: str,
         CoreNetworkId: str = ...,
         RegisteredGatewayArn: str = ...,
         AwsRegion: str = ...,
         AccountId: str = ...,
         ResourceType: str = ...,
         ResourceArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetNetworkResourceRelationshipsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetNetworkResourceRelationships.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#getnetworkresourcerelationshipspaginator)
         """
 
 
@@ -365,15 +363,15 @@
         GlobalNetworkId: str,
         CoreNetworkId: str = ...,
         RegisteredGatewayArn: str = ...,
         AwsRegion: str = ...,
         AccountId: str = ...,
         ResourceType: str = ...,
         ResourceArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetNetworkResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetNetworkResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#getnetworkresourcespaginator)
         """
 
 
@@ -389,15 +387,15 @@
         GlobalNetworkId: str,
         CoreNetworkId: str = ...,
         RegisteredGatewayArn: str = ...,
         AwsRegion: str = ...,
         AccountId: str = ...,
         ResourceType: str = ...,
         ResourceArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetNetworkTelemetryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetNetworkTelemetry.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#getnetworktelemetrypaginator)
         """
 
 
@@ -408,15 +406,15 @@
     """
 
     def paginate(
         self,
         *,
         GlobalNetworkId: str,
         SiteIds: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetSitesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetSites.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#getsitespaginator)
         """
 
 
@@ -427,15 +425,15 @@
     """
 
     def paginate(
         self,
         *,
         GlobalNetworkId: str,
         TransitGatewayConnectPeerArns: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetTransitGatewayConnectPeerAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetTransitGatewayConnectPeerAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#gettransitgatewayconnectpeerassociationspaginator)
         """
 
 
@@ -446,15 +444,15 @@
     """
 
     def paginate(
         self,
         *,
         GlobalNetworkId: str,
         TransitGatewayArns: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetTransitGatewayRegistrationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetTransitGatewayRegistrations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#gettransitgatewayregistrationspaginator)
         """
 
 
@@ -467,15 +465,15 @@
     def paginate(
         self,
         *,
         CoreNetworkId: str = ...,
         AttachmentType: AttachmentTypeType = ...,
         EdgeLocation: str = ...,
         State: AttachmentStateType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAttachmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.ListAttachments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#listattachmentspaginator)
         """
 
 
@@ -486,15 +484,15 @@
     """
 
     def paginate(
         self,
         *,
         CoreNetworkId: str = ...,
         ConnectAttachmentId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListConnectPeersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.ListConnectPeers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#listconnectpeerspaginator)
         """
 
 
@@ -537,13 +535,13 @@
     def paginate(
         self,
         *,
         CoreNetworkId: str = ...,
         PeeringType: Literal["TRANSIT_GATEWAY"] = ...,
         EdgeLocation: str = ...,
         State: PeeringStateType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPeeringsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.ListPeerings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#listpeeringspaginator)
         """
```

### Comparing `types-aiobotocore-networkmanager-2.9.0/types_aiobotocore_networkmanager/paginator.pyi` & `types-aiobotocore-networkmanager-2.9.1/types_aiobotocore_networkmanager/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#describeglobalnetworkspaginator)
     """
 
     def paginate(
         self,
         *,
         GlobalNetworkIds: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeGlobalNetworksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.DescribeGlobalNetworks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#describeglobalnetworkspaginator)
         """
 
 class GetConnectPeerAssociationsPaginator(AioPaginator):
@@ -154,15 +154,15 @@
     """
 
     def paginate(
         self,
         *,
         GlobalNetworkId: str,
         ConnectPeerIds: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetConnectPeerAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetConnectPeerAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#getconnectpeerassociationspaginator)
         """
 
 class GetConnectionsPaginator(AioPaginator):
@@ -173,15 +173,15 @@
 
     def paginate(
         self,
         *,
         GlobalNetworkId: str,
         ConnectionIds: Sequence[str] = ...,
         DeviceId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetConnectionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetConnections.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#getconnectionspaginator)
         """
 
 class GetCoreNetworkChangeEventsPaginator(AioPaginator):
@@ -191,15 +191,15 @@
     """
 
     def paginate(
         self,
         *,
         CoreNetworkId: str,
         PolicyVersionId: int,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetCoreNetworkChangeEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetCoreNetworkChangeEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#getcorenetworkchangeeventspaginator)
         """
 
 class GetCoreNetworkChangeSetPaginator(AioPaginator):
@@ -209,15 +209,15 @@
     """
 
     def paginate(
         self,
         *,
         CoreNetworkId: str,
         PolicyVersionId: int,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetCoreNetworkChangeSetResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetCoreNetworkChangeSet.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#getcorenetworkchangesetpaginator)
         """
 
 class GetCustomerGatewayAssociationsPaginator(AioPaginator):
@@ -227,15 +227,15 @@
     """
 
     def paginate(
         self,
         *,
         GlobalNetworkId: str,
         CustomerGatewayArns: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetCustomerGatewayAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetCustomerGatewayAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#getcustomergatewayassociationspaginator)
         """
 
 class GetDevicesPaginator(AioPaginator):
@@ -246,15 +246,15 @@
 
     def paginate(
         self,
         *,
         GlobalNetworkId: str,
         DeviceIds: Sequence[str] = ...,
         SiteId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetDevicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetDevices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#getdevicespaginator)
         """
 
 class GetLinkAssociationsPaginator(AioPaginator):
@@ -265,15 +265,15 @@
 
     def paginate(
         self,
         *,
         GlobalNetworkId: str,
         DeviceId: str = ...,
         LinkId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetLinkAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetLinkAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#getlinkassociationspaginator)
         """
 
 class GetLinksPaginator(AioPaginator):
@@ -286,15 +286,15 @@
         self,
         *,
         GlobalNetworkId: str,
         LinkIds: Sequence[str] = ...,
         SiteId: str = ...,
         Type: str = ...,
         Provider: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetLinksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetLinks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#getlinkspaginator)
         """
 
 class GetNetworkResourceCountsPaginator(AioPaginator):
@@ -304,15 +304,15 @@
     """
 
     def paginate(
         self,
         *,
         GlobalNetworkId: str,
         ResourceType: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetNetworkResourceCountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetNetworkResourceCounts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#getnetworkresourcecountspaginator)
         """
 
 class GetNetworkResourceRelationshipsPaginator(AioPaginator):
@@ -327,15 +327,15 @@
         GlobalNetworkId: str,
         CoreNetworkId: str = ...,
         RegisteredGatewayArn: str = ...,
         AwsRegion: str = ...,
         AccountId: str = ...,
         ResourceType: str = ...,
         ResourceArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetNetworkResourceRelationshipsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetNetworkResourceRelationships.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#getnetworkresourcerelationshipspaginator)
         """
 
 class GetNetworkResourcesPaginator(AioPaginator):
@@ -350,15 +350,15 @@
         GlobalNetworkId: str,
         CoreNetworkId: str = ...,
         RegisteredGatewayArn: str = ...,
         AwsRegion: str = ...,
         AccountId: str = ...,
         ResourceType: str = ...,
         ResourceArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetNetworkResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetNetworkResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#getnetworkresourcespaginator)
         """
 
 class GetNetworkTelemetryPaginator(AioPaginator):
@@ -373,15 +373,15 @@
         GlobalNetworkId: str,
         CoreNetworkId: str = ...,
         RegisteredGatewayArn: str = ...,
         AwsRegion: str = ...,
         AccountId: str = ...,
         ResourceType: str = ...,
         ResourceArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetNetworkTelemetryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetNetworkTelemetry.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#getnetworktelemetrypaginator)
         """
 
 class GetSitesPaginator(AioPaginator):
@@ -391,15 +391,15 @@
     """
 
     def paginate(
         self,
         *,
         GlobalNetworkId: str,
         SiteIds: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetSitesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetSites.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#getsitespaginator)
         """
 
 class GetTransitGatewayConnectPeerAssociationsPaginator(AioPaginator):
@@ -409,15 +409,15 @@
     """
 
     def paginate(
         self,
         *,
         GlobalNetworkId: str,
         TransitGatewayConnectPeerArns: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetTransitGatewayConnectPeerAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetTransitGatewayConnectPeerAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#gettransitgatewayconnectpeerassociationspaginator)
         """
 
 class GetTransitGatewayRegistrationsPaginator(AioPaginator):
@@ -427,15 +427,15 @@
     """
 
     def paginate(
         self,
         *,
         GlobalNetworkId: str,
         TransitGatewayArns: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetTransitGatewayRegistrationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetTransitGatewayRegistrations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#gettransitgatewayregistrationspaginator)
         """
 
 class ListAttachmentsPaginator(AioPaginator):
@@ -447,15 +447,15 @@
     def paginate(
         self,
         *,
         CoreNetworkId: str = ...,
         AttachmentType: AttachmentTypeType = ...,
         EdgeLocation: str = ...,
         State: AttachmentStateType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAttachmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.ListAttachments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#listattachmentspaginator)
         """
 
 class ListConnectPeersPaginator(AioPaginator):
@@ -465,15 +465,15 @@
     """
 
     def paginate(
         self,
         *,
         CoreNetworkId: str = ...,
         ConnectAttachmentId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListConnectPeersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.ListConnectPeers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#listconnectpeerspaginator)
         """
 
 class ListCoreNetworkPolicyVersionsPaginator(AioPaginator):
@@ -513,13 +513,13 @@
     def paginate(
         self,
         *,
         CoreNetworkId: str = ...,
         PeeringType: Literal["TRANSIT_GATEWAY"] = ...,
         EdgeLocation: str = ...,
         State: PeeringStateType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPeeringsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.ListPeerings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#listpeeringspaginator)
         """
```

### Comparing `types-aiobotocore-networkmanager-2.9.0/types_aiobotocore_networkmanager/type_defs.py` & `types-aiobotocore-networkmanager-2.9.1/types_aiobotocore_networkmanager/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AWSLocationTypeDef",
     "AcceptAttachmentRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AccountStatusTypeDef",
     "AssociateConnectPeerRequestRequestTypeDef",
     "ConnectPeerAssociationTypeDef",
```

### Comparing `types-aiobotocore-networkmanager-2.9.0/types_aiobotocore_networkmanager/type_defs.pyi` & `types-aiobotocore-networkmanager-2.9.1/types_aiobotocore_networkmanager/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-networkmanager-2.9.0/types_aiobotocore_networkmanager.egg-info/PKG-INFO` & `types-aiobotocore-networkmanager-2.9.1/types_aiobotocore_networkmanager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-networkmanager
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.NetworkManager 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.NetworkManager 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/
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
 
 <a id="types-aiobotocore-networkmanager"></a>
 
 # types-aiobotocore-networkmanager
 
 [![PyPI - types-aiobotocore-networkmanager](https://img.shields.io/pypi/v/types-aiobotocore-networkmanager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-networkmanager)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-networkmanager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-networkmanager)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-networkmanager)](https://pepy.tech/project/types-aiobotocore-networkmanager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.NetworkManager 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager)
+[aiobotocore.NetworkManager 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager)
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
 [types-aiobotocore-networkmanager docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-networkmanager-2.9.0/types_aiobotocore_networkmanager.egg-info/SOURCES.txt` & `types-aiobotocore-networkmanager-2.9.1/types_aiobotocore_networkmanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

