# Comparing `tmp/types-aiobotocore-ds-2.9.0.tar.gz` & `tmp/types-aiobotocore-ds-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ds-2.9.0.tar", last modified: Wed Dec 13 19:59:09 2023, max compression
+gzip compressed data, was "types-aiobotocore-ds-2.9.1.tar", last modified: Thu Jan 18 01:20:34 2024, max compression
```

## Comparing `types-aiobotocore-ds-2.9.0.tar` & `types-aiobotocore-ds-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:09.077813 types-aiobotocore-ds-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:44:26.000000 types-aiobotocore-ds-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15016 2023-12-13 19:59:09.077813 types-aiobotocore-ds-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13459 2023-12-13 19:44:26.000000 types-aiobotocore-ds-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:09.077813 types-aiobotocore-ds-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2023-12-13 19:44:26.000000 types-aiobotocore-ds-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:09.073813 types-aiobotocore-ds-2.9.0/types_aiobotocore_ds/
--rw-r--r--   0 runner    (1001) docker     (127)     3710 2023-12-13 19:44:26.000000 types-aiobotocore-ds-2.9.0/types_aiobotocore_ds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3709 2023-12-13 19:44:26.000000 types-aiobotocore-ds-2.9.0/types_aiobotocore_ds/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      929 2023-12-13 19:44:26.000000 types-aiobotocore-ds-2.9.0/types_aiobotocore_ds/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    54677 2023-12-13 19:44:27.000000 types-aiobotocore-ds-2.9.0/types_aiobotocore_ds/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    54673 2023-12-13 19:44:26.000000 types-aiobotocore-ds-2.9.0/types_aiobotocore_ds/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14199 2023-12-13 19:44:27.000000 types-aiobotocore-ds-2.9.0/types_aiobotocore_ds/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    14197 2023-12-13 19:44:27.000000 types-aiobotocore-ds-2.9.0/types_aiobotocore_ds/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    17768 2023-12-13 19:44:27.000000 types-aiobotocore-ds-2.9.0/types_aiobotocore_ds/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    17751 2023-12-13 19:44:27.000000 types-aiobotocore-ds-2.9.0/types_aiobotocore_ds/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:44:26.000000 types-aiobotocore-ds-2.9.0/types_aiobotocore_ds/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    48469 2023-12-13 19:44:29.000000 types-aiobotocore-ds-2.9.0/types_aiobotocore_ds/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    48468 2023-12-13 19:44:27.000000 types-aiobotocore-ds-2.9.0/types_aiobotocore_ds/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:44:26.000000 types-aiobotocore-ds-2.9.0/types_aiobotocore_ds/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:09.077813 types-aiobotocore-ds-2.9.0/types_aiobotocore_ds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15016 2023-12-13 19:59:09.000000 types-aiobotocore-ds-2.9.0/types_aiobotocore_ds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      718 2023-12-13 19:59:09.000000 types-aiobotocore-ds-2.9.0/types_aiobotocore_ds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:09.000000 types-aiobotocore-ds-2.9.0/types_aiobotocore_ds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:09.000000 types-aiobotocore-ds-2.9.0/types_aiobotocore_ds.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:09.000000 types-aiobotocore-ds-2.9.0/types_aiobotocore_ds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-12-13 19:59:09.000000 types-aiobotocore-ds-2.9.0/types_aiobotocore_ds.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:34.301373 types-aiobotocore-ds-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:06:21.000000 types-aiobotocore-ds-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15036 2024-01-18 01:20:34.301373 types-aiobotocore-ds-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13459 2024-01-18 01:06:21.000000 types-aiobotocore-ds-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:34.301373 types-aiobotocore-ds-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-01-18 01:06:21.000000 types-aiobotocore-ds-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:34.297373 types-aiobotocore-ds-2.9.1/types_aiobotocore_ds/
+-rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-01-18 01:06:21.000000 types-aiobotocore-ds-2.9.1/types_aiobotocore_ds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-01-18 01:06:21.000000 types-aiobotocore-ds-2.9.1/types_aiobotocore_ds/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-01-18 01:06:21.000000 types-aiobotocore-ds-2.9.1/types_aiobotocore_ds/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54694 2024-01-18 01:06:21.000000 types-aiobotocore-ds-2.9.1/types_aiobotocore_ds/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54691 2024-01-18 01:06:21.000000 types-aiobotocore-ds-2.9.1/types_aiobotocore_ds/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14197 2024-01-18 01:06:22.000000 types-aiobotocore-ds-2.9.1/types_aiobotocore_ds/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14197 2024-01-18 01:06:22.000000 types-aiobotocore-ds-2.9.1/types_aiobotocore_ds/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    17774 2024-01-18 01:06:22.000000 types-aiobotocore-ds-2.9.1/types_aiobotocore_ds/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17759 2024-01-18 01:06:22.000000 types-aiobotocore-ds-2.9.1/types_aiobotocore_ds/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:06:21.000000 types-aiobotocore-ds-2.9.1/types_aiobotocore_ds/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    48468 2024-01-18 01:06:23.000000 types-aiobotocore-ds-2.9.1/types_aiobotocore_ds/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48468 2024-01-18 01:06:22.000000 types-aiobotocore-ds-2.9.1/types_aiobotocore_ds/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:06:21.000000 types-aiobotocore-ds-2.9.1/types_aiobotocore_ds/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:34.297373 types-aiobotocore-ds-2.9.1/types_aiobotocore_ds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15036 2024-01-18 01:20:34.000000 types-aiobotocore-ds-2.9.1/types_aiobotocore_ds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-01-18 01:20:34.000000 types-aiobotocore-ds-2.9.1/types_aiobotocore_ds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:34.000000 types-aiobotocore-ds-2.9.1/types_aiobotocore_ds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:34.000000 types-aiobotocore-ds-2.9.1/types_aiobotocore_ds.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:34.000000 types-aiobotocore-ds-2.9.1/types_aiobotocore_ds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-18 01:20:34.000000 types-aiobotocore-ds-2.9.1/types_aiobotocore_ds.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ds-2.9.0/LICENSE` & `types-aiobotocore-ds-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-ds-2.9.0/PKG-INFO` & `types-aiobotocore-ds-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ds
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.DirectoryService 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.DirectoryService 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/
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
 
 <a id="types-aiobotocore-ds"></a>
 
 # types-aiobotocore-ds
 
 [![PyPI - types-aiobotocore-ds](https://img.shields.io/pypi/v/types-aiobotocore-ds.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ds)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ds.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ds)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ds)](https://pepy.tech/project/types-aiobotocore-ds)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DirectoryService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService)
+[aiobotocore.DirectoryService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService)
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
 [types-aiobotocore-ds docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-ds-2.9.0/README.md` & `types-aiobotocore-ds-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ds.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ds)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ds)](https://pepy.tech/project/types-aiobotocore-ds)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DirectoryService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService)
+[aiobotocore.DirectoryService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService)
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
 [types-aiobotocore-ds docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-ds-2.9.0/setup.py` & `types-aiobotocore-ds-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ds",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_ds"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.DirectoryService 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.DirectoryService 2.9.1 service generated with"
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
     keywords="aiobotocore ds type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_ds": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-ds-2.9.0/types_aiobotocore_ds/__init__.py` & `types-aiobotocore-ds-2.9.1/types_aiobotocore_ds/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,14 @@
     ListLogSubscriptionsPaginator,
     ListSchemaExtensionsPaginator,
     ListTagsForResourcePaginator,
 )
 
 Client = DirectoryServiceClient
 
-
 __all__ = (
     "Client",
     "DescribeClientAuthenticationSettingsPaginator",
     "DescribeDirectoriesPaginator",
     "DescribeDomainControllersPaginator",
     "DescribeLDAPSSettingsPaginator",
     "DescribeRegionsPaginator",
```

### Comparing `types-aiobotocore-ds-2.9.0/types_aiobotocore_ds/__init__.pyi` & `types-aiobotocore-ds-2.9.1/types_aiobotocore_ds/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ds-2.9.0/types_aiobotocore_ds/__main__.py` & `types-aiobotocore-ds-2.9.1/types_aiobotocore_ds/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.DirectoryService 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.DirectoryService 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService\nOther"
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

### Comparing `types-aiobotocore-ds-2.9.0/types_aiobotocore_ds/client.py` & `types-aiobotocore-ds-2.9.1/types_aiobotocore_ds/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("DirectoryServiceClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -188,15 +187,15 @@
         """
 
     async def add_ip_routes(
         self,
         *,
         DirectoryId: str,
         IpRoutes: Sequence[IpRouteTypeDef],
-        UpdateSecurityGroupForDirectoryControllers: bool = ...
+        UpdateSecurityGroupForDirectoryControllers: bool = ...,
     ) -> Dict[str, Any]:
         """
         If the DNS server for your self-managed domain uses a publicly addressable IP
         address, you must add a CIDR address block to correctly route traffic to and
         from your Microsoft AD on Amazon Web
         Services.
 
@@ -255,15 +254,15 @@
         *,
         Name: str,
         Password: str,
         Size: DirectorySizeType,
         ConnectSettings: DirectoryConnectSettingsTypeDef,
         ShortName: str = ...,
         Description: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> ConnectDirectoryResultTypeDef:
         """
         Creates an AD Connector to connect to a self-managed directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.connect_directory)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#connect_directory)
         """
@@ -279,15 +278,15 @@
     async def create_computer(
         self,
         *,
         DirectoryId: str,
         ComputerName: str,
         Password: str,
         OrganizationalUnitDistinguishedName: str = ...,
-        ComputerAttributes: Sequence[AttributeTypeDef] = ...
+        ComputerAttributes: Sequence[AttributeTypeDef] = ...,
     ) -> CreateComputerResultTypeDef:
         """
         Creates an Active Directory computer object in the specified directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.create_computer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#create_computer)
         """
@@ -308,15 +307,15 @@
         *,
         Name: str,
         Password: str,
         Size: DirectorySizeType,
         ShortName: str = ...,
         Description: str = ...,
         VpcSettings: DirectoryVpcSettingsTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDirectoryResultTypeDef:
         """
         Creates a Simple AD directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.create_directory)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#create_directory)
         """
@@ -339,15 +338,15 @@
         *,
         Name: str,
         Password: str,
         VpcSettings: DirectoryVpcSettingsTypeDef,
         ShortName: str = ...,
         Description: str = ...,
         Edition: DirectoryEditionType = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateMicrosoftADResultTypeDef:
         """
         Creates a Microsoft AD directory in the Amazon Web Services Cloud.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.create_microsoft_ad)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#create_microsoft_ad)
         """
@@ -369,15 +368,15 @@
         *,
         DirectoryId: str,
         RemoteDomainName: str,
         TrustPassword: str,
         TrustDirection: TrustDirectionType,
         TrustType: TrustTypeType = ...,
         ConditionalForwarderIpAddrs: Sequence[str] = ...,
-        SelectiveAuth: SelectiveAuthType = ...
+        SelectiveAuth: SelectiveAuthType = ...,
     ) -> CreateTrustResultTypeDef:
         """
         Directory Service for Microsoft Active Directory allows you to configure trust
         relationships.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.create_trust)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#create_trust)
@@ -466,15 +465,15 @@
 
     async def describe_client_authentication_settings(
         self,
         *,
         DirectoryId: str,
         Type: ClientAuthenticationTypeType = ...,
         NextToken: str = ...,
-        Limit: int = ...
+        Limit: int = ...,
     ) -> DescribeClientAuthenticationSettingsResultTypeDef:
         """
         Retrieves information about the type of client authentication for the specified
         directory, if the type is
         specified.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.describe_client_authentication_settings)
