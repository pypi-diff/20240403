# Comparing `tmp/types-aiobotocore-es-2.9.0.tar.gz` & `tmp/types-aiobotocore-es-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-es-2.9.0.tar", last modified: Wed Dec 13 19:59:17 2023, max compression
+gzip compressed data, was "types-aiobotocore-es-2.9.1.tar", last modified: Thu Jan 18 01:20:42 2024, max compression
```

## Comparing `types-aiobotocore-es-2.9.0.tar` & `types-aiobotocore-es-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:17.541747 types-aiobotocore-es-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:46:02.000000 types-aiobotocore-es-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13897 2023-12-13 19:59:17.541747 types-aiobotocore-es-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12336 2023-12-13 19:46:02.000000 types-aiobotocore-es-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:17.541747 types-aiobotocore-es-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2023-12-13 19:46:02.000000 types-aiobotocore-es-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:17.541747 types-aiobotocore-es-2.9.0/types_aiobotocore_es/
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2023-12-13 19:46:02.000000 types-aiobotocore-es-2.9.0/types_aiobotocore_es/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2023-12-13 19:46:02.000000 types-aiobotocore-es-2.9.0/types_aiobotocore_es/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      937 2023-12-13 19:46:02.000000 types-aiobotocore-es-2.9.0/types_aiobotocore_es/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43339 2023-12-13 19:46:02.000000 types-aiobotocore-es-2.9.0/types_aiobotocore_es/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    43335 2023-12-13 19:46:02.000000 types-aiobotocore-es-2.9.0/types_aiobotocore_es/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    15105 2023-12-13 19:46:03.000000 types-aiobotocore-es-2.9.0/types_aiobotocore_es/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    15103 2023-12-13 19:46:03.000000 types-aiobotocore-es-2.9.0/types_aiobotocore_es/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7555 2023-12-13 19:46:03.000000 types-aiobotocore-es-2.9.0/types_aiobotocore_es/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7548 2023-12-13 19:46:03.000000 types-aiobotocore-es-2.9.0/types_aiobotocore_es/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:46:02.000000 types-aiobotocore-es-2.9.0/types_aiobotocore_es/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    58486 2023-12-13 19:46:04.000000 types-aiobotocore-es-2.9.0/types_aiobotocore_es/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    58485 2023-12-13 19:46:03.000000 types-aiobotocore-es-2.9.0/types_aiobotocore_es/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:46:02.000000 types-aiobotocore-es-2.9.0/types_aiobotocore_es/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:17.541747 types-aiobotocore-es-2.9.0/types_aiobotocore_es.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13897 2023-12-13 19:59:17.000000 types-aiobotocore-es-2.9.0/types_aiobotocore_es.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      718 2023-12-13 19:59:17.000000 types-aiobotocore-es-2.9.0/types_aiobotocore_es.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:17.000000 types-aiobotocore-es-2.9.0/types_aiobotocore_es.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:17.000000 types-aiobotocore-es-2.9.0/types_aiobotocore_es.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:17.000000 types-aiobotocore-es-2.9.0/types_aiobotocore_es.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-12-13 19:59:17.000000 types-aiobotocore-es-2.9.0/types_aiobotocore_es.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:42.157336 types-aiobotocore-es-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:07:56.000000 types-aiobotocore-es-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13917 2024-01-18 01:20:42.157336 types-aiobotocore-es-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12336 2024-01-18 01:07:56.000000 types-aiobotocore-es-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:42.157336 types-aiobotocore-es-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-01-18 01:07:56.000000 types-aiobotocore-es-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:42.157336 types-aiobotocore-es-2.9.1/types_aiobotocore_es/
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-01-18 01:07:56.000000 types-aiobotocore-es-2.9.1/types_aiobotocore_es/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-01-18 01:07:56.000000 types-aiobotocore-es-2.9.1/types_aiobotocore_es/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-01-18 01:07:56.000000 types-aiobotocore-es-2.9.1/types_aiobotocore_es/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43349 2024-01-18 01:07:56.000000 types-aiobotocore-es-2.9.1/types_aiobotocore_es/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43346 2024-01-18 01:07:56.000000 types-aiobotocore-es-2.9.1/types_aiobotocore_es/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    15103 2024-01-18 01:07:57.000000 types-aiobotocore-es-2.9.1/types_aiobotocore_es/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15103 2024-01-18 01:07:57.000000 types-aiobotocore-es-2.9.1/types_aiobotocore_es/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7557 2024-01-18 01:07:57.000000 types-aiobotocore-es-2.9.1/types_aiobotocore_es/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7551 2024-01-18 01:07:57.000000 types-aiobotocore-es-2.9.1/types_aiobotocore_es/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:07:56.000000 types-aiobotocore-es-2.9.1/types_aiobotocore_es/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    58485 2024-01-18 01:07:59.000000 types-aiobotocore-es-2.9.1/types_aiobotocore_es/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58485 2024-01-18 01:07:59.000000 types-aiobotocore-es-2.9.1/types_aiobotocore_es/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:07:56.000000 types-aiobotocore-es-2.9.1/types_aiobotocore_es/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:42.157336 types-aiobotocore-es-2.9.1/types_aiobotocore_es.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13917 2024-01-18 01:20:42.000000 types-aiobotocore-es-2.9.1/types_aiobotocore_es.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-01-18 01:20:42.000000 types-aiobotocore-es-2.9.1/types_aiobotocore_es.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:42.000000 types-aiobotocore-es-2.9.1/types_aiobotocore_es.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:42.000000 types-aiobotocore-es-2.9.1/types_aiobotocore_es.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:42.000000 types-aiobotocore-es-2.9.1/types_aiobotocore_es.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-18 01:20:42.000000 types-aiobotocore-es-2.9.1/types_aiobotocore_es.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-es-2.9.0/LICENSE` & `types-aiobotocore-es-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-es-2.9.0/PKG-INFO` & `types-aiobotocore-es-2.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-es
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ElasticsearchService 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ElasticsearchService 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/
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
 
 <a id="types-aiobotocore-es"></a>
 
 # types-aiobotocore-es
 
 [![PyPI - types-aiobotocore-es](https://img.shields.io/pypi/v/types-aiobotocore-es.svg?color=blue)](https://pypi.org/project/types-aiobotocore-es)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-es.svg?color=blue)](https://pypi.org/project/types-aiobotocore-es)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-es)](https://pepy.tech/project/types-aiobotocore-es)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ElasticsearchService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService)
+[aiobotocore.ElasticsearchService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService)
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
 [types-aiobotocore-es docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-es-2.9.0/README.md` & `types-aiobotocore-es-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-es.svg?color=blue)](https://pypi.org/project/types-aiobotocore-es)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-es)](https://pepy.tech/project/types-aiobotocore-es)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ElasticsearchService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService)
+[aiobotocore.ElasticsearchService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService)
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
 [types-aiobotocore-es docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-es-2.9.0/setup.py` & `types-aiobotocore-es-2.9.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-es",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_es"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ElasticsearchService 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.ElasticsearchService 2.9.1 service generated with"
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
     keywords="aiobotocore es type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_es": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-es-2.9.0/types_aiobotocore_es/__init__.py` & `types-aiobotocore-es-2.9.1/types_aiobotocore_es/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     GetUpgradeHistoryPaginator,
     ListElasticsearchInstanceTypesPaginator,
     ListElasticsearchVersionsPaginator,
 )
 
 Client = ElasticsearchServiceClient
 
-
 __all__ = (
     "Client",
     "DescribeReservedElasticsearchInstanceOfferingsPaginator",
     "DescribeReservedElasticsearchInstancesPaginator",
     "ElasticsearchServiceClient",
     "GetUpgradeHistoryPaginator",
     "ListElasticsearchInstanceTypesPaginator",
```

### Comparing `types-aiobotocore-es-2.9.0/types_aiobotocore_es/__init__.pyi` & `types-aiobotocore-es-2.9.1/types_aiobotocore_es/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-es-2.9.0/types_aiobotocore_es/__main__.py` & `types-aiobotocore-es-2.9.1/types_aiobotocore_es/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ElasticsearchService 2.9.0\nVersion:        "
-        " 2.9.0\nBuilder version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.ElasticsearchService 2.9.1\nVersion:        "
+        " 2.9.1\nBuilder version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService\nOther"
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

### Comparing `types-aiobotocore-es-2.9.0/types_aiobotocore_es/client.py` & `types-aiobotocore-es-2.9.1/types_aiobotocore_es/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ElasticsearchServiceClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -229,29 +228,29 @@
         EncryptionAtRestOptions: EncryptionAtRestOptionsTypeDef = ...,
         NodeToNodeEncryptionOptions: NodeToNodeEncryptionOptionsTypeDef = ...,
         AdvancedOptions: Mapping[str, str] = ...,
         LogPublishingOptions: Mapping[LogTypeType, LogPublishingOptionTypeDef] = ...,
         DomainEndpointOptions: DomainEndpointOptionsTypeDef = ...,
         AdvancedSecurityOptions: AdvancedSecurityOptionsInputTypeDef = ...,
         AutoTuneOptions: AutoTuneOptionsInputTypeDef = ...,
-        TagList: Sequence[TagTypeDef] = ...
+        TagList: Sequence[TagTypeDef] = ...,
     ) -> CreateElasticsearchDomainResponseTypeDef:
         """
         Creates a new Elasticsearch domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Client.create_elasticsearch_domain)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/client/#create_elasticsearch_domain)
         """
 
     async def create_outbound_cross_cluster_search_connection(
         self,
         *,
         SourceDomainInfo: DomainInformationTypeDef,
         DestinationDomainInfo: DomainInformationTypeDef,
-        ConnectionAlias: str
+        ConnectionAlias: str,
     ) -> CreateOutboundCrossClusterSearchConnectionResponseTypeDef:
         """
         Creates a new cross-cluster search connection from a source domain to a
         destination
         domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Client.create_outbound_cross_cluster_search_connection)
@@ -260,15 +259,15 @@
 
     async def create_package(
         self,
         *,
         PackageName: str,
         PackageType: Literal["TXT-DICTIONARY"],
         PackageSource: PackageSourceTypeDef,
-        PackageDescription: str = ...
+        PackageDescription: str = ...,
     ) -> CreatePackageResponseTypeDef:
         """
         Create a package for use with Amazon ES domains.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Client.create_package)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/client/#create_package)
         """
@@ -405,15 +404,15 @@
         """
 
     async def describe_elasticsearch_instance_type_limits(
         self,
         *,
         InstanceType: ESPartitionInstanceTypeType,
         ElasticsearchVersion: str,
-        DomainName: str = ...
+        DomainName: str = ...,
     ) -> DescribeElasticsearchInstanceTypeLimitsResponseTypeDef:
         """
         Describe Elasticsearch Limits for a given InstanceType and ElasticsearchVersion.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Client.describe_elasticsearch_instance_type_limits)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/client/#describe_elasticsearch_instance_type_limits)
         """
@@ -439,43 +438,43 @@
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
         Describes all packages available to Amazon ES.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Client.describe_packages)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/client/#describe_packages)
         """
 
     async def describe_reserved_elasticsearch_instance_offerings(
         self,
         *,
         ReservedElasticsearchInstanceOfferingId: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeReservedElasticsearchInstanceOfferingsResponseTypeDef:
         """
         Lists available reserved Elasticsearch instance offerings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Client.describe_reserved_elasticsearch_instance_offerings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/client/#describe_reserved_elasticsearch_instance_offerings)
         """
 
     async def describe_reserved_elasticsearch_instances(
         self,
         *,
         ReservedElasticsearchInstanceId: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeReservedElasticsearchInstancesResponseTypeDef:
         """
         Returns information about reserved Elasticsearch instances for this account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Client.describe_reserved_elasticsearch_instances)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/client/#describe_reserved_elasticsearch_instances)
         """
@@ -581,15 +580,15 @@
 
     async def list_elasticsearch_instance_types(
         self,
         *,
         ElasticsearchVersion: str,
         DomainName: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListElasticsearchInstanceTypesResponseTypeDef:
         """
         List all Elasticsearch instance types that are supported for given
         ElasticsearchVersion See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/es-2015-01-01/ListElasticsearchInstanceTypes).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Client.list_elasticsearch_instance_types)
