# Comparing `tmp/types-aiobotocore-xray-2.9.0.tar.gz` & `tmp/types-aiobotocore-xray-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-xray-2.9.0.tar", last modified: Wed Dec 13 20:00:49 2023, max compression
+gzip compressed data, was "types-aiobotocore-xray-2.9.1.tar", last modified: Thu Jan 18 01:22:05 2024, max compression
```

## Comparing `types-aiobotocore-xray-2.9.0.tar` & `types-aiobotocore-xray-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:49.000979 types-aiobotocore-xray-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:58:10.000000 types-aiobotocore-xray-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14200 2023-12-13 20:00:49.000979 types-aiobotocore-xray-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12649 2023-12-13 19:58:10.000000 types-aiobotocore-xray-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:49.000979 types-aiobotocore-xray-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2023-12-13 19:58:10.000000 types-aiobotocore-xray-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:49.000979 types-aiobotocore-xray-2.9.0/types_aiobotocore_xray/
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2023-12-13 19:58:10.000000 types-aiobotocore-xray-2.9.0/types_aiobotocore_xray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2023-12-13 19:58:10.000000 types-aiobotocore-xray-2.9.0/types_aiobotocore_xray/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      909 2023-12-13 19:58:10.000000 types-aiobotocore-xray-2.9.0/types_aiobotocore_xray/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27768 2023-12-13 19:58:11.000000 types-aiobotocore-xray-2.9.0/types_aiobotocore_xray/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    27764 2023-12-13 19:58:11.000000 types-aiobotocore-xray-2.9.0/types_aiobotocore_xray/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10531 2023-12-13 19:58:11.000000 types-aiobotocore-xray-2.9.0/types_aiobotocore_xray/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10529 2023-12-13 19:58:11.000000 types-aiobotocore-xray-2.9.0/types_aiobotocore_xray/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12667 2023-12-13 19:58:11.000000 types-aiobotocore-xray-2.9.0/types_aiobotocore_xray/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12655 2023-12-13 19:58:11.000000 types-aiobotocore-xray-2.9.0/types_aiobotocore_xray/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:10.000000 types-aiobotocore-xray-2.9.0/types_aiobotocore_xray/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    38984 2023-12-13 19:58:12.000000 types-aiobotocore-xray-2.9.0/types_aiobotocore_xray/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    38983 2023-12-13 19:58:11.000000 types-aiobotocore-xray-2.9.0/types_aiobotocore_xray/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:58:10.000000 types-aiobotocore-xray-2.9.0/types_aiobotocore_xray/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:49.000979 types-aiobotocore-xray-2.9.0/types_aiobotocore_xray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14200 2023-12-13 20:00:48.000000 types-aiobotocore-xray-2.9.0/types_aiobotocore_xray.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      756 2023-12-13 20:00:48.000000 types-aiobotocore-xray-2.9.0/types_aiobotocore_xray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:48.000000 types-aiobotocore-xray-2.9.0/types_aiobotocore_xray.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:48.000000 types-aiobotocore-xray-2.9.0/types_aiobotocore_xray.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:48.000000 types-aiobotocore-xray-2.9.0/types_aiobotocore_xray.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-13 20:00:48.000000 types-aiobotocore-xray-2.9.0/types_aiobotocore_xray.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:22:05.688958 types-aiobotocore-xray-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:19:36.000000 types-aiobotocore-xray-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14220 2024-01-18 01:22:05.688958 types-aiobotocore-xray-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12649 2024-01-18 01:19:36.000000 types-aiobotocore-xray-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:22:05.688958 types-aiobotocore-xray-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-01-18 01:19:36.000000 types-aiobotocore-xray-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:22:05.688958 types-aiobotocore-xray-2.9.1/types_aiobotocore_xray/
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-01-18 01:19:36.000000 types-aiobotocore-xray-2.9.1/types_aiobotocore_xray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-01-18 01:19:36.000000 types-aiobotocore-xray-2.9.1/types_aiobotocore_xray/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-01-18 01:19:36.000000 types-aiobotocore-xray-2.9.1/types_aiobotocore_xray/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27776 2024-01-18 01:19:36.000000 types-aiobotocore-xray-2.9.1/types_aiobotocore_xray/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27773 2024-01-18 01:19:36.000000 types-aiobotocore-xray-2.9.1/types_aiobotocore_xray/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10529 2024-01-18 01:19:36.000000 types-aiobotocore-xray-2.9.1/types_aiobotocore_xray/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10529 2024-01-18 01:19:36.000000 types-aiobotocore-xray-2.9.1/types_aiobotocore_xray/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12669 2024-01-18 01:19:36.000000 types-aiobotocore-xray-2.9.1/types_aiobotocore_xray/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12658 2024-01-18 01:19:36.000000 types-aiobotocore-xray-2.9.1/types_aiobotocore_xray/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:19:36.000000 types-aiobotocore-xray-2.9.1/types_aiobotocore_xray/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    38983 2024-01-18 01:19:37.000000 types-aiobotocore-xray-2.9.1/types_aiobotocore_xray/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38983 2024-01-18 01:19:37.000000 types-aiobotocore-xray-2.9.1/types_aiobotocore_xray/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:19:36.000000 types-aiobotocore-xray-2.9.1/types_aiobotocore_xray/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:22:05.688958 types-aiobotocore-xray-2.9.1/types_aiobotocore_xray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14220 2024-01-18 01:22:05.000000 types-aiobotocore-xray-2.9.1/types_aiobotocore_xray.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-01-18 01:22:05.000000 types-aiobotocore-xray-2.9.1/types_aiobotocore_xray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:22:05.000000 types-aiobotocore-xray-2.9.1/types_aiobotocore_xray.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:22:05.000000 types-aiobotocore-xray-2.9.1/types_aiobotocore_xray.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:22:05.000000 types-aiobotocore-xray-2.9.1/types_aiobotocore_xray.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-01-18 01:22:05.000000 types-aiobotocore-xray-2.9.1/types_aiobotocore_xray.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-xray-2.9.0/LICENSE` & `types-aiobotocore-xray-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-xray-2.9.0/PKG-INFO` & `types-aiobotocore-xray-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-xray
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.XRay 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.XRay 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/
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
 
 <a id="types-aiobotocore-xray"></a>
 
 # types-aiobotocore-xray
 
 [![PyPI - types-aiobotocore-xray](https://img.shields.io/pypi/v/types-aiobotocore-xray.svg?color=blue)](https://pypi.org/project/types-aiobotocore-xray)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-xray.svg?color=blue)](https://pypi.org/project/types-aiobotocore-xray)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-xray)](https://pepy.tech/project/types-aiobotocore-xray)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.XRay 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay)
+[aiobotocore.XRay 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay)
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
 [types-aiobotocore-xray docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-xray-2.9.0/README.md` & `types-aiobotocore-xray-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-xray.svg?color=blue)](https://pypi.org/project/types-aiobotocore-xray)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-xray)](https://pepy.tech/project/types-aiobotocore-xray)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.XRay 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay)
+[aiobotocore.XRay 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay)
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
 [types-aiobotocore-xray docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-xray-2.9.0/setup.py` & `types-aiobotocore-xray-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-xray",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_xray"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.XRay 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.XRay 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore xray type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_xray": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-xray-2.9.0/types_aiobotocore_xray/__init__.py` & `types-aiobotocore-xray-2.9.1/types_aiobotocore_xray/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,14 @@
     GetTraceSummariesPaginator,
     ListResourcePoliciesPaginator,
     ListTagsForResourcePaginator,
 )
 
 Client = XRayClient
 
-
 __all__ = (
     "BatchGetTracesPaginator",
     "Client",
     "GetGroupsPaginator",
     "GetSamplingRulesPaginator",
     "GetSamplingStatisticSummariesPaginator",
     "GetServiceGraphPaginator",
```

### Comparing `types-aiobotocore-xray-2.9.0/types_aiobotocore_xray/__init__.pyi` & `types-aiobotocore-xray-2.9.1/types_aiobotocore_xray/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-xray-2.9.0/types_aiobotocore_xray/__main__.py` & `types-aiobotocore-xray-2.9.1/types_aiobotocore_xray/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.XRay 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.XRay 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay\nOther"
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

### Comparing `types-aiobotocore-xray-2.9.0/types_aiobotocore_xray/client.py` & `types-aiobotocore-xray-2.9.1/types_aiobotocore_xray/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("XRayClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -146,15 +145,15 @@
 
     async def create_group(
         self,
         *,
         GroupName: str,
         FilterExpression: str = ...,
         InsightsConfiguration: InsightsConfigurationTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateGroupResultTypeDef:
         """
         Creates a group resource with a name and a filter expression.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.create_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/client/#create_group)
         """
@@ -259,15 +258,15 @@
 
     async def get_insight_impact_graph(
         self,
         *,
         InsightId: str,
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetInsightImpactGraphResultTypeDef:
         """
         Retrieves a service graph structure filtered by the specified insight.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_insight_impact_graph)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/client/#get_insight_impact_graph)
         """
@@ -277,15 +276,15 @@
         *,
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
         States: Sequence[InsightStateType] = ...,
         GroupARN: str = ...,
         GroupName: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetInsightSummariesResultTypeDef:
         """
         Retrieves the summaries of all insights in the specified group matching the
         provided filter
         values.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_insight_summaries)
@@ -324,15 +323,15 @@
     async def get_service_graph(
         self,
         *,
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
         GroupName: str = ...,
         GroupARN: str = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetServiceGraphResultTypeDef:
         """
         Retrieves a document that describes services that process incoming requests,
         and downstream services that they call as a
         result.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_service_graph)
@@ -345,15 +344,15 @@
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
         GroupName: str = ...,
         GroupARN: str = ...,
         EntitySelectorExpression: str = ...,
         Period: int = ...,
         ForecastStatistics: bool = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetTimeSeriesServiceStatisticsResultTypeDef:
         """
         Get an aggregation of service statistics defined by a specific time range.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_time_series_service_statistics)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/client/#get_time_series_service_statistics)
         """
@@ -373,15 +372,15 @@
         *,
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
         TimeRangeType: TimeRangeTypeType = ...,
         Sampling: bool = ...,
         SamplingStrategy: SamplingStrategyTypeDef = ...,
         FilterExpression: str = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetTraceSummariesResultTypeDef:
         """
         Retrieves IDs and annotations for traces available for a specified time frame
         using an optional
         filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_trace_summaries)
@@ -422,15 +421,15 @@
 
     async def put_resource_policy(
         self,
         *,
         PolicyName: str,
         PolicyDocument: str,
         PolicyRevisionId: str = ...,
-        BypassPolicyLockoutCheck: bool = ...
+        BypassPolicyLockoutCheck: bool = ...,
     ) -> PutResourcePolicyResultTypeDef:
         """
         Sets the resource policy to grant one or more Amazon Web Services services and
         accounts permissions to access
         X-Ray.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.put_resource_policy)
@@ -439,15 +438,15 @@
 
     async def put_telemetry_records(
         self,
         *,
         TelemetryRecords: Sequence[TelemetryRecordTypeDef],
         EC2InstanceId: str = ...,
         Hostname: str = ...,
-        ResourceARN: str = ...
+        ResourceARN: str = ...,
     ) -> Dict[str, Any]:
         """
         Used by the Amazon Web Services X-Ray daemon to upload telemetry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.put_telemetry_records)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/client/#put_telemetry_records)
         """
@@ -480,15 +479,15 @@
 
     async def update_group(
         self,
         *,
         GroupName: str = ...,
         GroupARN: str = ...,
         FilterExpression: str = ...,
-        InsightsConfiguration: InsightsConfigurationTypeDef = ...
+        InsightsConfiguration: InsightsConfigurationTypeDef = ...,
     ) -> UpdateGroupResultTypeDef:
         """
         Updates a group resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.update_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/client/#update_group)
         """
```

### Comparing `types-aiobotocore-xray-2.9.0/types_aiobotocore_xray/client.pyi` & `types-aiobotocore-xray-2.9.1/types_aiobotocore_xray/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
 
     async def create_group(
         self,
         *,
         GroupName: str,
         FilterExpression: str = ...,
         InsightsConfiguration: InsightsConfigurationTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateGroupResultTypeDef:
         """
         Creates a group resource with a name and a filter expression.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.create_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/client/#create_group)
         """
@@ -255,15 +255,15 @@
 
     async def get_insight_impact_graph(
         self,
         *,
         InsightId: str,
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetInsightImpactGraphResultTypeDef:
         """
         Retrieves a service graph structure filtered by the specified insight.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_insight_impact_graph)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/client/#get_insight_impact_graph)
         """
@@ -273,15 +273,15 @@
         *,
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
         States: Sequence[InsightStateType] = ...,
         GroupARN: str = ...,
         GroupName: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetInsightSummariesResultTypeDef:
         """
         Retrieves the summaries of all insights in the specified group matching the
         provided filter
         values.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_insight_summaries)
@@ -320,15 +320,15 @@
     async def get_service_graph(
         self,
         *,
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
         GroupName: str = ...,
         GroupARN: str = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetServiceGraphResultTypeDef:
         """
         Retrieves a document that describes services that process incoming requests,
         and downstream services that they call as a
         result.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_service_graph)
@@ -341,15 +341,15 @@
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
         GroupName: str = ...,
         GroupARN: str = ...,
         EntitySelectorExpression: str = ...,
         Period: int = ...,
         ForecastStatistics: bool = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetTimeSeriesServiceStatisticsResultTypeDef:
         """
         Get an aggregation of service statistics defined by a specific time range.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_time_series_service_statistics)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/client/#get_time_series_service_statistics)
         """
@@ -369,15 +369,15 @@
         *,
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
         TimeRangeType: TimeRangeTypeType = ...,
         Sampling: bool = ...,
         SamplingStrategy: SamplingStrategyTypeDef = ...,
         FilterExpression: str = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetTraceSummariesResultTypeDef:
         """
         Retrieves IDs and annotations for traces available for a specified time frame
         using an optional
         filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_trace_summaries)
@@ -418,15 +418,15 @@
 
     async def put_resource_policy(
         self,
         *,
         PolicyName: str,
         PolicyDocument: str,
         PolicyRevisionId: str = ...,
-        BypassPolicyLockoutCheck: bool = ...
+        BypassPolicyLockoutCheck: bool = ...,
     ) -> PutResourcePolicyResultTypeDef:
         """
         Sets the resource policy to grant one or more Amazon Web Services services and
         accounts permissions to access
         X-Ray.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.put_resource_policy)
@@ -435,15 +435,15 @@
 
     async def put_telemetry_records(
         self,
         *,
         TelemetryRecords: Sequence[TelemetryRecordTypeDef],
         EC2InstanceId: str = ...,
         Hostname: str = ...,
-        ResourceARN: str = ...
+        ResourceARN: str = ...,
     ) -> Dict[str, Any]:
         """
         Used by the Amazon Web Services X-Ray daemon to upload telemetry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.put_telemetry_records)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/client/#put_telemetry_records)
         """
@@ -476,15 +476,15 @@
 
     async def update_group(
         self,
         *,
         GroupName: str = ...,
         GroupARN: str = ...,
         FilterExpression: str = ...,
-        InsightsConfiguration: InsightsConfigurationTypeDef = ...
+        InsightsConfiguration: InsightsConfigurationTypeDef = ...,
     ) -> UpdateGroupResultTypeDef:
         """
         Updates a group resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.update_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/client/#update_group)
         """
```

### Comparing `types-aiobotocore-xray-2.9.0/types_aiobotocore_xray/literals.py` & `types-aiobotocore-xray-2.9.1/types_aiobotocore_xray/literals.py`

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
     "BatchGetTracesPaginatorName",
     "EncryptionStatusType",
     "EncryptionTypeType",
     "GetGroupsPaginatorName",
     "GetSamplingRulesPaginatorName",
     "GetSamplingStatisticSummariesPaginatorName",
@@ -40,15 +39,14 @@
     "XRayServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 BatchGetTracesPaginatorName = Literal["batch_get_traces"]
 EncryptionStatusType = Literal["ACTIVE", "UPDATING"]
 EncryptionTypeType = Literal["KMS", "NONE"]
 GetGroupsPaginatorName = Literal["get_groups"]
 GetSamplingRulesPaginatorName = Literal["get_sampling_rules"]
 GetSamplingStatisticSummariesPaginatorName = Literal["get_sampling_statistic_summaries"]
 GetServiceGraphPaginatorName = Literal["get_service_graph"]
```

### Comparing `types-aiobotocore-xray-2.9.0/types_aiobotocore_xray/literals.pyi` & `types-aiobotocore-xray-2.9.1/types_aiobotocore_xray/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-xray-2.9.0/types_aiobotocore_xray/paginator.py` & `types-aiobotocore-xray-2.9.1/types_aiobotocore_xray/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,14 @@
     "GetTimeSeriesServiceStatisticsPaginator",
     "GetTraceGraphPaginator",
     "GetTraceSummariesPaginator",
     "ListResourcePoliciesPaginator",
     "ListTagsForResourcePaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -154,15 +153,15 @@
     def paginate(
         self,
         *,
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
         GroupName: str = ...,
         GroupARN: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetServiceGraphResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetServiceGraph.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/paginators/#getservicegraphpaginator)
         """
 
 
@@ -178,15 +177,15 @@
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
         GroupName: str = ...,
         GroupARN: str = ...,
         EntitySelectorExpression: str = ...,
         Period: int = ...,
         ForecastStatistics: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetTimeSeriesServiceStatisticsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetTimeSeriesServiceStatistics.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/paginators/#gettimeseriesservicestatisticspaginator)
         """
 
 
@@ -216,15 +215,15 @@
         *,
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
         TimeRangeType: TimeRangeTypeType = ...,
         Sampling: bool = ...,
         SamplingStrategy: SamplingStrategyTypeDef = ...,
         FilterExpression: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetTraceSummariesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetTraceSummaries.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/paginators/#gettracesummariespaginator)
         """
```

### Comparing `types-aiobotocore-xray-2.9.0/types_aiobotocore_xray/paginator.pyi` & `types-aiobotocore-xray-2.9.1/types_aiobotocore_xray/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
     def paginate(
         self,
         *,
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
         GroupName: str = ...,
         GroupARN: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetServiceGraphResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetServiceGraph.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/paginators/#getservicegraphpaginator)
         """
 
 class GetTimeSeriesServiceStatisticsPaginator(AioPaginator):
@@ -170,15 +170,15 @@
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
         GroupName: str = ...,
         GroupARN: str = ...,
         EntitySelectorExpression: str = ...,
         Period: int = ...,
         ForecastStatistics: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetTimeSeriesServiceStatisticsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetTimeSeriesServiceStatistics.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/paginators/#gettimeseriesservicestatisticspaginator)
         """
 
 class GetTraceGraphPaginator(AioPaginator):
@@ -206,15 +206,15 @@
         *,
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
         TimeRangeType: TimeRangeTypeType = ...,
         Sampling: bool = ...,
         SamplingStrategy: SamplingStrategyTypeDef = ...,
         FilterExpression: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetTraceSummariesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetTraceSummaries.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/paginators/#gettracesummariespaginator)
         """
 
 class ListResourcePoliciesPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-xray-2.9.0/types_aiobotocore_xray/type_defs.py` & `types-aiobotocore-xray-2.9.1/types_aiobotocore_xray/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AliasTypeDef",
     "AnnotationValueTypeDef",
     "ServiceIdTypeDef",
     "AvailabilityZoneDetailTypeDef",
     "BackendConnectionErrorsTypeDef",
     "PaginatorConfigTypeDef",
```

### Comparing `types-aiobotocore-xray-2.9.0/types_aiobotocore_xray/type_defs.pyi` & `types-aiobotocore-xray-2.9.1/types_aiobotocore_xray/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-xray-2.9.0/types_aiobotocore_xray.egg-info/PKG-INFO` & `types-aiobotocore-xray-2.9.1/types_aiobotocore_xray.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-xray
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.XRay 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.XRay 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/
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
 
 <a id="types-aiobotocore-xray"></a>
 
 # types-aiobotocore-xray
 
 [![PyPI - types-aiobotocore-xray](https://img.shields.io/pypi/v/types-aiobotocore-xray.svg?color=blue)](https://pypi.org/project/types-aiobotocore-xray)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-xray.svg?color=blue)](https://pypi.org/project/types-aiobotocore-xray)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-xray)](https://pepy.tech/project/types-aiobotocore-xray)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.XRay 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay)
+[aiobotocore.XRay 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay)
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
 [types-aiobotocore-xray docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-xray-2.9.0/types_aiobotocore_xray.egg-info/SOURCES.txt` & `types-aiobotocore-xray-2.9.1/types_aiobotocore_xray.egg-info/SOURCES.txt`

 * *Files identical despite different names*

