# Comparing `tmp/types-aiobotocore-forecast-2.9.0.tar.gz` & `tmp/types-aiobotocore-forecast-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-forecast-2.9.0.tar", last modified: Wed Dec 13 19:59:20 2023, max compression
+gzip compressed data, was "types-aiobotocore-forecast-2.9.1.tar", last modified: Thu Jan 18 01:20:44 2024, max compression
```

## Comparing `types-aiobotocore-forecast-2.9.0.tar` & `types-aiobotocore-forecast-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:20.521746 types-aiobotocore-forecast-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:46:21.000000 types-aiobotocore-forecast-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15185 2023-12-13 19:59:20.521746 types-aiobotocore-forecast-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13611 2023-12-13 19:46:21.000000 types-aiobotocore-forecast-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:20.521746 types-aiobotocore-forecast-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2023-12-13 19:46:21.000000 types-aiobotocore-forecast-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:20.521746 types-aiobotocore-forecast-2.9.0/types_aiobotocore_forecast/
--rw-r--r--   0 runner    (1001) docker     (127)     3669 2023-12-13 19:46:21.000000 types-aiobotocore-forecast-2.9.0/types_aiobotocore_forecast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3668 2023-12-13 19:46:21.000000 types-aiobotocore-forecast-2.9.0/types_aiobotocore_forecast/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      950 2023-12-13 19:46:21.000000 types-aiobotocore-forecast-2.9.0/types_aiobotocore_forecast/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    54569 2023-12-13 19:46:21.000000 types-aiobotocore-forecast-2.9.0/types_aiobotocore_forecast/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    54565 2023-12-13 19:46:21.000000 types-aiobotocore-forecast-2.9.0/types_aiobotocore_forecast/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2023-12-13 19:46:21.000000 types-aiobotocore-forecast-2.9.0/types_aiobotocore_forecast/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    12109 2023-12-13 19:46:21.000000 types-aiobotocore-forecast-2.9.0/types_aiobotocore_forecast/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    17810 2023-12-13 19:46:21.000000 types-aiobotocore-forecast-2.9.0/types_aiobotocore_forecast/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    17794 2023-12-13 19:46:21.000000 types-aiobotocore-forecast-2.9.0/types_aiobotocore_forecast/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:46:21.000000 types-aiobotocore-forecast-2.9.0/types_aiobotocore_forecast/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    59970 2023-12-13 19:46:24.000000 types-aiobotocore-forecast-2.9.0/types_aiobotocore_forecast/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    59969 2023-12-13 19:46:22.000000 types-aiobotocore-forecast-2.9.0/types_aiobotocore_forecast/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:46:21.000000 types-aiobotocore-forecast-2.9.0/types_aiobotocore_forecast/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:20.521746 types-aiobotocore-forecast-2.9.0/types_aiobotocore_forecast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15185 2023-12-13 19:59:20.000000 types-aiobotocore-forecast-2.9.0/types_aiobotocore_forecast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      832 2023-12-13 19:59:20.000000 types-aiobotocore-forecast-2.9.0/types_aiobotocore_forecast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:20.000000 types-aiobotocore-forecast-2.9.0/types_aiobotocore_forecast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:20.000000 types-aiobotocore-forecast-2.9.0/types_aiobotocore_forecast.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:20.000000 types-aiobotocore-forecast-2.9.0/types_aiobotocore_forecast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-13 19:59:20.000000 types-aiobotocore-forecast-2.9.0/types_aiobotocore_forecast.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:44.885323 types-aiobotocore-forecast-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:08:15.000000 types-aiobotocore-forecast-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15205 2024-01-18 01:20:44.885323 types-aiobotocore-forecast-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13611 2024-01-18 01:08:15.000000 types-aiobotocore-forecast-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:44.885323 types-aiobotocore-forecast-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-01-18 01:08:14.000000 types-aiobotocore-forecast-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:44.885323 types-aiobotocore-forecast-2.9.1/types_aiobotocore_forecast/
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-01-18 01:08:15.000000 types-aiobotocore-forecast-2.9.1/types_aiobotocore_forecast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-01-18 01:08:15.000000 types-aiobotocore-forecast-2.9.1/types_aiobotocore_forecast/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-01-18 01:08:15.000000 types-aiobotocore-forecast-2.9.1/types_aiobotocore_forecast/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54582 2024-01-18 01:08:15.000000 types-aiobotocore-forecast-2.9.1/types_aiobotocore_forecast/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54579 2024-01-18 01:08:15.000000 types-aiobotocore-forecast-2.9.1/types_aiobotocore_forecast/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12109 2024-01-18 01:08:15.000000 types-aiobotocore-forecast-2.9.1/types_aiobotocore_forecast/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12109 2024-01-18 01:08:15.000000 types-aiobotocore-forecast-2.9.1/types_aiobotocore_forecast/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    17821 2024-01-18 01:08:15.000000 types-aiobotocore-forecast-2.9.1/types_aiobotocore_forecast/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17806 2024-01-18 01:08:15.000000 types-aiobotocore-forecast-2.9.1/types_aiobotocore_forecast/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:08:15.000000 types-aiobotocore-forecast-2.9.1/types_aiobotocore_forecast/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    59969 2024-01-18 01:08:16.000000 types-aiobotocore-forecast-2.9.1/types_aiobotocore_forecast/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59969 2024-01-18 01:08:16.000000 types-aiobotocore-forecast-2.9.1/types_aiobotocore_forecast/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:08:15.000000 types-aiobotocore-forecast-2.9.1/types_aiobotocore_forecast/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:44.885323 types-aiobotocore-forecast-2.9.1/types_aiobotocore_forecast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15205 2024-01-18 01:20:44.000000 types-aiobotocore-forecast-2.9.1/types_aiobotocore_forecast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-01-18 01:20:44.000000 types-aiobotocore-forecast-2.9.1/types_aiobotocore_forecast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:44.000000 types-aiobotocore-forecast-2.9.1/types_aiobotocore_forecast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:44.000000 types-aiobotocore-forecast-2.9.1/types_aiobotocore_forecast.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:44.000000 types-aiobotocore-forecast-2.9.1/types_aiobotocore_forecast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-18 01:20:44.000000 types-aiobotocore-forecast-2.9.1/types_aiobotocore_forecast.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-forecast-2.9.0/LICENSE` & `types-aiobotocore-forecast-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-forecast-2.9.0/PKG-INFO` & `types-aiobotocore-forecast-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-forecast
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ForecastService 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ForecastService 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/
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
 
 <a id="types-aiobotocore-forecast"></a>
 
 # types-aiobotocore-forecast
 
 [![PyPI - types-aiobotocore-forecast](https://img.shields.io/pypi/v/types-aiobotocore-forecast.svg?color=blue)](https://pypi.org/project/types-aiobotocore-forecast)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-forecast.svg?color=blue)](https://pypi.org/project/types-aiobotocore-forecast)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-forecast)](https://pepy.tech/project/types-aiobotocore-forecast)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ForecastService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService)
+[aiobotocore.ForecastService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService)
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
 [types-aiobotocore-forecast docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-forecast-2.9.0/README.md` & `types-aiobotocore-forecast-2.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-forecast.svg?color=blue)](https://pypi.org/project/types-aiobotocore-forecast)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-forecast)](https://pepy.tech/project/types-aiobotocore-forecast)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ForecastService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService)
+[aiobotocore.ForecastService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService)
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
 [types-aiobotocore-forecast docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-forecast-2.9.0/setup.py` & `types-aiobotocore-forecast-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-forecast",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_forecast"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ForecastService 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.ForecastService 2.9.1 service generated with"
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
     keywords="aiobotocore forecast type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_forecast": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-forecast-2.9.0/types_aiobotocore_forecast/__init__.py` & `types-aiobotocore-forecast-2.9.1/types_aiobotocore_forecast/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,14 @@
     ListWhatIfAnalysesPaginator,
     ListWhatIfForecastExportsPaginator,
     ListWhatIfForecastsPaginator,
 )
 
 Client = ForecastServiceClient
 
-
 __all__ = (
     "Client",
     "ForecastServiceClient",
     "ListDatasetGroupsPaginator",
     "ListDatasetImportJobsPaginator",
     "ListDatasetsPaginator",
     "ListExplainabilitiesPaginator",
```

### Comparing `types-aiobotocore-forecast-2.9.0/types_aiobotocore_forecast/__init__.pyi` & `types-aiobotocore-forecast-2.9.1/types_aiobotocore_forecast/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-forecast-2.9.0/types_aiobotocore_forecast/__main__.py` & `types-aiobotocore-forecast-2.9.1/types_aiobotocore_forecast/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ForecastService 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.ForecastService 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService\nOther"
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

### Comparing `types-aiobotocore-forecast-2.9.0/types_aiobotocore_forecast/client.py` & `types-aiobotocore-forecast-2.9.1/types_aiobotocore_forecast/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ForecastServiceClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -180,15 +179,15 @@
         DataConfig: DataConfigTypeDef = ...,
         EncryptionConfig: EncryptionConfigTypeDef = ...,
         ReferencePredictorArn: str = ...,
         OptimizationMetric: OptimizationMetricType = ...,
         ExplainPredictor: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
         MonitorConfig: MonitorConfigTypeDef = ...,
-        TimeAlignmentBoundary: TimeAlignmentBoundaryTypeDef = ...
+        TimeAlignmentBoundary: TimeAlignmentBoundaryTypeDef = ...,
     ) -> CreateAutoPredictorResponseTypeDef:
         """
         Creates an Amazon Forecast predictor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.create_auto_predictor)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/client/#create_auto_predictor)
         """
@@ -198,30 +197,30 @@
         *,
         DatasetName: str,
         Domain: DomainType,
         DatasetType: DatasetTypeType,
         Schema: SchemaTypeDef,
         DataFrequency: str = ...,
         EncryptionConfig: EncryptionConfigTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDatasetResponseTypeDef:
         """
         Creates an Amazon Forecast dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.create_dataset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/client/#create_dataset)
         """
 
     async def create_dataset_group(
         self,
         *,
         DatasetGroupName: str,
         Domain: DomainType,
         DatasetArns: Sequence[str] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDatasetGroupResponseTypeDef:
         """
         Creates a dataset group, which holds a collection of related datasets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.create_dataset_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/client/#create_dataset_group)
         """
@@ -234,15 +233,15 @@
         DataSource: DataSourceTypeDef,
         TimestampFormat: str = ...,
         TimeZone: str = ...,
         UseGeolocationForTimeZone: bool = ...,
         GeolocationFormat: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         Format: str = ...,
-        ImportMode: ImportModeType = ...
+        ImportMode: ImportModeType = ...,
     ) -> CreateDatasetImportJobResponseTypeDef:
         """
         Imports your training data to an Amazon Forecast dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.create_dataset_import_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/client/#create_dataset_import_job)
         """
@@ -254,15 +253,15 @@
         ResourceArn: str,
         ExplainabilityConfig: ExplainabilityConfigTypeDef,
         DataSource: DataSourceTypeDef = ...,
         Schema: SchemaTypeDef = ...,
         EnableVisualization: bool = ...,
         StartDateTime: str = ...,
         EndDateTime: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateExplainabilityResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.create_explainability)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/client/#create_explainability)
         """
@@ -270,15 +269,15 @@
     async def create_explainability_export(
         self,
         *,
         ExplainabilityExportName: str,
         ExplainabilityArn: str,
         Destination: DataDestinationTypeDef,
         Tags: Sequence[TagTypeDef] = ...,
-        Format: str = ...
+        Format: str = ...,
     ) -> CreateExplainabilityExportResponseTypeDef:
         """
         Exports an Explainability resource created by the  CreateExplainability
         operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.create_explainability_export)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/client/#create_explainability_export)
