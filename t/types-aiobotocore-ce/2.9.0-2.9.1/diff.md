# Comparing `tmp/types-aiobotocore-ce-2.9.0.tar.gz` & `tmp/types-aiobotocore-ce-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ce-2.9.0.tar", last modified: Wed Dec 13 19:58:44 2023, max compression
+gzip compressed data, was "types-aiobotocore-ce-2.9.1.tar", last modified: Thu Jan 18 01:20:11 2024, max compression
```

## Comparing `types-aiobotocore-ce-2.9.0.tar` & `types-aiobotocore-ce-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:44.318014 types-aiobotocore-ce-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:41:52.000000 types-aiobotocore-ce-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12058 2023-12-13 19:58:44.318014 types-aiobotocore-ce-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10505 2023-12-13 19:41:52.000000 types-aiobotocore-ce-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:44.318014 types-aiobotocore-ce-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2023-12-13 19:41:51.000000 types-aiobotocore-ce-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:44.318014 types-aiobotocore-ce-2.9.0/types_aiobotocore_ce/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2023-12-13 19:41:52.000000 types-aiobotocore-ce-2.9.0/types_aiobotocore_ce/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2023-12-13 19:41:52.000000 types-aiobotocore-ce-2.9.0/types_aiobotocore_ce/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      921 2023-12-13 19:41:52.000000 types-aiobotocore-ce-2.9.0/types_aiobotocore_ce/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34595 2023-12-13 19:41:52.000000 types-aiobotocore-ce-2.9.0/types_aiobotocore_ce/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    34591 2023-12-13 19:41:52.000000 types-aiobotocore-ce-2.9.0/types_aiobotocore_ce/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13206 2023-12-13 19:41:52.000000 types-aiobotocore-ce-2.9.0/types_aiobotocore_ce/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    13204 2023-12-13 19:41:52.000000 types-aiobotocore-ce-2.9.0/types_aiobotocore_ce/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:41:52.000000 types-aiobotocore-ce-2.9.0/types_aiobotocore_ce/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    60128 2023-12-13 19:41:53.000000 types-aiobotocore-ce-2.9.0/types_aiobotocore_ce/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    60127 2023-12-13 19:41:52.000000 types-aiobotocore-ce-2.9.0/types_aiobotocore_ce/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:41:52.000000 types-aiobotocore-ce-2.9.0/types_aiobotocore_ce/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:44.318014 types-aiobotocore-ce-2.9.0/types_aiobotocore_ce.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12058 2023-12-13 19:58:44.000000 types-aiobotocore-ce-2.9.0/types_aiobotocore_ce.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      649 2023-12-13 19:58:44.000000 types-aiobotocore-ce-2.9.0/types_aiobotocore_ce.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:44.000000 types-aiobotocore-ce-2.9.0/types_aiobotocore_ce.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:44.000000 types-aiobotocore-ce-2.9.0/types_aiobotocore_ce.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:44.000000 types-aiobotocore-ce-2.9.0/types_aiobotocore_ce.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-12-13 19:58:44.000000 types-aiobotocore-ce-2.9.0/types_aiobotocore_ce.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:11.537483 types-aiobotocore-ce-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:03:49.000000 types-aiobotocore-ce-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12078 2024-01-18 01:20:11.537483 types-aiobotocore-ce-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10505 2024-01-18 01:03:49.000000 types-aiobotocore-ce-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:11.537483 types-aiobotocore-ce-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-01-18 01:03:48.000000 types-aiobotocore-ce-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:11.533483 types-aiobotocore-ce-2.9.1/types_aiobotocore_ce/
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-01-18 01:03:49.000000 types-aiobotocore-ce-2.9.1/types_aiobotocore_ce/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-01-18 01:03:49.000000 types-aiobotocore-ce-2.9.1/types_aiobotocore_ce/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-01-18 01:03:49.000000 types-aiobotocore-ce-2.9.1/types_aiobotocore_ce/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34619 2024-01-18 01:03:49.000000 types-aiobotocore-ce-2.9.1/types_aiobotocore_ce/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34616 2024-01-18 01:03:49.000000 types-aiobotocore-ce-2.9.1/types_aiobotocore_ce/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13204 2024-01-18 01:03:50.000000 types-aiobotocore-ce-2.9.1/types_aiobotocore_ce/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13204 2024-01-18 01:03:50.000000 types-aiobotocore-ce-2.9.1/types_aiobotocore_ce/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:03:49.000000 types-aiobotocore-ce-2.9.1/types_aiobotocore_ce/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    60127 2024-01-18 01:03:51.000000 types-aiobotocore-ce-2.9.1/types_aiobotocore_ce/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60127 2024-01-18 01:03:50.000000 types-aiobotocore-ce-2.9.1/types_aiobotocore_ce/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:03:49.000000 types-aiobotocore-ce-2.9.1/types_aiobotocore_ce/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:11.537483 types-aiobotocore-ce-2.9.1/types_aiobotocore_ce.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12078 2024-01-18 01:20:11.000000 types-aiobotocore-ce-2.9.1/types_aiobotocore_ce.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-01-18 01:20:11.000000 types-aiobotocore-ce-2.9.1/types_aiobotocore_ce.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:11.000000 types-aiobotocore-ce-2.9.1/types_aiobotocore_ce.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:11.000000 types-aiobotocore-ce-2.9.1/types_aiobotocore_ce.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:11.000000 types-aiobotocore-ce-2.9.1/types_aiobotocore_ce.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-18 01:20:11.000000 types-aiobotocore-ce-2.9.1/types_aiobotocore_ce.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ce-2.9.0/LICENSE` & `types-aiobotocore-ce-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-ce-2.9.0/PKG-INFO` & `types-aiobotocore-ce-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ce
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CostExplorer 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CostExplorer 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/
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
 
 <a id="types-aiobotocore-ce"></a>
 
 # types-aiobotocore-ce
 
 [![PyPI - types-aiobotocore-ce](https://img.shields.io/pypi/v/types-aiobotocore-ce.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ce)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ce.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ce)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ce)](https://pepy.tech/project/types-aiobotocore-ce)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CostExplorer 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
+[aiobotocore.CostExplorer 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
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
 [types-aiobotocore-ce docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-ce-2.9.0/README.md` & `types-aiobotocore-ce-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ce.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ce)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ce)](https://pepy.tech/project/types-aiobotocore-ce)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CostExplorer 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
+[aiobotocore.CostExplorer 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
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
 [types-aiobotocore-ce docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-ce-2.9.0/setup.py` & `types-aiobotocore-ce-2.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ce",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_ce"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CostExplorer 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.CostExplorer 2.9.1 service generated with"
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
     keywords="aiobotocore ce type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_ce": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-ce-2.9.0/types_aiobotocore_ce/__main__.py` & `types-aiobotocore-ce-2.9.1/types_aiobotocore_ce/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CostExplorer 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.CostExplorer 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer\nOther"
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

### Comparing `types-aiobotocore-ce-2.9.0/types_aiobotocore_ce/client.py` & `types-aiobotocore-ce-2.9.1/types_aiobotocore_ce/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("CostExplorerClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -156,30 +155,30 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#close)
         """
 
     async def create_anomaly_monitor(
         self,
         *,
         AnomalyMonitor: AnomalyMonitorTypeDef,
-        ResourceTags: Sequence[ResourceTagTypeDef] = ...
+        ResourceTags: Sequence[ResourceTagTypeDef] = ...,
     ) -> CreateAnomalyMonitorResponseTypeDef:
         """
         Creates a new cost anomaly detection monitor with the requested type and
         monitor
         specification.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.create_anomaly_monitor)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#create_anomaly_monitor)
         """
 
     async def create_anomaly_subscription(
         self,
         *,
         AnomalySubscription: AnomalySubscriptionTypeDef,
-        ResourceTags: Sequence[ResourceTagTypeDef] = ...
+        ResourceTags: Sequence[ResourceTagTypeDef] = ...,
     ) -> CreateAnomalySubscriptionResponseTypeDef:
         """
         Adds an alert subscription to a cost anomaly detection monitor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.create_anomaly_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#create_anomaly_subscription)
         """
@@ -189,15 +188,15 @@
         *,
         Name: str,
         RuleVersion: Literal["CostCategoryExpression.v1"],
         Rules: Sequence[CostCategoryRuleTypeDef],
         EffectiveStart: str = ...,
         DefaultValue: str = ...,
         SplitChargeRules: Sequence[CostCategorySplitChargeRuleTypeDef] = ...,
-        ResourceTags: Sequence[ResourceTagTypeDef] = ...
+        ResourceTags: Sequence[ResourceTagTypeDef] = ...,
     ) -> CreateCostCategoryDefinitionResponseTypeDef:
         """
         Creates a new Cost Category with the requested name and rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.create_cost_category_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#create_cost_category_definition)
         """
@@ -258,15 +257,15 @@
         self,
         *,
         DateInterval: AnomalyDateIntervalTypeDef,
         MonitorArn: str = ...,
         Feedback: AnomalyFeedbackTypeType = ...,
         TotalImpact: TotalImpactFilterTypeDef = ...,
         NextPageToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> GetAnomaliesResponseTypeDef:
         """
         Retrieves all of the cost anomalies detected on your account during the time
         period that's specified by the `DateInterval`
         object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_anomalies)
@@ -274,30 +273,30 @@
         """
 
     async def get_anomaly_monitors(
         self,
         *,
         MonitorArnList: Sequence[str] = ...,
         NextPageToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> GetAnomalyMonitorsResponseTypeDef:
         """
         Retrieves the cost anomaly monitor definitions for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_anomaly_monitors)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#get_anomaly_monitors)
         """
 
     async def get_anomaly_subscriptions(
         self,
         *,
         SubscriptionArnList: Sequence[str] = ...,
         MonitorArn: str = ...,
         NextPageToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> GetAnomalySubscriptionsResponseTypeDef:
         """
         Retrieves the cost anomaly subscription objects for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_anomaly_subscriptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#get_anomaly_subscriptions)
         """
@@ -306,15 +305,15 @@
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Granularity: GranularityType,
         Metrics: Sequence[str],
         Filter: "ExpressionTypeDef" = ...,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
-        NextPageToken: str = ...
+        NextPageToken: str = ...,
     ) -> GetCostAndUsageResponseTypeDef:
         """
         Retrieves cost and usage metrics for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_cost_and_usage)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#get_cost_and_usage)
         """
@@ -323,15 +322,15 @@
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Granularity: GranularityType,
         Filter: "ExpressionTypeDef",
         Metrics: Sequence[str] = ...,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
-        NextPageToken: str = ...
+        NextPageToken: str = ...,
     ) -> GetCostAndUsageWithResourcesResponseTypeDef:
         """
         Retrieves cost and usage metrics with resources for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_cost_and_usage_with_resources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#get_cost_and_usage_with_resources)
         """
@@ -341,15 +340,15 @@
         *,
         TimePeriod: DateIntervalTypeDef,
         SearchString: str = ...,
         CostCategoryName: str = ...,
         Filter: "ExpressionTypeDef" = ...,
         SortBy: Sequence[SortDefinitionTypeDef] = ...,
         MaxResults: int = ...,
-        NextPageToken: str = ...
+        NextPageToken: str = ...,
     ) -> GetCostCategoriesResponseTypeDef:
         """
         Retrieves an array of Cost Category names and values incurred cost.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_cost_categories)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#get_cost_categories)
         """
@@ -357,15 +356,15 @@
     async def get_cost_forecast(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Metric: MetricType,
         Granularity: GranularityType,
         Filter: "ExpressionTypeDef" = ...,
-        PredictionIntervalLevel: int = ...
+        PredictionIntervalLevel: int = ...,
     ) -> GetCostForecastResponseTypeDef:
         """
         Retrieves a forecast for how much Amazon Web Services predicts that you will
         spend over the forecast time period that you select, based on your past
         costs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_cost_forecast)