@@ -503,15 +502,15 @@
 
     async def describe_domain_controllers(
         self,
         *,
         DirectoryId: str,
         DomainControllerIds: Sequence[str] = ...,
         NextToken: str = ...,
-        Limit: int = ...
+        Limit: int = ...,
     ) -> DescribeDomainControllersResultTypeDef:
         """
         Provides information about any domain controllers in your directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.describe_domain_controllers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#describe_domain_controllers)
         """
@@ -530,15 +529,15 @@
 
     async def describe_ldaps_settings(
         self,
         *,
         DirectoryId: str,
         Type: Literal["Client"] = ...,
         NextToken: str = ...,
-        Limit: int = ...
+        Limit: int = ...,
     ) -> DescribeLDAPSSettingsResultTypeDef:
         """
         Describes the status of LDAP security for the specified directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.describe_ldaps_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#describe_ldaps_settings)
         """
@@ -555,15 +554,15 @@
         """
 
     async def describe_settings(
         self,
         *,
         DirectoryId: str,
         Status: DirectoryConfigurationStatusType = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeSettingsResultTypeDef:
         """
         Retrieves information about the configurable settings for the specified
         directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.describe_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#describe_settings)
@@ -571,60 +570,60 @@
 
     async def describe_shared_directories(
         self,
         *,
         OwnerDirectoryId: str,
         SharedDirectoryIds: Sequence[str] = ...,
         NextToken: str = ...,
-        Limit: int = ...
+        Limit: int = ...,
     ) -> DescribeSharedDirectoriesResultTypeDef:
         """
         Returns the shared directories in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.describe_shared_directories)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#describe_shared_directories)
         """
 
     async def describe_snapshots(
         self,
         *,
         DirectoryId: str = ...,
         SnapshotIds: Sequence[str] = ...,
         NextToken: str = ...,
-        Limit: int = ...
+        Limit: int = ...,
     ) -> DescribeSnapshotsResultTypeDef:
         """
         Obtains information about the directory snapshots that belong to this account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.describe_snapshots)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#describe_snapshots)
         """
 
     async def describe_trusts(
         self,
         *,
         DirectoryId: str = ...,
         TrustIds: Sequence[str] = ...,
         NextToken: str = ...,
-        Limit: int = ...
+        Limit: int = ...,
     ) -> DescribeTrustsResultTypeDef:
         """
         Obtains information about the trust relationships for this account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.describe_trusts)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#describe_trusts)
         """
 
     async def describe_update_directory(
         self,
         *,
         DirectoryId: str,
         UpdateType: Literal["OS"],
         RegionName: str = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeUpdateDirectoryResultTypeDef:
         """
         Describes the updates of a directory for a particular update type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.describe_update_directory)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#describe_update_directory)
         """
@@ -791,15 +790,15 @@
 
     async def register_certificate(
         self,
         *,
         DirectoryId: str,
         CertificateData: str,
         Type: CertificateTypeType = ...,
-        ClientCertAuthSettings: ClientCertAuthSettingsTypeDef = ...
+        ClientCertAuthSettings: ClientCertAuthSettingsTypeDef = ...,
     ) -> RegisterCertificateResultTypeDef:
         """
         Registers a certificate for a secure LDAP or client certificate authentication.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.register_certificate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#register_certificate)
         """
@@ -871,15 +870,15 @@
 
     async def share_directory(
         self,
         *,
         DirectoryId: str,
         ShareTarget: ShareTargetTypeDef,
         ShareMethod: ShareMethodType,
-        ShareNotes: str = ...
+        ShareNotes: str = ...,
     ) -> ShareDirectoryResultTypeDef:
         """
         Shares a specified directory ( `DirectoryId`) in your Amazon Web Services
         account (directory owner) with another Amazon Web Services account (directory
         consumer).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.share_directory)
@@ -888,15 +887,15 @@
 
     async def start_schema_extension(
         self,
         *,
         DirectoryId: str,
         CreateSnapshotBeforeSchemaExtension: bool,
         LdifContent: str,
-        Description: str
+        Description: str,
     ) -> StartSchemaExtensionResultTypeDef:
         """
         Applies a schema extension to a Microsoft AD directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.start_schema_extension)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#start_schema_extension)
         """
@@ -925,15 +924,15 @@
 
     async def update_directory_setup(
         self,
         *,
         DirectoryId: str,
         UpdateType: Literal["OS"],
         OSUpdateSettings: OSUpdateSettingsTypeDef = ...,
-        CreateSnapshotBeforeUpdate: bool = ...
+        CreateSnapshotBeforeUpdate: bool = ...,
     ) -> Dict[str, Any]:
         """
         Updates the directory for a particular update type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.update_directory_setup)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#update_directory_setup)
         """
```

### Comparing `types-aiobotocore-ds-2.9.0/types_aiobotocore_ds/client.pyi` & `types-aiobotocore-ds-2.9.1/types_aiobotocore_ds/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -184,15 +184,15 @@
         """
 
     async def add_ip_routes(
         self,
         *,
         DirectoryId: str,
         IpRoutes: Sequence[IpRouteTypeDef],
-        UpdateSecurityGroupForDirectoryControllers: bool = ...
+        UpdateSecurityGroupForDirectoryControllers: bool = ...,
     ) -> Dict[str, Any]:
         """
         If the DNS server for your self-managed domain uses a publicly addressable IP
         address, you must add a CIDR address block to correctly route traffic to and
         from your Microsoft AD on Amazon Web
         Services.
 
@@ -251,15 +251,15 @@
         *,
         Name: str,
         Password: str,
         Size: DirectorySizeType,
         ConnectSettings: DirectoryConnectSettingsTypeDef,
         ShortName: str = ...,
         Description: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> ConnectDirectoryResultTypeDef:
         """
         Creates an AD Connector to connect to a self-managed directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.connect_directory)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#connect_directory)
         """
@@ -275,15 +275,15 @@
     async def create_computer(
         self,
         *,
         DirectoryId: str,
         ComputerName: str,
         Password: str,
         OrganizationalUnitDistinguishedName: str = ...,
-        ComputerAttributes: Sequence[AttributeTypeDef] = ...
+        ComputerAttributes: Sequence[AttributeTypeDef] = ...,
     ) -> CreateComputerResultTypeDef:
         """
         Creates an Active Directory computer object in the specified directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.create_computer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#create_computer)
         """
@@ -304,15 +304,15 @@
         *,
         Name: str,
         Password: str,
         Size: DirectorySizeType,
         ShortName: str = ...,
         Description: str = ...,
         VpcSettings: DirectoryVpcSettingsTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDirectoryResultTypeDef:
         """
         Creates a Simple AD directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.create_directory)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#create_directory)
         """
@@ -335,15 +335,15 @@
         *,
         Name: str,
         Password: str,
         VpcSettings: DirectoryVpcSettingsTypeDef,
         ShortName: str = ...,
         Description: str = ...,
         Edition: DirectoryEditionType = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateMicrosoftADResultTypeDef:
         """
         Creates a Microsoft AD directory in the Amazon Web Services Cloud.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.create_microsoft_ad)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#create_microsoft_ad)
         """
@@ -365,15 +365,15 @@
         *,
         DirectoryId: str,
         RemoteDomainName: str,
         TrustPassword: str,
         TrustDirection: TrustDirectionType,
         TrustType: TrustTypeType = ...,
         ConditionalForwarderIpAddrs: Sequence[str] = ...,
-        SelectiveAuth: SelectiveAuthType = ...
+        SelectiveAuth: SelectiveAuthType = ...,
     ) -> CreateTrustResultTypeDef:
         """
         Directory Service for Microsoft Active Directory allows you to configure trust
         relationships.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.create_trust)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#create_trust)
