# Comparing `tmp/types-aiobotocore-location-2.9.0.tar.gz` & `tmp/types-aiobotocore-location-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-location-2.9.0.tar", last modified: Wed Dec 13 19:59:46 2023, max compression
+gzip compressed data, was "types-aiobotocore-location-2.9.1.tar", last modified: Thu Jan 18 01:21:09 2024, max compression
```

## Comparing `types-aiobotocore-location-2.9.0.tar` & `types-aiobotocore-location-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:46.705518 types-aiobotocore-location-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:49:22.000000 types-aiobotocore-location-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14413 2023-12-13 19:59:46.705518 types-aiobotocore-location-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12839 2023-12-13 19:49:22.000000 types-aiobotocore-location-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:46.705518 types-aiobotocore-location-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2023-12-13 19:49:22.000000 types-aiobotocore-location-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:46.705518 types-aiobotocore-location-2.9.0/types_aiobotocore_location/
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2023-12-13 19:49:22.000000 types-aiobotocore-location-2.9.0/types_aiobotocore_location/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2023-12-13 19:49:22.000000 types-aiobotocore-location-2.9.0/types_aiobotocore_location/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      950 2023-12-13 19:49:22.000000 types-aiobotocore-location-2.9.0/types_aiobotocore_location/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    48614 2023-12-13 19:49:22.000000 types-aiobotocore-location-2.9.0/types_aiobotocore_location/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    48610 2023-12-13 19:49:22.000000 types-aiobotocore-location-2.9.0/types_aiobotocore_location/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10941 2023-12-13 19:49:22.000000 types-aiobotocore-location-2.9.0/types_aiobotocore_location/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10939 2023-12-13 19:49:22.000000 types-aiobotocore-location-2.9.0/types_aiobotocore_location/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12494 2023-12-13 19:49:22.000000 types-aiobotocore-location-2.9.0/types_aiobotocore_location/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12482 2023-12-13 19:49:22.000000 types-aiobotocore-location-2.9.0/types_aiobotocore_location/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:49:22.000000 types-aiobotocore-location-2.9.0/types_aiobotocore_location/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    52626 2023-12-13 19:49:23.000000 types-aiobotocore-location-2.9.0/types_aiobotocore_location/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    52625 2023-12-13 19:49:23.000000 types-aiobotocore-location-2.9.0/types_aiobotocore_location/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:49:22.000000 types-aiobotocore-location-2.9.0/types_aiobotocore_location/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:46.705518 types-aiobotocore-location-2.9.0/types_aiobotocore_location.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14413 2023-12-13 19:59:46.000000 types-aiobotocore-location-2.9.0/types_aiobotocore_location.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      832 2023-12-13 19:59:46.000000 types-aiobotocore-location-2.9.0/types_aiobotocore_location.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:46.000000 types-aiobotocore-location-2.9.0/types_aiobotocore_location.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:46.000000 types-aiobotocore-location-2.9.0/types_aiobotocore_location.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:46.000000 types-aiobotocore-location-2.9.0/types_aiobotocore_location.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-13 19:59:46.000000 types-aiobotocore-location-2.9.0/types_aiobotocore_location.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:09.137214 types-aiobotocore-location-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:11:08.000000 types-aiobotocore-location-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14433 2024-01-18 01:21:09.137214 types-aiobotocore-location-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12839 2024-01-18 01:11:08.000000 types-aiobotocore-location-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:09.137214 types-aiobotocore-location-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-01-18 01:11:08.000000 types-aiobotocore-location-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:09.137214 types-aiobotocore-location-2.9.1/types_aiobotocore_location/
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-01-18 01:11:08.000000 types-aiobotocore-location-2.9.1/types_aiobotocore_location/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-01-18 01:11:08.000000 types-aiobotocore-location-2.9.1/types_aiobotocore_location/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-01-18 01:11:08.000000 types-aiobotocore-location-2.9.1/types_aiobotocore_location/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48632 2024-01-18 01:11:08.000000 types-aiobotocore-location-2.9.1/types_aiobotocore_location/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48629 2024-01-18 01:11:08.000000 types-aiobotocore-location-2.9.1/types_aiobotocore_location/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10939 2024-01-18 01:11:09.000000 types-aiobotocore-location-2.9.1/types_aiobotocore_location/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10939 2024-01-18 01:11:08.000000 types-aiobotocore-location-2.9.1/types_aiobotocore_location/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12495 2024-01-18 01:11:08.000000 types-aiobotocore-location-2.9.1/types_aiobotocore_location/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12484 2024-01-18 01:11:08.000000 types-aiobotocore-location-2.9.1/types_aiobotocore_location/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:11:08.000000 types-aiobotocore-location-2.9.1/types_aiobotocore_location/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    52625 2024-01-18 01:11:09.000000 types-aiobotocore-location-2.9.1/types_aiobotocore_location/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52625 2024-01-18 01:11:09.000000 types-aiobotocore-location-2.9.1/types_aiobotocore_location/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:11:08.000000 types-aiobotocore-location-2.9.1/types_aiobotocore_location/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:09.137214 types-aiobotocore-location-2.9.1/types_aiobotocore_location.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14433 2024-01-18 01:21:09.000000 types-aiobotocore-location-2.9.1/types_aiobotocore_location.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-01-18 01:21:09.000000 types-aiobotocore-location-2.9.1/types_aiobotocore_location.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:09.000000 types-aiobotocore-location-2.9.1/types_aiobotocore_location.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:09.000000 types-aiobotocore-location-2.9.1/types_aiobotocore_location.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:09.000000 types-aiobotocore-location-2.9.1/types_aiobotocore_location.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-18 01:21:09.000000 types-aiobotocore-location-2.9.1/types_aiobotocore_location.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-location-2.9.0/LICENSE` & `types-aiobotocore-location-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-location-2.9.0/PKG-INFO` & `types-aiobotocore-location-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-location
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.LocationService 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.LocationService 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/
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
 
 <a id="types-aiobotocore-location"></a>
 
 # types-aiobotocore-location
 
 [![PyPI - types-aiobotocore-location](https://img.shields.io/pypi/v/types-aiobotocore-location.svg?color=blue)](https://pypi.org/project/types-aiobotocore-location)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-location.svg?color=blue)](https://pypi.org/project/types-aiobotocore-location)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-location)](https://pepy.tech/project/types-aiobotocore-location)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LocationService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
+[aiobotocore.LocationService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
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
 [types-aiobotocore-location docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-location-2.9.0/README.md` & `types-aiobotocore-location-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-location.svg?color=blue)](https://pypi.org/project/types-aiobotocore-location)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-location)](https://pepy.tech/project/types-aiobotocore-location)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LocationService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
+[aiobotocore.LocationService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
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
 [types-aiobotocore-location docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-location-2.9.0/setup.py` & `types-aiobotocore-location-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-location",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_location"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.LocationService 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.LocationService 2.9.1 service generated with"
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
     keywords="aiobotocore location type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_location": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-location-2.9.0/types_aiobotocore_location/__init__.py` & `types-aiobotocore-location-2.9.1/types_aiobotocore_location/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,14 @@
     ListRouteCalculatorsPaginator,
     ListTrackerConsumersPaginator,
     ListTrackersPaginator,
 )
 
 Client = LocationServiceClient
 
-
 __all__ = (
     "Client",
     "GetDevicePositionHistoryPaginator",
     "ListDevicePositionsPaginator",
     "ListGeofenceCollectionsPaginator",
     "ListGeofencesPaginator",
     "ListKeysPaginator",
```

### Comparing `types-aiobotocore-location-2.9.0/types_aiobotocore_location/__init__.pyi` & `types-aiobotocore-location-2.9.1/types_aiobotocore_location/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-location-2.9.0/types_aiobotocore_location/__main__.py` & `types-aiobotocore-location-2.9.1/types_aiobotocore_location/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.LocationService 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.LocationService 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService\nOther"
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

### Comparing `types-aiobotocore-location-2.9.0/types_aiobotocore_location/client.py` & `types-aiobotocore-location-2.9.1/types_aiobotocore_location/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("LocationServiceClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -237,15 +236,15 @@
         DepartureTime: TimestampTypeDef = ...,
         DistanceUnit: DistanceUnitType = ...,
         IncludeLegGeometry: bool = ...,
         Key: str = ...,
         OptimizeFor: OptimizationModeType = ...,
         TravelMode: TravelModeType = ...,
         TruckModeOptions: CalculateRouteTruckModeOptionsTypeDef = ...,
-        WaypointPositions: Sequence[Sequence[float]] = ...
+        WaypointPositions: Sequence[Sequence[float]] = ...,
     ) -> CalculateRouteResponseTypeDef:
         """
         [Calculates a
         route](https://docs.aws.amazon.com/location/latest/developerguide/calculate-route.html)
         given the following required parameters: `DeparturePosition` and
         `DestinationPosition`.
 
@@ -261,15 +260,15 @@
         DestinationPositions: Sequence[Sequence[float]],
         CarModeOptions: CalculateRouteCarModeOptionsTypeDef = ...,
         DepartNow: bool = ...,
         DepartureTime: TimestampTypeDef = ...,
         DistanceUnit: DistanceUnitType = ...,
         Key: str = ...,
         TravelMode: TravelModeType = ...,
-        TruckModeOptions: CalculateRouteTruckModeOptionsTypeDef = ...
+        TruckModeOptions: CalculateRouteTruckModeOptionsTypeDef = ...,
     ) -> CalculateRouteMatrixResponseTypeDef:
         """
         [Calculates a route
         matrix](https://docs.aws.amazon.com/location/latest/developerguide/calculate-route-matrix.html)
         given the following required parameters: `DeparturePositions` and
         `DestinationPositions`.
 
@@ -297,15 +296,15 @@
         self,
         *,
         CollectionName: str,
         Description: str = ...,
         KmsKeyId: str = ...,
         PricingPlan: PricingPlanType = ...,
         PricingPlanDataSource: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateGeofenceCollectionResponseTypeDef:
         """
         Creates a geofence collection, which manages and stores geofences.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.create_geofence_collection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/client/#create_geofence_collection)
         """
@@ -314,15 +313,15 @@
         self,
         *,
         KeyName: str,
         Restrictions: ApiKeyRestrictionsTypeDef,
         Description: str = ...,
         ExpireTime: TimestampTypeDef = ...,
         NoExpiry: bool = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateKeyResponseTypeDef:
         """
         Creates an API key resource in your Amazon Web Services account, which lets you
         grant actions for Amazon Location resources to the API key
         bearer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.create_key)
@@ -332,15 +331,15 @@
     async def create_map(
         self,
         *,
         Configuration: MapConfigurationTypeDef,
         MapName: str,
         Description: str = ...,
         PricingPlan: PricingPlanType = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateMapResponseTypeDef:
         """
         Creates a map resource in your Amazon Web Services account, which provides map
         tiles of different styles sourced from global location data
         providers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.create_map)
@@ -351,15 +350,15 @@
         self,
         *,
         DataSource: str,
         IndexName: str,
         DataSourceConfiguration: DataSourceConfigurationTypeDef = ...,
         Description: str = ...,
         PricingPlan: PricingPlanType = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreatePlaceIndexResponseTypeDef:
         """
         Creates a place index resource in your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.create_place_index)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/client/#create_place_index)
         """
@@ -367,15 +366,15 @@
     async def create_route_calculator(
         self,
         *,
         CalculatorName: str,
         DataSource: str,
         Description: str = ...,
         PricingPlan: PricingPlanType = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateRouteCalculatorResponseTypeDef:
         """
         Creates a route calculator resource in your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.create_route_calculator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/client/#create_route_calculator)
         """
@@ -387,15 +386,15 @@
         Description: str = ...,
         EventBridgeEnabled: bool = ...,
         KmsKeyEnableGeospatialQueries: bool = ...,
         KmsKeyId: str = ...,
         PositionFiltering: PositionFilteringType = ...,
         PricingPlan: PricingPlanType = ...,
         PricingPlanDataSource: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateTrackerResponseTypeDef:
         """
         Creates a tracker resource in your Amazon Web Services account, which lets you
         retrieve current and historical location of
         devices.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.create_tracker)
@@ -540,15 +539,15 @@
         self,
         *,
         DeviceId: str,
         TrackerName: str,
         EndTimeExclusive: TimestampTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        StartTimeInclusive: TimestampTypeDef = ...
+        StartTimeInclusive: TimestampTypeDef = ...,
     ) -> GetDevicePositionHistoryResponseTypeDef:
         """
         Retrieves the device position history from a tracker resource within a
         specified range of
         time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.get_device_position_history)
@@ -617,15 +616,15 @@
 
     async def list_device_positions(
         self,
         *,
         TrackerName: str,
         FilterGeometry: TrackingFilterGeometryTypeDef = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListDevicePositionsResponseTypeDef:
         """
         A batch request to retrieve all device positions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.list_device_positions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/client/#list_device_positions)
         """
@@ -723,15 +722,15 @@
 
     async def put_geofence(
         self,
         *,
         CollectionName: str,
         GeofenceId: str,
         Geometry: GeofenceGeometryTypeDef,
-        GeofenceProperties: Mapping[str, str] = ...
+        GeofenceProperties: Mapping[str, str] = ...,
     ) -> PutGeofenceResponseTypeDef:
         """
         Stores a geofence geometry in a given geofence collection, or updates the
         geometry of an existing geofence if a geofence ID is included in the
         request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.put_geofence)
@@ -741,15 +740,15 @@
     async def search_place_index_for_position(
         self,
         *,
         IndexName: str,
         Position: Sequence[float],
         Key: str = ...,
         Language: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> SearchPlaceIndexForPositionResponseTypeDef:
         """
         Reverse geocodes a given coordinate and returns a legible address.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.search_place_index_for_position)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/client/#search_place_index_for_position)
         """
@@ -761,15 +760,15 @@
         Text: str,
         BiasPosition: Sequence[float] = ...,
         FilterBBox: Sequence[float] = ...,
         FilterCategories: Sequence[str] = ...,
         FilterCountries: Sequence[str] = ...,
         Key: str = ...,
         Language: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> SearchPlaceIndexForSuggestionsResponseTypeDef:
         """
         Generates suggestions for addresses and points of interest based on partial or
         misspelled free-form
         text.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.search_place_index_for_suggestions)
@@ -783,15 +782,15 @@
         Text: str,
         BiasPosition: Sequence[float] = ...,
         FilterBBox: Sequence[float] = ...,
         FilterCategories: Sequence[str] = ...,
         FilterCountries: Sequence[str] = ...,
         Key: str = ...,
         Language: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> SearchPlaceIndexForTextResponseTypeDef:
         """
         Geocodes free-form text, such as an address, name, city, or region to allow you
         to search for Places or points of
         interest.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.search_place_index_for_text)
@@ -818,15 +817,15 @@
 
     async def update_geofence_collection(
         self,
         *,
         CollectionName: str,
         Description: str = ...,
         PricingPlan: PricingPlanType = ...,
-        PricingPlanDataSource: str = ...
+        PricingPlanDataSource: str = ...,
     ) -> UpdateGeofenceCollectionResponseTypeDef:
         """
         Updates the specified properties of a given geofence collection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.update_geofence_collection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/client/#update_geofence_collection)
         """
@@ -835,45 +834,45 @@
         self,
         *,
         KeyName: str,
         Description: str = ...,
         ExpireTime: TimestampTypeDef = ...,
         ForceUpdate: bool = ...,
         NoExpiry: bool = ...,
-        Restrictions: ApiKeyRestrictionsTypeDef = ...
+        Restrictions: ApiKeyRestrictionsTypeDef = ...,
     ) -> UpdateKeyResponseTypeDef:
         """
         Updates the specified properties of a given API key resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.update_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/client/#update_key)
         """
 
     async def update_map(
         self,
         *,
         MapName: str,
         ConfigurationUpdate: MapConfigurationUpdateTypeDef = ...,
         Description: str = ...,
-        PricingPlan: PricingPlanType = ...
+        PricingPlan: PricingPlanType = ...,
     ) -> UpdateMapResponseTypeDef:
         """
         Updates the specified properties of a given map resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.update_map)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/client/#update_map)
         """
 
     async def update_place_index(
         self,
         *,
         IndexName: str,
         DataSourceConfiguration: DataSourceConfigurationTypeDef = ...,
         Description: str = ...,
-        PricingPlan: PricingPlanType = ...
+        PricingPlan: PricingPlanType = ...,
     ) -> UpdatePlaceIndexResponseTypeDef:
         """
         Updates the specified properties of a given place index resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.update_place_index)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/client/#update_place_index)
         """
@@ -893,15 +892,15 @@
         *,
         TrackerName: str,
         Description: str = ...,
         EventBridgeEnabled: bool = ...,
         KmsKeyEnableGeospatialQueries: bool = ...,
         PositionFiltering: PositionFilteringType = ...,
         PricingPlan: PricingPlanType = ...,
-        PricingPlanDataSource: str = ...
+        PricingPlanDataSource: str = ...,
     ) -> UpdateTrackerResponseTypeDef:
         """
         Updates the specified properties of a given tracker resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.update_tracker)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/client/#update_tracker)
         """
```

### Comparing `types-aiobotocore-location-2.9.0/types_aiobotocore_location/client.pyi` & `types-aiobotocore-location-2.9.1/types_aiobotocore_location/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -233,15 +233,15 @@
         DepartureTime: TimestampTypeDef = ...,
         DistanceUnit: DistanceUnitType = ...,
         IncludeLegGeometry: bool = ...,
         Key: str = ...,
         OptimizeFor: OptimizationModeType = ...,
         TravelMode: TravelModeType = ...,
         TruckModeOptions: CalculateRouteTruckModeOptionsTypeDef = ...,
-        WaypointPositions: Sequence[Sequence[float]] = ...
+        WaypointPositions: Sequence[Sequence[float]] = ...,
     ) -> CalculateRouteResponseTypeDef:
         """
         [Calculates a
         route](https://docs.aws.amazon.com/location/latest/developerguide/calculate-route.html)
         given the following required parameters: `DeparturePosition` and
         `DestinationPosition`.
 
@@ -257,15 +257,15 @@
         DestinationPositions: Sequence[Sequence[float]],
         CarModeOptions: CalculateRouteCarModeOptionsTypeDef = ...,
         DepartNow: bool = ...,
         DepartureTime: TimestampTypeDef = ...,
         DistanceUnit: DistanceUnitType = ...,
         Key: str = ...,
         TravelMode: TravelModeType = ...,
-        TruckModeOptions: CalculateRouteTruckModeOptionsTypeDef = ...
+        TruckModeOptions: CalculateRouteTruckModeOptionsTypeDef = ...,
     ) -> CalculateRouteMatrixResponseTypeDef:
         """
         [Calculates a route
         matrix](https://docs.aws.amazon.com/location/latest/developerguide/calculate-route-matrix.html)
         given the following required parameters: `DeparturePositions` and
         `DestinationPositions`.
 
@@ -293,15 +293,15 @@
         self,
         *,
         CollectionName: str,
         Description: str = ...,
         KmsKeyId: str = ...,
         PricingPlan: PricingPlanType = ...,
         PricingPlanDataSource: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateGeofenceCollectionResponseTypeDef:
         """
         Creates a geofence collection, which manages and stores geofences.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.create_geofence_collection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/client/#create_geofence_collection)
         """
@@ -310,15 +310,15 @@
         self,
         *,
         KeyName: str,
         Restrictions: ApiKeyRestrictionsTypeDef,
         Description: str = ...,
         ExpireTime: TimestampTypeDef = ...,
         NoExpiry: bool = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateKeyResponseTypeDef:
         """
         Creates an API key resource in your Amazon Web Services account, which lets you
         grant actions for Amazon Location resources to the API key
         bearer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.create_key)