@@ -378,15 +377,15 @@
         TimePeriod: DateIntervalTypeDef,
         Dimension: DimensionType,
         SearchString: str = ...,
         Context: ContextType = ...,
         Filter: "ExpressionTypeDef" = ...,
         SortBy: Sequence[SortDefinitionTypeDef] = ...,
         MaxResults: int = ...,
-        NextPageToken: str = ...
+        NextPageToken: str = ...,
     ) -> GetDimensionValuesResponseTypeDef:
         """
         Retrieves all available filter values for a specified filter over a period of
         time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_dimension_values)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#get_dimension_values)
@@ -398,15 +397,15 @@
         TimePeriod: DateIntervalTypeDef,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
         Granularity: GranularityType = ...,
         Filter: "ExpressionTypeDef" = ...,
         Metrics: Sequence[str] = ...,
         NextPageToken: str = ...,
         SortBy: SortDefinitionTypeDef = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> GetReservationCoverageResponseTypeDef:
         """
         Retrieves the reservation coverage for your account, which you can use to see
         how much of your Amazon Elastic Compute Cloud, Amazon ElastiCache, Amazon
         Relational Database Service, or Amazon Redshift usage is covered by a
         reservation.
 
@@ -422,15 +421,15 @@
         Filter: "ExpressionTypeDef" = ...,
         AccountScope: AccountScopeType = ...,
         LookbackPeriodInDays: LookbackPeriodInDaysType = ...,
         TermInYears: TermInYearsType = ...,
         PaymentOption: PaymentOptionType = ...,
         ServiceSpecification: ServiceSpecificationTypeDef = ...,
         PageSize: int = ...,
