# Comparing `tmp/types-aiobotocore-config-2.9.0.tar.gz` & `tmp/types-aiobotocore-config-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-config-2.9.0.tar", last modified: Wed Dec 13 19:58:59 2023, max compression
+gzip compressed data, was "types-aiobotocore-config-2.9.1.tar", last modified: Thu Jan 18 01:20:25 2024, max compression
```

## Comparing `types-aiobotocore-config-2.9.0.tar` & `types-aiobotocore-config-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:59.313894 types-aiobotocore-config-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:43:18.000000 types-aiobotocore-config-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    19715 2023-12-13 19:58:59.313894 types-aiobotocore-config-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18149 2023-12-13 19:43:18.000000 types-aiobotocore-config-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:59.313894 types-aiobotocore-config-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2023-12-13 19:43:18.000000 types-aiobotocore-config-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:59.309894 types-aiobotocore-config-2.9.0/types_aiobotocore_config/
--rw-r--r--   0 runner    (1001) docker     (127)     9919 2023-12-13 19:43:18.000000 types-aiobotocore-config-2.9.0/types_aiobotocore_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9918 2023-12-13 19:43:18.000000 types-aiobotocore-config-2.9.0/types_aiobotocore_config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      931 2023-12-13 19:43:18.000000 types-aiobotocore-config-2.9.0/types_aiobotocore_config/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    93018 2023-12-13 19:43:19.000000 types-aiobotocore-config-2.9.0/types_aiobotocore_config/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    93014 2023-12-13 19:43:18.000000 types-aiobotocore-config-2.9.0/types_aiobotocore_config/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    33350 2023-12-13 19:43:19.000000 types-aiobotocore-config-2.9.0/types_aiobotocore_config/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    33348 2023-12-13 19:43:19.000000 types-aiobotocore-config-2.9.0/types_aiobotocore_config/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    44400 2023-12-13 19:43:19.000000 types-aiobotocore-config-2.9.0/types_aiobotocore_config/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    44367 2023-12-13 19:43:19.000000 types-aiobotocore-config-2.9.0/types_aiobotocore_config/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:43:18.000000 types-aiobotocore-config-2.9.0/types_aiobotocore_config/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   104887 2023-12-13 19:43:22.000000 types-aiobotocore-config-2.9.0/types_aiobotocore_config/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   104886 2023-12-13 19:43:21.000000 types-aiobotocore-config-2.9.0/types_aiobotocore_config/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:43:18.000000 types-aiobotocore-config-2.9.0/types_aiobotocore_config/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:59.313894 types-aiobotocore-config-2.9.0/types_aiobotocore_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19715 2023-12-13 19:58:59.000000 types-aiobotocore-config-2.9.0/types_aiobotocore_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      794 2023-12-13 19:58:59.000000 types-aiobotocore-config-2.9.0/types_aiobotocore_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:59.000000 types-aiobotocore-config-2.9.0/types_aiobotocore_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:59.000000 types-aiobotocore-config-2.9.0/types_aiobotocore_config.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:59.000000 types-aiobotocore-config-2.9.0/types_aiobotocore_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-13 19:58:59.000000 types-aiobotocore-config-2.9.0/types_aiobotocore_config.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:25.273420 types-aiobotocore-config-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:05:13.000000 types-aiobotocore-config-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    19735 2024-01-18 01:20:25.273420 types-aiobotocore-config-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18149 2024-01-18 01:05:13.000000 types-aiobotocore-config-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:25.273420 types-aiobotocore-config-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-01-18 01:05:13.000000 types-aiobotocore-config-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:25.273420 types-aiobotocore-config-2.9.1/types_aiobotocore_config/
+-rw-r--r--   0 runner    (1001) docker     (127)     9918 2024-01-18 01:05:14.000000 types-aiobotocore-config-2.9.1/types_aiobotocore_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9918 2024-01-18 01:05:14.000000 types-aiobotocore-config-2.9.1/types_aiobotocore_config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-01-18 01:05:14.000000 types-aiobotocore-config-2.9.1/types_aiobotocore_config/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    93057 2024-01-18 01:05:14.000000 types-aiobotocore-config-2.9.1/types_aiobotocore_config/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    93054 2024-01-18 01:05:14.000000 types-aiobotocore-config-2.9.1/types_aiobotocore_config/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    33348 2024-01-18 01:05:16.000000 types-aiobotocore-config-2.9.1/types_aiobotocore_config/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33348 2024-01-18 01:05:15.000000 types-aiobotocore-config-2.9.1/types_aiobotocore_config/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    44425 2024-01-18 01:05:15.000000 types-aiobotocore-config-2.9.1/types_aiobotocore_config/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44393 2024-01-18 01:05:15.000000 types-aiobotocore-config-2.9.1/types_aiobotocore_config/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:05:14.000000 types-aiobotocore-config-2.9.1/types_aiobotocore_config/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   104886 2024-01-18 01:05:17.000000 types-aiobotocore-config-2.9.1/types_aiobotocore_config/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   104886 2024-01-18 01:05:17.000000 types-aiobotocore-config-2.9.1/types_aiobotocore_config/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:05:13.000000 types-aiobotocore-config-2.9.1/types_aiobotocore_config/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:25.273420 types-aiobotocore-config-2.9.1/types_aiobotocore_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19735 2024-01-18 01:20:25.000000 types-aiobotocore-config-2.9.1/types_aiobotocore_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-01-18 01:20:25.000000 types-aiobotocore-config-2.9.1/types_aiobotocore_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:25.000000 types-aiobotocore-config-2.9.1/types_aiobotocore_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:25.000000 types-aiobotocore-config-2.9.1/types_aiobotocore_config.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:25.000000 types-aiobotocore-config-2.9.1/types_aiobotocore_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-01-18 01:20:25.000000 types-aiobotocore-config-2.9.1/types_aiobotocore_config.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-config-2.9.0/LICENSE` & `types-aiobotocore-config-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-config-2.9.0/PKG-INFO` & `types-aiobotocore-config-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-config
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ConfigService 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ConfigService 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/
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
 
 <a id="types-aiobotocore-config"></a>
 
 # types-aiobotocore-config
 
 [![PyPI - types-aiobotocore-config](https://img.shields.io/pypi/v/types-aiobotocore-config.svg?color=blue)](https://pypi.org/project/types-aiobotocore-config)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-config.svg?color=blue)](https://pypi.org/project/types-aiobotocore-config)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-config)](https://pepy.tech/project/types-aiobotocore-config)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ConfigService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService)
+[aiobotocore.ConfigService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService)
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
 [types-aiobotocore-config docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-config-2.9.0/README.md` & `types-aiobotocore-config-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-config.svg?color=blue)](https://pypi.org/project/types-aiobotocore-config)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-config)](https://pepy.tech/project/types-aiobotocore-config)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ConfigService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService)
+[aiobotocore.ConfigService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService)
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
 [types-aiobotocore-config docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-config-2.9.0/setup.py` & `types-aiobotocore-config-2.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-config",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_config"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ConfigService 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.ConfigService 2.9.1 service generated with"
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
     keywords="aiobotocore config type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_config": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-config-2.9.0/types_aiobotocore_config/__init__.py` & `types-aiobotocore-config-2.9.1/types_aiobotocore_config/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,14 @@
     ListTagsForResourcePaginator,
     SelectAggregateResourceConfigPaginator,
     SelectResourceConfigPaginator,
 )
 
 Client = ConfigServiceClient
 
-
 __all__ = (
     "Client",
     "ConfigServiceClient",
     "DescribeAggregateComplianceByConfigRulesPaginator",
     "DescribeAggregateComplianceByConformancePacksPaginator",
     "DescribeAggregationAuthorizationsPaginator",
     "DescribeComplianceByConfigRulePaginator",
```

### Comparing `types-aiobotocore-config-2.9.0/types_aiobotocore_config/__init__.pyi` & `types-aiobotocore-config-2.9.1/types_aiobotocore_config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-config-2.9.0/types_aiobotocore_config/__main__.py` & `types-aiobotocore-config-2.9.1/types_aiobotocore_config/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ConfigService 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.ConfigService 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService\nOther"
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

### Comparing `types-aiobotocore-config-2.9.0/types_aiobotocore_config/client.py` & `types-aiobotocore-config-2.9.1/types_aiobotocore_config/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ConfigServiceClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -263,15 +262,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#exceptions)
         """
 
     async def batch_get_aggregate_resource_config(
         self,
         *,
         ConfigurationAggregatorName: str,
-        ResourceIdentifiers: Sequence[AggregateResourceIdentifierTypeDef]
+        ResourceIdentifiers: Sequence[AggregateResourceIdentifierTypeDef],
     ) -> BatchGetAggregateResourceConfigResponseTypeDef:
         """
         Returns the current configuration items for resources that are present in your
         Config
         aggregator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.batch_get_aggregate_resource_config)
@@ -476,15 +475,15 @@
 
     async def describe_aggregate_compliance_by_config_rules(
         self,
         *,
         ConfigurationAggregatorName: str,
         Filters: ConfigRuleComplianceFiltersTypeDef = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeAggregateComplianceByConfigRulesResponseTypeDef:
         """
         Returns a list of compliant and noncompliant rules with the number of resources
         for compliant and noncompliant
         rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.describe_aggregate_compliance_by_config_rules)
@@ -493,15 +492,15 @@
 
     async def describe_aggregate_compliance_by_conformance_packs(
         self,
         *,
         ConfigurationAggregatorName: str,
         Filters: AggregateConformancePackComplianceFiltersTypeDef = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeAggregateComplianceByConformancePacksResponseTypeDef:
         """
         Returns a list of the conformance packs and their associated compliance status
         with the count of compliant and noncompliant Config rules within each
         conformance
         pack.
 
@@ -521,15 +520,15 @@
         """
 
     async def describe_compliance_by_config_rule(
         self,
         *,
         ConfigRuleNames: Sequence[str] = ...,
         ComplianceTypes: Sequence[ComplianceTypeType] = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeComplianceByConfigRuleResponseTypeDef:
         """
         Indicates whether the specified Config rules are compliant.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.describe_compliance_by_config_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#describe_compliance_by_config_rule)
         """
@@ -537,15 +536,15 @@
     async def describe_compliance_by_resource(
         self,
         *,
         ResourceType: str = ...,
         ResourceId: str = ...,
         ComplianceTypes: Sequence[ComplianceTypeType] = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeComplianceByResourceResponseTypeDef:
         """
         Indicates whether the specified Amazon Web Services resources are compliant.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.describe_compliance_by_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#describe_compliance_by_resource)
         """
@@ -561,44 +560,44 @@
         """
 
     async def describe_config_rules(
         self,
         *,
         ConfigRuleNames: Sequence[str] = ...,
         NextToken: str = ...,
-        Filters: DescribeConfigRulesFiltersTypeDef = ...
+        Filters: DescribeConfigRulesFiltersTypeDef = ...,
     ) -> DescribeConfigRulesResponseTypeDef:
         """
         Returns details about your Config rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.describe_config_rules)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#describe_config_rules)
         """
 
     async def describe_configuration_aggregator_sources_status(
         self,
         *,
         ConfigurationAggregatorName: str,
         UpdateStatus: Sequence[AggregatedSourceStatusTypeType] = ...,
         NextToken: str = ...,
-        Limit: int = ...
+        Limit: int = ...,
     ) -> DescribeConfigurationAggregatorSourcesStatusResponseTypeDef:
         """
         Returns status information for sources within an aggregator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.describe_configuration_aggregator_sources_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#describe_configuration_aggregator_sources_status)
         """
 
     async def describe_configuration_aggregators(
         self,
         *,
         ConfigurationAggregatorNames: Sequence[str] = ...,
         NextToken: str = ...,
-        Limit: int = ...
+        Limit: int = ...,
     ) -> DescribeConfigurationAggregatorsResponseTypeDef:
         """
         Returns the details of one or more configuration aggregators.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.describe_configuration_aggregators)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#describe_configuration_aggregators)
         """
@@ -627,15 +626,15 @@
 
     async def describe_conformance_pack_compliance(
         self,
         *,
         ConformancePackName: str,
         Filters: ConformancePackComplianceFiltersTypeDef = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeConformancePackComplianceResponseTypeDef:
         """
         Returns compliance details for each rule in that conformance pack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.describe_conformance_pack_compliance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#describe_conformance_pack_compliance)
         """
@@ -681,57 +680,57 @@
         """
 
     async def describe_organization_config_rule_statuses(
         self,
         *,
         OrganizationConfigRuleNames: Sequence[str] = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeOrganizationConfigRuleStatusesResponseTypeDef:
         """
         Provides organization Config rule deployment status for an organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.describe_organization_config_rule_statuses)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#describe_organization_config_rule_statuses)
         """
 
     async def describe_organization_config_rules(
         self,
         *,
         OrganizationConfigRuleNames: Sequence[str] = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeOrganizationConfigRulesResponseTypeDef:
         """
         Returns a list of organization Config rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.describe_organization_config_rules)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#describe_organization_config_rules)
         """
 
     async def describe_organization_conformance_pack_statuses(
         self,
         *,
         OrganizationConformancePackNames: Sequence[str] = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeOrganizationConformancePackStatusesResponseTypeDef:
         """
         Provides organization conformance pack deployment status for an organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.describe_organization_conformance_pack_statuses)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#describe_organization_conformance_pack_statuses)
         """
 
     async def describe_organization_conformance_packs(
         self,
         *,
         OrganizationConformancePackNames: Sequence[str] = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeOrganizationConformancePacksResponseTypeDef:
         """
         Returns a list of organization conformance packs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.describe_organization_conformance_packs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#describe_organization_conformance_packs)
         """
@@ -758,30 +757,30 @@
 
     async def describe_remediation_exceptions(
         self,
         *,
         ConfigRuleName: str,
         ResourceKeys: Sequence[RemediationExceptionResourceKeyTypeDef] = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeRemediationExceptionsResponseTypeDef:
         """
         Returns the details of one or more remediation exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.describe_remediation_exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#describe_remediation_exceptions)
         """
 
     async def describe_remediation_execution_status(
         self,
         *,
         ConfigRuleName: str,
         ResourceKeys: Sequence[ResourceKeyTypeDef] = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeRemediationExecutionStatusResponseTypeDef:
         """
         Provides a detailed view of a Remediation Execution for a set of resources
         including state, timestamps for when steps for the remediation execution occur,
         and any error messages for steps that have
         failed.
 
@@ -818,15 +817,15 @@
         *,
         ConfigurationAggregatorName: str,
         ConfigRuleName: str,
         AccountId: str,
         AwsRegion: str,
         ComplianceType: ComplianceTypeType = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetAggregateComplianceDetailsByConfigRuleResponseTypeDef:
         """
         Returns the evaluation results for the specified Config rule for a specific
         resource in a
         rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.get_aggregate_compliance_details_by_config_rule)
@@ -836,15 +835,15 @@
     async def get_aggregate_config_rule_compliance_summary(
         self,
         *,
         ConfigurationAggregatorName: str,
         Filters: ConfigRuleComplianceSummaryFiltersTypeDef = ...,
         GroupByKey: ConfigRuleComplianceSummaryGroupKeyType = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetAggregateConfigRuleComplianceSummaryResponseTypeDef:
         """
         Returns the number of compliant and noncompliant rules for one or more accounts
         and regions in an
         aggregator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.get_aggregate_config_rule_compliance_summary)