@@ -287,15 +286,15 @@
     async def create_forecast(
         self,
         *,
         ForecastName: str,
         PredictorArn: str,
         ForecastTypes: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        TimeSeriesSelector: TimeSeriesSelectorTypeDef = ...
+        TimeSeriesSelector: TimeSeriesSelectorTypeDef = ...,
     ) -> CreateForecastResponseTypeDef:
         """
         Creates a forecast for each item in the `TARGET_TIME_SERIES` dataset that was
         used to train the
         predictor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.create_forecast)
@@ -305,15 +304,15 @@
     async def create_forecast_export_job(
         self,
         *,
         ForecastExportJobName: str,
         ForecastArn: str,
         Destination: DataDestinationTypeDef,
         Tags: Sequence[TagTypeDef] = ...,
-        Format: str = ...
+        Format: str = ...,
     ) -> CreateForecastExportJobResponseTypeDef:
         """
         Exports a forecast created by the  CreateForecast operation to your Amazon
         Simple Storage Service (Amazon S3)
         bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.create_forecast_export_job)
@@ -343,15 +342,15 @@
         AutoMLOverrideStrategy: AutoMLOverrideStrategyType = ...,
         PerformHPO: bool = ...,
         TrainingParameters: Mapping[str, str] = ...,
         EvaluationParameters: EvaluationParametersTypeDef = ...,
         HPOConfig: HyperParameterTuningJobConfigTypeDef = ...,
         EncryptionConfig: EncryptionConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        OptimizationMetric: OptimizationMetricType = ...