-        NextPageToken: str = ...
+        NextPageToken: str = ...,
     ) -> GetReservationPurchaseRecommendationResponseTypeDef:
         """
         Gets recommendations for reservation purchases.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_reservation_purchase_recommendation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#get_reservation_purchase_recommendation)
         """
@@ -440,15 +439,15 @@
         *,
         TimePeriod: DateIntervalTypeDef,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
         Granularity: GranularityType = ...,
         Filter: "ExpressionTypeDef" = ...,
         SortBy: SortDefinitionTypeDef = ...,
         NextPageToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> GetReservationUtilizationResponseTypeDef:
         """
         Retrieves the reservation utilization for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_reservation_utilization)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#get_reservation_utilization)
         """
@@ -456,15 +455,15 @@
     async def get_rightsizing_recommendation(
         self,
         *,
         Service: str,
         Filter: "ExpressionTypeDef" = ...,
         Configuration: RightsizingRecommendationConfigurationTypeDef = ...,
         PageSize: int = ...,
-        NextPageToken: str = ...
+        NextPageToken: str = ...,
     ) -> GetRightsizingRecommendationResponseTypeDef:
         """
         Creates recommendations that help you save cost by identifying idle and
         underutilized Amazon EC2
         instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_rightsizing_recommendation)
@@ -487,15 +486,15 @@
         TimePeriod: DateIntervalTypeDef,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
         Granularity: GranularityType = ...,
         Filter: "ExpressionTypeDef" = ...,
         Metrics: Sequence[str] = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        SortBy: SortDefinitionTypeDef = ...
+        SortBy: SortDefinitionTypeDef = ...,
     ) -> GetSavingsPlansCoverageResponseTypeDef:
         """
         Retrieves the Savings Plans covered for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_savings_plans_coverage)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#get_savings_plans_coverage)
         """
@@ -506,30 +505,30 @@
         SavingsPlansType: SupportedSavingsPlansTypeType,
         TermInYears: TermInYearsType,
         PaymentOption: PaymentOptionType,
         LookbackPeriodInDays: LookbackPeriodInDaysType,
         AccountScope: AccountScopeType = ...,
         NextPageToken: str = ...,
         PageSize: int = ...,
-        Filter: "ExpressionTypeDef" = ...
+        Filter: "ExpressionTypeDef" = ...,
     ) -> GetSavingsPlansPurchaseRecommendationResponseTypeDef:
         """
         Retrieves the Savings Plans recommendations for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_savings_plans_purchase_recommendation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#get_savings_plans_purchase_recommendation)
         """
 
     async def get_savings_plans_utilization(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Granularity: GranularityType = ...,
         Filter: "ExpressionTypeDef" = ...,
-        SortBy: SortDefinitionTypeDef = ...
+        SortBy: SortDefinitionTypeDef = ...,
     ) -> GetSavingsPlansUtilizationResponseTypeDef:
         """
         Retrieves the Savings Plans utilization for your account across date ranges
         with daily or monthly
         granularity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_savings_plans_utilization)