@@ -660,15 +659,15 @@
         """
 
     async def purchase_reserved_elasticsearch_instance_offering(
         self,
         *,
         ReservedElasticsearchInstanceOfferingId: str,
         ReservationName: str,
-        InstanceCount: int = ...
+        InstanceCount: int = ...,
     ) -> PurchaseReservedElasticsearchInstanceOfferingResponseTypeDef:
         """
         Allows you to purchase reserved Elasticsearch instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Client.purchase_reserved_elasticsearch_instance_offering)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/client/#purchase_reserved_elasticsearch_instance_offering)
         """
@@ -728,15 +727,15 @@
         AccessPolicies: str = ...,
         LogPublishingOptions: Mapping[LogTypeType, LogPublishingOptionTypeDef] = ...,
         DomainEndpointOptions: DomainEndpointOptionsTypeDef = ...,
         AdvancedSecurityOptions: AdvancedSecurityOptionsInputTypeDef = ...,
         NodeToNodeEncryptionOptions: NodeToNodeEncryptionOptionsTypeDef = ...,
         EncryptionAtRestOptions: EncryptionAtRestOptionsTypeDef = ...,
         AutoTuneOptions: AutoTuneOptionsTypeDef = ...,
-        DryRun: bool = ...
+        DryRun: bool = ...,
     ) -> UpdateElasticsearchDomainConfigResponseTypeDef:
         """
         Modifies the cluster configuration of the specified Elasticsearch domain,
         setting as setting the instance type and the number of
         instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Client.update_elasticsearch_domain_config)