@@ -854,15 +853,15 @@
     async def get_aggregate_conformance_pack_compliance_summary(
         self,
         *,
         ConfigurationAggregatorName: str,
         Filters: AggregateConformancePackComplianceSummaryFiltersTypeDef = ...,
         GroupByKey: AggregateConformancePackComplianceSummaryGroupKeyType = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetAggregateConformancePackComplianceSummaryResponseTypeDef:
         """
         Returns the count of compliant and noncompliant conformance packs across all
         Amazon Web Services accounts and Amazon Web Services Regions in an
         aggregator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.get_aggregate_conformance_pack_compliance_summary)
@@ -872,30 +871,30 @@
     async def get_aggregate_discovered_resource_counts(
         self,
         *,
         ConfigurationAggregatorName: str,
         Filters: ResourceCountFiltersTypeDef = ...,
         GroupByKey: ResourceCountGroupKeyType = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetAggregateDiscoveredResourceCountsResponseTypeDef:
         """
         Returns the resource counts across accounts and regions that are present in
         your Config
         aggregator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.get_aggregate_discovered_resource_counts)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#get_aggregate_discovered_resource_counts)
         """
 
     async def get_aggregate_resource_config(
         self,
         *,
         ConfigurationAggregatorName: str,
-        ResourceIdentifier: AggregateResourceIdentifierTypeDef
+        ResourceIdentifier: AggregateResourceIdentifierTypeDef,
     ) -> GetAggregateResourceConfigResponseTypeDef:
         """
         Returns configuration item that is aggregated for your specific resource in a
         specific source account and
         region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.get_aggregate_resource_config)