@@ -540,15 +539,15 @@
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Filter: "ExpressionTypeDef" = ...,
         DataType: Sequence[SavingsPlansDataTypeType] = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        SortBy: SortDefinitionTypeDef = ...
+        SortBy: SortDefinitionTypeDef = ...,
     ) -> GetSavingsPlansUtilizationDetailsResponseTypeDef:
         """
         Retrieves attribute data along with aggregate utilization and savings data for
         a given time
         period.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_savings_plans_utilization_details)
@@ -560,15 +559,15 @@
         *,
         TimePeriod: DateIntervalTypeDef,
         SearchString: str = ...,
         TagKey: str = ...,
         Filter: "ExpressionTypeDef" = ...,
         SortBy: Sequence[SortDefinitionTypeDef] = ...,
         MaxResults: int = ...,
-        NextPageToken: str = ...
+        NextPageToken: str = ...,
     ) -> GetTagsResponseTypeDef:
         """
         Queries for available tag keys and tag values for a specified period.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_tags)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#get_tags)
         """
@@ -576,15 +575,15 @@
     async def get_usage_forecast(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Metric: MetricType,
         Granularity: GranularityType,
         Filter: "ExpressionTypeDef" = ...,
-        PredictionIntervalLevel: int = ...
+        PredictionIntervalLevel: int = ...,
     ) -> GetUsageForecastResponseTypeDef:
         """
         Retrieves a forecast for how much Amazon Web Services predicts that you will
         use over the forecast time period that you select, based on your past
         usage.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_usage_forecast)