+        OptimizationMetric: OptimizationMetricType = ...,
     ) -> CreatePredictorResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.create_predictor)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/client/#create_predictor)
         """
@@ -359,15 +358,15 @@
     async def create_predictor_backtest_export_job(
         self,
         *,
         PredictorBacktestExportJobName: str,
         PredictorArn: str,
         Destination: DataDestinationTypeDef,
         Tags: Sequence[TagTypeDef] = ...,
-        Format: str = ...
+        Format: str = ...,
     ) -> CreatePredictorBacktestExportJobResponseTypeDef:
         """
         Exports backtest forecasts and accuracy metrics generated by the
         CreateAutoPredictor or  CreatePredictor
         operations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.create_predictor_backtest_export_job)
@@ -376,15 +375,15 @@
 
     async def create_what_if_analysis(
         self,
         *,
         WhatIfAnalysisName: str,
         ForecastArn: str,
         TimeSeriesSelector: TimeSeriesSelectorTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateWhatIfAnalysisResponseTypeDef:
         """
         What-if analysis is a scenario modeling technique where you make a hypothetical
         change to a time series and compare the forecasts generated by these changes
         against the baseline, unchanged time
         series.
 
@@ -395,15 +394,15 @@
     async def create_what_if_forecast(
         self,
         *,
         WhatIfForecastName: str,
         WhatIfAnalysisArn: str,
         TimeSeriesTransformations: Sequence[TimeSeriesTransformationTypeDef] = ...,
         TimeSeriesReplacementsDataSource: TimeSeriesReplacementsDataSourceTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateWhatIfForecastResponseTypeDef:
         """
         A what-if forecast is a forecast that is created from a modified version of the
         baseline
         forecast.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.create_what_if_forecast)