@@ -328,15 +328,15 @@
     async def create_map(
         self,
         *,
         Configuration: MapConfigurationTypeDef,
         MapName: str,
         Description: str = ...,
         PricingPlan: PricingPlanType = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateMapResponseTypeDef:
         """
         Creates a map resource in your Amazon Web Services account, which provides map
         tiles of different styles sourced from global location data
         providers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.create_map)
@@ -347,15 +347,15 @@
         self,
         *,
         DataSource: str,
         IndexName: str,
         DataSourceConfiguration: DataSourceConfigurationTypeDef = ...,
         Description: str = ...,
         PricingPlan: PricingPlanType = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreatePlaceIndexResponseTypeDef:
         """
         Creates a place index resource in your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.create_place_index)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/client/#create_place_index)
         """
@@ -363,15 +363,15 @@
     async def create_route_calculator(
         self,
         *,
         CalculatorName: str,
         DataSource: str,
         Description: str = ...,
         PricingPlan: PricingPlanType = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateRouteCalculatorResponseTypeDef:
         """
         Creates a route calculator resource in your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.create_route_calculator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/client/#create_route_calculator)
         """
@@ -383,15 +383,15 @@
         Description: str = ...,
         EventBridgeEnabled: bool = ...,
         KmsKeyEnableGeospatialQueries: bool = ...,
         KmsKeyId: str = ...,
         PositionFiltering: PositionFilteringType = ...,
         PricingPlan: PricingPlanType = ...,
         PricingPlanDataSource: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateTrackerResponseTypeDef:
         """
         Creates a tracker resource in your Amazon Web Services account, which lets you
         retrieve current and historical location of
         devices.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.create_tracker)
