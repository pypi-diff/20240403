# Comparing `tmp/types-aiobotocore-opensearch-2.9.0.tar.gz` & `tmp/types-aiobotocore-opensearch-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-opensearch-2.9.0.tar", last modified: Wed Dec 13 20:00:03 2023, max compression
+gzip compressed data, was "types-aiobotocore-opensearch-2.9.1.tar", last modified: Thu Jan 18 01:21:24 2024, max compression
```

## Comparing `types-aiobotocore-opensearch-2.9.0.tar` & `types-aiobotocore-opensearch-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:03.285373 types-aiobotocore-opensearch-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:51:08.000000 types-aiobotocore-opensearch-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12463 2023-12-13 20:00:03.285373 types-aiobotocore-opensearch-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10881 2023-12-13 19:51:08.000000 types-aiobotocore-opensearch-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:03.289373 types-aiobotocore-opensearch-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2023-12-13 19:51:08.000000 types-aiobotocore-opensearch-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:03.285373 types-aiobotocore-opensearch-2.9.0/types_aiobotocore_opensearch/
--rw-r--r--   0 runner    (1001) docker     (127)      502 2023-12-13 19:51:08.000000 types-aiobotocore-opensearch-2.9.0/types_aiobotocore_opensearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2023-12-13 19:51:08.000000 types-aiobotocore-opensearch-2.9.0/types_aiobotocore_opensearch/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      958 2023-12-13 19:51:08.000000 types-aiobotocore-opensearch-2.9.0/types_aiobotocore_opensearch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    48554 2023-12-13 19:51:08.000000 types-aiobotocore-opensearch-2.9.0/types_aiobotocore_opensearch/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    48551 2023-12-13 19:51:08.000000 types-aiobotocore-opensearch-2.9.0/types_aiobotocore_opensearch/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    16308 2023-12-13 19:51:08.000000 types-aiobotocore-opensearch-2.9.0/types_aiobotocore_opensearch/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    16306 2023-12-13 19:51:08.000000 types-aiobotocore-opensearch-2.9.0/types_aiobotocore_opensearch/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:51:08.000000 types-aiobotocore-opensearch-2.9.0/types_aiobotocore_opensearch/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    68938 2023-12-13 19:51:10.000000 types-aiobotocore-opensearch-2.9.0/types_aiobotocore_opensearch/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    68937 2023-12-13 19:51:09.000000 types-aiobotocore-opensearch-2.9.0/types_aiobotocore_opensearch/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:51:08.000000 types-aiobotocore-opensearch-2.9.0/types_aiobotocore_opensearch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:03.285373 types-aiobotocore-opensearch-2.9.0/types_aiobotocore_opensearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12463 2023-12-13 20:00:03.000000 types-aiobotocore-opensearch-2.9.0/types_aiobotocore_opensearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      785 2023-12-13 20:00:03.000000 types-aiobotocore-opensearch-2.9.0/types_aiobotocore_opensearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:03.000000 types-aiobotocore-opensearch-2.9.0/types_aiobotocore_opensearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:03.000000 types-aiobotocore-opensearch-2.9.0/types_aiobotocore_opensearch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:03.000000 types-aiobotocore-opensearch-2.9.0/types_aiobotocore_opensearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-13 20:00:03.000000 types-aiobotocore-opensearch-2.9.0/types_aiobotocore_opensearch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:24.277144 types-aiobotocore-opensearch-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:12:47.000000 types-aiobotocore-opensearch-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12483 2024-01-18 01:21:24.277144 types-aiobotocore-opensearch-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10881 2024-01-18 01:12:47.000000 types-aiobotocore-opensearch-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:24.277144 types-aiobotocore-opensearch-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-01-18 01:12:47.000000 types-aiobotocore-opensearch-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:24.277144 types-aiobotocore-opensearch-2.9.1/types_aiobotocore_opensearch/
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-01-18 01:12:47.000000 types-aiobotocore-opensearch-2.9.1/types_aiobotocore_opensearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-01-18 01:12:47.000000 types-aiobotocore-opensearch-2.9.1/types_aiobotocore_opensearch/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-01-18 01:12:47.000000 types-aiobotocore-opensearch-2.9.1/types_aiobotocore_opensearch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48567 2024-01-18 01:12:47.000000 types-aiobotocore-opensearch-2.9.1/types_aiobotocore_opensearch/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48564 2024-01-18 01:12:47.000000 types-aiobotocore-opensearch-2.9.1/types_aiobotocore_opensearch/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    16306 2024-01-18 01:12:50.000000 types-aiobotocore-opensearch-2.9.1/types_aiobotocore_opensearch/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16306 2024-01-18 01:12:48.000000 types-aiobotocore-opensearch-2.9.1/types_aiobotocore_opensearch/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:12:47.000000 types-aiobotocore-opensearch-2.9.1/types_aiobotocore_opensearch/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    68937 2024-01-18 01:12:51.000000 types-aiobotocore-opensearch-2.9.1/types_aiobotocore_opensearch/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68937 2024-01-18 01:12:51.000000 types-aiobotocore-opensearch-2.9.1/types_aiobotocore_opensearch/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:12:47.000000 types-aiobotocore-opensearch-2.9.1/types_aiobotocore_opensearch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:24.277144 types-aiobotocore-opensearch-2.9.1/types_aiobotocore_opensearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12483 2024-01-18 01:21:24.000000 types-aiobotocore-opensearch-2.9.1/types_aiobotocore_opensearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-01-18 01:21:24.000000 types-aiobotocore-opensearch-2.9.1/types_aiobotocore_opensearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:24.000000 types-aiobotocore-opensearch-2.9.1/types_aiobotocore_opensearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:24.000000 types-aiobotocore-opensearch-2.9.1/types_aiobotocore_opensearch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:24.000000 types-aiobotocore-opensearch-2.9.1/types_aiobotocore_opensearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-01-18 01:21:24.000000 types-aiobotocore-opensearch-2.9.1/types_aiobotocore_opensearch.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-opensearch-2.9.0/LICENSE` & `types-aiobotocore-opensearch-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-opensearch-2.9.0/PKG-INFO` & `types-aiobotocore-opensearch-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-opensearch
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.OpenSearchService 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.OpenSearchService 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearch/
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
 
 <a id="types-aiobotocore-opensearch"></a>
 
 # types-aiobotocore-opensearch
 
 [![PyPI - types-aiobotocore-opensearch](https://img.shields.io/pypi/v/types-aiobotocore-opensearch.svg?color=blue)](https://pypi.org/project/types-aiobotocore-opensearch)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-opensearch.svg?color=blue)](https://pypi.org/project/types-aiobotocore-opensearch)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearch/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-opensearch)](https://pepy.tech/project/types-aiobotocore-opensearch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.OpenSearchService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService)
+[aiobotocore.OpenSearchService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService)
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
 [types-aiobotocore-opensearch docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearch/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-opensearch-2.9.0/README.md` & `types-aiobotocore-opensearch-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-opensearch.svg?color=blue)](https://pypi.org/project/types-aiobotocore-opensearch)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearch/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-opensearch)](https://pepy.tech/project/types-aiobotocore-opensearch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.OpenSearchService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService)
+[aiobotocore.OpenSearchService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService)
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
 [types-aiobotocore-opensearch docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearch/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-opensearch-2.9.0/setup.py` & `types-aiobotocore-opensearch-2.9.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-opensearch",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_opensearch"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.OpenSearchService 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.OpenSearchService 2.9.1 service generated with"
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
     keywords="aiobotocore opensearch type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_opensearch": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearch/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-opensearch-2.9.0/types_aiobotocore_opensearch/__main__.py` & `types-aiobotocore-opensearch-2.9.1/types_aiobotocore_opensearch/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.OpenSearchService 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.OpenSearchService 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearch//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService\nOther"
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

### Comparing `types-aiobotocore-opensearch-2.9.0/types_aiobotocore_opensearch/client.py` & `types-aiobotocore-opensearch-2.9.1/types_aiobotocore_opensearch/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,15 +176,15 @@
 
     async def add_data_source(
         self,
         *,
         DomainName: str,
         Name: str,
         DataSourceType: DataSourceTypeTypeDef,
-        Description: str = ...
+        Description: str = ...,
     ) -> AddDataSourceResponseTypeDef:
         """
         Adds the data source on the domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.add_data_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearch/client/#add_data_source)
         """
@@ -265,15 +265,15 @@
         AdvancedOptions: Mapping[str, str] = ...,
         LogPublishingOptions: Mapping[LogTypeType, LogPublishingOptionTypeDef] = ...,
         DomainEndpointOptions: DomainEndpointOptionsTypeDef = ...,
         AdvancedSecurityOptions: AdvancedSecurityOptionsInputTypeDef = ...,
         TagList: Sequence[TagTypeDef] = ...,
         AutoTuneOptions: AutoTuneOptionsInputTypeDef = ...,
         OffPeakWindowOptions: OffPeakWindowOptionsTypeDef = ...,
-        SoftwareUpdateOptions: SoftwareUpdateOptionsTypeDef = ...
+        SoftwareUpdateOptions: SoftwareUpdateOptionsTypeDef = ...,
     ) -> CreateDomainResponseTypeDef:
         """
         Creates an Amazon OpenSearch Service domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.create_domain)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearch/client/#create_domain)
         """
@@ -281,15 +281,15 @@
     async def create_outbound_connection(
         self,
         *,
         LocalDomainInfo: DomainInformationContainerTypeDef,
         RemoteDomainInfo: DomainInformationContainerTypeDef,
         ConnectionAlias: str,
         ConnectionMode: ConnectionModeType = ...,
-        ConnectionProperties: ConnectionPropertiesTypeDef = ...
+        ConnectionProperties: ConnectionPropertiesTypeDef = ...,
     ) -> CreateOutboundConnectionResponseTypeDef:
         """
         Creates a new cross-cluster search connection from a source Amazon OpenSearch
         Service domain to a destination
         domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.create_outbound_connection)
@@ -298,15 +298,15 @@
 
     async def create_package(
         self,
         *,
         PackageName: str,
         PackageType: PackageTypeType,
         PackageSource: PackageSourceTypeDef,
-        PackageDescription: str = ...
+        PackageDescription: str = ...,
     ) -> CreatePackageResponseTypeDef:
         """
         Creates a package for use with Amazon OpenSearch Service domains.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.create_package)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearch/client/#create_package)
         """
@@ -483,15 +483,15 @@
         """
 
     async def describe_instance_type_limits(
         self,
         *,
         InstanceType: OpenSearchPartitionInstanceTypeType,
         EngineVersion: str,
-        DomainName: str = ...
+        DomainName: str = ...,
     ) -> DescribeInstanceTypeLimitsResponseTypeDef:
         """
         Describes the instance count, storage, and master node limits for a given
         OpenSearch or Elasticsearch version and instance
         type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.describe_instance_type_limits)
@@ -511,15 +511,15 @@
         """
 
     async def describe_packages(
         self,
         *,
         Filters: Sequence[DescribePackagesFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribePackagesResponseTypeDef:
         """
         Describes all packages available to OpenSearch Service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.describe_packages)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearch/client/#describe_packages)
         """
@@ -658,15 +658,15 @@
     async def list_domain_maintenances(
         self,
         *,
         DomainName: str,
         Action: MaintenanceTypeType = ...,
         Status: MaintenanceStatusType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListDomainMaintenancesResponseTypeDef:
         """
         A list of maintenance actions for the domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.list_domain_maintenances)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearch/client/#list_domain_maintenances)
         """
@@ -697,15 +697,15 @@
         self,
         *,
         EngineVersion: str,
         DomainName: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         RetrieveAZs: bool = ...,
-        InstanceType: str = ...
+        InstanceType: str = ...,
     ) -> ListInstanceTypeDetailsResponseTypeDef:
         """
         Lists all instance types and available features for a given OpenSearch or
         Elasticsearch
         version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.list_instance_type_details)
@@ -851,15 +851,15 @@
 
     async def update_data_source(
         self,
         *,
         DomainName: str,
         Name: str,
         DataSourceType: DataSourceTypeTypeDef,
-        Description: str = ...
+        Description: str = ...,
     ) -> UpdateDataSourceResponseTypeDef:
         """
         Updates the data source on the domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.update_data_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearch/client/#update_data_source)
         """
@@ -881,15 +881,15 @@
         DomainEndpointOptions: DomainEndpointOptionsTypeDef = ...,
         NodeToNodeEncryptionOptions: NodeToNodeEncryptionOptionsTypeDef = ...,
         AdvancedSecurityOptions: AdvancedSecurityOptionsInputTypeDef = ...,
         AutoTuneOptions: AutoTuneOptionsTypeDef = ...,
         DryRun: bool = ...,
         DryRunMode: DryRunModeType = ...,
         OffPeakWindowOptions: OffPeakWindowOptionsTypeDef = ...,
-        SoftwareUpdateOptions: SoftwareUpdateOptionsTypeDef = ...
+        SoftwareUpdateOptions: SoftwareUpdateOptionsTypeDef = ...,
     ) -> UpdateDomainConfigResponseTypeDef:
         """
         Modifies the cluster configuration of the specified Amazon OpenSearch Service
         domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.update_domain_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearch/client/#update_domain_config)
@@ -897,15 +897,15 @@
 
     async def update_package(
         self,
         *,
         PackageID: str,
         PackageSource: PackageSourceTypeDef,
         PackageDescription: str = ...,
-        CommitMessage: str = ...
+        CommitMessage: str = ...,
     ) -> UpdatePackageResponseTypeDef:
         """
         Updates a package for use with Amazon OpenSearch Service domains.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.update_package)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearch/client/#update_package)
         """
@@ -913,15 +913,15 @@
     async def update_scheduled_action(
         self,
         *,
         DomainName: str,
         ActionID: str,
         ActionType: ActionTypeType,
         ScheduleAt: ScheduleAtType,
-        DesiredStartTime: int = ...
+        DesiredStartTime: int = ...,
     ) -> UpdateScheduledActionResponseTypeDef:
         """
         Reschedules a planned domain configuration change for a later time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.update_scheduled_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearch/client/#update_scheduled_action)
         """
@@ -938,15 +938,15 @@
 
     async def upgrade_domain(
         self,
         *,
         DomainName: str,
         TargetVersion: str,
         PerformCheckOnly: bool = ...,
-        AdvancedOptions: Mapping[str, str] = ...
+        AdvancedOptions: Mapping[str, str] = ...,
     ) -> UpgradeDomainResponseTypeDef:
         """
         Allows you to either upgrade your Amazon OpenSearch Service domain or perform
         an upgrade eligibility check to a compatible version of OpenSearch or
         Elasticsearch.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.upgrade_domain)
```

### Comparing `types-aiobotocore-opensearch-2.9.0/types_aiobotocore_opensearch/client.pyi` & `types-aiobotocore-opensearch-2.9.1/types_aiobotocore_opensearch/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,15 @@
 
     async def add_data_source(
         self,
         *,
         DomainName: str,
         Name: str,
         DataSourceType: DataSourceTypeTypeDef,
-        Description: str = ...
+        Description: str = ...,
     ) -> AddDataSourceResponseTypeDef:
         """
         Adds the data source on the domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.add_data_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearch/client/#add_data_source)
         """
@@ -262,15 +262,15 @@
         AdvancedOptions: Mapping[str, str] = ...,
         LogPublishingOptions: Mapping[LogTypeType, LogPublishingOptionTypeDef] = ...,
         DomainEndpointOptions: DomainEndpointOptionsTypeDef = ...,
         AdvancedSecurityOptions: AdvancedSecurityOptionsInputTypeDef = ...,
         TagList: Sequence[TagTypeDef] = ...,
         AutoTuneOptions: AutoTuneOptionsInputTypeDef = ...,
         OffPeakWindowOptions: OffPeakWindowOptionsTypeDef = ...,
-        SoftwareUpdateOptions: SoftwareUpdateOptionsTypeDef = ...
+        SoftwareUpdateOptions: SoftwareUpdateOptionsTypeDef = ...,
     ) -> CreateDomainResponseTypeDef:
         """
         Creates an Amazon OpenSearch Service domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.create_domain)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearch/client/#create_domain)
         """
@@ -278,15 +278,15 @@
     async def create_outbound_connection(
         self,
         *,
         LocalDomainInfo: DomainInformationContainerTypeDef,
         RemoteDomainInfo: DomainInformationContainerTypeDef,
         ConnectionAlias: str,
         ConnectionMode: ConnectionModeType = ...,
-        ConnectionProperties: ConnectionPropertiesTypeDef = ...
+        ConnectionProperties: ConnectionPropertiesTypeDef = ...,
     ) -> CreateOutboundConnectionResponseTypeDef:
         """
         Creates a new cross-cluster search connection from a source Amazon OpenSearch
         Service domain to a destination
         domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.create_outbound_connection)
@@ -295,15 +295,15 @@
 
     async def create_package(
         self,
         *,
         PackageName: str,
         PackageType: PackageTypeType,
         PackageSource: PackageSourceTypeDef,
-        PackageDescription: str = ...
+        PackageDescription: str = ...,
     ) -> CreatePackageResponseTypeDef:
         """
         Creates a package for use with Amazon OpenSearch Service domains.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.create_package)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearch/client/#create_package)
         """
@@ -480,15 +480,15 @@
         """
 
     async def describe_instance_type_limits(
         self,
         *,
         InstanceType: OpenSearchPartitionInstanceTypeType,
         EngineVersion: str,
-        DomainName: str = ...
+        DomainName: str = ...,
     ) -> DescribeInstanceTypeLimitsResponseTypeDef:
         """
         Describes the instance count, storage, and master node limits for a given
         OpenSearch or Elasticsearch version and instance
         type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.describe_instance_type_limits)
