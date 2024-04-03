# Comparing `tmp/types-aiobotocore-backup-gateway-2.9.0.tar.gz` & `tmp/types-aiobotocore-backup-gateway-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-backup-gateway-2.9.0.tar", last modified: Wed Dec 13 19:58:39 2023, max compression
+gzip compressed data, was "types-aiobotocore-backup-gateway-2.9.1.tar", last modified: Thu Jan 18 01:20:07 2024, max compression
```

## Comparing `types-aiobotocore-backup-gateway-2.9.0.tar` & `types-aiobotocore-backup-gateway-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:39.854051 types-aiobotocore-backup-gateway-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:41:36.000000 types-aiobotocore-backup-gateway-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13673 2023-12-13 19:58:39.854051 types-aiobotocore-backup-gateway-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12083 2023-12-13 19:41:36.000000 types-aiobotocore-backup-gateway-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:39.854051 types-aiobotocore-backup-gateway-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2023-12-13 19:41:36.000000 types-aiobotocore-backup-gateway-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:39.854051 types-aiobotocore-backup-gateway-2.9.0/types_aiobotocore_backup_gateway/
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2023-12-13 19:41:36.000000 types-aiobotocore-backup-gateway-2.9.0/types_aiobotocore_backup_gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2023-12-13 19:41:36.000000 types-aiobotocore-backup-gateway-2.9.0/types_aiobotocore_backup_gateway/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      958 2023-12-13 19:41:36.000000 types-aiobotocore-backup-gateway-2.9.0/types_aiobotocore_backup_gateway/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21691 2023-12-13 19:41:36.000000 types-aiobotocore-backup-gateway-2.9.0/types_aiobotocore_backup_gateway/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    21687 2023-12-13 19:41:36.000000 types-aiobotocore-backup-gateway-2.9.0/types_aiobotocore_backup_gateway/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9243 2023-12-13 19:41:36.000000 types-aiobotocore-backup-gateway-2.9.0/types_aiobotocore_backup_gateway/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9241 2023-12-13 19:41:36.000000 types-aiobotocore-backup-gateway-2.9.0/types_aiobotocore_backup_gateway/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4331 2023-12-13 19:41:36.000000 types-aiobotocore-backup-gateway-2.9.0/types_aiobotocore_backup_gateway/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4326 2023-12-13 19:41:36.000000 types-aiobotocore-backup-gateway-2.9.0/types_aiobotocore_backup_gateway/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:41:36.000000 types-aiobotocore-backup-gateway-2.9.0/types_aiobotocore_backup_gateway/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    17795 2023-12-13 19:41:36.000000 types-aiobotocore-backup-gateway-2.9.0/types_aiobotocore_backup_gateway/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    17794 2023-12-13 19:41:36.000000 types-aiobotocore-backup-gateway-2.9.0/types_aiobotocore_backup_gateway/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:41:36.000000 types-aiobotocore-backup-gateway-2.9.0/types_aiobotocore_backup_gateway/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:39.854051 types-aiobotocore-backup-gateway-2.9.0/types_aiobotocore_backup_gateway.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13673 2023-12-13 19:58:39.000000 types-aiobotocore-backup-gateway-2.9.0/types_aiobotocore_backup_gateway.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      946 2023-12-13 19:58:39.000000 types-aiobotocore-backup-gateway-2.9.0/types_aiobotocore_backup_gateway.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:39.000000 types-aiobotocore-backup-gateway-2.9.0/types_aiobotocore_backup_gateway.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:39.000000 types-aiobotocore-backup-gateway-2.9.0/types_aiobotocore_backup_gateway.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:39.000000 types-aiobotocore-backup-gateway-2.9.0/types_aiobotocore_backup_gateway.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-13 19:58:39.000000 types-aiobotocore-backup-gateway-2.9.0/types_aiobotocore_backup_gateway.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:07.505498 types-aiobotocore-backup-gateway-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:03:34.000000 types-aiobotocore-backup-gateway-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13693 2024-01-18 01:20:07.505498 types-aiobotocore-backup-gateway-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12083 2024-01-18 01:03:34.000000 types-aiobotocore-backup-gateway-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:07.505498 types-aiobotocore-backup-gateway-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-01-18 01:03:34.000000 types-aiobotocore-backup-gateway-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:07.505498 types-aiobotocore-backup-gateway-2.9.1/types_aiobotocore_backup_gateway/
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-01-18 01:03:34.000000 types-aiobotocore-backup-gateway-2.9.1/types_aiobotocore_backup_gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-01-18 01:03:34.000000 types-aiobotocore-backup-gateway-2.9.1/types_aiobotocore_backup_gateway/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-01-18 01:03:34.000000 types-aiobotocore-backup-gateway-2.9.1/types_aiobotocore_backup_gateway/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21696 2024-01-18 01:03:34.000000 types-aiobotocore-backup-gateway-2.9.1/types_aiobotocore_backup_gateway/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21693 2024-01-18 01:03:34.000000 types-aiobotocore-backup-gateway-2.9.1/types_aiobotocore_backup_gateway/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9241 2024-01-18 01:03:34.000000 types-aiobotocore-backup-gateway-2.9.1/types_aiobotocore_backup_gateway/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9241 2024-01-18 01:03:34.000000 types-aiobotocore-backup-gateway-2.9.1/types_aiobotocore_backup_gateway/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-01-18 01:03:34.000000 types-aiobotocore-backup-gateway-2.9.1/types_aiobotocore_backup_gateway/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-01-18 01:03:34.000000 types-aiobotocore-backup-gateway-2.9.1/types_aiobotocore_backup_gateway/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:03:34.000000 types-aiobotocore-backup-gateway-2.9.1/types_aiobotocore_backup_gateway/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    17794 2024-01-18 01:03:35.000000 types-aiobotocore-backup-gateway-2.9.1/types_aiobotocore_backup_gateway/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17794 2024-01-18 01:03:35.000000 types-aiobotocore-backup-gateway-2.9.1/types_aiobotocore_backup_gateway/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:03:34.000000 types-aiobotocore-backup-gateway-2.9.1/types_aiobotocore_backup_gateway/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:07.505498 types-aiobotocore-backup-gateway-2.9.1/types_aiobotocore_backup_gateway.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13693 2024-01-18 01:20:07.000000 types-aiobotocore-backup-gateway-2.9.1/types_aiobotocore_backup_gateway.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-01-18 01:20:07.000000 types-aiobotocore-backup-gateway-2.9.1/types_aiobotocore_backup_gateway.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:07.000000 types-aiobotocore-backup-gateway-2.9.1/types_aiobotocore_backup_gateway.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:07.000000 types-aiobotocore-backup-gateway-2.9.1/types_aiobotocore_backup_gateway.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:07.000000 types-aiobotocore-backup-gateway-2.9.1/types_aiobotocore_backup_gateway.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-18 01:20:07.000000 types-aiobotocore-backup-gateway-2.9.1/types_aiobotocore_backup_gateway.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-backup-gateway-2.9.0/LICENSE` & `types-aiobotocore-backup-gateway-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-backup-gateway-2.9.0/PKG-INFO` & `types-aiobotocore-backup-gateway-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-backup-gateway
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.BackupGateway 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.BackupGateway 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/
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
 
 <a id="types-aiobotocore-backup-gateway"></a>
 
 # types-aiobotocore-backup-gateway
 
 [![PyPI - types-aiobotocore-backup-gateway](https://img.shields.io/pypi/v/types-aiobotocore-backup-gateway.svg?color=blue)](https://pypi.org/project/types-aiobotocore-backup-gateway)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-backup-gateway.svg?color=blue)](https://pypi.org/project/types-aiobotocore-backup-gateway)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-backup-gateway)](https://pepy.tech/project/types-aiobotocore-backup-gateway)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.BackupGateway 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway)
+[aiobotocore.BackupGateway 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway)
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
 [types-aiobotocore-backup-gateway docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-backup-gateway-2.9.0/README.md` & `types-aiobotocore-backup-gateway-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-backup-gateway.svg?color=blue)](https://pypi.org/project/types-aiobotocore-backup-gateway)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-backup-gateway)](https://pepy.tech/project/types-aiobotocore-backup-gateway)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.BackupGateway 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway)
+[aiobotocore.BackupGateway 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway)
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
 [types-aiobotocore-backup-gateway docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-backup-gateway-2.9.0/setup.py` & `types-aiobotocore-backup-gateway-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-backup-gateway",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_backup_gateway"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.BackupGateway 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.BackupGateway 2.9.1 service generated with"
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
     keywords="aiobotocore backup-gateway type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_backup_gateway": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-backup-gateway-2.9.0/types_aiobotocore_backup_gateway/__init__.py` & `types-aiobotocore-backup-gateway-2.9.1/types_aiobotocore_backup_gateway/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 """
 
 from .client import BackupGatewayClient
 from .paginator import ListGatewaysPaginator, ListHypervisorsPaginator, ListVirtualMachinesPaginator
 
 Client = BackupGatewayClient
 
-
 __all__ = (
     "BackupGatewayClient",
     "Client",
     "ListGatewaysPaginator",
     "ListHypervisorsPaginator",
     "ListVirtualMachinesPaginator",
 )
```

### Comparing `types-aiobotocore-backup-gateway-2.9.0/types_aiobotocore_backup_gateway/__init__.pyi` & `types-aiobotocore-backup-gateway-2.9.1/types_aiobotocore_backup_gateway/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backup-gateway-2.9.0/types_aiobotocore_backup_gateway/__main__.py` & `types-aiobotocore-backup-gateway-2.9.1/types_aiobotocore_backup_gateway/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.BackupGateway 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.BackupGateway 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway\nOther"
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

### Comparing `types-aiobotocore-backup-gateway-2.9.0/types_aiobotocore_backup_gateway/client.py` & `types-aiobotocore-backup-gateway-2.9.1/types_aiobotocore_backup_gateway/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("BackupGatewayClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -124,15 +123,15 @@
 
     async def create_gateway(
         self,
         *,
         ActivationKey: str,
         GatewayDisplayName: str,
         GatewayType: Literal["BACKUP_VM"],
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateGatewayOutputTypeDef:
         """
         Creates a backup gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client.create_gateway)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/client/#create_gateway)
         """
@@ -228,15 +227,15 @@
         self,
         *,
         Host: str,
         Name: str,
         KmsKeyArn: str = ...,
         Password: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        Username: str = ...
+        Username: str = ...,
     ) -> ImportHypervisorConfigurationOutputTypeDef:
         """
         Connect to a hypervisor by importing its configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client.import_hypervisor_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/client/#import_hypervisor_configuration)
         """
@@ -282,29 +281,29 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/client/#list_virtual_machines)
         """
 
     async def put_bandwidth_rate_limit_schedule(
         self,
         *,
         BandwidthRateLimitIntervals: Sequence[BandwidthRateLimitIntervalTypeDef],
-        GatewayArn: str
+        GatewayArn: str,
     ) -> PutBandwidthRateLimitScheduleOutputTypeDef:
         """
         This action sets the bandwidth rate limit schedule for a specified gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client.put_bandwidth_rate_limit_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/client/#put_bandwidth_rate_limit_schedule)
         """
 
     async def put_hypervisor_property_mappings(
         self,
         *,
         HypervisorArn: str,
         IamRoleArn: str,
-        VmwareToAwsTagMappings: Sequence[VmwareToAwsTagMappingTypeDef]
+        VmwareToAwsTagMappings: Sequence[VmwareToAwsTagMappingTypeDef],
     ) -> PutHypervisorPropertyMappingsOutputTypeDef:
         """
         This action sets the property mappings for the specified hypervisor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client.put_hypervisor_property_mappings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/client/#put_hypervisor_property_mappings)
         """
@@ -312,15 +311,15 @@
     async def put_maintenance_start_time(
         self,
         *,
         GatewayArn: str,
         HourOfDay: int,
         MinuteOfHour: int,
         DayOfMonth: int = ...,
-        DayOfWeek: int = ...
+        DayOfWeek: int = ...,
     ) -> PutMaintenanceStartTimeOutputTypeDef:
         """
         Set the maintenance start time for a gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client.put_maintenance_start_time)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/client/#put_maintenance_start_time)
         """
@@ -392,15 +391,15 @@
         self,
         *,
         HypervisorArn: str,
         Host: str = ...,
         LogGroupArn: str = ...,
         Name: str = ...,
         Password: str = ...,
-        Username: str = ...
+        Username: str = ...,
     ) -> UpdateHypervisorOutputTypeDef:
         """
         Updates a hypervisor metadata, including its host, username, and password.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client.update_hypervisor)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/client/#update_hypervisor)
         """
```

### Comparing `types-aiobotocore-backup-gateway-2.9.0/types_aiobotocore_backup_gateway/client.pyi` & `types-aiobotocore-backup-gateway-2.9.1/types_aiobotocore_backup_gateway/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,15 @@
 
     async def create_gateway(
         self,
         *,
         ActivationKey: str,
         GatewayDisplayName: str,
         GatewayType: Literal["BACKUP_VM"],
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateGatewayOutputTypeDef:
         """
         Creates a backup gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client.create_gateway)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/client/#create_gateway)
         """
@@ -224,15 +224,15 @@
         self,
         *,
         Host: str,
         Name: str,
         KmsKeyArn: str = ...,
         Password: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        Username: str = ...
+        Username: str = ...,
     ) -> ImportHypervisorConfigurationOutputTypeDef:
         """
         Connect to a hypervisor by importing its configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client.import_hypervisor_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/client/#import_hypervisor_configuration)
         """
@@ -278,29 +278,29 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/client/#list_virtual_machines)
         """
 
     async def put_bandwidth_rate_limit_schedule(
         self,
         *,
         BandwidthRateLimitIntervals: Sequence[BandwidthRateLimitIntervalTypeDef],
-        GatewayArn: str
+        GatewayArn: str,
     ) -> PutBandwidthRateLimitScheduleOutputTypeDef:
         """
         This action sets the bandwidth rate limit schedule for a specified gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client.put_bandwidth_rate_limit_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/client/#put_bandwidth_rate_limit_schedule)
         """
 
     async def put_hypervisor_property_mappings(
         self,
         *,
         HypervisorArn: str,
         IamRoleArn: str,
-        VmwareToAwsTagMappings: Sequence[VmwareToAwsTagMappingTypeDef]
+        VmwareToAwsTagMappings: Sequence[VmwareToAwsTagMappingTypeDef],
     ) -> PutHypervisorPropertyMappingsOutputTypeDef:
         """
         This action sets the property mappings for the specified hypervisor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client.put_hypervisor_property_mappings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/client/#put_hypervisor_property_mappings)
         """
@@ -308,15 +308,15 @@
     async def put_maintenance_start_time(
         self,
         *,
         GatewayArn: str,
         HourOfDay: int,
         MinuteOfHour: int,
         DayOfMonth: int = ...,
-        DayOfWeek: int = ...
+        DayOfWeek: int = ...,
     ) -> PutMaintenanceStartTimeOutputTypeDef:
         """
         Set the maintenance start time for a gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client.put_maintenance_start_time)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/client/#put_maintenance_start_time)
         """
@@ -388,15 +388,15 @@
         self,
         *,
         HypervisorArn: str,
         Host: str = ...,
         LogGroupArn: str = ...,
         Name: str = ...,
         Password: str = ...,
-        Username: str = ...
+        Username: str = ...,
     ) -> UpdateHypervisorOutputTypeDef:
         """
         Updates a hypervisor metadata, including its host, username, and password.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client.update_hypervisor)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/client/#update_hypervisor)
         """
```

### Comparing `types-aiobotocore-backup-gateway-2.9.0/types_aiobotocore_backup_gateway/literals.py` & `types-aiobotocore-backup-gateway-2.9.1/types_aiobotocore_backup_gateway/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,30 +15,28 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "GatewayTypeType",
     "HypervisorStateType",
     "ListGatewaysPaginatorName",
     "ListHypervisorsPaginatorName",
     "ListVirtualMachinesPaginatorName",
     "SyncMetadataStatusType",
     "BackupGatewayServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 GatewayTypeType = Literal["BACKUP_VM"]
 HypervisorStateType = Literal["ERROR", "OFFLINE", "ONLINE", "PENDING"]
 ListGatewaysPaginatorName = Literal["list_gateways"]
 ListHypervisorsPaginatorName = Literal["list_hypervisors"]
 ListVirtualMachinesPaginatorName = Literal["list_virtual_machines"]
 SyncMetadataStatusType = Literal["CREATED", "FAILED", "PARTIALLY_FAILED", "RUNNING", "SUCCEEDED"]
 BackupGatewayServiceName = Literal["backup-gateway"]
```

### Comparing `types-aiobotocore-backup-gateway-2.9.0/types_aiobotocore_backup_gateway/literals.pyi` & `types-aiobotocore-backup-gateway-2.9.1/types_aiobotocore_backup_gateway/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backup-gateway-2.9.0/types_aiobotocore_backup_gateway/paginator.py` & `types-aiobotocore-backup-gateway-2.9.1/types_aiobotocore_backup_gateway/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,14 @@
     ListHypervisorsOutputTypeDef,
     ListVirtualMachinesOutputTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("ListGatewaysPaginator", "ListHypervisorsPaginator", "ListVirtualMachinesPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
```

### Comparing `types-aiobotocore-backup-gateway-2.9.0/types_aiobotocore_backup_gateway/paginator.pyi` & `types-aiobotocore-backup-gateway-2.9.1/types_aiobotocore_backup_gateway/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backup-gateway-2.9.0/types_aiobotocore_backup_gateway/type_defs.py` & `types-aiobotocore-backup-gateway-2.9.1/types_aiobotocore_backup_gateway/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AssociateGatewayToServerInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "BandwidthRateLimitIntervalTypeDef",
     "TagTypeDef",
     "DeleteGatewayInputRequestTypeDef",
     "DeleteHypervisorInputRequestTypeDef",
```

### Comparing `types-aiobotocore-backup-gateway-2.9.0/types_aiobotocore_backup_gateway/type_defs.pyi` & `types-aiobotocore-backup-gateway-2.9.1/types_aiobotocore_backup_gateway/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backup-gateway-2.9.0/types_aiobotocore_backup_gateway.egg-info/PKG-INFO` & `types-aiobotocore-backup-gateway-2.9.1/types_aiobotocore_backup_gateway.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-backup-gateway
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.BackupGateway 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.BackupGateway 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/
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
 
 <a id="types-aiobotocore-backup-gateway"></a>
 
 # types-aiobotocore-backup-gateway
 
 [![PyPI - types-aiobotocore-backup-gateway](https://img.shields.io/pypi/v/types-aiobotocore-backup-gateway.svg?color=blue)](https://pypi.org/project/types-aiobotocore-backup-gateway)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-backup-gateway.svg?color=blue)](https://pypi.org/project/types-aiobotocore-backup-gateway)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-backup-gateway)](https://pepy.tech/project/types-aiobotocore-backup-gateway)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.BackupGateway 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway)
+[aiobotocore.BackupGateway 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway)
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
 [types-aiobotocore-backup-gateway docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-backup-gateway-2.9.0/types_aiobotocore_backup_gateway.egg-info/SOURCES.txt` & `types-aiobotocore-backup-gateway-2.9.1/types_aiobotocore_backup_gateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