@@ -536,15 +536,15 @@
         self,
         *,
         DeviceId: str,
         TrackerName: str,
         EndTimeExclusive: TimestampTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        StartTimeInclusive: TimestampTypeDef = ...
+        StartTimeInclusive: TimestampTypeDef = ...,
     ) -> GetDevicePositionHistoryResponseTypeDef:
         """
         Retrieves the device position history from a tracker resource within a
         specified range of
         time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.get_device_position_history)
@@ -613,15 +613,15 @@
 
     async def list_device_positions(
         self,
         *,
         TrackerName: str,
         FilterGeometry: TrackingFilterGeometryTypeDef = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListDevicePositionsResponseTypeDef:
         """
         A batch request to retrieve all device positions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.list_device_positions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/client/#list_device_positions)
         """
@@ -719,15 +719,15 @@
 
     async def put_geofence(
         self,
         *,
         CollectionName: str,
         GeofenceId: str,
         Geometry: GeofenceGeometryTypeDef,
-        GeofenceProperties: Mapping[str, str] = ...
+        GeofenceProperties: Mapping[str, str] = ...,
     ) -> PutGeofenceResponseTypeDef:
         """
         Stores a geofence geometry in a given geofence collection, or updates the
         geometry of an existing geofence if a geofence ID is included in the
         request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.put_geofence)
