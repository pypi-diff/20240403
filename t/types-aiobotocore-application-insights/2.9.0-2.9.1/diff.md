# Comparing `tmp/types-aiobotocore-application-insights-2.9.0.tar.gz` & `tmp/types-aiobotocore-application-insights-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-application-insights-2.9.0.tar", last modified: Wed Dec 13 19:58:35 2023, max compression
+gzip compressed data, was "types-aiobotocore-application-insights-2.9.1.tar", last modified: Thu Jan 18 01:20:03 2024, max compression
```

## Comparing `types-aiobotocore-application-insights-2.9.0.tar` & `types-aiobotocore-application-insights-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:35.346089 types-aiobotocore-application-insights-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:41:06.000000 types-aiobotocore-application-insights-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12937 2023-12-13 19:58:35.346089 types-aiobotocore-application-insights-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11323 2023-12-13 19:41:06.000000 types-aiobotocore-application-insights-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:35.346089 types-aiobotocore-application-insights-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2023-12-13 19:41:06.000000 types-aiobotocore-application-insights-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:35.346089 types-aiobotocore-application-insights-2.9.0/types_aiobotocore_application_insights/
--rw-r--r--   0 runner    (1001) docker     (127)      542 2023-12-13 19:41:06.000000 types-aiobotocore-application-insights-2.9.0/types_aiobotocore_application_insights/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2023-12-13 19:41:06.000000 types-aiobotocore-application-insights-2.9.0/types_aiobotocore_application_insights/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      982 2023-12-13 19:41:06.000000 types-aiobotocore-application-insights-2.9.0/types_aiobotocore_application_insights/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27262 2023-12-13 19:41:06.000000 types-aiobotocore-application-insights-2.9.0/types_aiobotocore_application_insights/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    27258 2023-12-13 19:41:06.000000 types-aiobotocore-application-insights-2.9.0/types_aiobotocore_application_insights/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10621 2023-12-13 19:41:06.000000 types-aiobotocore-application-insights-2.9.0/types_aiobotocore_application_insights/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10619 2023-12-13 19:41:06.000000 types-aiobotocore-application-insights-2.9.0/types_aiobotocore_application_insights/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:41:06.000000 types-aiobotocore-application-insights-2.9.0/types_aiobotocore_application_insights/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    23675 2023-12-13 19:41:07.000000 types-aiobotocore-application-insights-2.9.0/types_aiobotocore_application_insights/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    23674 2023-12-13 19:41:06.000000 types-aiobotocore-application-insights-2.9.0/types_aiobotocore_application_insights/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:41:06.000000 types-aiobotocore-application-insights-2.9.0/types_aiobotocore_application_insights/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:35.346089 types-aiobotocore-application-insights-2.9.0/types_aiobotocore_application_insights.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12937 2023-12-13 19:58:35.000000 types-aiobotocore-application-insights-2.9.0/types_aiobotocore_application_insights.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      955 2023-12-13 19:58:35.000000 types-aiobotocore-application-insights-2.9.0/types_aiobotocore_application_insights.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:35.000000 types-aiobotocore-application-insights-2.9.0/types_aiobotocore_application_insights.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:35.000000 types-aiobotocore-application-insights-2.9.0/types_aiobotocore_application_insights.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:35.000000 types-aiobotocore-application-insights-2.9.0/types_aiobotocore_application_insights.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-12-13 19:58:35.000000 types-aiobotocore-application-insights-2.9.0/types_aiobotocore_application_insights.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:03.385513 types-aiobotocore-application-insights-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:03:05.000000 types-aiobotocore-application-insights-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12957 2024-01-18 01:20:03.385513 types-aiobotocore-application-insights-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11323 2024-01-18 01:03:05.000000 types-aiobotocore-application-insights-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:03.385513 types-aiobotocore-application-insights-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-01-18 01:03:05.000000 types-aiobotocore-application-insights-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:03.385513 types-aiobotocore-application-insights-2.9.1/types_aiobotocore_application_insights/
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-01-18 01:03:05.000000 types-aiobotocore-application-insights-2.9.1/types_aiobotocore_application_insights/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-01-18 01:03:05.000000 types-aiobotocore-application-insights-2.9.1/types_aiobotocore_application_insights/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-01-18 01:03:05.000000 types-aiobotocore-application-insights-2.9.1/types_aiobotocore_application_insights/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27277 2024-01-18 01:03:05.000000 types-aiobotocore-application-insights-2.9.1/types_aiobotocore_application_insights/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27274 2024-01-18 01:03:05.000000 types-aiobotocore-application-insights-2.9.1/types_aiobotocore_application_insights/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10619 2024-01-18 01:03:05.000000 types-aiobotocore-application-insights-2.9.1/types_aiobotocore_application_insights/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10619 2024-01-18 01:03:05.000000 types-aiobotocore-application-insights-2.9.1/types_aiobotocore_application_insights/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:03:05.000000 types-aiobotocore-application-insights-2.9.1/types_aiobotocore_application_insights/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    23674 2024-01-18 01:03:06.000000 types-aiobotocore-application-insights-2.9.1/types_aiobotocore_application_insights/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23674 2024-01-18 01:03:05.000000 types-aiobotocore-application-insights-2.9.1/types_aiobotocore_application_insights/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:03:05.000000 types-aiobotocore-application-insights-2.9.1/types_aiobotocore_application_insights/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:03.385513 types-aiobotocore-application-insights-2.9.1/types_aiobotocore_application_insights.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12957 2024-01-18 01:20:03.000000 types-aiobotocore-application-insights-2.9.1/types_aiobotocore_application_insights.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-01-18 01:20:03.000000 types-aiobotocore-application-insights-2.9.1/types_aiobotocore_application_insights.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:03.000000 types-aiobotocore-application-insights-2.9.1/types_aiobotocore_application_insights.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:03.000000 types-aiobotocore-application-insights-2.9.1/types_aiobotocore_application_insights.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:03.000000 types-aiobotocore-application-insights-2.9.1/types_aiobotocore_application_insights.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-01-18 01:20:03.000000 types-aiobotocore-application-insights-2.9.1/types_aiobotocore_application_insights.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-application-insights-2.9.0/LICENSE` & `types-aiobotocore-application-insights-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-application-insights-2.9.0/PKG-INFO` & `types-aiobotocore-application-insights-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-application-insights
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ApplicationInsights 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ApplicationInsights 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/
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
 
 <a id="types-aiobotocore-application-insights"></a>
 
 # types-aiobotocore-application-insights
 
 [![PyPI - types-aiobotocore-application-insights](https://img.shields.io/pypi/v/types-aiobotocore-application-insights.svg?color=blue)](https://pypi.org/project/types-aiobotocore-application-insights)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-application-insights.svg?color=blue)](https://pypi.org/project/types-aiobotocore-application-insights)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-application-insights)](https://pepy.tech/project/types-aiobotocore-application-insights)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ApplicationInsights 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights)
+[aiobotocore.ApplicationInsights 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights)
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
 [types-aiobotocore-application-insights docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-application-insights-2.9.0/README.md` & `types-aiobotocore-application-insights-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-application-insights.svg?color=blue)](https://pypi.org/project/types-aiobotocore-application-insights)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-application-insights)](https://pepy.tech/project/types-aiobotocore-application-insights)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ApplicationInsights 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights)
+[aiobotocore.ApplicationInsights 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights)
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
 [types-aiobotocore-application-insights docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-application-insights-2.9.0/setup.py` & `types-aiobotocore-application-insights-2.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,50 +7,49 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-application-insights",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_application_insights"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ApplicationInsights 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.ApplicationInsights 2.9.1 service generated with"
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
     keywords=(
         "aiobotocore application-insights type-annotations botocore mypy typeshed autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_application_insights": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-application-insights-2.9.0/types_aiobotocore_application_insights/__init__.py` & `types-aiobotocore-application-insights-2.9.1/types_aiobotocore_application_insights/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,9 +18,8 @@
     ```
 """
 
 from .client import ApplicationInsightsClient
 
 Client = ApplicationInsightsClient
 
-
 __all__ = ("ApplicationInsightsClient", "Client")
```

### Comparing `types-aiobotocore-application-insights-2.9.0/types_aiobotocore_application_insights/__init__.pyi` & `types-aiobotocore-application-insights-2.9.1/types_aiobotocore_application_insights/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-application-insights-2.9.0/types_aiobotocore_application_insights/__main__.py` & `types-aiobotocore-application-insights-2.9.1/types_aiobotocore_application_insights/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ApplicationInsights 2.9.0\nVersion:        "
-        " 2.9.0\nBuilder version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.ApplicationInsights 2.9.1\nVersion:        "
+        " 2.9.1\nBuilder version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights\nOther"
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

### Comparing `types-aiobotocore-application-insights-2.9.0/types_aiobotocore_application_insights/client.py` & `types-aiobotocore-application-insights-2.9.1/types_aiobotocore_application_insights/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ApplicationInsightsClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -98,15 +97,15 @@
         """
 
     async def add_workload(
         self,
         *,
         ResourceGroupName: str,
         ComponentName: str,
-        WorkloadConfiguration: WorkloadConfigurationTypeDef
+        WorkloadConfiguration: WorkloadConfigurationTypeDef,
     ) -> AddWorkloadResponseTypeDef:
         """
         Adds a workload to a component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.add_workload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#add_workload)
         """
@@ -134,15 +133,15 @@
         OpsCenterEnabled: bool = ...,
         CWEMonitorEnabled: bool = ...,
         OpsItemSNSTopicArn: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         AutoConfigEnabled: bool = ...,
         AutoCreate: bool = ...,
         GroupingType: Literal["ACCOUNT_BASED"] = ...,
-        AttachMissingPermission: bool = ...
+        AttachMissingPermission: bool = ...,
     ) -> CreateApplicationResponseTypeDef:
         """
         Adds an application that is created from a resource group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.create_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#create_application)
         """
@@ -160,15 +159,15 @@
     async def create_log_pattern(
         self,
         *,
         ResourceGroupName: str,
         PatternSetName: str,
         PatternName: str,
         Pattern: str,
-        Rank: int
+        Rank: int,
     ) -> CreateLogPatternResponseTypeDef:
         """
         Adds an log pattern to a `LogPatternSet`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.create_log_pattern)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#create_log_pattern)
         """
@@ -235,15 +234,15 @@
     async def describe_component_configuration_recommendation(
         self,
         *,
         ResourceGroupName: str,
         ComponentName: str,
         Tier: TierType,
         WorkloadName: str = ...,
-        RecommendationType: RecommendationTypeType = ...
+        RecommendationType: RecommendationTypeType = ...,
     ) -> DescribeComponentConfigurationRecommendationResponseTypeDef:
         """
         Describes the recommended monitoring configuration of the component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.describe_component_configuration_recommendation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#describe_component_configuration_recommendation)
         """
@@ -324,15 +323,15 @@
 
     async def list_components(
         self,
         *,
         ResourceGroupName: str,
         MaxResults: int = ...,
         NextToken: str = ...,
-        AccountId: str = ...
+        AccountId: str = ...,
     ) -> ListComponentsResponseTypeDef:
         """
         Lists the auto-grouped, standalone, and custom components of the application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_components)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#list_components)
         """
@@ -342,15 +341,15 @@
         *,
         ResourceGroupName: str = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         EventStatus: ConfigurationEventStatusType = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        AccountId: str = ...
+        AccountId: str = ...,
     ) -> ListConfigurationHistoryResponseTypeDef:
         """
         Lists the INFO, WARN, and ERROR events for periodic configuration updates
         performed by Application
         Insights.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_configuration_history)
@@ -359,15 +358,15 @@
 
     async def list_log_pattern_sets(
         self,
         *,
         ResourceGroupName: str,
         MaxResults: int = ...,
         NextToken: str = ...,
-        AccountId: str = ...
+        AccountId: str = ...,
     ) -> ListLogPatternSetsResponseTypeDef:
         """
         Lists the log pattern sets in the specific application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_log_pattern_sets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#list_log_pattern_sets)
         """
@@ -375,15 +374,15 @@
     async def list_log_patterns(
         self,
         *,
         ResourceGroupName: str,
         PatternSetName: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        AccountId: str = ...
+        AccountId: str = ...,
     ) -> ListLogPatternsResponseTypeDef:
         """
         Lists the log patterns in the specific log `LogPatternSet`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_log_patterns)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#list_log_patterns)
         """
@@ -394,15 +393,15 @@
         AccountId: str = ...,
         ResourceGroupName: str = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         ComponentName: str = ...,
-        Visibility: VisibilityType = ...
+        Visibility: VisibilityType = ...,
     ) -> ListProblemsResponseTypeDef:
         """
         Lists the problems with your application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_problems)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#list_problems)
         """