@@ -508,15 +508,15 @@
         """
 
     async def describe_packages(
         self,
         *,
         Filters: Sequence[DescribePackagesFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribePackagesResponseTypeDef:
         """
         Describes all packages available to OpenSearch Service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.describe_packages)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearch/client/#describe_packages)
         """
@@ -655,15 +655,15 @@
     async def list_domain_maintenances(
         self,
         *,
         DomainName: str,
         Action: MaintenanceTypeType = ...,
         Status: MaintenanceStatusType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListDomainMaintenancesResponseTypeDef:
         """
         A list of maintenance actions for the domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.list_domain_maintenances)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearch/client/#list_domain_maintenances)
         """
@@ -694,15 +694,15 @@
         self,
         *,
         EngineVersion: str,
         DomainName: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         RetrieveAZs: bool = ...,
-        InstanceType: str = ...
+        InstanceType: str = ...,
     ) -> ListInstanceTypeDetailsResponseTypeDef:
         """
         Lists all instance types and available features for a given OpenSearch or
         Elasticsearch
         version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.list_instance_type_details)
@@ -848,15 +848,15 @@
 
     async def update_data_source(
         self,
         *,
         DomainName: str,
         Name: str,
         DataSourceType: DataSourceTypeTypeDef,
-        Description: str = ...
+        Description: str = ...,
     ) -> UpdateDataSourceResponseTypeDef:
         """
         Updates the data source on the domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.update_data_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearch/client/#update_data_source)
         """