@@ -737,15 +737,15 @@
     async def search_place_index_for_position(
         self,
         *,
         IndexName: str,
         Position: Sequence[float],
         Key: str = ...,
         Language: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> SearchPlaceIndexForPositionResponseTypeDef:
         """
         Reverse geocodes a given coordinate and returns a legible address.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.search_place_index_for_position)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/client/#search_place_index_for_position)
         """
@@ -757,15 +757,15 @@
         Text: str,
         BiasPosition: Sequence[float] = ...,
         FilterBBox: Sequence[float] = ...,
         FilterCategories: Sequence[str] = ...,
         FilterCountries: Sequence[str] = ...,
         Key: str = ...,
         Language: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> SearchPlaceIndexForSuggestionsResponseTypeDef:
         """
         Generates suggestions for addresses and points of interest based on partial or
         misspelled free-form
         text.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.search_place_index_for_suggestions)
@@ -779,15 +779,15 @@
         Text: str,
         BiasPosition: Sequence[float] = ...,
         FilterBBox: Sequence[float] = ...,
         FilterCategories: Sequence[str] = ...,
         FilterCountries: Sequence[str] = ...,
         Key: str = ...,
         Language: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> SearchPlaceIndexForTextResponseTypeDef:
         """
         Geocodes free-form text, such as an address, name, city, or region to allow you
         to search for Places or points of
         interest.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.search_place_index_for_text)