@@ -422,15 +421,15 @@
     async def list_workloads(
         self,
         *,
         ResourceGroupName: str,
         ComponentName: str,
         MaxResults: int = ...,
         NextToken: str = ...,
-        AccountId: str = ...
+        AccountId: str = ...,
     ) -> ListWorkloadsResponseTypeDef:
         """
         Lists the workloads that are configured on a given component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_workloads)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#list_workloads)
         """
@@ -466,30 +465,30 @@
         *,
         ResourceGroupName: str,
         OpsCenterEnabled: bool = ...,
         CWEMonitorEnabled: bool = ...,
         OpsItemSNSTopicArn: str = ...,
         RemoveSNSTopic: bool = ...,
         AutoConfigEnabled: bool = ...,
-        AttachMissingPermission: bool = ...
+        AttachMissingPermission: bool = ...,
     ) -> UpdateApplicationResponseTypeDef:
         """
         Updates the application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.update_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#update_application)
         """
 
     async def update_component(
         self,
         *,
         ResourceGroupName: str,
         ComponentName: str,
         NewComponentName: str = ...,
-        ResourceList: Sequence[str] = ...
+        ResourceList: Sequence[str] = ...,
     ) -> Dict[str, Any]:
         """
         Updates the custom component name and/or the list of resources that make up the
         component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.update_component)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#update_component)
@@ -499,15 +498,15 @@
         self,
         *,
         ResourceGroupName: str,
         ComponentName: str,
         Monitor: bool = ...,
         Tier: TierType = ...,
         ComponentConfiguration: str = ...,
-        AutoConfigEnabled: bool = ...
+        AutoConfigEnabled: bool = ...,
     ) -> Dict[str, Any]:
         """
         Updates the monitoring configurations for the component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.update_component_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#update_component_configuration)
         """
@@ -515,44 +514,44 @@
     async def update_log_pattern(
         self,
         *,
         ResourceGroupName: str,
         PatternSetName: str,
         PatternName: str,
         Pattern: str = ...,
-        Rank: int = ...
+        Rank: int = ...,
     ) -> UpdateLogPatternResponseTypeDef:
         """
         Adds a log pattern to a `LogPatternSet`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.update_log_pattern)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#update_log_pattern)
         """
 
     async def update_problem(
         self,
         *,
         ProblemId: str,
         UpdateStatus: Literal["RESOLVED"] = ...,
-        Visibility: VisibilityType = ...
+        Visibility: VisibilityType = ...,
     ) -> Dict[str, Any]:
         """
         Updates the visibility of the problem or specifies the problem as `RESOLVED`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.update_problem)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#update_problem)
         """
 
     async def update_workload(
         self,
         *,
         ResourceGroupName: str,
         ComponentName: str,
         WorkloadConfiguration: WorkloadConfigurationTypeDef,
-        WorkloadId: str = ...
+        WorkloadId: str = ...,
     ) -> UpdateWorkloadResponseTypeDef:
         """
         Adds a workload to a component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.update_workload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#update_workload)
         """
```

### Comparing `types-aiobotocore-application-insights-2.9.0/types_aiobotocore_application_insights/client.pyi` & `types-aiobotocore-application-insights-2.9.1/types_aiobotocore_application_insights/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         """
 
     async def add_workload(
         self,
         *,
         ResourceGroupName: str,
         ComponentName: str,
-        WorkloadConfiguration: WorkloadConfigurationTypeDef
+        WorkloadConfiguration: WorkloadConfigurationTypeDef,
     ) -> AddWorkloadResponseTypeDef:
         """
         Adds a workload to a component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.add_workload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#add_workload)
         """