@@ -904,15 +903,15 @@
 
     async def get_compliance_details_by_config_rule(
         self,
         *,
         ConfigRuleName: str,
         ComplianceTypes: Sequence[ComplianceTypeType] = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetComplianceDetailsByConfigRuleResponseTypeDef:
         """
         Returns the evaluation results for the specified Config rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.get_compliance_details_by_config_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#get_compliance_details_by_config_rule)
         """
@@ -920,15 +919,15 @@
     async def get_compliance_details_by_resource(
         self,
         *,
         ResourceType: str = ...,
         ResourceId: str = ...,
         ComplianceTypes: Sequence[ComplianceTypeType] = ...,
         NextToken: str = ...,
-        ResourceEvaluationId: str = ...
+        ResourceEvaluationId: str = ...,
     ) -> GetComplianceDetailsByResourceResponseTypeDef:
         """
         Returns the evaluation results for the specified Amazon Web Services resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.get_compliance_details_by_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#get_compliance_details_by_resource)
         """
@@ -958,15 +957,15 @@
 
     async def get_conformance_pack_compliance_details(
         self,
         *,
         ConformancePackName: str,
         Filters: ConformancePackEvaluationFiltersTypeDef = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetConformancePackComplianceDetailsResponseTypeDef:
         """
         Returns compliance details of a conformance pack for all Amazon Web Services
         resources that are monitered by conformance
         pack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.get_conformance_pack_compliance_details)
@@ -1012,15 +1011,15 @@
 
     async def get_organization_config_rule_detailed_status(
         self,
         *,
         OrganizationConfigRuleName: str,
         Filters: StatusDetailFiltersTypeDef = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetOrganizationConfigRuleDetailedStatusResponseTypeDef:
         """
         Returns detailed status for each member account within an organization for a
         given organization Config
         rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.get_organization_config_rule_detailed_status)
@@ -1029,15 +1028,15 @@
 
     async def get_organization_conformance_pack_detailed_status(
         self,
         *,
         OrganizationConformancePackName: str,
         Filters: OrganizationResourceDetailedStatusFiltersTypeDef = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetOrganizationConformancePackDetailedStatusResponseTypeDef:
         """
         Returns detailed status for each member account within an organization for a
         given organization conformance
         pack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.get_organization_conformance_pack_detailed_status)
@@ -1061,15 +1060,15 @@
         *,
         resourceType: ResourceTypeType,
         resourceId: str,
         laterTime: TimestampTypeDef = ...,
         earlierTime: TimestampTypeDef = ...,
         chronologicalOrder: ChronologicalOrderType = ...,
         limit: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> GetResourceConfigHistoryResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.get_resource_config_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#get_resource_config_history)
         """
@@ -1097,15 +1096,15 @@
     async def list_aggregate_discovered_resources(
         self,
         *,
         ConfigurationAggregatorName: str,
         ResourceType: ResourceTypeType,
         Filters: ResourceFiltersTypeDef = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListAggregateDiscoveredResourcesResponseTypeDef:
         """
         Accepts a resource type and returns a list of resource identifiers that are
         aggregated for a specific resource type across accounts and
         regions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.list_aggregate_discovered_resources)
@@ -1115,15 +1114,15 @@
     async def list_conformance_pack_compliance_scores(
         self,
         *,
         Filters: ConformancePackComplianceScoresFiltersTypeDef = ...,
         SortOrder: SortOrderType = ...,
         SortBy: Literal["SCORE"] = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListConformancePackComplianceScoresResponseTypeDef:
         """
         Returns a list of conformance pack compliance scores.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.list_conformance_pack_compliance_scores)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#list_conformance_pack_compliance_scores)
         """
@@ -1132,15 +1131,15 @@
         self,
         *,
         resourceType: ResourceTypeType,
         resourceIds: Sequence[str] = ...,
         resourceName: str = ...,
         limit: int = ...,
         includeDeletedResources: bool = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListDiscoveredResourcesResponseTypeDef:
         """
         Accepts a resource type and returns a list of resource identifiers for the
         resources of that
         type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.list_discovered_resources)
@@ -1148,15 +1147,15 @@
         """
 
     async def list_resource_evaluations(
         self,
         *,
         Filters: ResourceEvaluationFiltersTypeDef = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListResourceEvaluationsResponseTypeDef:
         """
         Returns a list of proactive resource evaluations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.list_resource_evaluations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#list_resource_evaluations)
         """
@@ -1184,15 +1183,15 @@
         """
 
     async def put_aggregation_authorization(
         self,
         *,
         AuthorizedAccountId: str,
         AuthorizedAwsRegion: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> PutAggregationAuthorizationResponseTypeDef:
         """
         Authorizes the aggregator account and region to collect data from the source
         account and
         region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_aggregation_authorization)
@@ -1213,15 +1212,15 @@
 
     async def put_configuration_aggregator(
         self,
         *,
         ConfigurationAggregatorName: str,
         AccountAggregationSources: Sequence[AccountAggregationSourceTypeDef] = ...,
         OrganizationAggregationSource: OrganizationAggregationSourceTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> PutConfigurationAggregatorResponseTypeDef:
         """
         Creates and updates the configuration aggregator with the selected source
         accounts and
         regions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_configuration_aggregator)
@@ -1245,15 +1244,15 @@
         *,
         ConformancePackName: str,
         TemplateS3Uri: str = ...,
         TemplateBody: str = ...,
         DeliveryS3Bucket: str = ...,
         DeliveryS3KeyPrefix: str = ...,
         ConformancePackInputParameters: Sequence[ConformancePackInputParameterTypeDef] = ...,
-        TemplateSSMDocumentDetails: TemplateSSMDocumentDetailsTypeDef = ...
+        TemplateSSMDocumentDetails: TemplateSSMDocumentDetailsTypeDef = ...,
     ) -> PutConformancePackResponseTypeDef:
         """
         Creates or updates a conformance pack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_conformance_pack)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#put_conformance_pack)
         """
@@ -1271,15 +1270,15 @@
         """
 
     async def put_evaluations(
         self,
         *,
         ResultToken: str,
         Evaluations: Sequence[EvaluationTypeDef] = ...,
-        TestMode: bool = ...
+        TestMode: bool = ...,
     ) -> PutEvaluationsResponseTypeDef:
         """
         Used by an Lambda function to deliver evaluation results to Config.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_evaluations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#put_evaluations)
         """
@@ -1297,15 +1296,15 @@
     async def put_organization_config_rule(
         self,
         *,
         OrganizationConfigRuleName: str,
         OrganizationManagedRuleMetadata: OrganizationManagedRuleMetadataTypeDef = ...,
         OrganizationCustomRuleMetadata: OrganizationCustomRuleMetadataTypeDef = ...,
         ExcludedAccounts: Sequence[str] = ...,
-        OrganizationCustomPolicyRuleMetadata: OrganizationCustomPolicyRuleMetadataTypeDef = ...
+        OrganizationCustomPolicyRuleMetadata: OrganizationCustomPolicyRuleMetadataTypeDef = ...,
     ) -> PutOrganizationConfigRuleResponseTypeDef:
         """
         Adds or updates an Config rule for your entire organization to evaluate if your
         Amazon Web Services resources comply with your desired
         configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_organization_config_rule)
@@ -1317,15 +1316,15 @@
         *,
         OrganizationConformancePackName: str,
         TemplateS3Uri: str = ...,
         TemplateBody: str = ...,
         DeliveryS3Bucket: str = ...,
         DeliveryS3KeyPrefix: str = ...,
         ConformancePackInputParameters: Sequence[ConformancePackInputParameterTypeDef] = ...,