@@ -462,15 +462,15 @@
 
     async def describe_client_authentication_settings(
         self,
         *,
         DirectoryId: str,
         Type: ClientAuthenticationTypeType = ...,
         NextToken: str = ...,
-        Limit: int = ...
+        Limit: int = ...,
     ) -> DescribeClientAuthenticationSettingsResultTypeDef:
         """
         Retrieves information about the type of client authentication for the specified
         directory, if the type is
         specified.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.describe_client_authentication_settings)
@@ -499,15 +499,15 @@
 
     async def describe_domain_controllers(
         self,
         *,
         DirectoryId: str,
         DomainControllerIds: Sequence[str] = ...,
         NextToken: str = ...,
-        Limit: int = ...
+        Limit: int = ...,
     ) -> DescribeDomainControllersResultTypeDef:
         """
         Provides information about any domain controllers in your directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.describe_domain_controllers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#describe_domain_controllers)
         """
@@ -526,15 +526,15 @@
 
     async def describe_ldaps_settings(
         self,
         *,
         DirectoryId: str,
         Type: Literal["Client"] = ...,
         NextToken: str = ...,
-        Limit: int = ...
+        Limit: int = ...,
     ) -> DescribeLDAPSSettingsResultTypeDef:
         """
         Describes the status of LDAP security for the specified directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.describe_ldaps_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#describe_ldaps_settings)
         """
@@ -551,15 +551,15 @@
         """
 
     async def describe_settings(
         self,
         *,
         DirectoryId: str,
         Status: DirectoryConfigurationStatusType = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeSettingsResultTypeDef:
         """
         Retrieves information about the configurable settings for the specified
         directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.describe_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#describe_settings)
@@ -567,60 +567,60 @@
 
     async def describe_shared_directories(
         self,
         *,
         OwnerDirectoryId: str,
         SharedDirectoryIds: Sequence[str] = ...,
         NextToken: str = ...,
-        Limit: int = ...
+        Limit: int = ...,
     ) -> DescribeSharedDirectoriesResultTypeDef:
         """
         Returns the shared directories in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.describe_shared_directories)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#describe_shared_directories)
         """
 
     async def describe_snapshots(
         self,
         *,
         DirectoryId: str = ...,
         SnapshotIds: Sequence[str] = ...,
         NextToken: str = ...,
-        Limit: int = ...
+        Limit: int = ...,
     ) -> DescribeSnapshotsResultTypeDef:
         """
         Obtains information about the directory snapshots that belong to this account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.describe_snapshots)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#describe_snapshots)
         """
 
     async def describe_trusts(
         self,
         *,
         DirectoryId: str = ...,
         TrustIds: Sequence[str] = ...,
         NextToken: str = ...,
-        Limit: int = ...
+        Limit: int = ...,
     ) -> DescribeTrustsResultTypeDef:
         """
         Obtains information about the trust relationships for this account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.describe_trusts)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#describe_trusts)
         """
 
     async def describe_update_directory(
         self,
         *,
         DirectoryId: str,
         UpdateType: Literal["OS"],
         RegionName: str = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeUpdateDirectoryResultTypeDef:
         """
         Describes the updates of a directory for a particular update type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.describe_update_directory)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#describe_update_directory)
         """
@@ -787,15 +787,15 @@
 
     async def register_certificate(
         self,
         *,
         DirectoryId: str,
         CertificateData: str,
         Type: CertificateTypeType = ...,
-        ClientCertAuthSettings: ClientCertAuthSettingsTypeDef = ...
+        ClientCertAuthSettings: ClientCertAuthSettingsTypeDef = ...,
     ) -> RegisterCertificateResultTypeDef:
         """
         Registers a certificate for a secure LDAP or client certificate authentication.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.register_certificate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#register_certificate)
         """
@@ -867,15 +867,15 @@
 
     async def share_directory(
         self,
         *,
         DirectoryId: str,
         ShareTarget: ShareTargetTypeDef,
         ShareMethod: ShareMethodType,
-        ShareNotes: str = ...
+        ShareNotes: str = ...,
     ) -> ShareDirectoryResultTypeDef:
         """
         Shares a specified directory ( `DirectoryId`) in your Amazon Web Services
         account (directory owner) with another Amazon Web Services account (directory
         consumer).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.share_directory)