@@ -130,15 +130,15 @@
         OpsCenterEnabled: bool = ...,
         CWEMonitorEnabled: bool = ...,
         OpsItemSNSTopicArn: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         AutoConfigEnabled: bool = ...,
         AutoCreate: bool = ...,
         GroupingType: Literal["ACCOUNT_BASED"] = ...,
-        AttachMissingPermission: bool = ...
+        AttachMissingPermission: bool = ...,
     ) -> CreateApplicationResponseTypeDef:
         """
         Adds an application that is created from a resource group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.create_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#create_application)
         """
@@ -156,15 +156,15 @@
     async def create_log_pattern(
         self,
         *,
         ResourceGroupName: str,
         PatternSetName: str,
         PatternName: str,
         Pattern: str,
-        Rank: int
+        Rank: int,
     ) -> CreateLogPatternResponseTypeDef:
         """
         Adds an log pattern to a `LogPatternSet`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.create_log_pattern)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#create_log_pattern)
         """
@@ -231,15 +231,15 @@
     async def describe_component_configuration_recommendation(
         self,
         *,
         ResourceGroupName: str,
         ComponentName: str,
         Tier: TierType,
         WorkloadName: str = ...,
-        RecommendationType: RecommendationTypeType = ...
+        RecommendationType: RecommendationTypeType = ...,
     ) -> DescribeComponentConfigurationRecommendationResponseTypeDef:
         """
         Describes the recommended monitoring configuration of the component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.describe_component_configuration_recommendation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#describe_component_configuration_recommendation)
         """
