# Comparing `tmp/types-aiobotocore-pi-2.9.0.tar.gz` & `tmp/types-aiobotocore-pi-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-pi-2.9.0.tar", last modified: Wed Dec 13 20:00:08 2023, max compression
+gzip compressed data, was "types-aiobotocore-pi-2.9.1.tar", last modified: Thu Jan 18 01:21:29 2024, max compression
```

## Comparing `types-aiobotocore-pi-2.9.0.tar` & `types-aiobotocore-pi-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:08.593327 types-aiobotocore-pi-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:51:34.000000 types-aiobotocore-pi-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11940 2023-12-13 20:00:08.593327 types-aiobotocore-pi-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10397 2023-12-13 19:51:34.000000 types-aiobotocore-pi-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:08.593327 types-aiobotocore-pi-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2023-12-13 19:51:34.000000 types-aiobotocore-pi-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:08.593327 types-aiobotocore-pi-2.9.0/types_aiobotocore_pi/
--rw-r--r--   0 runner    (1001) docker     (127)      403 2023-12-13 19:51:34.000000 types-aiobotocore-pi-2.9.0/types_aiobotocore_pi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2023-12-13 19:51:34.000000 types-aiobotocore-pi-2.9.0/types_aiobotocore_pi/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      901 2023-12-13 19:51:35.000000 types-aiobotocore-pi-2.9.0/types_aiobotocore_pi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13564 2023-12-13 19:51:35.000000 types-aiobotocore-pi-2.9.0/types_aiobotocore_pi/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13560 2023-12-13 19:51:35.000000 types-aiobotocore-pi-2.9.0/types_aiobotocore_pi/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9421 2023-12-13 19:51:35.000000 types-aiobotocore-pi-2.9.0/types_aiobotocore_pi/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9419 2023-12-13 19:51:35.000000 types-aiobotocore-pi-2.9.0/types_aiobotocore_pi/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:51:35.000000 types-aiobotocore-pi-2.9.0/types_aiobotocore_pi/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    14213 2023-12-13 19:51:35.000000 types-aiobotocore-pi-2.9.0/types_aiobotocore_pi/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    14212 2023-12-13 19:51:35.000000 types-aiobotocore-pi-2.9.0/types_aiobotocore_pi/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:51:34.000000 types-aiobotocore-pi-2.9.0/types_aiobotocore_pi/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:08.593327 types-aiobotocore-pi-2.9.0/types_aiobotocore_pi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11940 2023-12-13 20:00:08.000000 types-aiobotocore-pi-2.9.0/types_aiobotocore_pi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      649 2023-12-13 20:00:08.000000 types-aiobotocore-pi-2.9.0/types_aiobotocore_pi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:08.000000 types-aiobotocore-pi-2.9.0/types_aiobotocore_pi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:08.000000 types-aiobotocore-pi-2.9.0/types_aiobotocore_pi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:08.000000 types-aiobotocore-pi-2.9.0/types_aiobotocore_pi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-12-13 20:00:08.000000 types-aiobotocore-pi-2.9.0/types_aiobotocore_pi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:29.017123 types-aiobotocore-pi-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:13:12.000000 types-aiobotocore-pi-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11960 2024-01-18 01:21:29.017123 types-aiobotocore-pi-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10397 2024-01-18 01:13:12.000000 types-aiobotocore-pi-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:29.017123 types-aiobotocore-pi-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-01-18 01:13:12.000000 types-aiobotocore-pi-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:29.017123 types-aiobotocore-pi-2.9.1/types_aiobotocore_pi/
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-01-18 01:13:12.000000 types-aiobotocore-pi-2.9.1/types_aiobotocore_pi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-01-18 01:13:12.000000 types-aiobotocore-pi-2.9.1/types_aiobotocore_pi/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-01-18 01:13:12.000000 types-aiobotocore-pi-2.9.1/types_aiobotocore_pi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13571 2024-01-18 01:13:12.000000 types-aiobotocore-pi-2.9.1/types_aiobotocore_pi/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13568 2024-01-18 01:13:12.000000 types-aiobotocore-pi-2.9.1/types_aiobotocore_pi/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9419 2024-01-18 01:13:12.000000 types-aiobotocore-pi-2.9.1/types_aiobotocore_pi/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9419 2024-01-18 01:13:12.000000 types-aiobotocore-pi-2.9.1/types_aiobotocore_pi/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:13:12.000000 types-aiobotocore-pi-2.9.1/types_aiobotocore_pi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    14212 2024-01-18 01:13:13.000000 types-aiobotocore-pi-2.9.1/types_aiobotocore_pi/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14212 2024-01-18 01:13:13.000000 types-aiobotocore-pi-2.9.1/types_aiobotocore_pi/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:13:12.000000 types-aiobotocore-pi-2.9.1/types_aiobotocore_pi/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:29.017123 types-aiobotocore-pi-2.9.1/types_aiobotocore_pi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11960 2024-01-18 01:21:28.000000 types-aiobotocore-pi-2.9.1/types_aiobotocore_pi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-01-18 01:21:28.000000 types-aiobotocore-pi-2.9.1/types_aiobotocore_pi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:28.000000 types-aiobotocore-pi-2.9.1/types_aiobotocore_pi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:28.000000 types-aiobotocore-pi-2.9.1/types_aiobotocore_pi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:28.000000 types-aiobotocore-pi-2.9.1/types_aiobotocore_pi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-18 01:21:28.000000 types-aiobotocore-pi-2.9.1/types_aiobotocore_pi.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-pi-2.9.0/LICENSE` & `types-aiobotocore-pi-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-pi-2.9.0/PKG-INFO` & `types-aiobotocore-pi-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-pi
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.PI 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.PI 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pi/
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
 
 <a id="types-aiobotocore-pi"></a>
 
 # types-aiobotocore-pi
 
 [![PyPI - types-aiobotocore-pi](https://img.shields.io/pypi/v/types-aiobotocore-pi.svg?color=blue)](https://pypi.org/project/types-aiobotocore-pi)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-pi.svg?color=blue)](https://pypi.org/project/types-aiobotocore-pi)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pi/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-pi)](https://pepy.tech/project/types-aiobotocore-pi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.PI 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI)
+[aiobotocore.PI 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI)
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
 [types-aiobotocore-pi docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pi/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-pi-2.9.0/README.md` & `types-aiobotocore-pi-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-pi.svg?color=blue)](https://pypi.org/project/types-aiobotocore-pi)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pi/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-pi)](https://pepy.tech/project/types-aiobotocore-pi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.PI 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI)
+[aiobotocore.PI 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI)
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
 [types-aiobotocore-pi docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pi/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-pi-2.9.0/setup.py` & `types-aiobotocore-pi-2.9.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,47 +7,46 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-pi",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_pi"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.PI 2.9.0 service generated with mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.PI 2.9.1 service generated with mypy-boto3-builder 7.23.1"
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
     keywords="aiobotocore pi type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_pi": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pi/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-pi-2.9.0/types_aiobotocore_pi/__main__.py` & `types-aiobotocore-pi-2.9.1/types_aiobotocore_pi/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.PI 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.PI 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pi//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI\nOther"
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

### Comparing `types-aiobotocore-pi-2.9.0/types_aiobotocore_pi/client.py` & `types-aiobotocore-pi-2.9.1/types_aiobotocore_pi/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("PIClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -99,15 +98,15 @@
     async def create_performance_analysis_report(
         self,
         *,
         ServiceType: ServiceTypeType,
         Identifier: str,
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreatePerformanceAnalysisReportResponseTypeDef:
         """
         Creates a new performance analysis report for a specific time period for the DB
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client.create_performance_analysis_report)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pi/client/#create_performance_analysis_report)
@@ -133,15 +132,15 @@
         Metric: str,
         GroupBy: DimensionGroupTypeDef,
         PeriodInSeconds: int = ...,
         AdditionalMetrics: Sequence[str] = ...,
         PartitionBy: DimensionGroupTypeDef = ...,
         Filter: Mapping[str, str] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeDimensionKeysResponseTypeDef:
         """
         For a specific time period, retrieve the top `N` dimension keys for a metric.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client.describe_dimension_keys)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pi/client/#describe_dimension_keys)
         """
@@ -163,15 +162,15 @@
     async def get_dimension_key_details(
         self,
         *,
         ServiceType: ServiceTypeType,
         Identifier: str,
         Group: str,
         GroupIdentifier: str,
-        RequestedDimensions: Sequence[str] = ...
+        RequestedDimensions: Sequence[str] = ...,
     ) -> GetDimensionKeyDetailsResponseTypeDef:
         """
         Get the attributes of the specified dimension group for a DB instance or data
         source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client.get_dimension_key_details)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pi/client/#get_dimension_key_details)
@@ -180,15 +179,15 @@
     async def get_performance_analysis_report(
         self,
         *,
         ServiceType: ServiceTypeType,
         Identifier: str,
         AnalysisReportId: str,
         TextFormat: TextFormatType = ...,
-        AcceptLanguage: Literal["EN_US"] = ...
+        AcceptLanguage: Literal["EN_US"] = ...,
     ) -> GetPerformanceAnalysisReportResponseTypeDef:
         """
         Retrieves the report including the report ID, status, time details, and the
         insights with
         recommendations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client.get_performance_analysis_report)
@@ -212,15 +211,15 @@
         Identifier: str,
         MetricQueries: Sequence[MetricQueryTypeDef],
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
         PeriodInSeconds: int = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        PeriodAlignment: PeriodAlignmentType = ...
+        PeriodAlignment: PeriodAlignmentType = ...,
     ) -> GetResourceMetricsResponseTypeDef:
         """
         Retrieve Performance Insights metrics for a set of data sources over a time
         period.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client.get_resource_metrics)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pi/client/#get_resource_metrics)
@@ -229,15 +228,15 @@
     async def list_available_resource_dimensions(
         self,
         *,
         ServiceType: ServiceTypeType,
         Identifier: str,
         Metrics: Sequence[str],
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListAvailableResourceDimensionsResponseTypeDef:
         """
         Retrieve the dimensions that can be queried for each specified metric type on a
         specified DB
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client.list_available_resource_dimensions)
@@ -247,15 +246,15 @@
     async def list_available_resource_metrics(
         self,
         *,
         ServiceType: ServiceTypeType,
         Identifier: str,
         MetricTypes: Sequence[str],
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListAvailableResourceMetricsResponseTypeDef:
         """
         Retrieve metrics of the specified types that can be queried for a specified DB
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client.list_available_resource_metrics)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pi/client/#list_available_resource_metrics)
@@ -264,15 +263,15 @@
     async def list_performance_analysis_reports(
         self,
         *,
         ServiceType: ServiceTypeType,
         Identifier: str,
         NextToken: str = ...,
         MaxResults: int = ...,
-        ListTags: bool = ...
+        ListTags: bool = ...,
     ) -> ListPerformanceAnalysisReportsResponseTypeDef:
         """
         Lists all the analysis reports created for the DB instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client.list_performance_analysis_reports)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pi/client/#list_performance_analysis_reports)
         """
```

### Comparing `types-aiobotocore-pi-2.9.0/types_aiobotocore_pi/client.pyi` & `types-aiobotocore-pi-2.9.1/types_aiobotocore_pi/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
     async def create_performance_analysis_report(
         self,
         *,
         ServiceType: ServiceTypeType,
         Identifier: str,
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreatePerformanceAnalysisReportResponseTypeDef:
         """
         Creates a new performance analysis report for a specific time period for the DB
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client.create_performance_analysis_report)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pi/client/#create_performance_analysis_report)
@@ -129,15 +129,15 @@
         Metric: str,
         GroupBy: DimensionGroupTypeDef,
         PeriodInSeconds: int = ...,
         AdditionalMetrics: Sequence[str] = ...,
         PartitionBy: DimensionGroupTypeDef = ...,
         Filter: Mapping[str, str] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeDimensionKeysResponseTypeDef:
         """
         For a specific time period, retrieve the top `N` dimension keys for a metric.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client.describe_dimension_keys)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pi/client/#describe_dimension_keys)
         """
@@ -159,15 +159,15 @@
     async def get_dimension_key_details(
         self,
         *,
         ServiceType: ServiceTypeType,
         Identifier: str,
         Group: str,
         GroupIdentifier: str,
-        RequestedDimensions: Sequence[str] = ...
+        RequestedDimensions: Sequence[str] = ...,
     ) -> GetDimensionKeyDetailsResponseTypeDef:
         """
         Get the attributes of the specified dimension group for a DB instance or data
         source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client.get_dimension_key_details)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pi/client/#get_dimension_key_details)