@@ -594,15 +593,15 @@
     async def list_cost_allocation_tags(
         self,
         *,
         Status: CostAllocationTagStatusType = ...,
         TagKeys: Sequence[str] = ...,
         Type: CostAllocationTagTypeType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListCostAllocationTagsResponseTypeDef:
         """
         Get a list of cost allocation tags.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.list_cost_allocation_tags)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#list_cost_allocation_tags)
         """
@@ -621,15 +620,15 @@
 
     async def list_savings_plans_purchase_recommendation_generation(
         self,
         *,
         GenerationStatus: GenerationStatusType = ...,
         RecommendationIds: Sequence[str] = ...,
         PageSize: int = ...,
-        NextPageToken: str = ...
+        NextPageToken: str = ...,
     ) -> ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef:
         """
         Retrieves a list of your historical recommendation generations within the past
         30
         days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.list_savings_plans_purchase_recommendation_generation)
@@ -703,15 +702,15 @@
         *,
         SubscriptionArn: str,
         Threshold: float = ...,
         Frequency: AnomalySubscriptionFrequencyType = ...,
         MonitorArnList: Sequence[str] = ...,
         Subscribers: Sequence[SubscriberTypeDef] = ...,
         SubscriptionName: str = ...,
-        ThresholdExpression: "ExpressionTypeDef" = ...
+        ThresholdExpression: "ExpressionTypeDef" = ...,
     ) -> UpdateAnomalySubscriptionResponseTypeDef:
         """
         Updates an existing cost anomaly subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.update_anomaly_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#update_anomaly_subscription)
         """
@@ -730,15 +729,15 @@
         self,
         *,
         CostCategoryArn: str,
         RuleVersion: Literal["CostCategoryExpression.v1"],
         Rules: Sequence[CostCategoryRuleTypeDef],
         EffectiveStart: str = ...,
         DefaultValue: str = ...,
-        SplitChargeRules: Sequence[CostCategorySplitChargeRuleTypeDef] = ...
+        SplitChargeRules: Sequence[CostCategorySplitChargeRuleTypeDef] = ...,
     ) -> UpdateCostCategoryDefinitionResponseTypeDef:
         """
         Updates an existing Cost Category.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.update_cost_category_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#update_cost_category_definition)
         """
```

### Comparing `types-aiobotocore-ce-2.9.0/types_aiobotocore_ce/client.pyi` & `types-aiobotocore-ce-2.9.1/types_aiobotocore_ce/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -152,30 +152,30 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#close)
         """
 
     async def create_anomaly_monitor(
         self,
         *,
         AnomalyMonitor: AnomalyMonitorTypeDef,
-        ResourceTags: Sequence[ResourceTagTypeDef] = ...
+        ResourceTags: Sequence[ResourceTagTypeDef] = ...,
     ) -> CreateAnomalyMonitorResponseTypeDef:
         """
         Creates a new cost anomaly detection monitor with the requested type and
         monitor
         specification.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.create_anomaly_monitor)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#create_anomaly_monitor)
         """
 
     async def create_anomaly_subscription(
         self,
         *,
         AnomalySubscription: AnomalySubscriptionTypeDef,
-        ResourceTags: Sequence[ResourceTagTypeDef] = ...
+        ResourceTags: Sequence[ResourceTagTypeDef] = ...,
     ) -> CreateAnomalySubscriptionResponseTypeDef:
         """
         Adds an alert subscription to a cost anomaly detection monitor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.create_anomaly_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#create_anomaly_subscription)
         """
@@ -185,15 +185,15 @@
         *,
         Name: str,
         RuleVersion: Literal["CostCategoryExpression.v1"],
         Rules: Sequence[CostCategoryRuleTypeDef],
         EffectiveStart: str = ...,
         DefaultValue: str = ...,
         SplitChargeRules: Sequence[CostCategorySplitChargeRuleTypeDef] = ...,
-        ResourceTags: Sequence[ResourceTagTypeDef] = ...
+        ResourceTags: Sequence[ResourceTagTypeDef] = ...,
     ) -> CreateCostCategoryDefinitionResponseTypeDef:
         """
         Creates a new Cost Category with the requested name and rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.create_cost_category_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#create_cost_category_definition)
         """