@@ -320,15 +320,15 @@
 
     async def list_components(
         self,
         *,
         ResourceGroupName: str,
         MaxResults: int = ...,
         NextToken: str = ...,
-        AccountId: str = ...
+        AccountId: str = ...,
     ) -> ListComponentsResponseTypeDef:
         """
         Lists the auto-grouped, standalone, and custom components of the application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_components)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#list_components)
         """
@@ -338,15 +338,15 @@
         *,
         ResourceGroupName: str = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         EventStatus: ConfigurationEventStatusType = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        AccountId: str = ...
+        AccountId: str = ...,
     ) -> ListConfigurationHistoryResponseTypeDef:
         """
         Lists the INFO, WARN, and ERROR events for periodic configuration updates
         performed by Application
         Insights.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_configuration_history)
@@ -355,15 +355,15 @@
 
     async def list_log_pattern_sets(
         self,
         *,
         ResourceGroupName: str,
         MaxResults: int = ...,
         NextToken: str = ...,
-        AccountId: str = ...
+        AccountId: str = ...,
     ) -> ListLogPatternSetsResponseTypeDef:
         """
         Lists the log pattern sets in the specific application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_log_pattern_sets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#list_log_pattern_sets)
         """
@@ -371,15 +371,15 @@
     async def list_log_patterns(
         self,
         *,
         ResourceGroupName: str,
         PatternSetName: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        AccountId: str = ...
+        AccountId: str = ...,
     ) -> ListLogPatternsResponseTypeDef:
         """
         Lists the log patterns in the specific log `LogPatternSet`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_log_patterns)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#list_log_patterns)
         """
@@ -390,15 +390,15 @@
         AccountId: str = ...,
         ResourceGroupName: str = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         ComponentName: str = ...,
-        Visibility: VisibilityType = ...
+        Visibility: VisibilityType = ...,
     ) -> ListProblemsResponseTypeDef:
         """
         Lists the problems with your application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_problems)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#list_problems)
         """
@@ -418,15 +418,15 @@
     async def list_workloads(
         self,
         *,
         ResourceGroupName: str,
         ComponentName: str,
         MaxResults: int = ...,
         NextToken: str = ...,
-        AccountId: str = ...
+        AccountId: str = ...,
     ) -> ListWorkloadsResponseTypeDef:
         """
         Lists the workloads that are configured on a given component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_workloads)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#list_workloads)
         """
@@ -462,30 +462,30 @@
         *,
         ResourceGroupName: str,
         OpsCenterEnabled: bool = ...,
         CWEMonitorEnabled: bool = ...,
         OpsItemSNSTopicArn: str = ...,
         RemoveSNSTopic: bool = ...,
         AutoConfigEnabled: bool = ...,
-        AttachMissingPermission: bool = ...
+        AttachMissingPermission: bool = ...,
     ) -> UpdateApplicationResponseTypeDef:
         """
         Updates the application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.update_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#update_application)
         """
 
     async def update_component(
         self,
         *,
         ResourceGroupName: str,
         ComponentName: str,
         NewComponentName: str = ...,
-        ResourceList: Sequence[str] = ...
+        ResourceList: Sequence[str] = ...,
     ) -> Dict[str, Any]:
         """
         Updates the custom component name and/or the list of resources that make up the
         component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.update_component)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#update_component)