@@ -413,15 +412,15 @@
     async def create_what_if_forecast_export(
         self,
         *,
         WhatIfForecastExportName: str,
         WhatIfForecastArns: Sequence[str],
         Destination: DataDestinationTypeDef,
         Tags: Sequence[TagTypeDef] = ...,
-        Format: str = ...
+        Format: str = ...,
     ) -> CreateWhatIfForecastExportResponseTypeDef:
         """
         Exports a forecast created by the  CreateWhatIfForecast operation to your
         Amazon Simple Storage Service (Amazon S3)
         bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.create_what_if_forecast_export)
@@ -821,15 +820,15 @@
 
     async def list_monitor_evaluations(
         self,
         *,
         MonitorArn: str,
         NextToken: str = ...,
         MaxResults: int = ...,
-        Filters: Sequence[FilterTypeDef] = ...
+        Filters: Sequence[FilterTypeDef] = ...,
     ) -> ListMonitorEvaluationsResponseTypeDef:
         """
         Returns a list of the monitoring evaluation results and predictor events
         collected by the monitor resource during different windows of
         time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.list_monitor_evaluations)
```

### Comparing `types-aiobotocore-forecast-2.9.0/types_aiobotocore_forecast/client.pyi` & `types-aiobotocore-forecast-2.9.1/types_aiobotocore_forecast/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -176,15 +176,15 @@
         DataConfig: DataConfigTypeDef = ...,
         EncryptionConfig: EncryptionConfigTypeDef = ...,
         ReferencePredictorArn: str = ...,
         OptimizationMetric: OptimizationMetricType = ...,
         ExplainPredictor: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
         MonitorConfig: MonitorConfigTypeDef = ...,