@@ -254,15 +254,15 @@
         self,
         *,
         DateInterval: AnomalyDateIntervalTypeDef,
         MonitorArn: str = ...,
         Feedback: AnomalyFeedbackTypeType = ...,
         TotalImpact: TotalImpactFilterTypeDef = ...,
         NextPageToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> GetAnomaliesResponseTypeDef:
         """
         Retrieves all of the cost anomalies detected on your account during the time
         period that's specified by the `DateInterval`
         object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_anomalies)
@@ -270,30 +270,30 @@
         """
 
     async def get_anomaly_monitors(
         self,
         *,
         MonitorArnList: Sequence[str] = ...,
         NextPageToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> GetAnomalyMonitorsResponseTypeDef:
         """
         Retrieves the cost anomaly monitor definitions for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_anomaly_monitors)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#get_anomaly_monitors)
         """
 
     async def get_anomaly_subscriptions(
         self,
         *,
         SubscriptionArnList: Sequence[str] = ...,
         MonitorArn: str = ...,
         NextPageToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> GetAnomalySubscriptionsResponseTypeDef:
         """
         Retrieves the cost anomaly subscription objects for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_anomaly_subscriptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#get_anomaly_subscriptions)
         """
@@ -302,15 +302,15 @@
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Granularity: GranularityType,
         Metrics: Sequence[str],
         Filter: "ExpressionTypeDef" = ...,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
-        NextPageToken: str = ...
+        NextPageToken: str = ...,
     ) -> GetCostAndUsageResponseTypeDef:
         """
         Retrieves cost and usage metrics for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_cost_and_usage)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#get_cost_and_usage)
         """
@@ -319,15 +319,15 @@
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Granularity: GranularityType,
         Filter: "ExpressionTypeDef",
         Metrics: Sequence[str] = ...,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
-        NextPageToken: str = ...
+        NextPageToken: str = ...,
     ) -> GetCostAndUsageWithResourcesResponseTypeDef:
         """
         Retrieves cost and usage metrics with resources for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_cost_and_usage_with_resources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#get_cost_and_usage_with_resources)
         """
@@ -337,15 +337,15 @@
         *,
         TimePeriod: DateIntervalTypeDef,
         SearchString: str = ...,
         CostCategoryName: str = ...,
         Filter: "ExpressionTypeDef" = ...,
         SortBy: Sequence[SortDefinitionTypeDef] = ...,
         MaxResults: int = ...,
-        NextPageToken: str = ...
+        NextPageToken: str = ...,
     ) -> GetCostCategoriesResponseTypeDef:
         """
         Retrieves an array of Cost Category names and values incurred cost.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_cost_categories)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#get_cost_categories)
         """
@@ -353,15 +353,15 @@
     async def get_cost_forecast(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Metric: MetricType,
         Granularity: GranularityType,
         Filter: "ExpressionTypeDef" = ...,
-        PredictionIntervalLevel: int = ...
+        PredictionIntervalLevel: int = ...,
     ) -> GetCostForecastResponseTypeDef:
         """
         Retrieves a forecast for how much Amazon Web Services predicts that you will
         spend over the forecast time period that you select, based on your past
         costs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_cost_forecast)
@@ -374,15 +374,15 @@
         TimePeriod: DateIntervalTypeDef,
         Dimension: DimensionType,
         SearchString: str = ...,
         Context: ContextType = ...,
         Filter: "ExpressionTypeDef" = ...,
         SortBy: Sequence[SortDefinitionTypeDef] = ...,
         MaxResults: int = ...,
-        NextPageToken: str = ...
+        NextPageToken: str = ...,
     ) -> GetDimensionValuesResponseTypeDef:
         """
         Retrieves all available filter values for a specified filter over a period of
         time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_dimension_values)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#get_dimension_values)
@@ -394,15 +394,15 @@
         TimePeriod: DateIntervalTypeDef,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
         Granularity: GranularityType = ...,
         Filter: "ExpressionTypeDef" = ...,
         Metrics: Sequence[str] = ...,
         NextPageToken: str = ...,
         SortBy: SortDefinitionTypeDef = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> GetReservationCoverageResponseTypeDef:
         """
         Retrieves the reservation coverage for your account, which you can use to see
         how much of your Amazon Elastic Compute Cloud, Amazon ElastiCache, Amazon
         Relational Database Service, or Amazon Redshift usage is covered by a
         reservation.
 
@@ -418,15 +418,15 @@
         Filter: "ExpressionTypeDef" = ...,
         AccountScope: AccountScopeType = ...,
         LookbackPeriodInDays: LookbackPeriodInDaysType = ...,
         TermInYears: TermInYearsType = ...,
         PaymentOption: PaymentOptionType = ...,
         ServiceSpecification: ServiceSpecificationTypeDef = ...,
         PageSize: int = ...,
-        NextPageToken: str = ...
+        NextPageToken: str = ...,
     ) -> GetReservationPurchaseRecommendationResponseTypeDef:
         """
         Gets recommendations for reservation purchases.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_reservation_purchase_recommendation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#get_reservation_purchase_recommendation)
         """
@@ -436,15 +436,15 @@
         *,
         TimePeriod: DateIntervalTypeDef,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
         Granularity: GranularityType = ...,
         Filter: "ExpressionTypeDef" = ...,
         SortBy: SortDefinitionTypeDef = ...,
         NextPageToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> GetReservationUtilizationResponseTypeDef:
         """
         Retrieves the reservation utilization for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_reservation_utilization)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#get_reservation_utilization)
         """
@@ -452,15 +452,15 @@
     async def get_rightsizing_recommendation(
         self,
         *,
         Service: str,
         Filter: "ExpressionTypeDef" = ...,
         Configuration: RightsizingRecommendationConfigurationTypeDef = ...,
         PageSize: int = ...,
-        NextPageToken: str = ...
+        NextPageToken: str = ...,
     ) -> GetRightsizingRecommendationResponseTypeDef:
         """
         Creates recommendations that help you save cost by identifying idle and
         underutilized Amazon EC2
         instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_rightsizing_recommendation)
