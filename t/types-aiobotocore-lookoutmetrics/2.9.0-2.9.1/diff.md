# Comparing `tmp/types-aiobotocore-lookoutmetrics-2.9.0.tar.gz` & `tmp/types-aiobotocore-lookoutmetrics-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-lookoutmetrics-2.9.0.tar", last modified: Wed Dec 13 19:59:47 2023, max compression
+gzip compressed data, was "types-aiobotocore-lookoutmetrics-2.9.1.tar", last modified: Thu Jan 18 01:21:10 2024, max compression
```

## Comparing `types-aiobotocore-lookoutmetrics-2.9.0.tar` & `types-aiobotocore-lookoutmetrics-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:47.849509 types-aiobotocore-lookoutmetrics-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:49:29.000000 types-aiobotocore-lookoutmetrics-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12620 2023-12-13 19:59:47.849509 types-aiobotocore-lookoutmetrics-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11029 2023-12-13 19:49:29.000000 types-aiobotocore-lookoutmetrics-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:47.849509 types-aiobotocore-lookoutmetrics-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2023-12-13 19:49:29.000000 types-aiobotocore-lookoutmetrics-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:47.845509 types-aiobotocore-lookoutmetrics-2.9.0/types_aiobotocore_lookoutmetrics/
--rw-r--r--   0 runner    (1001) docker     (127)      499 2023-12-13 19:49:29.000000 types-aiobotocore-lookoutmetrics-2.9.0/types_aiobotocore_lookoutmetrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2023-12-13 19:49:29.000000 types-aiobotocore-lookoutmetrics-2.9.0/types_aiobotocore_lookoutmetrics/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      960 2023-12-13 19:49:29.000000 types-aiobotocore-lookoutmetrics-2.9.0/types_aiobotocore_lookoutmetrics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24335 2023-12-13 19:49:29.000000 types-aiobotocore-lookoutmetrics-2.9.0/types_aiobotocore_lookoutmetrics/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    24332 2023-12-13 19:49:29.000000 types-aiobotocore-lookoutmetrics-2.9.0/types_aiobotocore_lookoutmetrics/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10184 2023-12-13 19:49:29.000000 types-aiobotocore-lookoutmetrics-2.9.0/types_aiobotocore_lookoutmetrics/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10182 2023-12-13 19:49:29.000000 types-aiobotocore-lookoutmetrics-2.9.0/types_aiobotocore_lookoutmetrics/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:49:29.000000 types-aiobotocore-lookoutmetrics-2.9.0/types_aiobotocore_lookoutmetrics/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    33369 2023-12-13 19:49:30.000000 types-aiobotocore-lookoutmetrics-2.9.0/types_aiobotocore_lookoutmetrics/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    33368 2023-12-13 19:49:30.000000 types-aiobotocore-lookoutmetrics-2.9.0/types_aiobotocore_lookoutmetrics/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:49:29.000000 types-aiobotocore-lookoutmetrics-2.9.0/types_aiobotocore_lookoutmetrics/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:47.845509 types-aiobotocore-lookoutmetrics-2.9.0/types_aiobotocore_lookoutmetrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12620 2023-12-13 19:59:47.000000 types-aiobotocore-lookoutmetrics-2.9.0/types_aiobotocore_lookoutmetrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      853 2023-12-13 19:59:47.000000 types-aiobotocore-lookoutmetrics-2.9.0/types_aiobotocore_lookoutmetrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:47.000000 types-aiobotocore-lookoutmetrics-2.9.0/types_aiobotocore_lookoutmetrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:47.000000 types-aiobotocore-lookoutmetrics-2.9.0/types_aiobotocore_lookoutmetrics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:47.000000 types-aiobotocore-lookoutmetrics-2.9.0/types_aiobotocore_lookoutmetrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-13 19:59:47.000000 types-aiobotocore-lookoutmetrics-2.9.0/types_aiobotocore_lookoutmetrics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:10.165209 types-aiobotocore-lookoutmetrics-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:11:15.000000 types-aiobotocore-lookoutmetrics-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12640 2024-01-18 01:21:10.165209 types-aiobotocore-lookoutmetrics-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11029 2024-01-18 01:11:15.000000 types-aiobotocore-lookoutmetrics-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:10.165209 types-aiobotocore-lookoutmetrics-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-01-18 01:11:15.000000 types-aiobotocore-lookoutmetrics-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:10.165209 types-aiobotocore-lookoutmetrics-2.9.1/types_aiobotocore_lookoutmetrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-01-18 01:11:15.000000 types-aiobotocore-lookoutmetrics-2.9.1/types_aiobotocore_lookoutmetrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-01-18 01:11:15.000000 types-aiobotocore-lookoutmetrics-2.9.1/types_aiobotocore_lookoutmetrics/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-01-18 01:11:15.000000 types-aiobotocore-lookoutmetrics-2.9.1/types_aiobotocore_lookoutmetrics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24348 2024-01-18 01:11:16.000000 types-aiobotocore-lookoutmetrics-2.9.1/types_aiobotocore_lookoutmetrics/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24345 2024-01-18 01:11:16.000000 types-aiobotocore-lookoutmetrics-2.9.1/types_aiobotocore_lookoutmetrics/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10182 2024-01-18 01:11:16.000000 types-aiobotocore-lookoutmetrics-2.9.1/types_aiobotocore_lookoutmetrics/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10182 2024-01-18 01:11:16.000000 types-aiobotocore-lookoutmetrics-2.9.1/types_aiobotocore_lookoutmetrics/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:11:15.000000 types-aiobotocore-lookoutmetrics-2.9.1/types_aiobotocore_lookoutmetrics/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    33368 2024-01-18 01:11:16.000000 types-aiobotocore-lookoutmetrics-2.9.1/types_aiobotocore_lookoutmetrics/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33368 2024-01-18 01:11:16.000000 types-aiobotocore-lookoutmetrics-2.9.1/types_aiobotocore_lookoutmetrics/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:11:15.000000 types-aiobotocore-lookoutmetrics-2.9.1/types_aiobotocore_lookoutmetrics/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:10.165209 types-aiobotocore-lookoutmetrics-2.9.1/types_aiobotocore_lookoutmetrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12640 2024-01-18 01:21:10.000000 types-aiobotocore-lookoutmetrics-2.9.1/types_aiobotocore_lookoutmetrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-01-18 01:21:10.000000 types-aiobotocore-lookoutmetrics-2.9.1/types_aiobotocore_lookoutmetrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:10.000000 types-aiobotocore-lookoutmetrics-2.9.1/types_aiobotocore_lookoutmetrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:10.000000 types-aiobotocore-lookoutmetrics-2.9.1/types_aiobotocore_lookoutmetrics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:10.000000 types-aiobotocore-lookoutmetrics-2.9.1/types_aiobotocore_lookoutmetrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-18 01:21:10.000000 types-aiobotocore-lookoutmetrics-2.9.1/types_aiobotocore_lookoutmetrics.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-lookoutmetrics-2.9.0/LICENSE` & `types-aiobotocore-lookoutmetrics-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-lookoutmetrics-2.9.0/PKG-INFO` & `types-aiobotocore-lookoutmetrics-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-lookoutmetrics
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.LookoutMetrics 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.LookoutMetrics 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/
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
 
 <a id="types-aiobotocore-lookoutmetrics"></a>
 
 # types-aiobotocore-lookoutmetrics
 
 [![PyPI - types-aiobotocore-lookoutmetrics](https://img.shields.io/pypi/v/types-aiobotocore-lookoutmetrics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lookoutmetrics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lookoutmetrics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lookoutmetrics)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lookoutmetrics)](https://pepy.tech/project/types-aiobotocore-lookoutmetrics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LookoutMetrics 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics)
+[aiobotocore.LookoutMetrics 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics)
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
 [types-aiobotocore-lookoutmetrics docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-lookoutmetrics-2.9.0/README.md` & `types-aiobotocore-lookoutmetrics-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lookoutmetrics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lookoutmetrics)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lookoutmetrics)](https://pepy.tech/project/types-aiobotocore-lookoutmetrics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LookoutMetrics 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics)
+[aiobotocore.LookoutMetrics 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics)
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
 [types-aiobotocore-lookoutmetrics docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-lookoutmetrics-2.9.0/setup.py` & `types-aiobotocore-lookoutmetrics-2.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-lookoutmetrics",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_lookoutmetrics"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.LookoutMetrics 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.LookoutMetrics 2.9.1 service generated with"
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
     keywords="aiobotocore lookoutmetrics type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_lookoutmetrics": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-lookoutmetrics-2.9.0/types_aiobotocore_lookoutmetrics/__main__.py` & `types-aiobotocore-lookoutmetrics-2.9.1/types_aiobotocore_lookoutmetrics/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.LookoutMetrics 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.LookoutMetrics 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics\nOther"
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

### Comparing `types-aiobotocore-lookoutmetrics-2.9.0/types_aiobotocore_lookoutmetrics/client.py` & `types-aiobotocore-lookoutmetrics-2.9.1/types_aiobotocore_lookoutmetrics/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
         *,
         AlertName: str,
         AnomalyDetectorArn: str,
         Action: ActionTypeDef,
         AlertSensitivityThreshold: int = ...,
         AlertDescription: str = ...,
         Tags: Mapping[str, str] = ...,
-        AlertFilters: AlertFiltersTypeDef = ...
+        AlertFilters: AlertFiltersTypeDef = ...,
     ) -> CreateAlertResponseTypeDef:
         """
         Creates an alert for an anomaly detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.create_alert)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/client/#create_alert)
         """
@@ -149,15 +149,15 @@
     async def create_anomaly_detector(
         self,
         *,
         AnomalyDetectorName: str,
         AnomalyDetectorConfig: AnomalyDetectorConfigTypeDef,
         AnomalyDetectorDescription: str = ...,
         KmsKeyArn: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateAnomalyDetectorResponseTypeDef:
         """
         Creates an anomaly detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.create_anomaly_detector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/client/#create_anomaly_detector)
         """
@@ -172,15 +172,15 @@
         MetricSetDescription: str = ...,
         Offset: int = ...,
         TimestampColumn: TimestampColumnTypeDef = ...,
         DimensionList: Sequence[str] = ...,
         MetricSetFrequency: FrequencyType = ...,
         Timezone: str = ...,
         Tags: Mapping[str, str] = ...,
-        DimensionFilterList: Sequence[MetricSetDimensionFilterTypeDef] = ...
+        DimensionFilterList: Sequence[MetricSetDimensionFilterTypeDef] = ...,
     ) -> CreateMetricSetResponseTypeDef:
         """
         Creates a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.create_metric_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/client/#create_metric_set)
         """
@@ -219,15 +219,15 @@
 
     async def describe_anomaly_detection_executions(
         self,
         *,
         AnomalyDetectorArn: str,
         Timestamp: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeAnomalyDetectionExecutionsResponseTypeDef:
         """
         Returns information about the status of the specified anomaly detection jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.describe_anomaly_detection_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/client/#describe_anomaly_detection_executions)
         """
@@ -250,15 +250,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/client/#describe_metric_set)
         """
 
     async def detect_metric_set_config(
         self,
         *,
         AnomalyDetectorArn: str,
-        AutoDetectionMetricSource: AutoDetectionMetricSourceTypeDef
+        AutoDetectionMetricSource: AutoDetectionMetricSourceTypeDef,
     ) -> DetectMetricSetConfigResponseTypeDef:
         """
         Detects an Amazon S3 dataset's file format, interval, and offset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.detect_metric_set_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/client/#detect_metric_set_config)
         """
@@ -299,15 +299,15 @@
 
     async def get_feedback(
         self,
         *,
         AnomalyDetectorArn: str,
         AnomalyGroupTimeSeriesFeedback: AnomalyGroupTimeSeriesTypeDef,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetFeedbackResponseTypeDef:
         """
         Get feedback for an anomaly group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.get_feedback)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/client/#get_feedback)
         """
@@ -345,15 +345,15 @@
     async def list_anomaly_group_related_metrics(
         self,
         *,
         AnomalyDetectorArn: str,
         AnomalyGroupId: str,
         RelationshipTypeFilter: RelationshipTypeType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListAnomalyGroupRelatedMetricsResponseTypeDef:
         """
         Returns a list of measures that are potential causes or effects of an anomaly
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.list_anomaly_group_related_metrics)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/client/#list_anomaly_group_related_metrics)
@@ -361,15 +361,15 @@
 
     async def list_anomaly_group_summaries(
         self,
         *,
         AnomalyDetectorArn: str,
         SensitivityThreshold: int,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListAnomalyGroupSummariesResponseTypeDef:
         """
         Returns a list of anomaly groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.list_anomaly_group_summaries)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/client/#list_anomaly_group_summaries)
         """
@@ -377,15 +377,15 @@
     async def list_anomaly_group_time_series(
         self,
         *,
         AnomalyDetectorArn: str,
         AnomalyGroupId: str,
         MetricName: str,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListAnomalyGroupTimeSeriesResponseTypeDef:
         """
         Gets a list of anomalous metrics for a measure in an anomaly group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.list_anomaly_group_time_series)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/client/#list_anomaly_group_time_series)
         """
@@ -413,15 +413,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/client/#list_tags_for_resource)
         """
 
     async def put_feedback(
         self,
         *,
         AnomalyDetectorArn: str,
-        AnomalyGroupTimeSeriesFeedback: AnomalyGroupTimeSeriesFeedbackTypeDef
+        AnomalyGroupTimeSeriesFeedback: AnomalyGroupTimeSeriesFeedbackTypeDef,
     ) -> Dict[str, Any]:
         """
         Add feedback for an anomalous metric.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.put_feedback)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/client/#put_feedback)
         """
@@ -451,30 +451,30 @@
     async def update_alert(
         self,
         *,
         AlertArn: str,
         AlertDescription: str = ...,
         AlertSensitivityThreshold: int = ...,
         Action: ActionTypeDef = ...,
-        AlertFilters: AlertFiltersTypeDef = ...
+        AlertFilters: AlertFiltersTypeDef = ...,
     ) -> UpdateAlertResponseTypeDef:
         """
         Make changes to an existing alert.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.update_alert)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/client/#update_alert)
         """
 
     async def update_anomaly_detector(
         self,
         *,
         AnomalyDetectorArn: str,
         KmsKeyArn: str = ...,
         AnomalyDetectorDescription: str = ...,
-        AnomalyDetectorConfig: AnomalyDetectorConfigTypeDef = ...
+        AnomalyDetectorConfig: AnomalyDetectorConfigTypeDef = ...,
     ) -> UpdateAnomalyDetectorResponseTypeDef:
         """
         Updates a detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.update_anomaly_detector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/client/#update_anomaly_detector)
         """
@@ -486,15 +486,15 @@
         MetricSetDescription: str = ...,
         MetricList: Sequence[MetricTypeDef] = ...,
         Offset: int = ...,
         TimestampColumn: TimestampColumnTypeDef = ...,
         DimensionList: Sequence[str] = ...,
         MetricSetFrequency: FrequencyType = ...,
         MetricSource: MetricSourceTypeDef = ...,
-        DimensionFilterList: Sequence[MetricSetDimensionFilterTypeDef] = ...
+        DimensionFilterList: Sequence[MetricSetDimensionFilterTypeDef] = ...,
     ) -> UpdateMetricSetResponseTypeDef:
         """
         Updates a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.update_metric_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/client/#update_metric_set)
         """
```

### Comparing `types-aiobotocore-lookoutmetrics-2.9.0/types_aiobotocore_lookoutmetrics/client.pyi` & `types-aiobotocore-lookoutmetrics-2.9.1/types_aiobotocore_lookoutmetrics/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
         *,
         AlertName: str,
         AnomalyDetectorArn: str,
         Action: ActionTypeDef,
         AlertSensitivityThreshold: int = ...,
         AlertDescription: str = ...,
         Tags: Mapping[str, str] = ...,
-        AlertFilters: AlertFiltersTypeDef = ...
+        AlertFilters: AlertFiltersTypeDef = ...,
     ) -> CreateAlertResponseTypeDef:
         """
         Creates an alert for an anomaly detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.create_alert)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/client/#create_alert)
         """
@@ -146,15 +146,15 @@
     async def create_anomaly_detector(
         self,
         *,
         AnomalyDetectorName: str,
         AnomalyDetectorConfig: AnomalyDetectorConfigTypeDef,
         AnomalyDetectorDescription: str = ...,
         KmsKeyArn: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateAnomalyDetectorResponseTypeDef:
         """
         Creates an anomaly detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.create_anomaly_detector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/client/#create_anomaly_detector)
         """
@@ -169,15 +169,15 @@
         MetricSetDescription: str = ...,
         Offset: int = ...,
         TimestampColumn: TimestampColumnTypeDef = ...,
         DimensionList: Sequence[str] = ...,
         MetricSetFrequency: FrequencyType = ...,
         Timezone: str = ...,
         Tags: Mapping[str, str] = ...,
-        DimensionFilterList: Sequence[MetricSetDimensionFilterTypeDef] = ...
+        DimensionFilterList: Sequence[MetricSetDimensionFilterTypeDef] = ...,
     ) -> CreateMetricSetResponseTypeDef:
         """
         Creates a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.create_metric_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/client/#create_metric_set)
         """
@@ -216,15 +216,15 @@
 
     async def describe_anomaly_detection_executions(
         self,
         *,
         AnomalyDetectorArn: str,
         Timestamp: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeAnomalyDetectionExecutionsResponseTypeDef:
         """
         Returns information about the status of the specified anomaly detection jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.describe_anomaly_detection_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/client/#describe_anomaly_detection_executions)
         """
@@ -247,15 +247,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/client/#describe_metric_set)
         """
 
     async def detect_metric_set_config(
         self,
         *,
         AnomalyDetectorArn: str,
-        AutoDetectionMetricSource: AutoDetectionMetricSourceTypeDef
+        AutoDetectionMetricSource: AutoDetectionMetricSourceTypeDef,
     ) -> DetectMetricSetConfigResponseTypeDef:
         """
         Detects an Amazon S3 dataset's file format, interval, and offset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.detect_metric_set_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/client/#detect_metric_set_config)
         """