-        ExcludedAccounts: Sequence[str] = ...
+        ExcludedAccounts: Sequence[str] = ...,
     ) -> PutOrganizationConformancePackResponseTypeDef:
         """
         Deploys conformance packs across member accounts in an Amazon Web Services
         Organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_organization_conformance_pack)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#put_organization_conformance_pack)
@@ -1345,15 +1344,15 @@
 
     async def put_remediation_exceptions(
         self,
         *,
         ConfigRuleName: str,
         ResourceKeys: Sequence[RemediationExceptionResourceKeyTypeDef],
         Message: str = ...,
-        ExpirationTime: TimestampTypeDef = ...
+        ExpirationTime: TimestampTypeDef = ...,
     ) -> PutRemediationExceptionsResponseTypeDef:
         """
         A remediation exception is when a specified resource is no longer considered
         for
         auto-remediation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_remediation_exceptions)
@@ -1364,15 +1363,15 @@
         self,
         *,
         ResourceType: str,
         SchemaVersionId: str,
         ResourceId: str,
         Configuration: str,
         ResourceName: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Records the configuration state for the resource provided in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_resource_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#put_resource_config)
         """
@@ -1402,15 +1401,15 @@
     async def select_aggregate_resource_config(
         self,
         *,
         Expression: str,
         ConfigurationAggregatorName: str,
         Limit: int = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> SelectAggregateResourceConfigResponseTypeDef:
         """
         Accepts a structured query language (SQL) SELECT command and an aggregator to
         query configuration state of Amazon Web Services resources across multiple
         accounts and regions, performs the corresponding search, and returns resource
         configurations matching the
         properties.
@@ -1470,15 +1469,15 @@
     async def start_resource_evaluation(
         self,
         *,
         ResourceDetails: ResourceDetailsTypeDef,
         EvaluationMode: EvaluationModeType,
         EvaluationContext: EvaluationContextTypeDef = ...,
         EvaluationTimeout: int = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> StartResourceEvaluationResponseTypeDef:
         """
         Runs an on-demand evaluation for the specified resource to determine whether
         the resource details will comply with configured Config
         rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.start_resource_evaluation)
```

### Comparing `types-aiobotocore-config-2.9.0/types_aiobotocore_config/client.pyi` & `types-aiobotocore-config-2.9.1/types_aiobotocore_config/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -259,15 +259,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#exceptions)
         """
 
     async def batch_get_aggregate_resource_config(
         self,
         *,
         ConfigurationAggregatorName: str,
-        ResourceIdentifiers: Sequence[AggregateResourceIdentifierTypeDef]
+        ResourceIdentifiers: Sequence[AggregateResourceIdentifierTypeDef],
     ) -> BatchGetAggregateResourceConfigResponseTypeDef:
         """
         Returns the current configuration items for resources that are present in your
         Config
         aggregator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.batch_get_aggregate_resource_config)
@@ -472,15 +472,15 @@
 
     async def describe_aggregate_compliance_by_config_rules(
         self,
         *,
         ConfigurationAggregatorName: str,
         Filters: ConfigRuleComplianceFiltersTypeDef = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeAggregateComplianceByConfigRulesResponseTypeDef:
         """
         Returns a list of compliant and noncompliant rules with the number of resources
         for compliant and noncompliant
         rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.describe_aggregate_compliance_by_config_rules)