-        TimeAlignmentBoundary: TimeAlignmentBoundaryTypeDef = ...
+        TimeAlignmentBoundary: TimeAlignmentBoundaryTypeDef = ...,
     ) -> CreateAutoPredictorResponseTypeDef:
         """
         Creates an Amazon Forecast predictor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.create_auto_predictor)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/client/#create_auto_predictor)
         """
@@ -194,30 +194,30 @@
         *,
         DatasetName: str,
         Domain: DomainType,
         DatasetType: DatasetTypeType,
         Schema: SchemaTypeDef,
         DataFrequency: str = ...,
         EncryptionConfig: EncryptionConfigTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDatasetResponseTypeDef:
         """
         Creates an Amazon Forecast dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.create_dataset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/client/#create_dataset)
         """
 
     async def create_dataset_group(
         self,
         *,
         DatasetGroupName: str,
         Domain: DomainType,
         DatasetArns: Sequence[str] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDatasetGroupResponseTypeDef:
         """
         Creates a dataset group, which holds a collection of related datasets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.create_dataset_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/client/#create_dataset_group)
         """
@@ -230,15 +230,15 @@
         DataSource: DataSourceTypeDef,
         TimestampFormat: str = ...,
         TimeZone: str = ...,
         UseGeolocationForTimeZone: bool = ...,
         GeolocationFormat: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         Format: str = ...,
-        ImportMode: ImportModeType = ...
+        ImportMode: ImportModeType = ...,
     ) -> CreateDatasetImportJobResponseTypeDef:
         """
         Imports your training data to an Amazon Forecast dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.create_dataset_import_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/client/#create_dataset_import_job)
         """
@@ -250,15 +250,15 @@
         ResourceArn: str,
         ExplainabilityConfig: ExplainabilityConfigTypeDef,
         DataSource: DataSourceTypeDef = ...,
         Schema: SchemaTypeDef = ...,
         EnableVisualization: bool = ...,
         StartDateTime: str = ...,
         EndDateTime: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateExplainabilityResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.create_explainability)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/client/#create_explainability)
         """
@@ -266,15 +266,15 @@
     async def create_explainability_export(
         self,
         *,
         ExplainabilityExportName: str,
         ExplainabilityArn: str,
         Destination: DataDestinationTypeDef,
         Tags: Sequence[TagTypeDef] = ...,
-        Format: str = ...
+        Format: str = ...,
     ) -> CreateExplainabilityExportResponseTypeDef:
         """
         Exports an Explainability resource created by the  CreateExplainability
         operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.create_explainability_export)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/client/#create_explainability_export)
@@ -283,15 +283,15 @@
     async def create_forecast(
         self,
         *,
         ForecastName: str,
         PredictorArn: str,
         ForecastTypes: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        TimeSeriesSelector: TimeSeriesSelectorTypeDef = ...
+        TimeSeriesSelector: TimeSeriesSelectorTypeDef = ...,
     ) -> CreateForecastResponseTypeDef:
         """
         Creates a forecast for each item in the `TARGET_TIME_SERIES` dataset that was
         used to train the
         predictor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.create_forecast)
@@ -301,15 +301,15 @@
     async def create_forecast_export_job(
         self,
         *,
         ForecastExportJobName: str,
         ForecastArn: str,
         Destination: DataDestinationTypeDef,
         Tags: Sequence[TagTypeDef] = ...,
-        Format: str = ...
+        Format: str = ...,
     ) -> CreateForecastExportJobResponseTypeDef:
         """
         Exports a forecast created by the  CreateForecast operation to your Amazon
         Simple Storage Service (Amazon S3)
         bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.create_forecast_export_job)