@@ -176,15 +176,15 @@
     async def get_performance_analysis_report(
         self,
         *,
         ServiceType: ServiceTypeType,
         Identifier: str,
         AnalysisReportId: str,
         TextFormat: TextFormatType = ...,
-        AcceptLanguage: Literal["EN_US"] = ...
+        AcceptLanguage: Literal["EN_US"] = ...,
     ) -> GetPerformanceAnalysisReportResponseTypeDef:
         """
         Retrieves the report including the report ID, status, time details, and the
         insights with
         recommendations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client.get_performance_analysis_report)
@@ -208,15 +208,15 @@
         Identifier: str,
         MetricQueries: Sequence[MetricQueryTypeDef],
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
         PeriodInSeconds: int = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        PeriodAlignment: PeriodAlignmentType = ...
+        PeriodAlignment: PeriodAlignmentType = ...,
     ) -> GetResourceMetricsResponseTypeDef:
         """
         Retrieve Performance Insights metrics for a set of data sources over a time
         period.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client.get_resource_metrics)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pi/client/#get_resource_metrics)
@@ -225,15 +225,15 @@
     async def list_available_resource_dimensions(
         self,
         *,
         ServiceType: ServiceTypeType,
         Identifier: str,
         Metrics: Sequence[str],
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListAvailableResourceDimensionsResponseTypeDef:
         """
         Retrieve the dimensions that can be queried for each specified metric type on a
         specified DB
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client.list_available_resource_dimensions)
@@ -243,15 +243,15 @@
     async def list_available_resource_metrics(
         self,
         *,
         ServiceType: ServiceTypeType,
         Identifier: str,
         MetricTypes: Sequence[str],
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListAvailableResourceMetricsResponseTypeDef:
         """
         Retrieve metrics of the specified types that can be queried for a specified DB
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client.list_available_resource_metrics)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pi/client/#list_available_resource_metrics)
@@ -260,15 +260,15 @@
     async def list_performance_analysis_reports(
         self,
         *,
         ServiceType: ServiceTypeType,
         Identifier: str,
         NextToken: str = ...,
         MaxResults: int = ...,
-        ListTags: bool = ...
+        ListTags: bool = ...,
     ) -> ListPerformanceAnalysisReportsResponseTypeDef:
         """
         Lists all the analysis reports created for the DB instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client.list_performance_analysis_reports)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pi/client/#list_performance_analysis_reports)
         """