@@ -745,15 +744,15 @@
 
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
         Updates a package for use with Amazon ES domains.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Client.update_package)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/client/#update_package)
         """
```

### Comparing `types-aiobotocore-es-2.9.0/types_aiobotocore_es/client.pyi` & `types-aiobotocore-es-2.9.1/types_aiobotocore_es/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -225,29 +225,29 @@
         EncryptionAtRestOptions: EncryptionAtRestOptionsTypeDef = ...,
         NodeToNodeEncryptionOptions: NodeToNodeEncryptionOptionsTypeDef = ...,
         AdvancedOptions: Mapping[str, str] = ...,
         LogPublishingOptions: Mapping[LogTypeType, LogPublishingOptionTypeDef] = ...,
         DomainEndpointOptions: DomainEndpointOptionsTypeDef = ...,
         AdvancedSecurityOptions: AdvancedSecurityOptionsInputTypeDef = ...,
         AutoTuneOptions: AutoTuneOptionsInputTypeDef = ...,
-        TagList: Sequence[TagTypeDef] = ...
+        TagList: Sequence[TagTypeDef] = ...,
     ) -> CreateElasticsearchDomainResponseTypeDef:
         """
         Creates a new Elasticsearch domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Client.create_elasticsearch_domain)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/client/#create_elasticsearch_domain)
         """
 
     async def create_outbound_cross_cluster_search_connection(
         self,
         *,
         SourceDomainInfo: DomainInformationTypeDef,
         DestinationDomainInfo: DomainInformationTypeDef,
-        ConnectionAlias: str
+        ConnectionAlias: str,
     ) -> CreateOutboundCrossClusterSearchConnectionResponseTypeDef:
         """
         Creates a new cross-cluster search connection from a source domain to a
         destination
         domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Client.create_outbound_cross_cluster_search_connection)