@@ -296,15 +296,15 @@
 
     async def get_feedback(
         self,
         *,
         AnomalyDetectorArn: str,
         AnomalyGroupTimeSeriesFeedback: AnomalyGroupTimeSeriesTypeDef,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetFeedbackResponseTypeDef:
         """
         Get feedback for an anomaly group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.get_feedback)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/client/#get_feedback)
         """
@@ -342,15 +342,15 @@
     async def list_anomaly_group_related_metrics(
         self,
         *,
         AnomalyDetectorArn: str,
         AnomalyGroupId: str,
         RelationshipTypeFilter: RelationshipTypeType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListAnomalyGroupRelatedMetricsResponseTypeDef:
         """
         Returns a list of measures that are potential causes or effects of an anomaly
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.list_anomaly_group_related_metrics)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/client/#list_anomaly_group_related_metrics)
@@ -358,15 +358,15 @@
 
     async def list_anomaly_group_summaries(
         self,
         *,
         AnomalyDetectorArn: str,
         SensitivityThreshold: int,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListAnomalyGroupSummariesResponseTypeDef:
         """
         Returns a list of anomaly groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.list_anomaly_group_summaries)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/client/#list_anomaly_group_summaries)
         """
@@ -374,15 +374,15 @@
     async def list_anomaly_group_time_series(
         self,
         *,
         AnomalyDetectorArn: str,
         AnomalyGroupId: str,
         MetricName: str,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListAnomalyGroupTimeSeriesResponseTypeDef:
         """
         Gets a list of anomalous metrics for a measure in an anomaly group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.list_anomaly_group_time_series)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/client/#list_anomaly_group_time_series)
         """
@@ -410,15 +410,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/client/#list_tags_for_resource)
         """
 
     async def put_feedback(
         self,
         *,
         AnomalyDetectorArn: str,
-        AnomalyGroupTimeSeriesFeedback: AnomalyGroupTimeSeriesFeedbackTypeDef
+        AnomalyGroupTimeSeriesFeedback: AnomalyGroupTimeSeriesFeedbackTypeDef,
     ) -> Dict[str, Any]:
         """
         Add feedback for an anomalous metric.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.put_feedback)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/client/#put_feedback)
         """