@@ -339,15 +339,15 @@
         AutoMLOverrideStrategy: AutoMLOverrideStrategyType = ...,
         PerformHPO: bool = ...,
         TrainingParameters: Mapping[str, str] = ...,
         EvaluationParameters: EvaluationParametersTypeDef = ...,
         HPOConfig: HyperParameterTuningJobConfigTypeDef = ...,
         EncryptionConfig: EncryptionConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        OptimizationMetric: OptimizationMetricType = ...
+        OptimizationMetric: OptimizationMetricType = ...,
     ) -> CreatePredictorResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.create_predictor)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/client/#create_predictor)
         """
@@ -355,15 +355,15 @@
     async def create_predictor_backtest_export_job(
         self,
         *,
         PredictorBacktestExportJobName: str,
         PredictorArn: str,
         Destination: DataDestinationTypeDef,
         Tags: Sequence[TagTypeDef] = ...,
-        Format: str = ...
+        Format: str = ...,
     ) -> CreatePredictorBacktestExportJobResponseTypeDef:
         """
         Exports backtest forecasts and accuracy metrics generated by the
         CreateAutoPredictor or  CreatePredictor
         operations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.create_predictor_backtest_export_job)
@@ -372,15 +372,15 @@
 
     async def create_what_if_analysis(
         self,
         *,
         WhatIfAnalysisName: str,
         ForecastArn: str,
         TimeSeriesSelector: TimeSeriesSelectorTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateWhatIfAnalysisResponseTypeDef:
         """
         What-if analysis is a scenario modeling technique where you make a hypothetical
         change to a time series and compare the forecasts generated by these changes
         against the baseline, unchanged time
         series.
 
@@ -391,15 +391,15 @@
     async def create_what_if_forecast(
         self,
         *,
         WhatIfForecastName: str,
         WhatIfAnalysisArn: str,
         TimeSeriesTransformations: Sequence[TimeSeriesTransformationTypeDef] = ...,
         TimeSeriesReplacementsDataSource: TimeSeriesReplacementsDataSourceTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateWhatIfForecastResponseTypeDef:
         """
         A what-if forecast is a forecast that is created from a modified version of the
         baseline
         forecast.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.create_what_if_forecast)
@@ -409,15 +409,15 @@
     async def create_what_if_forecast_export(
         self,
         *,
         WhatIfForecastExportName: str,
         WhatIfForecastArns: Sequence[str],
         Destination: DataDestinationTypeDef,
         Tags: Sequence[TagTypeDef] = ...,
-        Format: str = ...
+        Format: str = ...,
     ) -> CreateWhatIfForecastExportResponseTypeDef:
         """
         Exports a forecast created by the  CreateWhatIfForecast operation to your
         Amazon Simple Storage Service (Amazon S3)
         bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.create_what_if_forecast_export)
@@ -817,15 +817,15 @@
 
     async def list_monitor_evaluations(
         self,
         *,
         MonitorArn: str,
         NextToken: str = ...,
         MaxResults: int = ...,
-        Filters: Sequence[FilterTypeDef] = ...
+        Filters: Sequence[FilterTypeDef] = ...,
     ) -> ListMonitorEvaluationsResponseTypeDef:
         """
         Returns a list of the monitoring evaluation results and predictor events
         collected by the monitor resource during different windows of
         time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.list_monitor_evaluations)