@@ -256,15 +256,15 @@
 
     async def create_package(
         self,
         *,
         PackageName: str,
         PackageType: Literal["TXT-DICTIONARY"],
         PackageSource: PackageSourceTypeDef,
-        PackageDescription: str = ...
+        PackageDescription: str = ...,
     ) -> CreatePackageResponseTypeDef:
         """
         Create a package for use with Amazon ES domains.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Client.create_package)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/client/#create_package)
         """
@@ -401,15 +401,15 @@
         """
 
     async def describe_elasticsearch_instance_type_limits(
         self,
         *,
         InstanceType: ESPartitionInstanceTypeType,
         ElasticsearchVersion: str,
-        DomainName: str = ...
+        DomainName: str = ...,
     ) -> DescribeElasticsearchInstanceTypeLimitsResponseTypeDef:
         """
         Describe Elasticsearch Limits for a given InstanceType and ElasticsearchVersion.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Client.describe_elasticsearch_instance_type_limits)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/client/#describe_elasticsearch_instance_type_limits)
         """
@@ -435,43 +435,43 @@
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
         Describes all packages available to Amazon ES.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Client.describe_packages)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/client/#describe_packages)
         """
 
     async def describe_reserved_elasticsearch_instance_offerings(
         self,
         *,
         ReservedElasticsearchInstanceOfferingId: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeReservedElasticsearchInstanceOfferingsResponseTypeDef:
         """
         Lists available reserved Elasticsearch instance offerings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Client.describe_reserved_elasticsearch_instance_offerings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/client/#describe_reserved_elasticsearch_instance_offerings)
         """
 
     async def describe_reserved_elasticsearch_instances(
         self,
         *,
         ReservedElasticsearchInstanceId: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeReservedElasticsearchInstancesResponseTypeDef:
         """
         Returns information about reserved Elasticsearch instances for this account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Client.describe_reserved_elasticsearch_instances)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/client/#describe_reserved_elasticsearch_instances)
         """
@@ -577,15 +577,15 @@
 
     async def list_elasticsearch_instance_types(
         self,
         *,
         ElasticsearchVersion: str,
         DomainName: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListElasticsearchInstanceTypesResponseTypeDef:
         """
         List all Elasticsearch instance types that are supported for given
         ElasticsearchVersion See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/es-2015-01-01/ListElasticsearchInstanceTypes).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Client.list_elasticsearch_instance_types)
@@ -656,15 +656,15 @@
         """
 
     async def purchase_reserved_elasticsearch_instance_offering(
         self,
         *,
         ReservedElasticsearchInstanceOfferingId: str,
         ReservationName: str,
-        InstanceCount: int = ...
+        InstanceCount: int = ...,
     ) -> PurchaseReservedElasticsearchInstanceOfferingResponseTypeDef:
         """
         Allows you to purchase reserved Elasticsearch instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Client.purchase_reserved_elasticsearch_instance_offering)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/client/#purchase_reserved_elasticsearch_instance_offering)
         """
@@ -724,15 +724,15 @@
         AccessPolicies: str = ...,
         LogPublishingOptions: Mapping[LogTypeType, LogPublishingOptionTypeDef] = ...,
         DomainEndpointOptions: DomainEndpointOptionsTypeDef = ...,
         AdvancedSecurityOptions: AdvancedSecurityOptionsInputTypeDef = ...,
         NodeToNodeEncryptionOptions: NodeToNodeEncryptionOptionsTypeDef = ...,
         EncryptionAtRestOptions: EncryptionAtRestOptionsTypeDef = ...,
         AutoTuneOptions: AutoTuneOptionsTypeDef = ...,
-        DryRun: bool = ...
+        DryRun: bool = ...,
     ) -> UpdateElasticsearchDomainConfigResponseTypeDef:
         """
         Modifies the cluster configuration of the specified Elasticsearch domain,
         setting as setting the instance type and the number of
         instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Client.update_elasticsearch_domain_config)
@@ -741,15 +741,15 @@
 
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
         Updates a package for use with Amazon ES domains.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Client.update_package)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/client/#update_package)
         """
```

### Comparing `types-aiobotocore-es-2.9.0/types_aiobotocore_es/literals.py` & `types-aiobotocore-es-2.9.1/types_aiobotocore_es/literals.py`

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
     "AutoTuneDesiredStateType",
     "AutoTuneStateType",
     "AutoTuneTypeType",
     "DeploymentStatusType",
     "DescribePackagesFilterNameType",
     "DescribeReservedElasticsearchInstanceOfferingsPaginatorName",
@@ -57,15 +56,14 @@
     "ElasticsearchServiceServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AutoTuneDesiredStateType = Literal["DISABLED", "ENABLED"]
 AutoTuneStateType = Literal[
     "DISABLED",
     "DISABLED_AND_ROLLBACK_COMPLETE",
     "DISABLED_AND_ROLLBACK_ERROR",
     "DISABLED_AND_ROLLBACK_IN_PROGRESS",
     "DISABLED_AND_ROLLBACK_SCHEDULED",
```

### Comparing `types-aiobotocore-es-2.9.0/types_aiobotocore_es/literals.pyi` & `types-aiobotocore-es-2.9.1/types_aiobotocore_es/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-es-2.9.0/types_aiobotocore_es/paginator.py` & `types-aiobotocore-es-2.9.1/types_aiobotocore_es/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,14 @@
     "DescribeReservedElasticsearchInstanceOfferingsPaginator",
     "DescribeReservedElasticsearchInstancesPaginator",
     "GetUpgradeHistoryPaginator",
     "ListElasticsearchInstanceTypesPaginator",
     "ListElasticsearchVersionsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -68,15 +67,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/paginators/#describereservedelasticsearchinstanceofferingspaginator)
     """
 
     def paginate(
         self,
         *,
         ReservedElasticsearchInstanceOfferingId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeReservedElasticsearchInstanceOfferingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Paginator.DescribeReservedElasticsearchInstanceOfferings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/paginators/#describereservedelasticsearchinstanceofferingspaginator)
         """
 
 
@@ -86,15 +85,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/paginators/#describereservedelasticsearchinstancespaginator)
     """
 
     def paginate(
         self,
         *,
         ReservedElasticsearchInstanceId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeReservedElasticsearchInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Paginator.DescribeReservedElasticsearchInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/paginators/#describereservedelasticsearchinstancespaginator)
         """
 
 
@@ -120,15 +119,15 @@
     """
 
     def paginate(
         self,
         *,
         ElasticsearchVersion: str,
         DomainName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListElasticsearchInstanceTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Paginator.ListElasticsearchInstanceTypes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/paginators/#listelasticsearchinstancetypespaginator)
         """
```

### Comparing `types-aiobotocore-es-2.9.0/types_aiobotocore_es/paginator.pyi` & `types-aiobotocore-es-2.9.1/types_aiobotocore_es/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/paginators/#describereservedelasticsearchinstanceofferingspaginator)
     """
 
     def paginate(
         self,
         *,
         ReservedElasticsearchInstanceOfferingId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeReservedElasticsearchInstanceOfferingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Paginator.DescribeReservedElasticsearchInstanceOfferings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/paginators/#describereservedelasticsearchinstanceofferingspaginator)
         """
 
 class DescribeReservedElasticsearchInstancesPaginator(AioPaginator):
@@ -82,15 +82,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/paginators/#describereservedelasticsearchinstancespaginator)
     """
 
     def paginate(
         self,
         *,
         ReservedElasticsearchInstanceId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeReservedElasticsearchInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Paginator.DescribeReservedElasticsearchInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/paginators/#describereservedelasticsearchinstancespaginator)
         """
 
 class GetUpgradeHistoryPaginator(AioPaginator):
@@ -114,15 +114,15 @@
     """
 
     def paginate(
         self,
         *,
         ElasticsearchVersion: str,
         DomainName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListElasticsearchInstanceTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Paginator.ListElasticsearchInstanceTypes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/paginators/#listelasticsearchinstancetypespaginator)
         """
 
 class ListElasticsearchVersionsPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-es-2.9.0/types_aiobotocore_es/type_defs.py` & `types-aiobotocore-es-2.9.1/types_aiobotocore_es/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AcceptInboundCrossClusterSearchConnectionRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "OptionStatusTypeDef",
     "TagTypeDef",
     "AdditionalLimitTypeDef",
     "MasterUserOptionsTypeDef",
```

### Comparing `types-aiobotocore-es-2.9.0/types_aiobotocore_es/type_defs.pyi` & `types-aiobotocore-es-2.9.1/types_aiobotocore_es/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-es-2.9.0/types_aiobotocore_es.egg-info/PKG-INFO` & `types-aiobotocore-es-2.9.1/types_aiobotocore_es.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-es
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ElasticsearchService 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ElasticsearchService 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/
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
 
 <a id="types-aiobotocore-es"></a>
 
 # types-aiobotocore-es
 
 [![PyPI - types-aiobotocore-es](https://img.shields.io/pypi/v/types-aiobotocore-es.svg?color=blue)](https://pypi.org/project/types-aiobotocore-es)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-es.svg?color=blue)](https://pypi.org/project/types-aiobotocore-es)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-es)](https://pepy.tech/project/types-aiobotocore-es)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ElasticsearchService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService)
+[aiobotocore.ElasticsearchService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService)
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
 [types-aiobotocore-es docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-es-2.9.0/types_aiobotocore_es.egg-info/SOURCES.txt` & `types-aiobotocore-es-2.9.1/types_aiobotocore_es.egg-info/SOURCES.txt`

 * *Files identical despite different names*