@@ -878,15 +878,15 @@
         DomainEndpointOptions: DomainEndpointOptionsTypeDef = ...,
         NodeToNodeEncryptionOptions: NodeToNodeEncryptionOptionsTypeDef = ...,
         AdvancedSecurityOptions: AdvancedSecurityOptionsInputTypeDef = ...,
         AutoTuneOptions: AutoTuneOptionsTypeDef = ...,
         DryRun: bool = ...,
         DryRunMode: DryRunModeType = ...,
         OffPeakWindowOptions: OffPeakWindowOptionsTypeDef = ...,
-        SoftwareUpdateOptions: SoftwareUpdateOptionsTypeDef = ...
+        SoftwareUpdateOptions: SoftwareUpdateOptionsTypeDef = ...,
     ) -> UpdateDomainConfigResponseTypeDef:
         """
         Modifies the cluster configuration of the specified Amazon OpenSearch Service
         domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.update_domain_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearch/client/#update_domain_config)
@@ -894,15 +894,15 @@
 
     async def update_package(
         self,
         *,
         PackageID: str,
         PackageSource: PackageSourceTypeDef,
         PackageDescription: str = ...,
-        CommitMessage: str = ...
+        CommitMessage: str = ...,
     ) -> UpdatePackageResponseTypeDef:
         """
         Updates a package for use with Amazon OpenSearch Service domains.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.update_package)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearch/client/#update_package)
         """
@@ -910,15 +910,15 @@
     async def update_scheduled_action(
         self,
         *,
         DomainName: str,
         ActionID: str,
         ActionType: ActionTypeType,
         ScheduleAt: ScheduleAtType,
-        DesiredStartTime: int = ...
+        DesiredStartTime: int = ...,
     ) -> UpdateScheduledActionResponseTypeDef:
         """
         Reschedules a planned domain configuration change for a later time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.update_scheduled_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearch/client/#update_scheduled_action)
         """
@@ -935,15 +935,15 @@
 
     async def upgrade_domain(
         self,
         *,
         DomainName: str,
         TargetVersion: str,
         PerformCheckOnly: bool = ...,
-        AdvancedOptions: Mapping[str, str] = ...
+        AdvancedOptions: Mapping[str, str] = ...,
     ) -> UpgradeDomainResponseTypeDef:
         """
         Allows you to either upgrade your Amazon OpenSearch Service domain or perform
         an upgrade eligibility check to a compatible version of OpenSearch or
         Elasticsearch.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.upgrade_domain)