```

### Comparing `types-aiobotocore-pi-2.9.0/types_aiobotocore_pi/literals.py` & `types-aiobotocore-pi-2.9.1/types_aiobotocore_pi/literals.py`

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
     "AcceptLanguageType",
     "AnalysisStatusType",
     "ContextTypeType",
     "DetailStatusType",
     "FeatureStatusType",
     "PeriodAlignmentType",
@@ -32,15 +31,14 @@
     "TextFormatType",
     "PIServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 AcceptLanguageType = Literal["EN_US"]
 AnalysisStatusType = Literal["FAILED", "RUNNING", "SUCCEEDED"]
 ContextTypeType = Literal["CAUSAL", "CONTEXTUAL"]
 DetailStatusType = Literal["AVAILABLE", "PROCESSING", "UNAVAILABLE"]
 FeatureStatusType = Literal[
     "DISABLED",
     "DISABLED_PENDING_REBOOT",
```

### Comparing `types-aiobotocore-pi-2.9.0/types_aiobotocore_pi/literals.pyi` & `types-aiobotocore-pi-2.9.1/types_aiobotocore_pi/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pi-2.9.0/types_aiobotocore_pi/type_defs.py` & `types-aiobotocore-pi-2.9.1/types_aiobotocore_pi/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "TagTypeDef",
     "AnalysisReportTypeDef",
     "TimestampTypeDef",
     "ResponseMetadataTypeDef",
     "DataPointTypeDef",
     "PerformanceInsightsMetricTypeDef",
```

### Comparing `types-aiobotocore-pi-2.9.0/types_aiobotocore_pi/type_defs.pyi` & `types-aiobotocore-pi-2.9.1/types_aiobotocore_pi/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pi-2.9.0/types_aiobotocore_pi.egg-info/PKG-INFO` & `types-aiobotocore-pi-2.9.1/types_aiobotocore_pi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-pi
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.PI 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.PI 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pi/
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
 
 <a id="types-aiobotocore-pi"></a>
 
 # types-aiobotocore-pi
 
 [![PyPI - types-aiobotocore-pi](https://img.shields.io/pypi/v/types-aiobotocore-pi.svg?color=blue)](https://pypi.org/project/types-aiobotocore-pi)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-pi.svg?color=blue)](https://pypi.org/project/types-aiobotocore-pi)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pi/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-pi)](https://pepy.tech/project/types-aiobotocore-pi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.PI 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI)
+[aiobotocore.PI 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI)
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
 [types-aiobotocore-pi docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pi/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-pi-2.9.0/types_aiobotocore_pi.egg-info/SOURCES.txt` & `types-aiobotocore-pi-2.9.1/types_aiobotocore_pi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