@@ -495,15 +495,15 @@
         self,
         *,
         ResourceGroupName: str,
         ComponentName: str,
         Monitor: bool = ...,
         Tier: TierType = ...,
         ComponentConfiguration: str = ...,
-        AutoConfigEnabled: bool = ...
+        AutoConfigEnabled: bool = ...,
     ) -> Dict[str, Any]:
         """
         Updates the monitoring configurations for the component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.update_component_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#update_component_configuration)
         """
@@ -511,44 +511,44 @@
     async def update_log_pattern(
         self,
         *,
         ResourceGroupName: str,
         PatternSetName: str,
         PatternName: str,
         Pattern: str = ...,
-        Rank: int = ...
+        Rank: int = ...,
     ) -> UpdateLogPatternResponseTypeDef:
         """
         Adds a log pattern to a `LogPatternSet`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.update_log_pattern)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#update_log_pattern)
         """
 
     async def update_problem(
         self,
         *,
         ProblemId: str,
         UpdateStatus: Literal["RESOLVED"] = ...,
-        Visibility: VisibilityType = ...
+        Visibility: VisibilityType = ...,
     ) -> Dict[str, Any]:
         """
         Updates the visibility of the problem or specifies the problem as `RESOLVED`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.update_problem)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#update_problem)
         """
 
     async def update_workload(
         self,
         *,
         ResourceGroupName: str,
         ComponentName: str,
         WorkloadConfiguration: WorkloadConfigurationTypeDef,
-        WorkloadId: str = ...
+        WorkloadId: str = ...,
     ) -> UpdateWorkloadResponseTypeDef:
         """
         Adds a workload to a component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.update_workload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#update_workload)
         """