@@ -814,15 +814,15 @@
 
     async def update_geofence_collection(
         self,
         *,
         CollectionName: str,
         Description: str = ...,
         PricingPlan: PricingPlanType = ...,
-        PricingPlanDataSource: str = ...
+        PricingPlanDataSource: str = ...,
     ) -> UpdateGeofenceCollectionResponseTypeDef:
         """
         Updates the specified properties of a given geofence collection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.update_geofence_collection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/client/#update_geofence_collection)
         """
@@ -831,45 +831,45 @@
         self,
         *,
         KeyName: str,
         Description: str = ...,
         ExpireTime: TimestampTypeDef = ...,
         ForceUpdate: bool = ...,
         NoExpiry: bool = ...,
-        Restrictions: ApiKeyRestrictionsTypeDef = ...
+        Restrictions: ApiKeyRestrictionsTypeDef = ...,
     ) -> UpdateKeyResponseTypeDef:
         """
         Updates the specified properties of a given API key resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.update_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/client/#update_key)
         """
 
     async def update_map(
         self,
         *,
         MapName: str,
         ConfigurationUpdate: MapConfigurationUpdateTypeDef = ...,
         Description: str = ...,
-        PricingPlan: PricingPlanType = ...
+        PricingPlan: PricingPlanType = ...,
     ) -> UpdateMapResponseTypeDef:
         """
         Updates the specified properties of a given map resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.update_map)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/client/#update_map)
         """
 
     async def update_place_index(
         self,
         *,
         IndexName: str,
         DataSourceConfiguration: DataSourceConfigurationTypeDef = ...,
         Description: str = ...,
-        PricingPlan: PricingPlanType = ...
+        PricingPlan: PricingPlanType = ...,
     ) -> UpdatePlaceIndexResponseTypeDef:
         """
         Updates the specified properties of a given place index resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.update_place_index)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/client/#update_place_index)
         """
