# Comparing `tmp/types-aiobotocore-health-2.9.0.tar.gz` & `tmp/types-aiobotocore-health-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-health-2.9.0.tar", last modified: Wed Dec 13 19:59:25 2023, max compression
+gzip compressed data, was "types-aiobotocore-health-2.9.1.tar", last modified: Thu Jan 18 01:20:49 2024, max compression
```

## Comparing `types-aiobotocore-health-2.9.0.tar` & `types-aiobotocore-health-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:25.817708 types-aiobotocore-health-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:47:10.000000 types-aiobotocore-health-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14194 2023-12-13 19:59:25.817708 types-aiobotocore-health-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12635 2023-12-13 19:47:10.000000 types-aiobotocore-health-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:25.817708 types-aiobotocore-health-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2023-12-13 19:47:10.000000 types-aiobotocore-health-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:25.817708 types-aiobotocore-health-2.9.0/types_aiobotocore_health/
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2023-12-13 19:47:10.000000 types-aiobotocore-health-2.9.0/types_aiobotocore_health/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2023-12-13 19:47:10.000000 types-aiobotocore-health-2.9.0/types_aiobotocore_health/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      917 2023-12-13 19:47:10.000000 types-aiobotocore-health-2.9.0/types_aiobotocore_health/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18022 2023-12-13 19:47:10.000000 types-aiobotocore-health-2.9.0/types_aiobotocore_health/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    18018 2023-12-13 19:47:10.000000 types-aiobotocore-health-2.9.0/types_aiobotocore_health/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9991 2023-12-13 19:47:11.000000 types-aiobotocore-health-2.9.0/types_aiobotocore_health/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9989 2023-12-13 19:47:11.000000 types-aiobotocore-health-2.9.0/types_aiobotocore_health/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10371 2023-12-13 19:47:11.000000 types-aiobotocore-health-2.9.0/types_aiobotocore_health/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10361 2023-12-13 19:47:11.000000 types-aiobotocore-health-2.9.0/types_aiobotocore_health/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:47:10.000000 types-aiobotocore-health-2.9.0/types_aiobotocore_health/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    19810 2023-12-13 19:47:11.000000 types-aiobotocore-health-2.9.0/types_aiobotocore_health/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    19809 2023-12-13 19:47:11.000000 types-aiobotocore-health-2.9.0/types_aiobotocore_health/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:47:10.000000 types-aiobotocore-health-2.9.0/types_aiobotocore_health/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:25.817708 types-aiobotocore-health-2.9.0/types_aiobotocore_health.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14194 2023-12-13 19:59:25.000000 types-aiobotocore-health-2.9.0/types_aiobotocore_health.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      794 2023-12-13 19:59:25.000000 types-aiobotocore-health-2.9.0/types_aiobotocore_health.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:25.000000 types-aiobotocore-health-2.9.0/types_aiobotocore_health.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:25.000000 types-aiobotocore-health-2.9.0/types_aiobotocore_health.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:25.000000 types-aiobotocore-health-2.9.0/types_aiobotocore_health.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-13 19:59:25.000000 types-aiobotocore-health-2.9.0/types_aiobotocore_health.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:49.765300 types-aiobotocore-health-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:09:03.000000 types-aiobotocore-health-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14214 2024-01-18 01:20:49.765300 types-aiobotocore-health-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12635 2024-01-18 01:09:03.000000 types-aiobotocore-health-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:49.765300 types-aiobotocore-health-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-01-18 01:09:03.000000 types-aiobotocore-health-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:49.765300 types-aiobotocore-health-2.9.1/types_aiobotocore_health/
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-01-18 01:09:03.000000 types-aiobotocore-health-2.9.1/types_aiobotocore_health/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-01-18 01:09:03.000000 types-aiobotocore-health-2.9.1/types_aiobotocore_health/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-01-18 01:09:03.000000 types-aiobotocore-health-2.9.1/types_aiobotocore_health/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18028 2024-01-18 01:09:03.000000 types-aiobotocore-health-2.9.1/types_aiobotocore_health/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18025 2024-01-18 01:09:03.000000 types-aiobotocore-health-2.9.1/types_aiobotocore_health/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9989 2024-01-18 01:09:03.000000 types-aiobotocore-health-2.9.1/types_aiobotocore_health/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9989 2024-01-18 01:09:03.000000 types-aiobotocore-health-2.9.1/types_aiobotocore_health/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10375 2024-01-18 01:09:03.000000 types-aiobotocore-health-2.9.1/types_aiobotocore_health/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10367 2024-01-18 01:09:03.000000 types-aiobotocore-health-2.9.1/types_aiobotocore_health/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:09:03.000000 types-aiobotocore-health-2.9.1/types_aiobotocore_health/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    19809 2024-01-18 01:09:03.000000 types-aiobotocore-health-2.9.1/types_aiobotocore_health/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19809 2024-01-18 01:09:03.000000 types-aiobotocore-health-2.9.1/types_aiobotocore_health/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:09:03.000000 types-aiobotocore-health-2.9.1/types_aiobotocore_health/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:49.765300 types-aiobotocore-health-2.9.1/types_aiobotocore_health.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14214 2024-01-18 01:20:49.000000 types-aiobotocore-health-2.9.1/types_aiobotocore_health.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-01-18 01:20:49.000000 types-aiobotocore-health-2.9.1/types_aiobotocore_health.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:49.000000 types-aiobotocore-health-2.9.1/types_aiobotocore_health.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:49.000000 types-aiobotocore-health-2.9.1/types_aiobotocore_health.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:49.000000 types-aiobotocore-health-2.9.1/types_aiobotocore_health.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-01-18 01:20:49.000000 types-aiobotocore-health-2.9.1/types_aiobotocore_health.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-health-2.9.0/LICENSE` & `types-aiobotocore-health-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-health-2.9.0/PKG-INFO` & `types-aiobotocore-health-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-health
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Health 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Health 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/
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
 
 <a id="types-aiobotocore-health"></a>
 
 # types-aiobotocore-health
 
 [![PyPI - types-aiobotocore-health](https://img.shields.io/pypi/v/types-aiobotocore-health.svg?color=blue)](https://pypi.org/project/types-aiobotocore-health)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-health.svg?color=blue)](https://pypi.org/project/types-aiobotocore-health)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-health)](https://pepy.tech/project/types-aiobotocore-health)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Health 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health)
+[aiobotocore.Health 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health)
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
 [types-aiobotocore-health docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-health-2.9.0/README.md` & `types-aiobotocore-health-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-health.svg?color=blue)](https://pypi.org/project/types-aiobotocore-health)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-health)](https://pepy.tech/project/types-aiobotocore-health)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Health 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health)
+[aiobotocore.Health 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health)
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
 [types-aiobotocore-health docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-health-2.9.0/setup.py` & `types-aiobotocore-health-2.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-health",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_health"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Health 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.Health 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore health type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_health": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-health-2.9.0/types_aiobotocore_health/__init__.py` & `types-aiobotocore-health-2.9.1/types_aiobotocore_health/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,14 @@
     DescribeEventsForOrganizationPaginator,
     DescribeEventsPaginator,
     DescribeEventTypesPaginator,
 )
 
 Client = HealthClient
 
-
 __all__ = (
     "Client",
     "DescribeAffectedAccountsForOrganizationPaginator",
     "DescribeAffectedEntitiesForOrganizationPaginator",
     "DescribeAffectedEntitiesPaginator",
     "DescribeEventAggregatesPaginator",
     "DescribeEventTypesPaginator",
```

### Comparing `types-aiobotocore-health-2.9.0/types_aiobotocore_health/__init__.pyi` & `types-aiobotocore-health-2.9.1/types_aiobotocore_health/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-health-2.9.0/types_aiobotocore_health/__main__.py` & `types-aiobotocore-health-2.9.1/types_aiobotocore_health/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Health 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Health 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health\nOther"
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

### Comparing `types-aiobotocore-health-2.9.0/types_aiobotocore_health/client.py` & `types-aiobotocore-health-2.9.1/types_aiobotocore_health/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("HealthClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -123,15 +122,15 @@
 
     async def describe_affected_entities(
         self,
         *,
         filter: EntityFilterTypeDef,
         locale: str = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> DescribeAffectedEntitiesResponseTypeDef:
         """
         Returns a list of entities that have been affected by the specified events,
         based on the specified filter
         criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Client.describe_affected_entities)
@@ -141,15 +140,15 @@
     async def describe_affected_entities_for_organization(
         self,
         *,
         organizationEntityFilters: Sequence[EventAccountFilterTypeDef] = ...,
         locale: str = ...,
         nextToken: str = ...,
         maxResults: int = ...,
-        organizationEntityAccountFilters: Sequence[EntityAccountFilterTypeDef] = ...
+        organizationEntityAccountFilters: Sequence[EntityAccountFilterTypeDef] = ...,
     ) -> DescribeAffectedEntitiesForOrganizationResponseTypeDef:
         """
         Returns a list of entities that have been affected by one or more events for
         one or more accounts in your organization in Organizations, based on the filter
         criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Client.describe_affected_entities_for_organization)
@@ -181,15 +180,15 @@
 
     async def describe_event_aggregates(
         self,
         *,
         aggregateField: Literal["eventTypeCategory"],
         filter: EventFilterTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeEventAggregatesResponseTypeDef:
         """
         Returns the number of events of each event type (issue, scheduled change, and
         account
         notification).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Client.describe_event_aggregates)
@@ -206,15 +205,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/client/#describe_event_details)
         """
 
     async def describe_event_details_for_organization(
         self,
         *,
         organizationEventDetailFilters: Sequence[EventAccountFilterTypeDef],
-        locale: str = ...
+        locale: str = ...,
     ) -> DescribeEventDetailsForOrganizationResponseTypeDef:
         """
         Returns detailed information about one or more specified events for one or more
         Amazon Web Services accounts in your
         organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Client.describe_event_details_for_organization)
@@ -223,45 +222,45 @@
 
     async def describe_event_types(
         self,
         *,
         filter: EventTypeFilterTypeDef = ...,
         locale: str = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> DescribeEventTypesResponseTypeDef:
         """
         Returns the event types that meet the specified filter criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Client.describe_event_types)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/client/#describe_event_types)
         """
 
     async def describe_events(
         self,
         *,
         filter: EventFilterTypeDef = ...,
         nextToken: str = ...,
         maxResults: int = ...,
-        locale: str = ...
+        locale: str = ...,
     ) -> DescribeEventsResponseTypeDef:
         """
         Returns information about events that meet the specified filter criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Client.describe_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/client/#describe_events)
         """
 
     async def describe_events_for_organization(
         self,
         *,
         filter: OrganizationEventFilterTypeDef = ...,
         nextToken: str = ...,
         maxResults: int = ...,
-        locale: str = ...
+        locale: str = ...,
     ) -> DescribeEventsForOrganizationResponseTypeDef:
         """
         Returns information about events across your organization in Organizations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Client.describe_events_for_organization)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/client/#describe_events_for_organization)
         """
```

### Comparing `types-aiobotocore-health-2.9.0/types_aiobotocore_health/client.pyi` & `types-aiobotocore-health-2.9.1/types_aiobotocore_health/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 
     async def describe_affected_entities(
         self,
         *,
         filter: EntityFilterTypeDef,
         locale: str = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> DescribeAffectedEntitiesResponseTypeDef:
         """
         Returns a list of entities that have been affected by the specified events,
         based on the specified filter
         criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Client.describe_affected_entities)
@@ -137,15 +137,15 @@
     async def describe_affected_entities_for_organization(
         self,
         *,
         organizationEntityFilters: Sequence[EventAccountFilterTypeDef] = ...,
         locale: str = ...,
         nextToken: str = ...,
         maxResults: int = ...,
-        organizationEntityAccountFilters: Sequence[EntityAccountFilterTypeDef] = ...
+        organizationEntityAccountFilters: Sequence[EntityAccountFilterTypeDef] = ...,
     ) -> DescribeAffectedEntitiesForOrganizationResponseTypeDef:
         """
         Returns a list of entities that have been affected by one or more events for
         one or more accounts in your organization in Organizations, based on the filter
         criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Client.describe_affected_entities_for_organization)
@@ -177,15 +177,15 @@
 
     async def describe_event_aggregates(
         self,
         *,
         aggregateField: Literal["eventTypeCategory"],
         filter: EventFilterTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeEventAggregatesResponseTypeDef:
         """
         Returns the number of events of each event type (issue, scheduled change, and
         account
         notification).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Client.describe_event_aggregates)