@@ -448,30 +448,30 @@
     async def update_alert(
         self,
         *,
         AlertArn: str,
         AlertDescription: str = ...,
         AlertSensitivityThreshold: int = ...,
         Action: ActionTypeDef = ...,
-        AlertFilters: AlertFiltersTypeDef = ...
+        AlertFilters: AlertFiltersTypeDef = ...,
     ) -> UpdateAlertResponseTypeDef:
         """
         Make changes to an existing alert.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.update_alert)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/client/#update_alert)
         """
 
     async def update_anomaly_detector(
         self,
         *,
         AnomalyDetectorArn: str,
         KmsKeyArn: str = ...,
         AnomalyDetectorDescription: str = ...,
-        AnomalyDetectorConfig: AnomalyDetectorConfigTypeDef = ...
+        AnomalyDetectorConfig: AnomalyDetectorConfigTypeDef = ...,
     ) -> UpdateAnomalyDetectorResponseTypeDef:
         """
         Updates a detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.update_anomaly_detector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/client/#update_anomaly_detector)
         """
@@ -483,15 +483,15 @@
         MetricSetDescription: str = ...,
         MetricList: Sequence[MetricTypeDef] = ...,
         Offset: int = ...,
         TimestampColumn: TimestampColumnTypeDef = ...,
         DimensionList: Sequence[str] = ...,
         MetricSetFrequency: FrequencyType = ...,
         MetricSource: MetricSourceTypeDef = ...,