@@ -483,15 +483,15 @@
         TimePeriod: DateIntervalTypeDef,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
         Granularity: GranularityType = ...,
         Filter: "ExpressionTypeDef" = ...,
         Metrics: Sequence[str] = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        SortBy: SortDefinitionTypeDef = ...
+        SortBy: SortDefinitionTypeDef = ...,
     ) -> GetSavingsPlansCoverageResponseTypeDef:
         """
         Retrieves the Savings Plans covered for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_savings_plans_coverage)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#get_savings_plans_coverage)
         """
@@ -502,30 +502,30 @@
         SavingsPlansType: SupportedSavingsPlansTypeType,
         TermInYears: TermInYearsType,
         PaymentOption: PaymentOptionType,
         LookbackPeriodInDays: LookbackPeriodInDaysType,
         AccountScope: AccountScopeType = ...,
         NextPageToken: str = ...,
         PageSize: int = ...,
-        Filter: "ExpressionTypeDef" = ...
+        Filter: "ExpressionTypeDef" = ...,
     ) -> GetSavingsPlansPurchaseRecommendationResponseTypeDef:
         """
         Retrieves the Savings Plans recommendations for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_savings_plans_purchase_recommendation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#get_savings_plans_purchase_recommendation)
         """
 
     async def get_savings_plans_utilization(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Granularity: GranularityType = ...,
         Filter: "ExpressionTypeDef" = ...,
-        SortBy: SortDefinitionTypeDef = ...
+        SortBy: SortDefinitionTypeDef = ...,
     ) -> GetSavingsPlansUtilizationResponseTypeDef:
         """
         Retrieves the Savings Plans utilization for your account across date ranges
         with daily or monthly
         granularity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_savings_plans_utilization)
@@ -536,15 +536,15 @@
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Filter: "ExpressionTypeDef" = ...,
         DataType: Sequence[SavingsPlansDataTypeType] = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        SortBy: SortDefinitionTypeDef = ...
+        SortBy: SortDefinitionTypeDef = ...,
     ) -> GetSavingsPlansUtilizationDetailsResponseTypeDef:
         """
         Retrieves attribute data along with aggregate utilization and savings data for
         a given time
         period.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_savings_plans_utilization_details)
@@ -556,15 +556,15 @@
         *,
         TimePeriod: DateIntervalTypeDef,
         SearchString: str = ...,
         TagKey: str = ...,
         Filter: "ExpressionTypeDef" = ...,
         SortBy: Sequence[SortDefinitionTypeDef] = ...,
         MaxResults: int = ...,
-        NextPageToken: str = ...
+        NextPageToken: str = ...,
     ) -> GetTagsResponseTypeDef:
         """
         Queries for available tag keys and tag values for a specified period.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_tags)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#get_tags)
         """
@@ -572,15 +572,15 @@
     async def get_usage_forecast(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Metric: MetricType,
         Granularity: GranularityType,
         Filter: "ExpressionTypeDef" = ...,
-        PredictionIntervalLevel: int = ...
+        PredictionIntervalLevel: int = ...,
     ) -> GetUsageForecastResponseTypeDef:
         """
         Retrieves a forecast for how much Amazon Web Services predicts that you will
         use over the forecast time period that you select, based on your past
         usage.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_usage_forecast)
@@ -590,15 +590,15 @@
     async def list_cost_allocation_tags(
         self,
         *,
         Status: CostAllocationTagStatusType = ...,
         TagKeys: Sequence[str] = ...,
         Type: CostAllocationTagTypeType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListCostAllocationTagsResponseTypeDef:
         """
         Get a list of cost allocation tags.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.list_cost_allocation_tags)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#list_cost_allocation_tags)
         """
@@ -617,15 +617,15 @@
 
     async def list_savings_plans_purchase_recommendation_generation(
         self,
         *,
         GenerationStatus: GenerationStatusType = ...,
         RecommendationIds: Sequence[str] = ...,
         PageSize: int = ...,
-        NextPageToken: str = ...
+        NextPageToken: str = ...,
     ) -> ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef:
         """
         Retrieves a list of your historical recommendation generations within the past
         30
         days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.list_savings_plans_purchase_recommendation_generation)