```

### Comparing `types-aiobotocore-opensearch-2.9.0/types_aiobotocore_opensearch/literals.py` & `types-aiobotocore-opensearch-2.9.1/types_aiobotocore_opensearch/literals.py`

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
     "ActionSeverityType",
     "ActionStatusType",
     "ActionTypeType",
     "AutoTuneDesiredStateType",
     "AutoTuneStateType",
     "AutoTuneTypeType",
@@ -68,15 +67,14 @@
     "ZoneStatusType",
     "OpenSearchServiceServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 ActionSeverityType = Literal["HIGH", "LOW", "MEDIUM"]
 ActionStatusType = Literal[
     "COMPLETED", "ELIGIBLE", "FAILED", "IN_PROGRESS", "NOT_ELIGIBLE", "PENDING_UPDATE"
 ]
 ActionTypeType = Literal["JVM_HEAP_SIZE_TUNING", "JVM_YOUNG_GEN_TUNING", "SERVICE_SOFTWARE_UPDATE"]
 AutoTuneDesiredStateType = Literal["DISABLED", "ENABLED"]
 AutoTuneStateType = Literal[
```

### Comparing `types-aiobotocore-opensearch-2.9.0/types_aiobotocore_opensearch/literals.pyi` & `types-aiobotocore-opensearch-2.9.1/types_aiobotocore_opensearch/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opensearch-2.9.0/types_aiobotocore_opensearch/type_defs.py` & `types-aiobotocore-opensearch-2.9.1/types_aiobotocore_opensearch/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AWSDomainInformationTypeDef",
     "AcceptInboundConnectionRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "OptionStatusTypeDef",
     "TagTypeDef",
     "AdditionalLimitTypeDef",