-        DimensionFilterList: Sequence[MetricSetDimensionFilterTypeDef] = ...
+        DimensionFilterList: Sequence[MetricSetDimensionFilterTypeDef] = ...,
     ) -> UpdateMetricSetResponseTypeDef:
         """
         Updates a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.update_metric_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/client/#update_metric_set)
         """
```

### Comparing `types-aiobotocore-lookoutmetrics-2.9.0/types_aiobotocore_lookoutmetrics/literals.py` & `types-aiobotocore-lookoutmetrics-2.9.1/types_aiobotocore_lookoutmetrics/literals.py`

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
     "AggregationFunctionType",
     "AlertStatusType",
     "AlertTypeType",
     "AnomalyDetectionTaskStatusType",
     "AnomalyDetectorFailureTypeType",
     "AnomalyDetectorStatusType",
@@ -37,15 +36,14 @@
     "SnsFormatType",
     "LookoutMetricsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 AggregationFunctionType = Literal["AVG", "SUM"]
 AlertStatusType = Literal["ACTIVE", "INACTIVE"]
 AlertTypeType = Literal["LAMBDA", "SNS"]
 AnomalyDetectionTaskStatusType = Literal[
     "COMPLETED", "FAILED", "FAILED_TO_SCHEDULE", "IN_PROGRESS", "PENDING"
 ]
 AnomalyDetectorFailureTypeType = Literal[
```