@@ -699,15 +699,15 @@
         *,
         SubscriptionArn: str,
         Threshold: float = ...,
         Frequency: AnomalySubscriptionFrequencyType = ...,
         MonitorArnList: Sequence[str] = ...,
         Subscribers: Sequence[SubscriberTypeDef] = ...,
         SubscriptionName: str = ...,
-        ThresholdExpression: "ExpressionTypeDef" = ...
+        ThresholdExpression: "ExpressionTypeDef" = ...,
     ) -> UpdateAnomalySubscriptionResponseTypeDef:
         """
         Updates an existing cost anomaly subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.update_anomaly_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#update_anomaly_subscription)
         """
@@ -726,15 +726,15 @@
         self,
         *,
         CostCategoryArn: str,
         RuleVersion: Literal["CostCategoryExpression.v1"],
         Rules: Sequence[CostCategoryRuleTypeDef],
         EffectiveStart: str = ...,
         DefaultValue: str = ...,
-        SplitChargeRules: Sequence[CostCategorySplitChargeRuleTypeDef] = ...
+        SplitChargeRules: Sequence[CostCategorySplitChargeRuleTypeDef] = ...,
     ) -> UpdateCostCategoryDefinitionResponseTypeDef:
         """
         Updates an existing Cost Category.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.update_cost_category_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#update_cost_category_definition)
         """
```

### Comparing `types-aiobotocore-ce-2.9.0/types_aiobotocore_ce/literals.py` & `types-aiobotocore-ce-2.9.1/types_aiobotocore_ce/literals.py`

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
     "AccountScopeType",
     "AnomalyFeedbackTypeType",
     "AnomalySubscriptionFrequencyType",
     "ContextType",
     "CostAllocationTagStatusType",
     "CostAllocationTagTypeType",
@@ -57,15 +56,14 @@
     "SupportedSavingsPlansTypeType",
     "TermInYearsType",
     "CostExplorerServiceName",
     "ServiceName",
     "ResourceServiceName",
 )
 
-
 AccountScopeType = Literal["LINKED", "PAYER"]
 AnomalyFeedbackTypeType = Literal["NO", "PLANNED_ACTIVITY", "YES"]
 AnomalySubscriptionFrequencyType = Literal["DAILY", "IMMEDIATE", "WEEKLY"]
 ContextType = Literal["COST_AND_USAGE", "RESERVATIONS", "SAVINGS_PLANS"]
 CostAllocationTagStatusType = Literal["Active", "Inactive"]
 CostAllocationTagTypeType = Literal["AWSGenerated", "UserDefined"]
 CostCategoryInheritedValueDimensionNameType = Literal["LINKED_ACCOUNT_NAME", "TAG"]
```

### Comparing `types-aiobotocore-ce-2.9.0/types_aiobotocore_ce/literals.pyi` & `types-aiobotocore-ce-2.9.1/types_aiobotocore_ce/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ce-2.9.0/types_aiobotocore_ce/type_defs.py` & `types-aiobotocore-ce-2.9.1/types_aiobotocore_ce/type_defs.py`

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
     "AnomalyDateIntervalTypeDef",
     "AnomalyMonitorTypeDef",
     "AnomalyScoreTypeDef",
     "SubscriberTypeDef",
     "ImpactTypeDef",
     "RootCauseTypeDef",
```

### Comparing `types-aiobotocore-ce-2.9.0/types_aiobotocore_ce/type_defs.pyi` & `types-aiobotocore-ce-2.9.1/types_aiobotocore_ce/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ce-2.9.0/types_aiobotocore_ce.egg-info/PKG-INFO` & `types-aiobotocore-ce-2.9.1/types_aiobotocore_ce.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ce
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CostExplorer 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CostExplorer 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/
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
 
 <a id="types-aiobotocore-ce"></a>
 
 # types-aiobotocore-ce
 
 [![PyPI - types-aiobotocore-ce](https://img.shields.io/pypi/v/types-aiobotocore-ce.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ce)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ce.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ce)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ce)](https://pepy.tech/project/types-aiobotocore-ce)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CostExplorer 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
+[aiobotocore.CostExplorer 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
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
 [types-aiobotocore-ce docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-ce-2.9.0/types_aiobotocore_ce.egg-info/SOURCES.txt` & `types-aiobotocore-ce-2.9.1/types_aiobotocore_ce.egg-info/SOURCES.txt`

 * *Files identical despite different names*