```

### Comparing `types-aiobotocore-opensearch-2.9.0/types_aiobotocore_opensearch/type_defs.pyi` & `types-aiobotocore-opensearch-2.9.1/types_aiobotocore_opensearch/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opensearch-2.9.0/types_aiobotocore_opensearch.egg-info/PKG-INFO` & `types-aiobotocore-opensearch-2.9.1/types_aiobotocore_opensearch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-opensearch
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.OpenSearchService 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.OpenSearchService 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearch/
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
 
 <a id="types-aiobotocore-opensearch"></a>
 
 # types-aiobotocore-opensearch
 
 [![PyPI - types-aiobotocore-opensearch](https://img.shields.io/pypi/v/types-aiobotocore-opensearch.svg?color=blue)](https://pypi.org/project/types-aiobotocore-opensearch)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-opensearch.svg?color=blue)](https://pypi.org/project/types-aiobotocore-opensearch)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearch/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-opensearch)](https://pepy.tech/project/types-aiobotocore-opensearch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.OpenSearchService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService)
+[aiobotocore.OpenSearchService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService)
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
 [types-aiobotocore-opensearch docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearch/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-opensearch-2.9.0/types_aiobotocore_opensearch.egg-info/SOURCES.txt` & `types-aiobotocore-opensearch-2.9.1/types_aiobotocore_opensearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