### Comparing `types-aiobotocore-lookoutmetrics-2.9.0/types_aiobotocore_lookoutmetrics/literals.pyi` & `types-aiobotocore-lookoutmetrics-2.9.1/types_aiobotocore_lookoutmetrics/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lookoutmetrics-2.9.0/types_aiobotocore_lookoutmetrics/type_defs.py` & `types-aiobotocore-lookoutmetrics-2.9.1/types_aiobotocore_lookoutmetrics/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "LambdaConfigurationTypeDef",
     "SNSConfigurationTypeDef",
     "ActivateAnomalyDetectorRequestRequestTypeDef",
     "DimensionFilterTypeDef",
     "AlertSummaryTypeDef",
     "AnomalyDetectorConfigSummaryTypeDef",
```

### Comparing `types-aiobotocore-lookoutmetrics-2.9.0/types_aiobotocore_lookoutmetrics/type_defs.pyi` & `types-aiobotocore-lookoutmetrics-2.9.1/types_aiobotocore_lookoutmetrics/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lookoutmetrics-2.9.0/types_aiobotocore_lookoutmetrics.egg-info/PKG-INFO` & `types-aiobotocore-lookoutmetrics-2.9.1/types_aiobotocore_lookoutmetrics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-lookoutmetrics
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.LookoutMetrics 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.LookoutMetrics 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/
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
 
 <a id="types-aiobotocore-lookoutmetrics"></a>
 
 # types-aiobotocore-lookoutmetrics
 
 [![PyPI - types-aiobotocore-lookoutmetrics](https://img.shields.io/pypi/v/types-aiobotocore-lookoutmetrics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lookoutmetrics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lookoutmetrics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lookoutmetrics)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lookoutmetrics)](https://pepy.tech/project/types-aiobotocore-lookoutmetrics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LookoutMetrics 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics)
+[aiobotocore.LookoutMetrics 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics)
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
 [types-aiobotocore-lookoutmetrics docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-lookoutmetrics-2.9.0/types_aiobotocore_lookoutmetrics.egg-info/SOURCES.txt` & `types-aiobotocore-lookoutmetrics-2.9.1/types_aiobotocore_lookoutmetrics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