```

### Comparing `types-aiobotocore-forecast-2.9.0/types_aiobotocore_forecast/literals.py` & `types-aiobotocore-forecast-2.9.1/types_aiobotocore_forecast/literals.py`

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
     "AttributeTypeType",
     "AutoMLOverrideStrategyType",
     "ConditionType",
     "DatasetTypeType",
     "DayOfWeekType",
     "DomainType",
@@ -55,15 +54,14 @@
     "ForecastServiceServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AttributeTypeType = Literal["float", "geolocation", "integer", "string", "timestamp"]
 AutoMLOverrideStrategyType = Literal["AccuracyOptimized", "LatencyOptimized"]
 ConditionType = Literal["EQUALS", "GREATER_THAN", "LESS_THAN", "NOT_EQUALS"]
 DatasetTypeType = Literal["ITEM_METADATA", "RELATED_TIME_SERIES", "TARGET_TIME_SERIES"]
 DayOfWeekType = Literal[
     "FRIDAY", "MONDAY", "SATURDAY", "SUNDAY", "THURSDAY", "TUESDAY", "WEDNESDAY"
 ]
```

### Comparing `types-aiobotocore-forecast-2.9.0/types_aiobotocore_forecast/literals.pyi` & `types-aiobotocore-forecast-2.9.1/types_aiobotocore_forecast/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-forecast-2.9.0/types_aiobotocore_forecast/paginator.py` & `types-aiobotocore-forecast-2.9.1/types_aiobotocore_forecast/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,14 @@
     "ListPredictorBacktestExportJobsPaginator",
     "ListPredictorsPaginator",
     "ListWhatIfAnalysesPaginator",
     "ListWhatIfForecastExportsPaginator",
     "ListWhatIfForecastsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -120,15 +119,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listdatasetimportjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDatasetImportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListDatasetImportJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listdatasetimportjobspaginator)
         """
 
 
@@ -153,15 +152,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listexplainabilitiespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListExplainabilitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListExplainabilities.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listexplainabilitiespaginator)
         """
 
 
@@ -171,15 +170,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listexplainabilityexportspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListExplainabilityExportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListExplainabilityExports.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listexplainabilityexportspaginator)
         """
 
 
@@ -189,15 +188,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listforecastexportjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListForecastExportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListForecastExportJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listforecastexportjobspaginator)
         """
 
 
@@ -207,15 +206,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listforecastspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListForecastsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListForecasts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listforecastspaginator)
         """
 
 
@@ -226,15 +225,15 @@
     """
 
     def paginate(
         self,
         *,
         MonitorArn: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListMonitorEvaluationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListMonitorEvaluations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listmonitorevaluationspaginator)
         """
 
 
@@ -244,15 +243,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listmonitorspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListMonitorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListMonitors.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listmonitorspaginator)
         """
 
 
@@ -262,15 +261,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listpredictorbacktestexportjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPredictorBacktestExportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListPredictorBacktestExportJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listpredictorbacktestexportjobspaginator)
         """
 
 
@@ -280,15 +279,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listpredictorspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPredictorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListPredictors.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listpredictorspaginator)
         """
 
 
@@ -298,15 +297,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listwhatifanalysespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListWhatIfAnalysesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListWhatIfAnalyses.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listwhatifanalysespaginator)
         """
 
 
@@ -316,15 +315,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listwhatifforecastexportspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListWhatIfForecastExportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListWhatIfForecastExports.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listwhatifforecastexportspaginator)
         """
 
 
@@ -334,13 +333,13 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listwhatifforecastspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListWhatIfForecastsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListWhatIfForecasts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listwhatifforecastspaginator)
         """
```

### Comparing `types-aiobotocore-forecast-2.9.0/types_aiobotocore_forecast/paginator.pyi` & `types-aiobotocore-forecast-2.9.1/types_aiobotocore_forecast/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listdatasetimportjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDatasetImportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListDatasetImportJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listdatasetimportjobspaginator)
         """
 
 class ListDatasetsPaginator(AioPaginator):