@@ -889,15 +889,15 @@
         *,
         TrackerName: str,
         Description: str = ...,
         EventBridgeEnabled: bool = ...,
         KmsKeyEnableGeospatialQueries: bool = ...,
         PositionFiltering: PositionFilteringType = ...,
         PricingPlan: PricingPlanType = ...,
-        PricingPlanDataSource: str = ...
+        PricingPlanDataSource: str = ...,
     ) -> UpdateTrackerResponseTypeDef:
         """
         Updates the specified properties of a given tracker resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.update_tracker)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/client/#update_tracker)
         """
```

### Comparing `types-aiobotocore-location-2.9.0/types_aiobotocore_location/literals.py` & `types-aiobotocore-location-2.9.1/types_aiobotocore_location/literals.py`

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
     "BatchItemErrorCodeType",
     "DimensionUnitType",
     "DistanceUnitType",
     "GetDevicePositionHistoryPaginatorName",
     "IntendedUseType",
     "ListDevicePositionsPaginatorName",
@@ -45,15 +44,14 @@
     "LocationServiceServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 BatchItemErrorCodeType = Literal[
     "AccessDeniedError",
     "ConflictError",
     "InternalServerError",
     "ResourceNotFoundError",
     "ThrottlingError",
     "ValidationError",
```