@@ -202,15 +202,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/client/#describe_event_details)
         """
 
     async def describe_event_details_for_organization(
         self,
         *,
         organizationEventDetailFilters: Sequence[EventAccountFilterTypeDef],
-        locale: str = ...
+        locale: str = ...,
     ) -> DescribeEventDetailsForOrganizationResponseTypeDef:
         """
         Returns detailed information about one or more specified events for one or more
         Amazon Web Services accounts in your
         organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Client.describe_event_details_for_organization)
@@ -219,45 +219,45 @@
 
     async def describe_event_types(
         self,
         *,
         filter: EventTypeFilterTypeDef = ...,
         locale: str = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> DescribeEventTypesResponseTypeDef:
         """
         Returns the event types that meet the specified filter criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Client.describe_event_types)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/client/#describe_event_types)
         """
 
     async def describe_events(
         self,
         *,
         filter: EventFilterTypeDef = ...,
         nextToken: str = ...,
         maxResults: int = ...,
-        locale: str = ...
+        locale: str = ...,
     ) -> DescribeEventsResponseTypeDef:
         """
         Returns information about events that meet the specified filter criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Client.describe_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/client/#describe_events)
         """
 
     async def describe_events_for_organization(
         self,
         *,
         filter: OrganizationEventFilterTypeDef = ...,
         nextToken: str = ...,
         maxResults: int = ...,
-        locale: str = ...
+        locale: str = ...,
     ) -> DescribeEventsForOrganizationResponseTypeDef:
         """
         Returns information about events across your organization in Organizations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Client.describe_events_for_organization)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/client/#describe_events_for_organization)
         """
```

### Comparing `types-aiobotocore-health-2.9.0/types_aiobotocore_health/literals.py` & `types-aiobotocore-health-2.9.1/types_aiobotocore_health/literals.py`

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
     "DescribeAffectedAccountsForOrganizationPaginatorName",
     "DescribeAffectedEntitiesForOrganizationPaginatorName",
     "DescribeAffectedEntitiesPaginatorName",
     "DescribeEventAggregatesPaginatorName",
     "DescribeEventTypesPaginatorName",
     "DescribeEventsForOrganizationPaginatorName",
@@ -36,15 +35,14 @@
     "HealthServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 DescribeAffectedAccountsForOrganizationPaginatorName = Literal[
     "describe_affected_accounts_for_organization"
 ]
 DescribeAffectedEntitiesForOrganizationPaginatorName = Literal[
     "describe_affected_entities_for_organization"
 ]
 DescribeAffectedEntitiesPaginatorName = Literal["describe_affected_entities"]
```

### Comparing `types-aiobotocore-health-2.9.0/types_aiobotocore_health/literals.pyi` & `types-aiobotocore-health-2.9.1/types_aiobotocore_health/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-health-2.9.0/types_aiobotocore_health/paginator.py` & `types-aiobotocore-health-2.9.1/types_aiobotocore_health/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,26 +57,24 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "DescribeAffectedAccountsForOrganizationPaginator",
     "DescribeAffectedEntitiesPaginator",
     "DescribeAffectedEntitiesForOrganizationPaginator",
     "DescribeEventAggregatesPaginator",
     "DescribeEventTypesPaginator",
     "DescribeEventsPaginator",
     "DescribeEventsForOrganizationPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -105,15 +103,15 @@
     """
 
     def paginate(
         self,
         *,
         filter: EntityFilterTypeDef,
         locale: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeAffectedEntitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeAffectedEntities.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/paginators/#describeaffectedentitiespaginator)
         """
 
 
@@ -125,15 +123,15 @@
 
     def paginate(
         self,
         *,
         organizationEntityFilters: Sequence[EventAccountFilterTypeDef] = ...,
         locale: str = ...,
         organizationEntityAccountFilters: Sequence[EntityAccountFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeAffectedEntitiesForOrganizationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeAffectedEntitiesForOrganization.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/paginators/#describeaffectedentitiesfororganizationpaginator)
         """
 
 
@@ -144,15 +142,15 @@
     """
 
     def paginate(
         self,
         *,
         aggregateField: Literal["eventTypeCategory"],
         filter: EventFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeEventAggregatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeEventAggregates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/paginators/#describeeventaggregatespaginator)
         """
 
 
@@ -163,15 +161,15 @@
     """
 
     def paginate(
         self,
         *,
         filter: EventTypeFilterTypeDef = ...,
         locale: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeEventTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeEventTypes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/paginators/#describeeventtypespaginator)
         """
 
 
@@ -182,15 +180,15 @@
     """
 
     def paginate(
         self,
         *,
         filter: EventFilterTypeDef = ...,
         locale: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/paginators/#describeeventspaginator)
         """
 
 
@@ -201,13 +199,13 @@
     """
 
     def paginate(
         self,
         *,
         filter: OrganizationEventFilterTypeDef = ...,
         locale: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeEventsForOrganizationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeEventsForOrganization.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/paginators/#describeeventsfororganizationpaginator)
         """
```

### Comparing `types-aiobotocore-health-2.9.0/types_aiobotocore_health/paginator.pyi` & `types-aiobotocore-health-2.9.1/types_aiobotocore_health/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     """
 
     def paginate(
         self,
         *,
         filter: EntityFilterTypeDef,
         locale: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeAffectedEntitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeAffectedEntities.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/paginators/#describeaffectedentitiespaginator)
         """
 
 class DescribeAffectedEntitiesForOrganizationPaginator(AioPaginator):
@@ -119,15 +119,15 @@
 
     def paginate(
         self,
         *,
         organizationEntityFilters: Sequence[EventAccountFilterTypeDef] = ...,
         locale: str = ...,
         organizationEntityAccountFilters: Sequence[EntityAccountFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeAffectedEntitiesForOrganizationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeAffectedEntitiesForOrganization.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/paginators/#describeaffectedentitiesfororganizationpaginator)
         """
 
 class DescribeEventAggregatesPaginator(AioPaginator):
@@ -137,15 +137,15 @@
     """
 
     def paginate(
         self,
         *,
         aggregateField: Literal["eventTypeCategory"],
         filter: EventFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeEventAggregatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeEventAggregates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/paginators/#describeeventaggregatespaginator)
         """
 
 class DescribeEventTypesPaginator(AioPaginator):
@@ -155,15 +155,15 @@
     """
 
     def paginate(
         self,
         *,
         filter: EventTypeFilterTypeDef = ...,
         locale: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeEventTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeEventTypes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/paginators/#describeeventtypespaginator)
         """
 
 class DescribeEventsPaginator(AioPaginator):
@@ -173,15 +173,15 @@
     """
 
     def paginate(
         self,
         *,
         filter: EventFilterTypeDef = ...,
         locale: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/paginators/#describeeventspaginator)
         """
 
 class DescribeEventsForOrganizationPaginator(AioPaginator):
@@ -191,13 +191,13 @@
     """
 
     def paginate(
         self,
         *,
         filter: OrganizationEventFilterTypeDef = ...,
         locale: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeEventsForOrganizationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeEventsForOrganization.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/paginators/#describeeventsfororganizationpaginator)
         """
```

### Comparing `types-aiobotocore-health-2.9.0/types_aiobotocore_health/type_defs.py` & `types-aiobotocore-health-2.9.1/types_aiobotocore_health/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccountEntityAggregateTypeDef",
     "AffectedEntityTypeDef",
     "TimestampTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeAffectedAccountsForOrganizationRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
```

### Comparing `types-aiobotocore-health-2.9.0/types_aiobotocore_health/type_defs.pyi` & `types-aiobotocore-health-2.9.1/types_aiobotocore_health/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-health-2.9.0/types_aiobotocore_health.egg-info/PKG-INFO` & `types-aiobotocore-health-2.9.1/types_aiobotocore_health.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-health
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Health 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Health 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/
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
 
 <a id="types-aiobotocore-health"></a>
 
 # types-aiobotocore-health
 
 [![PyPI - types-aiobotocore-health](https://img.shields.io/pypi/v/types-aiobotocore-health.svg?color=blue)](https://pypi.org/project/types-aiobotocore-health)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-health.svg?color=blue)](https://pypi.org/project/types-aiobotocore-health)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-health)](https://pepy.tech/project/types-aiobotocore-health)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Health 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health)
+[aiobotocore.Health 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health)
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
 [types-aiobotocore-health docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-health-2.9.0/types_aiobotocore_health.egg-info/SOURCES.txt` & `types-aiobotocore-health-2.9.1/types_aiobotocore_health.egg-info/SOURCES.txt`

 * *Files identical despite different names*