@@ -147,15 +147,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listexplainabilitiespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListExplainabilitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListExplainabilities.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listexplainabilitiespaginator)
         """
 
 class ListExplainabilityExportsPaginator(AioPaginator):
@@ -164,15 +164,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listexplainabilityexportspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListExplainabilityExportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListExplainabilityExports.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listexplainabilityexportspaginator)
         """
 
 class ListForecastExportJobsPaginator(AioPaginator):
@@ -181,15 +181,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listforecastexportjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListForecastExportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListForecastExportJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listforecastexportjobspaginator)
         """
 
 class ListForecastsPaginator(AioPaginator):
@@ -198,15 +198,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listforecastspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListForecastsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListForecasts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listforecastspaginator)
         """
 
 class ListMonitorEvaluationsPaginator(AioPaginator):
@@ -216,15 +216,15 @@
     """
 
     def paginate(
         self,
         *,
         MonitorArn: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListMonitorEvaluationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListMonitorEvaluations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listmonitorevaluationspaginator)
         """
 
 class ListMonitorsPaginator(AioPaginator):
@@ -233,15 +233,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listmonitorspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListMonitorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListMonitors.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listmonitorspaginator)
         """
 
 class ListPredictorBacktestExportJobsPaginator(AioPaginator):
@@ -250,15 +250,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listpredictorbacktestexportjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPredictorBacktestExportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListPredictorBacktestExportJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listpredictorbacktestexportjobspaginator)
         """
 
 class ListPredictorsPaginator(AioPaginator):
@@ -267,15 +267,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listpredictorspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPredictorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListPredictors.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listpredictorspaginator)
         """
 
 class ListWhatIfAnalysesPaginator(AioPaginator):
@@ -284,15 +284,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listwhatifanalysespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListWhatIfAnalysesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListWhatIfAnalyses.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listwhatifanalysespaginator)
         """
 
 class ListWhatIfForecastExportsPaginator(AioPaginator):
@@ -301,15 +301,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listwhatifforecastexportspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListWhatIfForecastExportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListWhatIfForecastExports.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listwhatifforecastexportspaginator)
         """
 
 class ListWhatIfForecastsPaginator(AioPaginator):
@@ -318,13 +318,13 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listwhatifforecastspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListWhatIfForecastsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListWhatIfForecasts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listwhatifforecastspaginator)
         """
```

### Comparing `types-aiobotocore-forecast-2.9.0/types_aiobotocore_forecast/type_defs.py` & `types-aiobotocore-forecast-2.9.1/types_aiobotocore_forecast/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ActionTypeDef",
     "AdditionalDatasetTypeDef",
     "AttributeConfigTypeDef",
     "BaselineMetricTypeDef",
     "CategoricalParameterRangeTypeDef",
     "ContinuousParameterRangeTypeDef",
```

### Comparing `types-aiobotocore-forecast-2.9.0/types_aiobotocore_forecast/type_defs.pyi` & `types-aiobotocore-forecast-2.9.1/types_aiobotocore_forecast/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-forecast-2.9.0/types_aiobotocore_forecast.egg-info/PKG-INFO` & `types-aiobotocore-forecast-2.9.1/types_aiobotocore_forecast.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-forecast
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ForecastService 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ForecastService 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/
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
 
 <a id="types-aiobotocore-forecast"></a>
 
 # types-aiobotocore-forecast
 
 [![PyPI - types-aiobotocore-forecast](https://img.shields.io/pypi/v/types-aiobotocore-forecast.svg?color=blue)](https://pypi.org/project/types-aiobotocore-forecast)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-forecast.svg?color=blue)](https://pypi.org/project/types-aiobotocore-forecast)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-forecast)](https://pepy.tech/project/types-aiobotocore-forecast)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ForecastService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService)
+[aiobotocore.ForecastService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService)
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
 [types-aiobotocore-forecast docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-forecast-2.9.0/types_aiobotocore_forecast.egg-info/SOURCES.txt` & `types-aiobotocore-forecast-2.9.1/types_aiobotocore_forecast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