@@ -884,15 +884,15 @@
 
     async def start_schema_extension(
         self,
         *,
         DirectoryId: str,
         CreateSnapshotBeforeSchemaExtension: bool,
         LdifContent: str,
-        Description: str
+        Description: str,
     ) -> StartSchemaExtensionResultTypeDef:
         """
         Applies a schema extension to a Microsoft AD directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.start_schema_extension)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#start_schema_extension)
         """
@@ -921,15 +921,15 @@
 
     async def update_directory_setup(
         self,
         *,
         DirectoryId: str,
         UpdateType: Literal["OS"],
         OSUpdateSettings: OSUpdateSettingsTypeDef = ...,
-        CreateSnapshotBeforeUpdate: bool = ...
+        CreateSnapshotBeforeUpdate: bool = ...,
     ) -> Dict[str, Any]:
         """
         Updates the directory for a particular update type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.update_directory_setup)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#update_directory_setup)
         """
```

### Comparing `types-aiobotocore-ds-2.9.0/types_aiobotocore_ds/literals.py` & `types-aiobotocore-ds-2.9.1/types_aiobotocore_ds/literals.py`

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
     "CertificateStateType",
     "CertificateTypeType",
     "ClientAuthenticationStatusType",
     "ClientAuthenticationTypeType",
     "DescribeClientAuthenticationSettingsPaginatorName",
     "DescribeDirectoriesPaginatorName",
@@ -69,15 +68,14 @@
     "DirectoryServiceServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 CertificateStateType = Literal[
     "DeregisterFailed",
     "Deregistered",
     "Deregistering",
     "RegisterFailed",
     "Registered",
     "Registering",
```