@@ -489,15 +489,15 @@
 
     async def describe_aggregate_compliance_by_conformance_packs(
         self,
         *,
         ConfigurationAggregatorName: str,
         Filters: AggregateConformancePackComplianceFiltersTypeDef = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeAggregateComplianceByConformancePacksResponseTypeDef:
         """
         Returns a list of the conformance packs and their associated compliance status
         with the count of compliant and noncompliant Config rules within each
         conformance
         pack.
 
@@ -517,15 +517,15 @@
         """
 
     async def describe_compliance_by_config_rule(
         self,
         *,
         ConfigRuleNames: Sequence[str] = ...,
         ComplianceTypes: Sequence[ComplianceTypeType] = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeComplianceByConfigRuleResponseTypeDef:
         """
         Indicates whether the specified Config rules are compliant.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.describe_compliance_by_config_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#describe_compliance_by_config_rule)
         """
@@ -533,15 +533,15 @@
     async def describe_compliance_by_resource(
         self,
         *,
         ResourceType: str = ...,
         ResourceId: str = ...,
         ComplianceTypes: Sequence[ComplianceTypeType] = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeComplianceByResourceResponseTypeDef:
         """
         Indicates whether the specified Amazon Web Services resources are compliant.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.describe_compliance_by_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#describe_compliance_by_resource)
         """
@@ -557,44 +557,44 @@
         """
 
     async def describe_config_rules(
         self,
         *,
         ConfigRuleNames: Sequence[str] = ...,
         NextToken: str = ...,
-        Filters: DescribeConfigRulesFiltersTypeDef = ...
+        Filters: DescribeConfigRulesFiltersTypeDef = ...,
     ) -> DescribeConfigRulesResponseTypeDef:
         """
         Returns details about your Config rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.describe_config_rules)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#describe_config_rules)
         """
 
     async def describe_configuration_aggregator_sources_status(
         self,
         *,
         ConfigurationAggregatorName: str,
         UpdateStatus: Sequence[AggregatedSourceStatusTypeType] = ...,
         NextToken: str = ...,
-        Limit: int = ...
+        Limit: int = ...,
     ) -> DescribeConfigurationAggregatorSourcesStatusResponseTypeDef:
         """
         Returns status information for sources within an aggregator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.describe_configuration_aggregator_sources_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#describe_configuration_aggregator_sources_status)
         """
 
     async def describe_configuration_aggregators(
         self,
         *,
         ConfigurationAggregatorNames: Sequence[str] = ...,
         NextToken: str = ...,
-        Limit: int = ...
+        Limit: int = ...,
     ) -> DescribeConfigurationAggregatorsResponseTypeDef:
         """
         Returns the details of one or more configuration aggregators.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.describe_configuration_aggregators)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#describe_configuration_aggregators)
         """
@@ -623,15 +623,15 @@
 
     async def describe_conformance_pack_compliance(
         self,
         *,
         ConformancePackName: str,
         Filters: ConformancePackComplianceFiltersTypeDef = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeConformancePackComplianceResponseTypeDef:
         """
         Returns compliance details for each rule in that conformance pack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.describe_conformance_pack_compliance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#describe_conformance_pack_compliance)
         """
@@ -677,57 +677,57 @@
         """
 
     async def describe_organization_config_rule_statuses(
         self,
         *,
         OrganizationConfigRuleNames: Sequence[str] = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeOrganizationConfigRuleStatusesResponseTypeDef:
         """
         Provides organization Config rule deployment status for an organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.describe_organization_config_rule_statuses)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#describe_organization_config_rule_statuses)
         """
 
     async def describe_organization_config_rules(
         self,
         *,
         OrganizationConfigRuleNames: Sequence[str] = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeOrganizationConfigRulesResponseTypeDef:
         """
         Returns a list of organization Config rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.describe_organization_config_rules)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#describe_organization_config_rules)
         """
 
     async def describe_organization_conformance_pack_statuses(
         self,
         *,
         OrganizationConformancePackNames: Sequence[str] = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeOrganizationConformancePackStatusesResponseTypeDef:
         """
         Provides organization conformance pack deployment status for an organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.describe_organization_conformance_pack_statuses)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#describe_organization_conformance_pack_statuses)
         """
 
     async def describe_organization_conformance_packs(
         self,
         *,
         OrganizationConformancePackNames: Sequence[str] = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeOrganizationConformancePacksResponseTypeDef:
         """
         Returns a list of organization conformance packs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.describe_organization_conformance_packs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#describe_organization_conformance_packs)
         """
@@ -754,30 +754,30 @@
 
     async def describe_remediation_exceptions(
         self,
         *,
         ConfigRuleName: str,
         ResourceKeys: Sequence[RemediationExceptionResourceKeyTypeDef] = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeRemediationExceptionsResponseTypeDef:
         """
         Returns the details of one or more remediation exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.describe_remediation_exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#describe_remediation_exceptions)
         """
 
     async def describe_remediation_execution_status(
         self,
         *,
         ConfigRuleName: str,
         ResourceKeys: Sequence[ResourceKeyTypeDef] = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeRemediationExecutionStatusResponseTypeDef:
         """
         Provides a detailed view of a Remediation Execution for a set of resources
         including state, timestamps for when steps for the remediation execution occur,
         and any error messages for steps that have
         failed.
 
@@ -814,15 +814,15 @@
         *,
         ConfigurationAggregatorName: str,
         ConfigRuleName: str,
         AccountId: str,
         AwsRegion: str,
         ComplianceType: ComplianceTypeType = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetAggregateComplianceDetailsByConfigRuleResponseTypeDef:
         """
         Returns the evaluation results for the specified Config rule for a specific
         resource in a
         rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.get_aggregate_compliance_details_by_config_rule)
@@ -832,15 +832,15 @@
     async def get_aggregate_config_rule_compliance_summary(
         self,
         *,
         ConfigurationAggregatorName: str,
         Filters: ConfigRuleComplianceSummaryFiltersTypeDef = ...,
         GroupByKey: ConfigRuleComplianceSummaryGroupKeyType = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetAggregateConfigRuleComplianceSummaryResponseTypeDef:
         """
         Returns the number of compliant and noncompliant rules for one or more accounts
         and regions in an
         aggregator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.get_aggregate_config_rule_compliance_summary)
@@ -850,15 +850,15 @@
     async def get_aggregate_conformance_pack_compliance_summary(
         self,
         *,
         ConfigurationAggregatorName: str,
         Filters: AggregateConformancePackComplianceSummaryFiltersTypeDef = ...,
         GroupByKey: AggregateConformancePackComplianceSummaryGroupKeyType = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetAggregateConformancePackComplianceSummaryResponseTypeDef:
         """
         Returns the count of compliant and noncompliant conformance packs across all
         Amazon Web Services accounts and Amazon Web Services Regions in an
         aggregator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.get_aggregate_conformance_pack_compliance_summary)
@@ -868,30 +868,30 @@
     async def get_aggregate_discovered_resource_counts(
         self,
         *,
         ConfigurationAggregatorName: str,
         Filters: ResourceCountFiltersTypeDef = ...,
         GroupByKey: ResourceCountGroupKeyType = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetAggregateDiscoveredResourceCountsResponseTypeDef:
         """
         Returns the resource counts across accounts and regions that are present in
         your Config
         aggregator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.get_aggregate_discovered_resource_counts)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#get_aggregate_discovered_resource_counts)
         """
 
     async def get_aggregate_resource_config(
         self,
         *,
         ConfigurationAggregatorName: str,
-        ResourceIdentifier: AggregateResourceIdentifierTypeDef
+        ResourceIdentifier: AggregateResourceIdentifierTypeDef,
     ) -> GetAggregateResourceConfigResponseTypeDef:
         """
         Returns configuration item that is aggregated for your specific resource in a
         specific source account and
         region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.get_aggregate_resource_config)
@@ -900,15 +900,15 @@
 
     async def get_compliance_details_by_config_rule(
         self,
         *,
         ConfigRuleName: str,
         ComplianceTypes: Sequence[ComplianceTypeType] = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetComplianceDetailsByConfigRuleResponseTypeDef:
         """
         Returns the evaluation results for the specified Config rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.get_compliance_details_by_config_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#get_compliance_details_by_config_rule)
         """
@@ -916,15 +916,15 @@
     async def get_compliance_details_by_resource(
         self,
         *,
         ResourceType: str = ...,
         ResourceId: str = ...,
         ComplianceTypes: Sequence[ComplianceTypeType] = ...,
         NextToken: str = ...,
-        ResourceEvaluationId: str = ...
+        ResourceEvaluationId: str = ...,
     ) -> GetComplianceDetailsByResourceResponseTypeDef:
         """
         Returns the evaluation results for the specified Amazon Web Services resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.get_compliance_details_by_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#get_compliance_details_by_resource)
         """
@@ -954,15 +954,15 @@
 
     async def get_conformance_pack_compliance_details(
         self,
         *,
         ConformancePackName: str,
         Filters: ConformancePackEvaluationFiltersTypeDef = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetConformancePackComplianceDetailsResponseTypeDef:
         """
         Returns compliance details of a conformance pack for all Amazon Web Services
         resources that are monitered by conformance
         pack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.get_conformance_pack_compliance_details)
@@ -1008,15 +1008,15 @@
 
     async def get_organization_config_rule_detailed_status(
         self,
         *,
         OrganizationConfigRuleName: str,
         Filters: StatusDetailFiltersTypeDef = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetOrganizationConfigRuleDetailedStatusResponseTypeDef:
         """
         Returns detailed status for each member account within an organization for a
         given organization Config
         rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.get_organization_config_rule_detailed_status)
@@ -1025,15 +1025,15 @@
 
     async def get_organization_conformance_pack_detailed_status(
         self,
         *,
         OrganizationConformancePackName: str,
         Filters: OrganizationResourceDetailedStatusFiltersTypeDef = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetOrganizationConformancePackDetailedStatusResponseTypeDef:
         """
         Returns detailed status for each member account within an organization for a
         given organization conformance
         pack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.get_organization_conformance_pack_detailed_status)
@@ -1057,15 +1057,15 @@
         *,
         resourceType: ResourceTypeType,
         resourceId: str,
         laterTime: TimestampTypeDef = ...,
         earlierTime: TimestampTypeDef = ...,
         chronologicalOrder: ChronologicalOrderType = ...,
         limit: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> GetResourceConfigHistoryResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.get_resource_config_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#get_resource_config_history)
         """
@@ -1093,15 +1093,15 @@
     async def list_aggregate_discovered_resources(
         self,
         *,
         ConfigurationAggregatorName: str,
         ResourceType: ResourceTypeType,
         Filters: ResourceFiltersTypeDef = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListAggregateDiscoveredResourcesResponseTypeDef:
         """
         Accepts a resource type and returns a list of resource identifiers that are
         aggregated for a specific resource type across accounts and
         regions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.list_aggregate_discovered_resources)
@@ -1111,15 +1111,15 @@
     async def list_conformance_pack_compliance_scores(
         self,
         *,
         Filters: ConformancePackComplianceScoresFiltersTypeDef = ...,
         SortOrder: SortOrderType = ...,
         SortBy: Literal["SCORE"] = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListConformancePackComplianceScoresResponseTypeDef:
         """
         Returns a list of conformance pack compliance scores.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.list_conformance_pack_compliance_scores)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#list_conformance_pack_compliance_scores)
         """
@@ -1128,15 +1128,15 @@
         self,
         *,
         resourceType: ResourceTypeType,
         resourceIds: Sequence[str] = ...,
         resourceName: str = ...,
         limit: int = ...,
         includeDeletedResources: bool = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListDiscoveredResourcesResponseTypeDef:
         """
         Accepts a resource type and returns a list of resource identifiers for the
         resources of that
         type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.list_discovered_resources)
@@ -1144,15 +1144,15 @@
         """
 
     async def list_resource_evaluations(
         self,
         *,
         Filters: ResourceEvaluationFiltersTypeDef = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListResourceEvaluationsResponseTypeDef:
         """
         Returns a list of proactive resource evaluations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.list_resource_evaluations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#list_resource_evaluations)
         """
@@ -1180,15 +1180,15 @@
         """
 
     async def put_aggregation_authorization(
         self,
         *,
         AuthorizedAccountId: str,
         AuthorizedAwsRegion: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> PutAggregationAuthorizationResponseTypeDef:
         """
         Authorizes the aggregator account and region to collect data from the source
         account and
         region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_aggregation_authorization)
@@ -1209,15 +1209,15 @@
 
     async def put_configuration_aggregator(
         self,
         *,
         ConfigurationAggregatorName: str,
         AccountAggregationSources: Sequence[AccountAggregationSourceTypeDef] = ...,
         OrganizationAggregationSource: OrganizationAggregationSourceTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> PutConfigurationAggregatorResponseTypeDef:
         """
         Creates and updates the configuration aggregator with the selected source
         accounts and
         regions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_configuration_aggregator)
@@ -1241,15 +1241,15 @@
         *,
         ConformancePackName: str,
         TemplateS3Uri: str = ...,
         TemplateBody: str = ...,
         DeliveryS3Bucket: str = ...,
         DeliveryS3KeyPrefix: str = ...,
         ConformancePackInputParameters: Sequence[ConformancePackInputParameterTypeDef] = ...,
-        TemplateSSMDocumentDetails: TemplateSSMDocumentDetailsTypeDef = ...
+        TemplateSSMDocumentDetails: TemplateSSMDocumentDetailsTypeDef = ...,
     ) -> PutConformancePackResponseTypeDef:
         """
         Creates or updates a conformance pack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_conformance_pack)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#put_conformance_pack)
         """
@@ -1267,15 +1267,15 @@
         """
 
     async def put_evaluations(
         self,
         *,
         ResultToken: str,
         Evaluations: Sequence[EvaluationTypeDef] = ...,
-        TestMode: bool = ...
+        TestMode: bool = ...,
     ) -> PutEvaluationsResponseTypeDef:
         """
         Used by an Lambda function to deliver evaluation results to Config.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_evaluations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#put_evaluations)
         """
@@ -1293,15 +1293,15 @@
     async def put_organization_config_rule(
         self,
         *,
         OrganizationConfigRuleName: str,
         OrganizationManagedRuleMetadata: OrganizationManagedRuleMetadataTypeDef = ...,
         OrganizationCustomRuleMetadata: OrganizationCustomRuleMetadataTypeDef = ...,
         ExcludedAccounts: Sequence[str] = ...,
-        OrganizationCustomPolicyRuleMetadata: OrganizationCustomPolicyRuleMetadataTypeDef = ...
+        OrganizationCustomPolicyRuleMetadata: OrganizationCustomPolicyRuleMetadataTypeDef = ...,
     ) -> PutOrganizationConfigRuleResponseTypeDef:
         """
         Adds or updates an Config rule for your entire organization to evaluate if your
         Amazon Web Services resources comply with your desired
         configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_organization_config_rule)
@@ -1313,15 +1313,15 @@
         *,
         OrganizationConformancePackName: str,
         TemplateS3Uri: str = ...,
         TemplateBody: str = ...,
         DeliveryS3Bucket: str = ...,
         DeliveryS3KeyPrefix: str = ...,
         ConformancePackInputParameters: Sequence[ConformancePackInputParameterTypeDef] = ...,
-        ExcludedAccounts: Sequence[str] = ...
+        ExcludedAccounts: Sequence[str] = ...,
     ) -> PutOrganizationConformancePackResponseTypeDef:
         """
         Deploys conformance packs across member accounts in an Amazon Web Services
         Organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_organization_conformance_pack)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#put_organization_conformance_pack)
@@ -1341,15 +1341,15 @@
 
     async def put_remediation_exceptions(
         self,
         *,
         ConfigRuleName: str,
         ResourceKeys: Sequence[RemediationExceptionResourceKeyTypeDef],
         Message: str = ...,
-        ExpirationTime: TimestampTypeDef = ...
+        ExpirationTime: TimestampTypeDef = ...,
     ) -> PutRemediationExceptionsResponseTypeDef:
         """
         A remediation exception is when a specified resource is no longer considered
         for
         auto-remediation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_remediation_exceptions)
@@ -1360,15 +1360,15 @@
         self,
         *,
         ResourceType: str,
         SchemaVersionId: str,
         ResourceId: str,
         Configuration: str,
         ResourceName: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Records the configuration state for the resource provided in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_resource_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#put_resource_config)
         """
@@ -1398,15 +1398,15 @@
     async def select_aggregate_resource_config(
         self,
         *,
         Expression: str,
         ConfigurationAggregatorName: str,
         Limit: int = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> SelectAggregateResourceConfigResponseTypeDef:
         """
         Accepts a structured query language (SQL) SELECT command and an aggregator to
         query configuration state of Amazon Web Services resources across multiple
         accounts and regions, performs the corresponding search, and returns resource
         configurations matching the
         properties.
@@ -1466,15 +1466,15 @@
     async def start_resource_evaluation(
         self,
         *,
         ResourceDetails: ResourceDetailsTypeDef,
         EvaluationMode: EvaluationModeType,
         EvaluationContext: EvaluationContextTypeDef = ...,
         EvaluationTimeout: int = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> StartResourceEvaluationResponseTypeDef:
         """
         Runs an on-demand evaluation for the specified resource to determine whether
         the resource details will comply with configured Config
         rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.start_resource_evaluation)
```

### Comparing `types-aiobotocore-config-2.9.0/types_aiobotocore_config/literals.py` & `types-aiobotocore-config-2.9.1/types_aiobotocore_config/literals.py`

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
     "AggregateConformancePackComplianceSummaryGroupKeyType",
     "AggregatedSourceStatusTypeType",
     "AggregatedSourceTypeType",
     "ChronologicalOrderType",
     "ComplianceTypeType",
     "ConfigRuleComplianceSummaryGroupKeyType",
@@ -90,15 +89,14 @@
     "ConfigServiceServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AggregateConformancePackComplianceSummaryGroupKeyType = Literal["ACCOUNT_ID", "AWS_REGION"]
 AggregatedSourceStatusTypeType = Literal["FAILED", "OUTDATED", "SUCCEEDED"]
 AggregatedSourceTypeType = Literal["ACCOUNT", "ORGANIZATION"]
 ChronologicalOrderType = Literal["Forward", "Reverse"]
 ComplianceTypeType = Literal["COMPLIANT", "INSUFFICIENT_DATA", "NON_COMPLIANT", "NOT_APPLICABLE"]
 ConfigRuleComplianceSummaryGroupKeyType = Literal["ACCOUNT_ID", "AWS_REGION"]
 ConfigRuleStateType = Literal["ACTIVE", "DELETING", "DELETING_RESULTS", "EVALUATING"]
```

### Comparing `types-aiobotocore-config-2.9.0/types_aiobotocore_config/literals.pyi` & `types-aiobotocore-config-2.9.1/types_aiobotocore_config/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-config-2.9.0/types_aiobotocore_config/paginator.py` & `types-aiobotocore-config-2.9.1/types_aiobotocore_config/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,15 +166,14 @@
     "ListDiscoveredResourcesPaginator",
     "ListResourceEvaluationsPaginator",
     "ListTagsForResourcePaginator",
     "SelectAggregateResourceConfigPaginator",
     "SelectResourceConfigPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -188,15 +187,15 @@
     """
 
     def paginate(
         self,
         *,
         ConfigurationAggregatorName: str,
         Filters: ConfigRuleComplianceFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeAggregateComplianceByConfigRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeAggregateComplianceByConfigRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeaggregatecompliancebyconfigrulespaginator)
         """
 
 
@@ -207,15 +206,15 @@
     """
 
     def paginate(
         self,
         *,
         ConfigurationAggregatorName: str,
         Filters: AggregateConformancePackComplianceFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeAggregateComplianceByConformancePacksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeAggregateComplianceByConformancePacks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeaggregatecompliancebyconformancepackspaginator)
         """
 
 
@@ -241,15 +240,15 @@
     """
 
     def paginate(
         self,
         *,
         ConfigRuleNames: Sequence[str] = ...,
         ComplianceTypes: Sequence[ComplianceTypeType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeComplianceByConfigRuleResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeComplianceByConfigRule.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describecompliancebyconfigrulepaginator)
         """
 
 
@@ -261,15 +260,15 @@
 
     def paginate(
         self,
         *,
         ResourceType: str = ...,
         ResourceId: str = ...,
         ComplianceTypes: Sequence[ComplianceTypeType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeComplianceByResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeComplianceByResource.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describecompliancebyresourcepaginator)
         """
 
 
@@ -279,15 +278,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeconfigruleevaluationstatuspaginator)
     """
 
     def paginate(
         self,
         *,
         ConfigRuleNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeConfigRuleEvaluationStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeConfigRuleEvaluationStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeconfigruleevaluationstatuspaginator)
         """
 
 
@@ -298,15 +297,15 @@
     """
 
     def paginate(
         self,
         *,
         ConfigRuleNames: Sequence[str] = ...,
         Filters: DescribeConfigRulesFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeConfigRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeConfigRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeconfigrulespaginator)
         """
 
 
@@ -317,15 +316,15 @@
     """
 
     def paginate(
         self,
         *,
         ConfigurationAggregatorName: str,
         UpdateStatus: Sequence[AggregatedSourceStatusTypeType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeConfigurationAggregatorSourcesStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeConfigurationAggregatorSourcesStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeconfigurationaggregatorsourcesstatuspaginator)
         """
 
 
@@ -335,15 +334,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeconfigurationaggregatorspaginator)
     """
 
     def paginate(
         self,
         *,
         ConfigurationAggregatorNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeConfigurationAggregatorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeConfigurationAggregators.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeconfigurationaggregatorspaginator)
         """
 
 
@@ -353,15 +352,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeconformancepackstatuspaginator)
     """
 
     def paginate(
         self,
         *,
         ConformancePackNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeConformancePackStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeConformancePackStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeconformancepackstatuspaginator)
         """
 
 
@@ -371,15 +370,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeconformancepackspaginator)
     """
 
     def paginate(
         self,
         *,
         ConformancePackNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeConformancePacksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeConformancePacks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeconformancepackspaginator)
         """
 
 
@@ -389,15 +388,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeorganizationconfigrulestatusespaginator)
     """
 
     def paginate(
         self,
         *,
         OrganizationConfigRuleNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeOrganizationConfigRuleStatusesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeOrganizationConfigRuleStatuses.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeorganizationconfigrulestatusespaginator)
         """
 
 
@@ -407,15 +406,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeorganizationconfigrulespaginator)
     """
 
     def paginate(
         self,
         *,
         OrganizationConfigRuleNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeOrganizationConfigRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeOrganizationConfigRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeorganizationconfigrulespaginator)
         """
 
 
@@ -425,15 +424,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeorganizationconformancepackstatusespaginator)
     """
 
     def paginate(
         self,
         *,
         OrganizationConformancePackNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeOrganizationConformancePackStatusesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeOrganizationConformancePackStatuses.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeorganizationconformancepackstatusespaginator)
         """
 
 
@@ -443,15 +442,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeorganizationconformancepackspaginator)
     """
 
     def paginate(
         self,
         *,
         OrganizationConformancePackNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeOrganizationConformancePacksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeOrganizationConformancePacks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeorganizationconformancepackspaginator)
         """
 
 
@@ -477,15 +476,15 @@
     """
 
     def paginate(
         self,
         *,
         ConfigRuleName: str,
         ResourceKeys: Sequence[ResourceKeyTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeRemediationExecutionStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeRemediationExecutionStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeremediationexecutionstatuspaginator)
         """
 
 
@@ -495,15 +494,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeretentionconfigurationspaginator)
     """
 
     def paginate(
         self,
         *,
         RetentionConfigurationNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeRetentionConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeRetentionConfigurations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeretentionconfigurationspaginator)
         """
 
 
@@ -517,15 +516,15 @@
         self,
         *,
         ConfigurationAggregatorName: str,
         ConfigRuleName: str,
         AccountId: str,
         AwsRegion: str,
         ComplianceType: ComplianceTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetAggregateComplianceDetailsByConfigRuleResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.GetAggregateComplianceDetailsByConfigRule.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#getaggregatecompliancedetailsbyconfigrulepaginator)
         """
 
 
@@ -536,15 +535,15 @@
     """
 
     def paginate(
         self,
         *,
         ConfigRuleName: str,
         ComplianceTypes: Sequence[ComplianceTypeType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetComplianceDetailsByConfigRuleResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.GetComplianceDetailsByConfigRule.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#getcompliancedetailsbyconfigrulepaginator)
         """
 
 
@@ -557,15 +556,15 @@
     def paginate(
         self,
         *,
         ResourceType: str = ...,
         ResourceId: str = ...,
         ComplianceTypes: Sequence[ComplianceTypeType] = ...,
         ResourceEvaluationId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetComplianceDetailsByResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.GetComplianceDetailsByResource.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#getcompliancedetailsbyresourcepaginator)
         """
 
 
@@ -591,15 +590,15 @@
     """
 
     def paginate(
         self,
         *,
         OrganizationConfigRuleName: str,
         Filters: StatusDetailFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetOrganizationConfigRuleDetailedStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.GetOrganizationConfigRuleDetailedStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#getorganizationconfigruledetailedstatuspaginator)
         """
 
 
@@ -610,15 +609,15 @@
     """
 
     def paginate(
         self,
         *,
         OrganizationConformancePackName: str,
         Filters: OrganizationResourceDetailedStatusFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetOrganizationConformancePackDetailedStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.GetOrganizationConformancePackDetailedStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#getorganizationconformancepackdetailedstatuspaginator)
         """
 
 
@@ -632,15 +631,15 @@
         self,
         *,
         resourceType: ResourceTypeType,
         resourceId: str,
         laterTime: TimestampTypeDef = ...,
         earlierTime: TimestampTypeDef = ...,
         chronologicalOrder: ChronologicalOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetResourceConfigHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.GetResourceConfigHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#getresourceconfighistorypaginator)
         """
 
 
@@ -652,15 +651,15 @@
 
     def paginate(
         self,
         *,
         ConfigurationAggregatorName: str,
         ResourceType: ResourceTypeType,
         Filters: ResourceFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAggregateDiscoveredResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.ListAggregateDiscoveredResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#listaggregatediscoveredresourcespaginator)
         """
 
 
@@ -673,15 +672,15 @@
     def paginate(
         self,
         *,
         resourceType: ResourceTypeType,
         resourceIds: Sequence[str] = ...,
         resourceName: str = ...,
         includeDeletedResources: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDiscoveredResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.ListDiscoveredResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#listdiscoveredresourcespaginator)
         """
 
 
@@ -691,15 +690,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#listresourceevaluationspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: ResourceEvaluationFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListResourceEvaluationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.ListResourceEvaluations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#listresourceevaluationspaginator)
         """
 
 
@@ -726,15 +725,15 @@
 
     def paginate(
         self,
         *,
         Expression: str,
         ConfigurationAggregatorName: str,
         MaxResults: int = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SelectAggregateResourceConfigResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.SelectAggregateResourceConfig.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#selectaggregateresourceconfigpaginator)
         """
```

### Comparing `types-aiobotocore-config-2.9.0/types_aiobotocore_config/paginator.pyi` & `types-aiobotocore-config-2.9.1/types_aiobotocore_config/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,15 @@
     """
 
     def paginate(
         self,
         *,
         ConfigurationAggregatorName: str,
         Filters: ConfigRuleComplianceFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeAggregateComplianceByConfigRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeAggregateComplianceByConfigRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeaggregatecompliancebyconfigrulespaginator)
         """
 
 class DescribeAggregateComplianceByConformancePacksPaginator(AioPaginator):
@@ -203,15 +203,15 @@
     """
 
     def paginate(
         self,
         *,
         ConfigurationAggregatorName: str,
         Filters: AggregateConformancePackComplianceFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeAggregateComplianceByConformancePacksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeAggregateComplianceByConformancePacks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeaggregatecompliancebyconformancepackspaginator)
         """
 
 class DescribeAggregationAuthorizationsPaginator(AioPaginator):
@@ -235,15 +235,15 @@
     """
 
     def paginate(
         self,
         *,
         ConfigRuleNames: Sequence[str] = ...,
         ComplianceTypes: Sequence[ComplianceTypeType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeComplianceByConfigRuleResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeComplianceByConfigRule.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describecompliancebyconfigrulepaginator)
         """
 
 class DescribeComplianceByResourcePaginator(AioPaginator):
@@ -254,15 +254,15 @@
 
     def paginate(
         self,
         *,
         ResourceType: str = ...,
         ResourceId: str = ...,
         ComplianceTypes: Sequence[ComplianceTypeType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeComplianceByResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeComplianceByResource.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describecompliancebyresourcepaginator)
         """
 
 class DescribeConfigRuleEvaluationStatusPaginator(AioPaginator):
@@ -271,15 +271,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeconfigruleevaluationstatuspaginator)
     """
 
     def paginate(
         self,
         *,
         ConfigRuleNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeConfigRuleEvaluationStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeConfigRuleEvaluationStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeconfigruleevaluationstatuspaginator)
         """
 
 class DescribeConfigRulesPaginator(AioPaginator):
@@ -289,15 +289,15 @@
     """
 
     def paginate(
         self,
         *,
         ConfigRuleNames: Sequence[str] = ...,
         Filters: DescribeConfigRulesFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeConfigRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeConfigRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeconfigrulespaginator)
         """
 
 class DescribeConfigurationAggregatorSourcesStatusPaginator(AioPaginator):
@@ -307,15 +307,15 @@
     """
 
     def paginate(
         self,
         *,
         ConfigurationAggregatorName: str,
         UpdateStatus: Sequence[AggregatedSourceStatusTypeType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeConfigurationAggregatorSourcesStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeConfigurationAggregatorSourcesStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeconfigurationaggregatorsourcesstatuspaginator)
         """
 
 class DescribeConfigurationAggregatorsPaginator(AioPaginator):
@@ -324,15 +324,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeconfigurationaggregatorspaginator)
     """
 
     def paginate(
         self,
         *,
         ConfigurationAggregatorNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeConfigurationAggregatorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeConfigurationAggregators.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeconfigurationaggregatorspaginator)
         """
 
 class DescribeConformancePackStatusPaginator(AioPaginator):
@@ -341,15 +341,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeconformancepackstatuspaginator)
     """
 
     def paginate(
         self,
         *,
         ConformancePackNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeConformancePackStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeConformancePackStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeconformancepackstatuspaginator)
         """
 
 class DescribeConformancePacksPaginator(AioPaginator):
@@ -358,15 +358,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeconformancepackspaginator)
     """
 
     def paginate(
         self,
         *,
         ConformancePackNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeConformancePacksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeConformancePacks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeconformancepackspaginator)
         """
 
 class DescribeOrganizationConfigRuleStatusesPaginator(AioPaginator):
@@ -375,15 +375,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeorganizationconfigrulestatusespaginator)
     """
 
     def paginate(
         self,
         *,
         OrganizationConfigRuleNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeOrganizationConfigRuleStatusesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeOrganizationConfigRuleStatuses.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeorganizationconfigrulestatusespaginator)
         """
 
 class DescribeOrganizationConfigRulesPaginator(AioPaginator):
@@ -392,15 +392,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeorganizationconfigrulespaginator)
     """
 
     def paginate(
         self,
         *,
         OrganizationConfigRuleNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeOrganizationConfigRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeOrganizationConfigRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeorganizationconfigrulespaginator)
         """
 
 class DescribeOrganizationConformancePackStatusesPaginator(AioPaginator):
@@ -409,15 +409,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeorganizationconformancepackstatusespaginator)
     """
 
     def paginate(
         self,
         *,
         OrganizationConformancePackNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeOrganizationConformancePackStatusesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeOrganizationConformancePackStatuses.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeorganizationconformancepackstatusespaginator)
         """
 
 class DescribeOrganizationConformancePacksPaginator(AioPaginator):
@@ -426,15 +426,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeorganizationconformancepackspaginator)
     """
 
     def paginate(
         self,
         *,
         OrganizationConformancePackNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeOrganizationConformancePacksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeOrganizationConformancePacks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeorganizationconformancepackspaginator)
         """
 
 class DescribePendingAggregationRequestsPaginator(AioPaginator):
@@ -458,15 +458,15 @@
     """
 
     def paginate(
         self,
         *,
         ConfigRuleName: str,
         ResourceKeys: Sequence[ResourceKeyTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeRemediationExecutionStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeRemediationExecutionStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeremediationexecutionstatuspaginator)
         """
 
 class DescribeRetentionConfigurationsPaginator(AioPaginator):
@@ -475,15 +475,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeretentionconfigurationspaginator)
     """
 
     def paginate(
         self,
         *,
         RetentionConfigurationNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeRetentionConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeRetentionConfigurations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeretentionconfigurationspaginator)
         """
 
 class GetAggregateComplianceDetailsByConfigRulePaginator(AioPaginator):
@@ -496,15 +496,15 @@
         self,
         *,
         ConfigurationAggregatorName: str,
         ConfigRuleName: str,
         AccountId: str,
         AwsRegion: str,
         ComplianceType: ComplianceTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetAggregateComplianceDetailsByConfigRuleResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.GetAggregateComplianceDetailsByConfigRule.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#getaggregatecompliancedetailsbyconfigrulepaginator)
         """
 
 class GetComplianceDetailsByConfigRulePaginator(AioPaginator):
@@ -514,15 +514,15 @@
     """
 
     def paginate(
         self,
         *,
         ConfigRuleName: str,
         ComplianceTypes: Sequence[ComplianceTypeType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetComplianceDetailsByConfigRuleResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.GetComplianceDetailsByConfigRule.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#getcompliancedetailsbyconfigrulepaginator)
         """
 
 class GetComplianceDetailsByResourcePaginator(AioPaginator):
@@ -534,15 +534,15 @@
     def paginate(
         self,
         *,
         ResourceType: str = ...,
         ResourceId: str = ...,
         ComplianceTypes: Sequence[ComplianceTypeType] = ...,
         ResourceEvaluationId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetComplianceDetailsByResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.GetComplianceDetailsByResource.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#getcompliancedetailsbyresourcepaginator)
         """
 
 class GetConformancePackComplianceSummaryPaginator(AioPaginator):
@@ -566,15 +566,15 @@
     """
 
     def paginate(
         self,
         *,
         OrganizationConfigRuleName: str,
         Filters: StatusDetailFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetOrganizationConfigRuleDetailedStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.GetOrganizationConfigRuleDetailedStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#getorganizationconfigruledetailedstatuspaginator)
         """
 
 class GetOrganizationConformancePackDetailedStatusPaginator(AioPaginator):
@@ -584,15 +584,15 @@
     """
 
     def paginate(
         self,
         *,
         OrganizationConformancePackName: str,
         Filters: OrganizationResourceDetailedStatusFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetOrganizationConformancePackDetailedStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.GetOrganizationConformancePackDetailedStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#getorganizationconformancepackdetailedstatuspaginator)
         """
 
 class GetResourceConfigHistoryPaginator(AioPaginator):
@@ -605,15 +605,15 @@
         self,
         *,
         resourceType: ResourceTypeType,
         resourceId: str,
         laterTime: TimestampTypeDef = ...,
         earlierTime: TimestampTypeDef = ...,
         chronologicalOrder: ChronologicalOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetResourceConfigHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.GetResourceConfigHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#getresourceconfighistorypaginator)
         """
 
 class ListAggregateDiscoveredResourcesPaginator(AioPaginator):
@@ -624,15 +624,15 @@
 
     def paginate(
         self,
         *,
         ConfigurationAggregatorName: str,
         ResourceType: ResourceTypeType,
         Filters: ResourceFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAggregateDiscoveredResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.ListAggregateDiscoveredResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#listaggregatediscoveredresourcespaginator)
         """
 
 class ListDiscoveredResourcesPaginator(AioPaginator):
@@ -644,15 +644,15 @@
     def paginate(
         self,
         *,
         resourceType: ResourceTypeType,
         resourceIds: Sequence[str] = ...,
         resourceName: str = ...,
         includeDeletedResources: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDiscoveredResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.ListDiscoveredResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#listdiscoveredresourcespaginator)
         """
 
 class ListResourceEvaluationsPaginator(AioPaginator):
@@ -661,15 +661,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#listresourceevaluationspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: ResourceEvaluationFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListResourceEvaluationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.ListResourceEvaluations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#listresourceevaluationspaginator)
         """
 
 class ListTagsForResourcePaginator(AioPaginator):
@@ -694,15 +694,15 @@
 
     def paginate(
         self,
         *,
         Expression: str,
         ConfigurationAggregatorName: str,
         MaxResults: int = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SelectAggregateResourceConfigResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.SelectAggregateResourceConfig.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#selectaggregateresourceconfigpaginator)
         """
 
 class SelectResourceConfigPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-config-2.9.0/types_aiobotocore_config/type_defs.py` & `types-aiobotocore-config-2.9.1/types_aiobotocore_config/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccountAggregationSourceTypeDef",
     "AggregateConformancePackComplianceTypeDef",
     "AggregateConformancePackComplianceCountTypeDef",
     "AggregateConformancePackComplianceFiltersTypeDef",
     "AggregateConformancePackComplianceSummaryFiltersTypeDef",
     "AggregateResourceIdentifierTypeDef",
```

### Comparing `types-aiobotocore-config-2.9.0/types_aiobotocore_config/type_defs.pyi` & `types-aiobotocore-config-2.9.1/types_aiobotocore_config/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-config-2.9.0/types_aiobotocore_config.egg-info/PKG-INFO` & `types-aiobotocore-config-2.9.1/types_aiobotocore_config.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-config
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ConfigService 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ConfigService 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/
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
 
 <a id="types-aiobotocore-config"></a>
 
 # types-aiobotocore-config
 
 [![PyPI - types-aiobotocore-config](https://img.shields.io/pypi/v/types-aiobotocore-config.svg?color=blue)](https://pypi.org/project/types-aiobotocore-config)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-config.svg?color=blue)](https://pypi.org/project/types-aiobotocore-config)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-config)](https://pepy.tech/project/types-aiobotocore-config)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ConfigService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService)
+[aiobotocore.ConfigService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService)
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
 [types-aiobotocore-config docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-config-2.9.0/types_aiobotocore_config.egg-info/SOURCES.txt` & `types-aiobotocore-config-2.9.1/types_aiobotocore_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