### Comparing `types-aiobotocore-location-2.9.0/types_aiobotocore_location/literals.pyi` & `types-aiobotocore-location-2.9.1/types_aiobotocore_location/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-location-2.9.0/types_aiobotocore_location/paginator.py` & `types-aiobotocore-location-2.9.1/types_aiobotocore_location/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,14 @@
     "ListMapsPaginator",
     "ListPlaceIndexesPaginator",
     "ListRouteCalculatorsPaginator",
     "ListTrackerConsumersPaginator",
     "ListTrackersPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -94,15 +93,15 @@
     def paginate(
         self,
         *,
         DeviceId: str,
         TrackerName: str,
         EndTimeExclusive: TimestampTypeDef = ...,
         StartTimeInclusive: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetDevicePositionHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.GetDevicePositionHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/paginators/#getdevicepositionhistorypaginator)
         """
 
 
@@ -113,15 +112,15 @@
     """
 
     def paginate(
         self,
         *,
         TrackerName: str,
         FilterGeometry: TrackingFilterGeometryTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDevicePositionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListDevicePositions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/paginators/#listdevicepositionspaginator)
         """
```

### Comparing `types-aiobotocore-location-2.9.0/types_aiobotocore_location/paginator.pyi` & `types-aiobotocore-location-2.9.1/types_aiobotocore_location/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
     def paginate(
         self,
         *,
         DeviceId: str,
         TrackerName: str,
         EndTimeExclusive: TimestampTypeDef = ...,
         StartTimeInclusive: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetDevicePositionHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.GetDevicePositionHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/paginators/#getdevicepositionhistorypaginator)
         """
 
 class ListDevicePositionsPaginator(AioPaginator):
@@ -109,15 +109,15 @@
     """
 
     def paginate(
         self,
         *,
         TrackerName: str,
         FilterGeometry: TrackingFilterGeometryTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDevicePositionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListDevicePositions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/paginators/#listdevicepositionspaginator)
         """
 
 class ListGeofenceCollectionsPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-location-2.9.0/types_aiobotocore_location/type_defs.py` & `types-aiobotocore-location-2.9.1/types_aiobotocore_location/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ApiKeyFilterTypeDef",
     "ApiKeyRestrictionsPaginatorTypeDef",
     "ApiKeyRestrictionsTypeDef",
     "AssociateTrackerConsumerRequestRequestTypeDef",
     "BatchItemErrorTypeDef",
     "BatchDeleteDevicePositionHistoryRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-location-2.9.0/types_aiobotocore_location/type_defs.pyi` & `types-aiobotocore-location-2.9.1/types_aiobotocore_location/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-location-2.9.0/types_aiobotocore_location.egg-info/PKG-INFO` & `types-aiobotocore-location-2.9.1/types_aiobotocore_location.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-location
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.LocationService 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.LocationService 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/
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
 
 <a id="types-aiobotocore-location"></a>
 
 # types-aiobotocore-location
 
 [![PyPI - types-aiobotocore-location](https://img.shields.io/pypi/v/types-aiobotocore-location.svg?color=blue)](https://pypi.org/project/types-aiobotocore-location)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-location.svg?color=blue)](https://pypi.org/project/types-aiobotocore-location)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-location)](https://pepy.tech/project/types-aiobotocore-location)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LocationService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
+[aiobotocore.LocationService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
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
 [types-aiobotocore-location docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-location-2.9.0/types_aiobotocore_location.egg-info/SOURCES.txt` & `types-aiobotocore-location-2.9.1/types_aiobotocore_location.egg-info/SOURCES.txt`

 * *Files identical despite different names*