### Comparing `types-aiobotocore-ds-2.9.0/types_aiobotocore_ds/literals.pyi` & `types-aiobotocore-ds-2.9.1/types_aiobotocore_ds/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ds-2.9.0/types_aiobotocore_ds/paginator.py` & `types-aiobotocore-ds-2.9.1/types_aiobotocore_ds/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,15 +73,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "DescribeClientAuthenticationSettingsPaginator",
     "DescribeDirectoriesPaginator",
     "DescribeDomainControllersPaginator",
     "DescribeLDAPSSettingsPaginator",
     "DescribeRegionsPaginator",
     "DescribeSharedDirectoriesPaginator",
@@ -91,15 +90,14 @@
     "ListCertificatesPaginator",
     "ListIpRoutesPaginator",
     "ListLogSubscriptionsPaginator",
     "ListSchemaExtensionsPaginator",
     "ListTagsForResourcePaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -113,15 +111,15 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryId: str,
         Type: ClientAuthenticationTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeClientAuthenticationSettingsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeClientAuthenticationSettings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#describeclientauthenticationsettingspaginator)
         """
 
 
@@ -147,15 +145,15 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryId: str,
         DomainControllerIds: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeDomainControllersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeDomainControllers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#describedomaincontrollerspaginator)
         """
 
 