```

### Comparing `types-aiobotocore-application-insights-2.9.0/types_aiobotocore_application_insights/literals.py` & `types-aiobotocore-application-insights-2.9.1/types_aiobotocore_application_insights/literals.py`

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
     "CloudWatchEventSourceType",
     "ConfigurationEventResourceTypeType",
     "ConfigurationEventStatusType",
     "DiscoveryTypeType",
     "FeedbackKeyType",
     "FeedbackValueType",
@@ -39,15 +38,14 @@
     "VisibilityType",
     "ApplicationInsightsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 CloudWatchEventSourceType = Literal["CODE_DEPLOY", "EC2", "HEALTH", "RDS"]
 ConfigurationEventResourceTypeType = Literal[
     "CLOUDFORMATION", "CLOUDWATCH_ALARM", "CLOUDWATCH_LOG", "SSM_ASSOCIATION"
 ]
 ConfigurationEventStatusType = Literal["ERROR", "INFO", "WARN"]
 DiscoveryTypeType = Literal["ACCOUNT_BASED", "RESOURCE_GROUP_BASED"]
 FeedbackKeyType = Literal["INSIGHTS_FEEDBACK"]
```

### Comparing `types-aiobotocore-application-insights-2.9.0/types_aiobotocore_application_insights/literals.pyi` & `types-aiobotocore-application-insights-2.9.1/types_aiobotocore_application_insights/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-application-insights-2.9.0/types_aiobotocore_application_insights/type_defs.py` & `types-aiobotocore-application-insights-2.9.1/types_aiobotocore_application_insights/type_defs.py`

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
     "WorkloadConfigurationTypeDef",
     "ResponseMetadataTypeDef",
     "ApplicationComponentTypeDef",
     "ApplicationInfoTypeDef",
     "ConfigurationEventTypeDef",
     "TagTypeDef",
```

### Comparing `types-aiobotocore-application-insights-2.9.0/types_aiobotocore_application_insights/type_defs.pyi` & `types-aiobotocore-application-insights-2.9.1/types_aiobotocore_application_insights/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-application-insights-2.9.0/types_aiobotocore_application_insights.egg-info/PKG-INFO` & `types-aiobotocore-application-insights-2.9.1/types_aiobotocore_application_insights.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-application-insights
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ApplicationInsights 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ApplicationInsights 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/
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
 
 <a id="types-aiobotocore-application-insights"></a>
 
 # types-aiobotocore-application-insights
 
 [![PyPI - types-aiobotocore-application-insights](https://img.shields.io/pypi/v/types-aiobotocore-application-insights.svg?color=blue)](https://pypi.org/project/types-aiobotocore-application-insights)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-application-insights.svg?color=blue)](https://pypi.org/project/types-aiobotocore-application-insights)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-application-insights)](https://pepy.tech/project/types-aiobotocore-application-insights)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ApplicationInsights 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights)
+[aiobotocore.ApplicationInsights 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights)
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
 [types-aiobotocore-application-insights docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-application-insights-2.9.0/types_aiobotocore_application_insights.egg-info/SOURCES.txt` & `types-aiobotocore-application-insights-2.9.1/types_aiobotocore_application_insights.egg-info/SOURCES.txt`

 * *Files identical despite different names*