@@ -166,15 +164,15 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryId: str,
         Type: Literal["Client"] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeLDAPSSettingsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeLDAPSSettings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#describeldapssettingspaginator)
         """
 
 
@@ -185,15 +183,15 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryId: str,
         RegionName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeRegionsResultPaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeRegions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#describeregionspaginator)
         """
 
 
@@ -204,15 +202,15 @@
     """
 
     def paginate(
         self,
         *,
         OwnerDirectoryId: str,
         SharedDirectoryIds: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeSharedDirectoriesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeSharedDirectories.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#describeshareddirectoriespaginator)
         """
 
 
@@ -223,15 +221,15 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryId: str = ...,
         SnapshotIds: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeSnapshotsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeSnapshots.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#describesnapshotspaginator)
         """
 
 
@@ -242,15 +240,15 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryId: str = ...,
         TrustIds: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeTrustsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeTrusts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#describetrustspaginator)
         """
 
 
@@ -262,15 +260,15 @@
 
     def paginate(
         self,
         *,
         DirectoryId: str,
         UpdateType: Literal["OS"],
         RegionName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeUpdateDirectoryResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeUpdateDirectory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#describeupdatedirectorypaginator)
         """
```

### Comparing `types-aiobotocore-ds-2.9.0/types_aiobotocore_ds/paginator.pyi` & `types-aiobotocore-ds-2.9.1/types_aiobotocore_ds/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryId: str,
         Type: ClientAuthenticationTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeClientAuthenticationSettingsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeClientAuthenticationSettings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#describeclientauthenticationsettingspaginator)
         """
 
 class DescribeDirectoriesPaginator(AioPaginator):
@@ -141,15 +141,15 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryId: str,
         DomainControllerIds: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeDomainControllersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeDomainControllers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#describedomaincontrollerspaginator)
         """
 
 class DescribeLDAPSSettingsPaginator(AioPaginator):
@@ -159,15 +159,15 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryId: str,
         Type: Literal["Client"] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeLDAPSSettingsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeLDAPSSettings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#describeldapssettingspaginator)
         """
 
 class DescribeRegionsPaginator(AioPaginator):
@@ -177,15 +177,15 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryId: str,
         RegionName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeRegionsResultPaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeRegions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#describeregionspaginator)
         """
 
 class DescribeSharedDirectoriesPaginator(AioPaginator):
@@ -195,15 +195,15 @@
     """
 
     def paginate(
         self,
         *,
         OwnerDirectoryId: str,
         SharedDirectoryIds: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeSharedDirectoriesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeSharedDirectories.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#describeshareddirectoriespaginator)
         """
 
 class DescribeSnapshotsPaginator(AioPaginator):
@@ -213,15 +213,15 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryId: str = ...,
         SnapshotIds: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeSnapshotsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeSnapshots.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#describesnapshotspaginator)
         """
 
 class DescribeTrustsPaginator(AioPaginator):
@@ -231,15 +231,15 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryId: str = ...,
         TrustIds: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeTrustsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeTrusts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#describetrustspaginator)
         """
 
 class DescribeUpdateDirectoryPaginator(AioPaginator):
@@ -250,15 +250,15 @@
 
     def paginate(
         self,
         *,
         DirectoryId: str,
         UpdateType: Literal["OS"],
         RegionName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeUpdateDirectoryResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeUpdateDirectory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#describeupdatedirectorypaginator)
         """
 
 class ListCertificatesPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-ds-2.9.0/types_aiobotocore_ds/type_defs.py` & `types-aiobotocore-ds-2.9.1/types_aiobotocore_ds/type_defs.py`

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
     "AcceptSharedDirectoryRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "SharedDirectoryTypeDef",
     "IpRouteTypeDef",
     "DirectoryVpcSettingsTypeDef",
     "TagTypeDef",
```

### Comparing `types-aiobotocore-ds-2.9.0/types_aiobotocore_ds/type_defs.pyi` & `types-aiobotocore-ds-2.9.1/types_aiobotocore_ds/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ds-2.9.0/types_aiobotocore_ds.egg-info/PKG-INFO` & `types-aiobotocore-ds-2.9.1/types_aiobotocore_ds.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ds
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.DirectoryService 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.DirectoryService 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/
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
 
 <a id="types-aiobotocore-ds"></a>
 
 # types-aiobotocore-ds
 
 [![PyPI - types-aiobotocore-ds](https://img.shields.io/pypi/v/types-aiobotocore-ds.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ds)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ds.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ds)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ds)](https://pepy.tech/project/types-aiobotocore-ds)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DirectoryService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService)
+[aiobotocore.DirectoryService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService)
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
 [types-aiobotocore-ds docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-ds-2.9.0/types_aiobotocore_ds.egg-info/SOURCES.txt` & `types-aiobotocore-ds-2.9.1/types_aiobotocore_ds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

