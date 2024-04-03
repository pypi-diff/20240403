# Comparing `tmp/types-aiobotocore-datazone-2.9.0.tar.gz` & `tmp/types-aiobotocore-datazone-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-datazone-2.9.0.tar", last modified: Wed Dec 13 19:59:04 2023, max compression
+gzip compressed data, was "types-aiobotocore-datazone-2.9.1.tar", last modified: Thu Jan 18 01:20:30 2024, max compression
```

## Comparing `types-aiobotocore-datazone-2.9.0.tar` & `types-aiobotocore-datazone-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:04.577850 types-aiobotocore-datazone-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:43:52.000000 types-aiobotocore-datazone-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16202 2023-12-13 19:59:04.577850 types-aiobotocore-datazone-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14635 2023-12-13 19:43:52.000000 types-aiobotocore-datazone-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:04.577850 types-aiobotocore-datazone-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2023-12-13 19:43:52.000000 types-aiobotocore-datazone-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:04.573850 types-aiobotocore-datazone-2.9.0/types_aiobotocore_datazone/
--rw-r--r--   0 runner    (1001) docker     (127)     5124 2023-12-13 19:43:52.000000 types-aiobotocore-datazone-2.9.0/types_aiobotocore_datazone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5123 2023-12-13 19:43:52.000000 types-aiobotocore-datazone-2.9.0/types_aiobotocore_datazone/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      936 2023-12-13 19:43:52.000000 types-aiobotocore-datazone-2.9.0/types_aiobotocore_datazone/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    83005 2023-12-13 19:43:53.000000 types-aiobotocore-datazone-2.9.0/types_aiobotocore_datazone/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    83001 2023-12-13 19:43:52.000000 types-aiobotocore-datazone-2.9.0/types_aiobotocore_datazone/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    17856 2023-12-13 19:43:54.000000 types-aiobotocore-datazone-2.9.0/types_aiobotocore_datazone/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    17854 2023-12-13 19:43:54.000000 types-aiobotocore-datazone-2.9.0/types_aiobotocore_datazone/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    29178 2023-12-13 19:43:54.000000 types-aiobotocore-datazone-2.9.0/types_aiobotocore_datazone/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    29154 2023-12-13 19:43:53.000000 types-aiobotocore-datazone-2.9.0/types_aiobotocore_datazone/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:43:52.000000 types-aiobotocore-datazone-2.9.0/types_aiobotocore_datazone/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   118843 2023-12-13 19:43:57.000000 types-aiobotocore-datazone-2.9.0/types_aiobotocore_datazone/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   118842 2023-12-13 19:43:55.000000 types-aiobotocore-datazone-2.9.0/types_aiobotocore_datazone/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:43:52.000000 types-aiobotocore-datazone-2.9.0/types_aiobotocore_datazone/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:04.577850 types-aiobotocore-datazone-2.9.0/types_aiobotocore_datazone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16202 2023-12-13 19:59:04.000000 types-aiobotocore-datazone-2.9.0/types_aiobotocore_datazone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      832 2023-12-13 19:59:04.000000 types-aiobotocore-datazone-2.9.0/types_aiobotocore_datazone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:04.000000 types-aiobotocore-datazone-2.9.0/types_aiobotocore_datazone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:04.000000 types-aiobotocore-datazone-2.9.0/types_aiobotocore_datazone.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:04.000000 types-aiobotocore-datazone-2.9.0/types_aiobotocore_datazone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-13 19:59:04.000000 types-aiobotocore-datazone-2.9.0/types_aiobotocore_datazone.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:30.113396 types-aiobotocore-datazone-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:05:48.000000 types-aiobotocore-datazone-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16222 2024-01-18 01:20:30.113396 types-aiobotocore-datazone-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14635 2024-01-18 01:05:48.000000 types-aiobotocore-datazone-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:30.113396 types-aiobotocore-datazone-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-01-18 01:05:47.000000 types-aiobotocore-datazone-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:30.113396 types-aiobotocore-datazone-2.9.1/types_aiobotocore_datazone/
+-rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-01-18 01:05:48.000000 types-aiobotocore-datazone-2.9.1/types_aiobotocore_datazone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-01-18 01:05:48.000000 types-aiobotocore-datazone-2.9.1/types_aiobotocore_datazone/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-01-18 01:05:48.000000 types-aiobotocore-datazone-2.9.1/types_aiobotocore_datazone/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83052 2024-01-18 01:05:48.000000 types-aiobotocore-datazone-2.9.1/types_aiobotocore_datazone/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83049 2024-01-18 01:05:48.000000 types-aiobotocore-datazone-2.9.1/types_aiobotocore_datazone/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    17854 2024-01-18 01:05:49.000000 types-aiobotocore-datazone-2.9.1/types_aiobotocore_datazone/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17854 2024-01-18 01:05:49.000000 types-aiobotocore-datazone-2.9.1/types_aiobotocore_datazone/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    29195 2024-01-18 01:05:48.000000 types-aiobotocore-datazone-2.9.1/types_aiobotocore_datazone/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29173 2024-01-18 01:05:48.000000 types-aiobotocore-datazone-2.9.1/types_aiobotocore_datazone/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:05:48.000000 types-aiobotocore-datazone-2.9.1/types_aiobotocore_datazone/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   118842 2024-01-18 01:05:52.000000 types-aiobotocore-datazone-2.9.1/types_aiobotocore_datazone/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   118842 2024-01-18 01:05:51.000000 types-aiobotocore-datazone-2.9.1/types_aiobotocore_datazone/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:05:48.000000 types-aiobotocore-datazone-2.9.1/types_aiobotocore_datazone/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:30.113396 types-aiobotocore-datazone-2.9.1/types_aiobotocore_datazone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16222 2024-01-18 01:20:30.000000 types-aiobotocore-datazone-2.9.1/types_aiobotocore_datazone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-01-18 01:20:30.000000 types-aiobotocore-datazone-2.9.1/types_aiobotocore_datazone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:30.000000 types-aiobotocore-datazone-2.9.1/types_aiobotocore_datazone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:30.000000 types-aiobotocore-datazone-2.9.1/types_aiobotocore_datazone.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:30.000000 types-aiobotocore-datazone-2.9.1/types_aiobotocore_datazone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-18 01:20:30.000000 types-aiobotocore-datazone-2.9.1/types_aiobotocore_datazone.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-datazone-2.9.0/LICENSE` & `types-aiobotocore-datazone-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-datazone-2.9.0/PKG-INFO` & `types-aiobotocore-datazone-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-datazone
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.DataZone 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.DataZone 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/
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
 
 <a id="types-aiobotocore-datazone"></a>
 
 # types-aiobotocore-datazone
 
 [![PyPI - types-aiobotocore-datazone](https://img.shields.io/pypi/v/types-aiobotocore-datazone.svg?color=blue)](https://pypi.org/project/types-aiobotocore-datazone)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-datazone.svg?color=blue)](https://pypi.org/project/types-aiobotocore-datazone)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-datazone)](https://pepy.tech/project/types-aiobotocore-datazone)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DataZone 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone)
+[aiobotocore.DataZone 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone)
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
 [types-aiobotocore-datazone docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-datazone-2.9.0/README.md` & `types-aiobotocore-datazone-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-datazone.svg?color=blue)](https://pypi.org/project/types-aiobotocore-datazone)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-datazone)](https://pepy.tech/project/types-aiobotocore-datazone)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DataZone 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone)
+[aiobotocore.DataZone 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone)
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
 [types-aiobotocore-datazone docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-datazone-2.9.0/setup.py` & `types-aiobotocore-datazone-2.9.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-datazone",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_datazone"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.DataZone 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.DataZone 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore datazone type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_datazone": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-datazone-2.9.0/types_aiobotocore_datazone/__init__.py` & `types-aiobotocore-datazone-2.9.1/types_aiobotocore_datazone/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,14 @@
     SearchPaginator,
     SearchTypesPaginator,
     SearchUserProfilesPaginator,
 )
 
 Client = DataZoneClient
 
-
 __all__ = (
     "Client",
     "DataZoneClient",
     "ListAssetRevisionsPaginator",
     "ListDataSourceRunActivitiesPaginator",
     "ListDataSourceRunsPaginator",
     "ListDataSourcesPaginator",
```

### Comparing `types-aiobotocore-datazone-2.9.0/types_aiobotocore_datazone/__init__.pyi` & `types-aiobotocore-datazone-2.9.1/types_aiobotocore_datazone/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-datazone-2.9.0/types_aiobotocore_datazone/__main__.py` & `types-aiobotocore-datazone-2.9.1/types_aiobotocore_datazone/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.DataZone 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.DataZone 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone\nOther"
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

### Comparing `types-aiobotocore-datazone-2.9.0/types_aiobotocore_datazone/client.py` & `types-aiobotocore-datazone-2.9.1/types_aiobotocore_datazone/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,15 +185,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("DataZoneClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -234,15 +233,15 @@
         self,
         *,
         domainIdentifier: str,
         identifier: str,
         acceptChoices: Sequence[AcceptChoiceTypeDef] = ...,
         acceptRule: AcceptRuleTypeDef = ...,
         clientToken: str = ...,
-        revision: str = ...
+        revision: str = ...,
     ) -> AcceptPredictionsOutputTypeDef:
         """
         Accepts automatically generated business-friendly metadata for your Amazon
         DataZone
         assets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.accept_predictions)
@@ -294,15 +293,15 @@
         typeIdentifier: str,
         clientToken: str = ...,
         description: str = ...,
         externalIdentifier: str = ...,
         formsInput: Sequence[FormInputTypeDef] = ...,
         glossaryTerms: Sequence[str] = ...,
         predictionConfiguration: PredictionConfigurationTypeDef = ...,
-        typeRevision: str = ...
+        typeRevision: str = ...,
     ) -> CreateAssetOutputTypeDef:
         """
         Creates an asset in Amazon DataZone catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_asset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#create_asset)
         """
@@ -314,15 +313,15 @@
         identifier: str,
         name: str,
         clientToken: str = ...,
         description: str = ...,
         formsInput: Sequence[FormInputTypeDef] = ...,
         glossaryTerms: Sequence[str] = ...,
         predictionConfiguration: PredictionConfigurationTypeDef = ...,
-        typeRevision: str = ...
+        typeRevision: str = ...,
     ) -> CreateAssetRevisionOutputTypeDef:
         """
         Creates a revision of the asset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_asset_revision)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#create_asset_revision)
         """
@@ -330,15 +329,15 @@
     async def create_asset_type(
         self,
         *,
         domainIdentifier: str,
         formsInput: Mapping[str, FormEntryInputTypeDef],
         name: str,
         owningProjectIdentifier: str,
-        description: str = ...
+        description: str = ...,
     ) -> CreateAssetTypeOutputTypeDef:
         """
         Creates a custom asset type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_asset_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#create_asset_type)
         """
@@ -354,15 +353,15 @@
         assetFormsInput: Sequence[FormInputTypeDef] = ...,
         clientToken: str = ...,
         configuration: DataSourceConfigurationInputTypeDef = ...,
         description: str = ...,
         enableSetting: EnableSettingType = ...,
         publishOnImport: bool = ...,
         recommendation: RecommendationConfigurationTypeDef = ...,
-        schedule: ScheduleConfigurationTypeDef = ...
+        schedule: ScheduleConfigurationTypeDef = ...,
     ) -> CreateDataSourceOutputTypeDef:
         """
         Creates an Amazon DataZone data source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_data_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#create_data_source)
         """
@@ -372,15 +371,15 @@
         *,
         domainExecutionRole: str,
         name: str,
         clientToken: str = ...,
         description: str = ...,
         kmsKeyIdentifier: str = ...,
         singleSignOn: SingleSignOnTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateDomainOutputTypeDef:
         """
         Creates an Amazon DataZone domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_domain)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#create_domain)
         """
@@ -390,15 +389,15 @@
         *,
         domainIdentifier: str,
         environmentProfileIdentifier: str,
         name: str,
         projectIdentifier: str,
         description: str = ...,
         glossaryTerms: Sequence[str] = ...,
-        userParameters: Sequence[EnvironmentParameterTypeDef] = ...
+        userParameters: Sequence[EnvironmentParameterTypeDef] = ...,
     ) -> CreateEnvironmentOutputTypeDef:
         """
         Create an Amazon DataZone environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#create_environment)
         """
@@ -409,15 +408,15 @@
         domainIdentifier: str,
         environmentBlueprintIdentifier: str,
         name: str,
         projectIdentifier: str,
         awsAccountId: str = ...,
         awsAccountRegion: str = ...,
         description: str = ...,
-        userParameters: Sequence[EnvironmentParameterTypeDef] = ...
+        userParameters: Sequence[EnvironmentParameterTypeDef] = ...,
     ) -> CreateEnvironmentProfileOutputTypeDef:
         """
         Creates an Amazon DataZone environment profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_environment_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#create_environment_profile)
         """
@@ -426,15 +425,15 @@
         self,
         *,
         domainIdentifier: str,
         model: ModelTypeDef,
         name: str,
         owningProjectIdentifier: str,
         description: str = ...,
-        status: FormTypeStatusType = ...
+        status: FormTypeStatusType = ...,
     ) -> CreateFormTypeOutputTypeDef:
         """
         Creates a metadata form type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_form_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#create_form_type)
         """
@@ -443,15 +442,15 @@
         self,
         *,
         domainIdentifier: str,
         name: str,
         owningProjectIdentifier: str,
         clientToken: str = ...,
         description: str = ...,
-        status: GlossaryStatusType = ...
+        status: GlossaryStatusType = ...,
     ) -> CreateGlossaryOutputTypeDef:
         """
         Creates an Amazon DataZone business glossary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_glossary)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#create_glossary)
         """
@@ -462,15 +461,15 @@
         domainIdentifier: str,
         glossaryIdentifier: str,
         name: str,
         clientToken: str = ...,
         longDescription: str = ...,
         shortDescription: str = ...,
         status: GlossaryTermStatusType = ...,
-        termRelations: TermRelationsTypeDef = ...
+        termRelations: TermRelationsTypeDef = ...,
     ) -> CreateGlossaryTermOutputTypeDef:
         """
         Creates a business glossary term.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_glossary_term)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#create_glossary_term)
         """
@@ -489,15 +488,15 @@
         self,
         *,
         action: ChangeActionType,
         domainIdentifier: str,
         entityIdentifier: str,
         entityType: Literal["ASSET"],
         clientToken: str = ...,
-        entityRevision: str = ...
+        entityRevision: str = ...,
     ) -> CreateListingChangeSetOutputTypeDef:
         """
         See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/datazone-2018-05-10/CreateListingChangeSet).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_listing_change_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#create_listing_change_set)
@@ -505,30 +504,30 @@
 
     async def create_project(
         self,
         *,
         domainIdentifier: str,
         name: str,
         description: str = ...,
-        glossaryTerms: Sequence[str] = ...
+        glossaryTerms: Sequence[str] = ...,
     ) -> CreateProjectOutputTypeDef:
         """
         Creates an Amazon DataZone project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#create_project)
         """
 
     async def create_project_membership(
         self,
         *,
         designation: UserDesignationType,
         domainIdentifier: str,
         member: MemberTypeDef,
-        projectIdentifier: str
+        projectIdentifier: str,
     ) -> Dict[str, Any]:
         """
         Creates a project membership in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_project_membership)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#create_project_membership)
         """
@@ -537,15 +536,15 @@
         self,
         *,
         domainIdentifier: str,
         environmentIdentifier: str,
         grantedEntity: GrantedEntityInputTypeDef,
         subscriptionTargetIdentifier: str,
         assetTargetNames: Sequence[AssetTargetNameMapTypeDef] = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> CreateSubscriptionGrantOutputTypeDef:
         """
         Creates a subsscription grant in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_subscription_grant)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#create_subscription_grant)
         """
@@ -553,15 +552,15 @@
     async def create_subscription_request(
         self,
         *,
         domainIdentifier: str,
         requestReason: str,
         subscribedListings: Sequence[SubscribedListingInputTypeDef],
         subscribedPrincipals: Sequence[SubscribedPrincipalInputTypeDef],
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> CreateSubscriptionRequestOutputTypeDef:
         """
         Creates a subscription request in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_subscription_request)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#create_subscription_request)
         """
@@ -574,30 +573,30 @@
         domainIdentifier: str,
         environmentIdentifier: str,
         manageAccessRole: str,
         name: str,
         subscriptionTargetConfig: Sequence[SubscriptionTargetFormTypeDef],
         type: str,
         clientToken: str = ...,
-        provider: str = ...
+        provider: str = ...,
     ) -> CreateSubscriptionTargetOutputTypeDef:
         """
         Creates a subscription target in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_subscription_target)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#create_subscription_target)
         """
 
     async def create_user_profile(
         self,
         *,
         domainIdentifier: str,
         userIdentifier: str,
         clientToken: str = ...,
-        userType: UserTypeType = ...
+        userType: UserTypeType = ...,
     ) -> CreateUserProfileOutputTypeDef:
         """
         Creates a user profile in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_user_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#create_user_profile)
         """
@@ -989,15 +988,15 @@
     async def list_data_source_run_activities(
         self,
         *,
         domainIdentifier: str,
         identifier: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        status: DataAssetActivityStatusType = ...
+        status: DataAssetActivityStatusType = ...,
     ) -> ListDataSourceRunActivitiesOutputTypeDef:
         """
         Lists data source run activities.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.list_data_source_run_activities)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#list_data_source_run_activities)
         """
@@ -1005,15 +1004,15 @@
     async def list_data_source_runs(
         self,
         *,
         dataSourceIdentifier: str,
         domainIdentifier: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        status: DataSourceRunStatusType = ...
+        status: DataSourceRunStatusType = ...,
     ) -> ListDataSourceRunsOutputTypeDef:
         """
         Lists data source runs in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.list_data_source_runs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#list_data_source_runs)
         """
@@ -1024,15 +1023,15 @@
         domainIdentifier: str,
         projectIdentifier: str,
         environmentIdentifier: str = ...,
         maxResults: int = ...,
         name: str = ...,
         nextToken: str = ...,
         status: DataSourceStatusType = ...,
-        type: str = ...
+        type: str = ...,
     ) -> ListDataSourcesOutputTypeDef:
         """
         Lists data sources in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.list_data_sources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#list_data_sources)
         """
@@ -1060,15 +1059,15 @@
     async def list_environment_blueprints(
         self,
         *,
         domainIdentifier: str,
         managed: bool = ...,
         maxResults: int = ...,
         name: str = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListEnvironmentBlueprintsOutputTypeDef:
         """
         Lists blueprints in an Amazon DataZone environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.list_environment_blueprints)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#list_environment_blueprints)
         """
@@ -1079,15 +1078,15 @@
         domainIdentifier: str,
         awsAccountId: str = ...,
         awsAccountRegion: str = ...,
         environmentBlueprintIdentifier: str = ...,
         maxResults: int = ...,
         name: str = ...,
         nextToken: str = ...,
-        projectIdentifier: str = ...
+        projectIdentifier: str = ...,
     ) -> ListEnvironmentProfilesOutputTypeDef:
         """
         Lists Amazon DataZone environment profiles.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.list_environment_profiles)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#list_environment_profiles)
         """
@@ -1101,15 +1100,15 @@
         awsAccountRegion: str = ...,
         environmentBlueprintIdentifier: str = ...,
         environmentProfileIdentifier: str = ...,
         maxResults: int = ...,
         name: str = ...,
         nextToken: str = ...,
         provider: str = ...,
-        status: EnvironmentStatusType = ...
+        status: EnvironmentStatusType = ...,
     ) -> ListEnvironmentsOutputTypeDef:
         """
         Lists Amazon DataZone environments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.list_environments)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#list_environments)
         """
@@ -1120,15 +1119,15 @@
         domainIdentifier: str,
         type: NotificationTypeType,
         afterTimestamp: TimestampTypeDef = ...,
         beforeTimestamp: TimestampTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         subjects: Sequence[str] = ...,
-        taskStatus: TaskStatusType = ...
+        taskStatus: TaskStatusType = ...,
     ) -> ListNotificationsOutputTypeDef:
         """
         Lists all Amazon DataZone notifications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.list_notifications)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#list_notifications)
         """
@@ -1137,15 +1136,15 @@
         self,
         *,
         domainIdentifier: str,
         projectIdentifier: str,
         maxResults: int = ...,
         nextToken: str = ...,
         sortBy: Literal["NAME"] = ...,
-        sortOrder: SortOrderType = ...
+        sortOrder: SortOrderType = ...,
     ) -> ListProjectMembershipsOutputTypeDef:
         """
         Lists all members of the specified project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.list_project_memberships)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#list_project_memberships)
         """
@@ -1154,15 +1153,15 @@
         self,
         *,
         domainIdentifier: str,
         groupIdentifier: str = ...,
         maxResults: int = ...,
         name: str = ...,
         nextToken: str = ...,
-        userIdentifier: str = ...
+        userIdentifier: str = ...,
     ) -> ListProjectsOutputTypeDef:
         """
         Lists Amazon DataZone projects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.list_projects)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#list_projects)
         """
@@ -1174,15 +1173,15 @@
         environmentId: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         sortBy: SortKeyType = ...,
         sortOrder: SortOrderType = ...,
         subscribedListingId: str = ...,
         subscriptionId: str = ...,
-        subscriptionTargetId: str = ...
+        subscriptionTargetId: str = ...,
     ) -> ListSubscriptionGrantsOutputTypeDef:
         """
         Lists subscription grants.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.list_subscription_grants)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#list_subscription_grants)
         """
@@ -1194,15 +1193,15 @@
         approverProjectId: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         owningProjectId: str = ...,
         sortBy: SortKeyType = ...,
         sortOrder: SortOrderType = ...,
         status: SubscriptionRequestStatusType = ...,
-        subscribedListingId: str = ...
+        subscribedListingId: str = ...,
     ) -> ListSubscriptionRequestsOutputTypeDef:
         """
         Lists Amazon DataZone subscription requests.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.list_subscription_requests)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#list_subscription_requests)
         """
@@ -1211,15 +1210,15 @@
         self,
         *,
         domainIdentifier: str,
         environmentIdentifier: str,
         maxResults: int = ...,
         nextToken: str = ...,
         sortBy: SortKeyType = ...,
-        sortOrder: SortOrderType = ...
+        sortOrder: SortOrderType = ...,
     ) -> ListSubscriptionTargetsOutputTypeDef:
         """
         Lists subscription targets in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.list_subscription_targets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#list_subscription_targets)
         """
@@ -1232,15 +1231,15 @@
         maxResults: int = ...,
         nextToken: str = ...,
         owningProjectId: str = ...,
         sortBy: SortKeyType = ...,
         sortOrder: SortOrderType = ...,
         status: SubscriptionStatusType = ...,
         subscribedListingId: str = ...,
-        subscriptionRequestIdentifier: str = ...
+        subscriptionRequestIdentifier: str = ...,
     ) -> ListSubscriptionsOutputTypeDef:
         """
         Lists subscriptions in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.list_subscriptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#list_subscriptions)
         """
@@ -1259,15 +1258,15 @@
         self,
         *,
         domainIdentifier: str,
         enabledRegions: Sequence[str],
         environmentBlueprintIdentifier: str,
         manageAccessRoleArn: str = ...,
         provisioningRoleArn: str = ...,
-        regionalParameters: Mapping[str, Mapping[str, str]] = ...
+        regionalParameters: Mapping[str, Mapping[str, str]] = ...,
     ) -> PutEnvironmentBlueprintConfigurationOutputTypeDef:
         """
         Writes the configuration for the specified environment blueprint in Amazon
         DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.put_environment_blueprint_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#put_environment_blueprint_configuration)
@@ -1277,15 +1276,15 @@
         self,
         *,
         domainIdentifier: str,
         identifier: str,
         clientToken: str = ...,
         rejectChoices: Sequence[RejectChoiceTypeDef] = ...,
         rejectRule: RejectRuleTypeDef = ...,
-        revision: str = ...
+        revision: str = ...,
     ) -> RejectPredictionsOutputTypeDef:
         """
         Rejects automatically generated business-friendly metadata for your Amazon
         DataZone
         assets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.reject_predictions)
@@ -1320,15 +1319,15 @@
         additionalAttributes: Sequence[Literal["FORMS"]] = ...,
         filters: "FilterClauseTypeDef" = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         owningProjectIdentifier: str = ...,
         searchIn: Sequence[SearchInItemTypeDef] = ...,
         searchText: str = ...,
-        sort: SearchSortTypeDef = ...
+        sort: SearchSortTypeDef = ...,
     ) -> SearchOutputTypeDef:
         """
         Searches for assets in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.search)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#search)
         """
@@ -1336,15 +1335,15 @@
     async def search_group_profiles(
         self,
         *,
         domainIdentifier: str,
         groupType: GroupSearchTypeType,
         maxResults: int = ...,
         nextToken: str = ...,
-        searchText: str = ...
+        searchText: str = ...,
     ) -> SearchGroupProfilesOutputTypeDef:
         """
         Searches group profiles in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.search_group_profiles)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#search_group_profiles)
         """
@@ -1355,15 +1354,15 @@
         domainIdentifier: str,
         additionalAttributes: Sequence[Literal["FORMS"]] = ...,
         filters: "FilterClauseTypeDef" = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         searchIn: Sequence[SearchInItemTypeDef] = ...,
         searchText: str = ...,
-        sort: SearchSortTypeDef = ...
+        sort: SearchSortTypeDef = ...,
     ) -> SearchListingsOutputTypeDef:
         """
         Searches listings in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.search_listings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#search_listings)
         """
@@ -1375,15 +1374,15 @@
         managed: bool,
         searchScope: TypesSearchScopeType,
         filters: "FilterClauseTypeDef" = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         searchIn: Sequence[SearchInItemTypeDef] = ...,
         searchText: str = ...,
-        sort: SearchSortTypeDef = ...
+        sort: SearchSortTypeDef = ...,
     ) -> SearchTypesOutputTypeDef:
         """
         Searches for types in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.search_types)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#search_types)
         """
@@ -1391,15 +1390,15 @@
     async def search_user_profiles(
         self,
         *,
         domainIdentifier: str,
         userType: UserSearchTypeType,
         maxResults: int = ...,
         nextToken: str = ...,
-        searchText: str = ...
+        searchText: str = ...,
     ) -> SearchUserProfilesOutputTypeDef:
         """
         Searches user profiles in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.search_user_profiles)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#search_user_profiles)
         """
@@ -1438,15 +1437,15 @@
         assetFormsInput: Sequence[FormInputTypeDef] = ...,
         configuration: DataSourceConfigurationInputTypeDef = ...,
         description: str = ...,
         enableSetting: EnableSettingType = ...,
         name: str = ...,
         publishOnImport: bool = ...,
         recommendation: RecommendationConfigurationTypeDef = ...,
-        schedule: ScheduleConfigurationTypeDef = ...
+        schedule: ScheduleConfigurationTypeDef = ...,
     ) -> UpdateDataSourceOutputTypeDef:
         """
         Updates the specified data source in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.update_data_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#update_data_source)
         """
@@ -1455,15 +1454,15 @@
         self,
         *,
         identifier: str,
         clientToken: str = ...,
         description: str = ...,
         domainExecutionRole: str = ...,
         name: str = ...,
-        singleSignOn: SingleSignOnTypeDef = ...
+        singleSignOn: SingleSignOnTypeDef = ...,
     ) -> UpdateDomainOutputTypeDef:
         """
         Updates a Amazon DataZone domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.update_domain)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#update_domain)
         """
@@ -1471,15 +1470,15 @@
     async def update_environment(
         self,
         *,
         domainIdentifier: str,
         identifier: str,
         description: str = ...,
         glossaryTerms: Sequence[str] = ...,
-        name: str = ...
+        name: str = ...,
     ) -> UpdateEnvironmentOutputTypeDef:
         """
         Updates the specified environment in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.update_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#update_environment)
         """
@@ -1489,15 +1488,15 @@
         *,
         domainIdentifier: str,
         identifier: str,
         awsAccountId: str = ...,
         awsAccountRegion: str = ...,
         description: str = ...,
         name: str = ...,
-        userParameters: Sequence[EnvironmentParameterTypeDef] = ...
+        userParameters: Sequence[EnvironmentParameterTypeDef] = ...,
     ) -> UpdateEnvironmentProfileOutputTypeDef:
         """
         Updates the specified environment profile in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.update_environment_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#update_environment_profile)
         """
@@ -1506,15 +1505,15 @@
         self,
         *,
         domainIdentifier: str,
         identifier: str,
         clientToken: str = ...,
         description: str = ...,
         name: str = ...,
-        status: GlossaryStatusType = ...
+        status: GlossaryStatusType = ...,
     ) -> UpdateGlossaryOutputTypeDef:
         """
         Updates the business glossary in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.update_glossary)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#update_glossary)
         """
@@ -1525,15 +1524,15 @@
         domainIdentifier: str,
         identifier: str,
         glossaryIdentifier: str = ...,
         longDescription: str = ...,
         name: str = ...,
         shortDescription: str = ...,
         status: GlossaryTermStatusType = ...,
-        termRelations: TermRelationsTypeDef = ...
+        termRelations: TermRelationsTypeDef = ...,
     ) -> UpdateGlossaryTermOutputTypeDef:
         """
         Updates a business glossary term in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.update_glossary_term)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#update_glossary_term)
         """
@@ -1551,15 +1550,15 @@
     async def update_project(
         self,
         *,
         domainIdentifier: str,
         identifier: str,
         description: str = ...,
         glossaryTerms: Sequence[str] = ...,
-        name: str = ...
+        name: str = ...,
     ) -> UpdateProjectOutputTypeDef:
         """
         Updates the specified project in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.update_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#update_project)
         """
@@ -1568,15 +1567,15 @@
         self,
         *,
         assetIdentifier: str,
         domainIdentifier: str,
         identifier: str,
         status: SubscriptionGrantStatusType,
         failureCause: FailureCauseTypeDef = ...,
-        targetName: str = ...
+        targetName: str = ...,
     ) -> UpdateSubscriptionGrantStatusOutputTypeDef:
         """
         Updates the status of the specified subscription grant status in Amazon
         DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.update_subscription_grant_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#update_subscription_grant_status)
@@ -1599,30 +1598,30 @@
         environmentIdentifier: str,
         identifier: str,
         applicableAssetTypes: Sequence[str] = ...,
         authorizedPrincipals: Sequence[str] = ...,
         manageAccessRole: str = ...,
         name: str = ...,
         provider: str = ...,
-        subscriptionTargetConfig: Sequence[SubscriptionTargetFormTypeDef] = ...
+        subscriptionTargetConfig: Sequence[SubscriptionTargetFormTypeDef] = ...,
     ) -> UpdateSubscriptionTargetOutputTypeDef:
         """
         Updates the specified subscription target in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.update_subscription_target)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#update_subscription_target)
         """
 
     async def update_user_profile(
         self,
         *,
         domainIdentifier: str,
         status: UserProfileStatusType,
         userIdentifier: str,
-        type: UserProfileTypeType = ...
+        type: UserProfileTypeType = ...,
     ) -> UpdateUserProfileOutputTypeDef:
         """
         Updates the specified user profile in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.update_user_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#update_user_profile)
         """
```

### Comparing `types-aiobotocore-datazone-2.9.0/types_aiobotocore_datazone/client.pyi` & `types-aiobotocore-datazone-2.9.1/types_aiobotocore_datazone/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -230,15 +230,15 @@
         self,
         *,
         domainIdentifier: str,
         identifier: str,
         acceptChoices: Sequence[AcceptChoiceTypeDef] = ...,
         acceptRule: AcceptRuleTypeDef = ...,
         clientToken: str = ...,
-        revision: str = ...
+        revision: str = ...,
     ) -> AcceptPredictionsOutputTypeDef:
         """
         Accepts automatically generated business-friendly metadata for your Amazon
         DataZone
         assets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.accept_predictions)
@@ -290,15 +290,15 @@
         typeIdentifier: str,
         clientToken: str = ...,
         description: str = ...,
         externalIdentifier: str = ...,
         formsInput: Sequence[FormInputTypeDef] = ...,
         glossaryTerms: Sequence[str] = ...,
         predictionConfiguration: PredictionConfigurationTypeDef = ...,
-        typeRevision: str = ...
+        typeRevision: str = ...,
     ) -> CreateAssetOutputTypeDef:
         """
         Creates an asset in Amazon DataZone catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_asset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#create_asset)
         """
@@ -310,15 +310,15 @@
         identifier: str,
         name: str,
         clientToken: str = ...,
         description: str = ...,
         formsInput: Sequence[FormInputTypeDef] = ...,
         glossaryTerms: Sequence[str] = ...,
         predictionConfiguration: PredictionConfigurationTypeDef = ...,
-        typeRevision: str = ...
+        typeRevision: str = ...,
     ) -> CreateAssetRevisionOutputTypeDef:
         """
         Creates a revision of the asset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_asset_revision)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#create_asset_revision)
         """
@@ -326,15 +326,15 @@
     async def create_asset_type(
         self,
         *,
         domainIdentifier: str,
         formsInput: Mapping[str, FormEntryInputTypeDef],
         name: str,
         owningProjectIdentifier: str,
-        description: str = ...
+        description: str = ...,
     ) -> CreateAssetTypeOutputTypeDef:
         """
         Creates a custom asset type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_asset_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#create_asset_type)
         """
@@ -350,15 +350,15 @@
         assetFormsInput: Sequence[FormInputTypeDef] = ...,
         clientToken: str = ...,
         configuration: DataSourceConfigurationInputTypeDef = ...,
         description: str = ...,
         enableSetting: EnableSettingType = ...,
         publishOnImport: bool = ...,
         recommendation: RecommendationConfigurationTypeDef = ...,
-        schedule: ScheduleConfigurationTypeDef = ...
+        schedule: ScheduleConfigurationTypeDef = ...,
     ) -> CreateDataSourceOutputTypeDef:
         """
         Creates an Amazon DataZone data source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_data_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#create_data_source)
         """
@@ -368,15 +368,15 @@
         *,
         domainExecutionRole: str,
         name: str,
         clientToken: str = ...,
         description: str = ...,
         kmsKeyIdentifier: str = ...,
         singleSignOn: SingleSignOnTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateDomainOutputTypeDef:
         """
         Creates an Amazon DataZone domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_domain)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#create_domain)
         """
@@ -386,15 +386,15 @@
         *,
         domainIdentifier: str,
         environmentProfileIdentifier: str,
         name: str,
         projectIdentifier: str,
         description: str = ...,
         glossaryTerms: Sequence[str] = ...,
-        userParameters: Sequence[EnvironmentParameterTypeDef] = ...
+        userParameters: Sequence[EnvironmentParameterTypeDef] = ...,
     ) -> CreateEnvironmentOutputTypeDef:
         """
         Create an Amazon DataZone environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#create_environment)
         """
@@ -405,15 +405,15 @@
         domainIdentifier: str,
         environmentBlueprintIdentifier: str,
         name: str,
         projectIdentifier: str,
         awsAccountId: str = ...,
         awsAccountRegion: str = ...,
         description: str = ...,
-        userParameters: Sequence[EnvironmentParameterTypeDef] = ...
+        userParameters: Sequence[EnvironmentParameterTypeDef] = ...,
     ) -> CreateEnvironmentProfileOutputTypeDef:
         """
         Creates an Amazon DataZone environment profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_environment_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#create_environment_profile)
         """
@@ -422,15 +422,15 @@
         self,
         *,
         domainIdentifier: str,
         model: ModelTypeDef,
         name: str,
         owningProjectIdentifier: str,
         description: str = ...,
-        status: FormTypeStatusType = ...
+        status: FormTypeStatusType = ...,
     ) -> CreateFormTypeOutputTypeDef:
         """
         Creates a metadata form type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_form_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#create_form_type)
         """
@@ -439,15 +439,15 @@
         self,
         *,
         domainIdentifier: str,
         name: str,
         owningProjectIdentifier: str,
         clientToken: str = ...,
         description: str = ...,
-        status: GlossaryStatusType = ...
+        status: GlossaryStatusType = ...,
     ) -> CreateGlossaryOutputTypeDef:
         """
         Creates an Amazon DataZone business glossary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_glossary)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#create_glossary)
         """
@@ -458,15 +458,15 @@
         domainIdentifier: str,
         glossaryIdentifier: str,
         name: str,
         clientToken: str = ...,
         longDescription: str = ...,
         shortDescription: str = ...,
         status: GlossaryTermStatusType = ...,
-        termRelations: TermRelationsTypeDef = ...
+        termRelations: TermRelationsTypeDef = ...,
     ) -> CreateGlossaryTermOutputTypeDef:
         """
         Creates a business glossary term.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_glossary_term)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#create_glossary_term)
         """
@@ -485,15 +485,15 @@
         self,
         *,
         action: ChangeActionType,
         domainIdentifier: str,
         entityIdentifier: str,
         entityType: Literal["ASSET"],
         clientToken: str = ...,
-        entityRevision: str = ...
+        entityRevision: str = ...,
     ) -> CreateListingChangeSetOutputTypeDef:
         """
         See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/datazone-2018-05-10/CreateListingChangeSet).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_listing_change_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#create_listing_change_set)
@@ -501,30 +501,30 @@
 
     async def create_project(
         self,
         *,
         domainIdentifier: str,
         name: str,
         description: str = ...,
-        glossaryTerms: Sequence[str] = ...
+        glossaryTerms: Sequence[str] = ...,
     ) -> CreateProjectOutputTypeDef:
         """
         Creates an Amazon DataZone project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#create_project)
         """
 
     async def create_project_membership(
         self,
         *,
         designation: UserDesignationType,
         domainIdentifier: str,
         member: MemberTypeDef,
-        projectIdentifier: str
+        projectIdentifier: str,
     ) -> Dict[str, Any]:
         """
         Creates a project membership in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_project_membership)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#create_project_membership)
         """
@@ -533,15 +533,15 @@
         self,
         *,
         domainIdentifier: str,
         environmentIdentifier: str,
         grantedEntity: GrantedEntityInputTypeDef,
         subscriptionTargetIdentifier: str,
         assetTargetNames: Sequence[AssetTargetNameMapTypeDef] = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> CreateSubscriptionGrantOutputTypeDef:
         """
         Creates a subsscription grant in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_subscription_grant)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#create_subscription_grant)
         """
@@ -549,15 +549,15 @@
     async def create_subscription_request(
         self,
         *,
         domainIdentifier: str,
         requestReason: str,
         subscribedListings: Sequence[SubscribedListingInputTypeDef],
         subscribedPrincipals: Sequence[SubscribedPrincipalInputTypeDef],
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> CreateSubscriptionRequestOutputTypeDef:
         """
         Creates a subscription request in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_subscription_request)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#create_subscription_request)
         """
@@ -570,30 +570,30 @@
         domainIdentifier: str,
         environmentIdentifier: str,
         manageAccessRole: str,
         name: str,
         subscriptionTargetConfig: Sequence[SubscriptionTargetFormTypeDef],
         type: str,
         clientToken: str = ...,
-        provider: str = ...
+        provider: str = ...,
     ) -> CreateSubscriptionTargetOutputTypeDef:
         """
         Creates a subscription target in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_subscription_target)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#create_subscription_target)
         """
 
     async def create_user_profile(
         self,
         *,
         domainIdentifier: str,
         userIdentifier: str,
         clientToken: str = ...,
-        userType: UserTypeType = ...
+        userType: UserTypeType = ...,
     ) -> CreateUserProfileOutputTypeDef:
         """
         Creates a user profile in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_user_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#create_user_profile)
         """
@@ -985,15 +985,15 @@
     async def list_data_source_run_activities(
         self,
         *,
         domainIdentifier: str,
         identifier: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        status: DataAssetActivityStatusType = ...
+        status: DataAssetActivityStatusType = ...,
     ) -> ListDataSourceRunActivitiesOutputTypeDef:
         """
         Lists data source run activities.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.list_data_source_run_activities)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#list_data_source_run_activities)
         """
@@ -1001,15 +1001,15 @@
     async def list_data_source_runs(
         self,
         *,
         dataSourceIdentifier: str,
         domainIdentifier: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        status: DataSourceRunStatusType = ...
+        status: DataSourceRunStatusType = ...,
     ) -> ListDataSourceRunsOutputTypeDef:
         """
         Lists data source runs in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.list_data_source_runs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#list_data_source_runs)
         """
@@ -1020,15 +1020,15 @@
         domainIdentifier: str,
         projectIdentifier: str,
         environmentIdentifier: str = ...,
         maxResults: int = ...,
         name: str = ...,
         nextToken: str = ...,
         status: DataSourceStatusType = ...,
-        type: str = ...
+        type: str = ...,
     ) -> ListDataSourcesOutputTypeDef:
         """
         Lists data sources in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.list_data_sources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#list_data_sources)
         """
@@ -1056,15 +1056,15 @@
     async def list_environment_blueprints(
         self,
         *,
         domainIdentifier: str,
         managed: bool = ...,
         maxResults: int = ...,
         name: str = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListEnvironmentBlueprintsOutputTypeDef:
         """
         Lists blueprints in an Amazon DataZone environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.list_environment_blueprints)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#list_environment_blueprints)
         """
@@ -1075,15 +1075,15 @@
         domainIdentifier: str,
         awsAccountId: str = ...,
         awsAccountRegion: str = ...,
         environmentBlueprintIdentifier: str = ...,
         maxResults: int = ...,
         name: str = ...,
         nextToken: str = ...,
-        projectIdentifier: str = ...
+        projectIdentifier: str = ...,
     ) -> ListEnvironmentProfilesOutputTypeDef:
         """
         Lists Amazon DataZone environment profiles.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.list_environment_profiles)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#list_environment_profiles)
         """
@@ -1097,15 +1097,15 @@
         awsAccountRegion: str = ...,
         environmentBlueprintIdentifier: str = ...,
         environmentProfileIdentifier: str = ...,
         maxResults: int = ...,
         name: str = ...,
         nextToken: str = ...,
         provider: str = ...,
-        status: EnvironmentStatusType = ...
+        status: EnvironmentStatusType = ...,
     ) -> ListEnvironmentsOutputTypeDef:
         """
         Lists Amazon DataZone environments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.list_environments)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#list_environments)
         """
@@ -1116,15 +1116,15 @@
         domainIdentifier: str,
         type: NotificationTypeType,
         afterTimestamp: TimestampTypeDef = ...,
         beforeTimestamp: TimestampTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         subjects: Sequence[str] = ...,
-        taskStatus: TaskStatusType = ...
+        taskStatus: TaskStatusType = ...,
     ) -> ListNotificationsOutputTypeDef:
         """
         Lists all Amazon DataZone notifications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.list_notifications)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#list_notifications)
         """
@@ -1133,15 +1133,15 @@
         self,
         *,
         domainIdentifier: str,
         projectIdentifier: str,
         maxResults: int = ...,
         nextToken: str = ...,
         sortBy: Literal["NAME"] = ...,
-        sortOrder: SortOrderType = ...
+        sortOrder: SortOrderType = ...,
     ) -> ListProjectMembershipsOutputTypeDef:
         """
         Lists all members of the specified project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.list_project_memberships)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#list_project_memberships)
         """
@@ -1150,15 +1150,15 @@
         self,
         *,
         domainIdentifier: str,
         groupIdentifier: str = ...,
         maxResults: int = ...,
         name: str = ...,
         nextToken: str = ...,
-        userIdentifier: str = ...
+        userIdentifier: str = ...,
     ) -> ListProjectsOutputTypeDef:
         """
         Lists Amazon DataZone projects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.list_projects)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#list_projects)
         """
@@ -1170,15 +1170,15 @@
         environmentId: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         sortBy: SortKeyType = ...,
         sortOrder: SortOrderType = ...,
         subscribedListingId: str = ...,
         subscriptionId: str = ...,
-        subscriptionTargetId: str = ...
+        subscriptionTargetId: str = ...,
     ) -> ListSubscriptionGrantsOutputTypeDef:
         """
         Lists subscription grants.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.list_subscription_grants)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#list_subscription_grants)
         """
@@ -1190,15 +1190,15 @@
         approverProjectId: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         owningProjectId: str = ...,
         sortBy: SortKeyType = ...,
         sortOrder: SortOrderType = ...,
         status: SubscriptionRequestStatusType = ...,
-        subscribedListingId: str = ...
+        subscribedListingId: str = ...,
     ) -> ListSubscriptionRequestsOutputTypeDef:
         """
         Lists Amazon DataZone subscription requests.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.list_subscription_requests)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#list_subscription_requests)
         """
@@ -1207,15 +1207,15 @@
         self,
         *,
         domainIdentifier: str,
         environmentIdentifier: str,
         maxResults: int = ...,
         nextToken: str = ...,
         sortBy: SortKeyType = ...,
-        sortOrder: SortOrderType = ...
+        sortOrder: SortOrderType = ...,
     ) -> ListSubscriptionTargetsOutputTypeDef:
         """
         Lists subscription targets in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.list_subscription_targets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#list_subscription_targets)
         """
@@ -1228,15 +1228,15 @@
         maxResults: int = ...,
         nextToken: str = ...,
         owningProjectId: str = ...,
         sortBy: SortKeyType = ...,
         sortOrder: SortOrderType = ...,
         status: SubscriptionStatusType = ...,
         subscribedListingId: str = ...,
-        subscriptionRequestIdentifier: str = ...
+        subscriptionRequestIdentifier: str = ...,
     ) -> ListSubscriptionsOutputTypeDef:
         """
         Lists subscriptions in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.list_subscriptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#list_subscriptions)
         """
@@ -1255,15 +1255,15 @@
         self,
         *,
         domainIdentifier: str,
         enabledRegions: Sequence[str],
         environmentBlueprintIdentifier: str,
         manageAccessRoleArn: str = ...,
         provisioningRoleArn: str = ...,
-        regionalParameters: Mapping[str, Mapping[str, str]] = ...
+        regionalParameters: Mapping[str, Mapping[str, str]] = ...,
     ) -> PutEnvironmentBlueprintConfigurationOutputTypeDef:
         """
         Writes the configuration for the specified environment blueprint in Amazon
         DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.put_environment_blueprint_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#put_environment_blueprint_configuration)
@@ -1273,15 +1273,15 @@
         self,
         *,
         domainIdentifier: str,
         identifier: str,
         clientToken: str = ...,
         rejectChoices: Sequence[RejectChoiceTypeDef] = ...,
         rejectRule: RejectRuleTypeDef = ...,
-        revision: str = ...
+        revision: str = ...,
     ) -> RejectPredictionsOutputTypeDef:
         """
         Rejects automatically generated business-friendly metadata for your Amazon
         DataZone
         assets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.reject_predictions)
@@ -1316,15 +1316,15 @@
         additionalAttributes: Sequence[Literal["FORMS"]] = ...,
         filters: "FilterClauseTypeDef" = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         owningProjectIdentifier: str = ...,
         searchIn: Sequence[SearchInItemTypeDef] = ...,
         searchText: str = ...,
-        sort: SearchSortTypeDef = ...
+        sort: SearchSortTypeDef = ...,
     ) -> SearchOutputTypeDef:
         """
         Searches for assets in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.search)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#search)
         """
@@ -1332,15 +1332,15 @@
     async def search_group_profiles(
         self,
         *,
         domainIdentifier: str,
         groupType: GroupSearchTypeType,
         maxResults: int = ...,
         nextToken: str = ...,
-        searchText: str = ...
+        searchText: str = ...,
     ) -> SearchGroupProfilesOutputTypeDef:
         """
         Searches group profiles in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.search_group_profiles)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#search_group_profiles)
         """
@@ -1351,15 +1351,15 @@
         domainIdentifier: str,
         additionalAttributes: Sequence[Literal["FORMS"]] = ...,
         filters: "FilterClauseTypeDef" = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         searchIn: Sequence[SearchInItemTypeDef] = ...,
         searchText: str = ...,
-        sort: SearchSortTypeDef = ...
+        sort: SearchSortTypeDef = ...,
     ) -> SearchListingsOutputTypeDef:
         """
         Searches listings in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.search_listings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#search_listings)
         """
@@ -1371,15 +1371,15 @@
         managed: bool,
         searchScope: TypesSearchScopeType,
         filters: "FilterClauseTypeDef" = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         searchIn: Sequence[SearchInItemTypeDef] = ...,
         searchText: str = ...,
-        sort: SearchSortTypeDef = ...
+        sort: SearchSortTypeDef = ...,
     ) -> SearchTypesOutputTypeDef:
         """
         Searches for types in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.search_types)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#search_types)
         """
@@ -1387,15 +1387,15 @@
     async def search_user_profiles(
         self,
         *,
         domainIdentifier: str,
         userType: UserSearchTypeType,
         maxResults: int = ...,
         nextToken: str = ...,
-        searchText: str = ...
+        searchText: str = ...,
     ) -> SearchUserProfilesOutputTypeDef:
         """
         Searches user profiles in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.search_user_profiles)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#search_user_profiles)
         """
@@ -1434,15 +1434,15 @@
         assetFormsInput: Sequence[FormInputTypeDef] = ...,
         configuration: DataSourceConfigurationInputTypeDef = ...,
         description: str = ...,
         enableSetting: EnableSettingType = ...,
         name: str = ...,
         publishOnImport: bool = ...,
         recommendation: RecommendationConfigurationTypeDef = ...,
-        schedule: ScheduleConfigurationTypeDef = ...
+        schedule: ScheduleConfigurationTypeDef = ...,
     ) -> UpdateDataSourceOutputTypeDef:
         """
         Updates the specified data source in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.update_data_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#update_data_source)
         """
@@ -1451,15 +1451,15 @@
         self,
         *,
         identifier: str,
         clientToken: str = ...,
         description: str = ...,
         domainExecutionRole: str = ...,
         name: str = ...,
-        singleSignOn: SingleSignOnTypeDef = ...
+        singleSignOn: SingleSignOnTypeDef = ...,
     ) -> UpdateDomainOutputTypeDef:
         """
         Updates a Amazon DataZone domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.update_domain)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#update_domain)
         """
@@ -1467,15 +1467,15 @@
     async def update_environment(
         self,
         *,
         domainIdentifier: str,
         identifier: str,
         description: str = ...,
         glossaryTerms: Sequence[str] = ...,
-        name: str = ...
+        name: str = ...,
     ) -> UpdateEnvironmentOutputTypeDef:
         """
         Updates the specified environment in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.update_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#update_environment)
         """
@@ -1485,15 +1485,15 @@
         *,
         domainIdentifier: str,
         identifier: str,
         awsAccountId: str = ...,
         awsAccountRegion: str = ...,
         description: str = ...,
         name: str = ...,
-        userParameters: Sequence[EnvironmentParameterTypeDef] = ...
+        userParameters: Sequence[EnvironmentParameterTypeDef] = ...,
     ) -> UpdateEnvironmentProfileOutputTypeDef:
         """
         Updates the specified environment profile in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.update_environment_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#update_environment_profile)
         """
@@ -1502,15 +1502,15 @@
         self,
         *,
         domainIdentifier: str,
         identifier: str,
         clientToken: str = ...,
         description: str = ...,
         name: str = ...,
-        status: GlossaryStatusType = ...
+        status: GlossaryStatusType = ...,
     ) -> UpdateGlossaryOutputTypeDef:
         """
         Updates the business glossary in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.update_glossary)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#update_glossary)
         """
@@ -1521,15 +1521,15 @@
         domainIdentifier: str,
         identifier: str,
         glossaryIdentifier: str = ...,
         longDescription: str = ...,
         name: str = ...,
         shortDescription: str = ...,
         status: GlossaryTermStatusType = ...,
-        termRelations: TermRelationsTypeDef = ...
+        termRelations: TermRelationsTypeDef = ...,
     ) -> UpdateGlossaryTermOutputTypeDef:
         """
         Updates a business glossary term in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.update_glossary_term)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#update_glossary_term)
         """
@@ -1547,15 +1547,15 @@
     async def update_project(
         self,
         *,
         domainIdentifier: str,
         identifier: str,
         description: str = ...,
         glossaryTerms: Sequence[str] = ...,
-        name: str = ...
+        name: str = ...,
     ) -> UpdateProjectOutputTypeDef:
         """
         Updates the specified project in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.update_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#update_project)
         """
@@ -1564,15 +1564,15 @@
         self,
         *,
         assetIdentifier: str,
         domainIdentifier: str,
         identifier: str,
         status: SubscriptionGrantStatusType,
         failureCause: FailureCauseTypeDef = ...,
-        targetName: str = ...
+        targetName: str = ...,
     ) -> UpdateSubscriptionGrantStatusOutputTypeDef:
         """
         Updates the status of the specified subscription grant status in Amazon
         DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.update_subscription_grant_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#update_subscription_grant_status)
@@ -1595,30 +1595,30 @@
         environmentIdentifier: str,
         identifier: str,
         applicableAssetTypes: Sequence[str] = ...,
         authorizedPrincipals: Sequence[str] = ...,
         manageAccessRole: str = ...,
         name: str = ...,
         provider: str = ...,
-        subscriptionTargetConfig: Sequence[SubscriptionTargetFormTypeDef] = ...
+        subscriptionTargetConfig: Sequence[SubscriptionTargetFormTypeDef] = ...,
     ) -> UpdateSubscriptionTargetOutputTypeDef:
         """
         Updates the specified subscription target in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.update_subscription_target)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#update_subscription_target)
         """
 
     async def update_user_profile(
         self,
         *,
         domainIdentifier: str,
         status: UserProfileStatusType,
         userIdentifier: str,
-        type: UserProfileTypeType = ...
+        type: UserProfileTypeType = ...,
     ) -> UpdateUserProfileOutputTypeDef:
         """
         Updates the specified user profile in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.update_user_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/client/#update_user_profile)
         """
```

### Comparing `types-aiobotocore-datazone-2.9.0/types_aiobotocore_datazone/literals.py` & `types-aiobotocore-datazone-2.9.1/types_aiobotocore_datazone/literals.py`

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
     "AcceptRuleBehaviorType",
     "AuthTypeType",
     "ChangeActionType",
     "ConfigurableActionTypeAuthorizationType",
     "DataAssetActivityStatusType",
     "DataSourceErrorTypeType",
@@ -89,15 +88,14 @@
     "DataZoneServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AcceptRuleBehaviorType = Literal["ALL", "NONE"]
 AuthTypeType = Literal["DISABLED", "IAM_IDC"]
 ChangeActionType = Literal["PUBLISH", "UNPUBLISH"]
 ConfigurableActionTypeAuthorizationType = Literal["HTTPS", "IAM"]
 DataAssetActivityStatusType = Literal[
     "FAILED",
     "PUBLISHING_FAILED",
```

### Comparing `types-aiobotocore-datazone-2.9.0/types_aiobotocore_datazone/literals.pyi` & `types-aiobotocore-datazone-2.9.1/types_aiobotocore_datazone/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-datazone-2.9.0/types_aiobotocore_datazone/paginator.py` & `types-aiobotocore-datazone-2.9.1/types_aiobotocore_datazone/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ListAssetRevisionsPaginator",
     "ListDataSourceRunActivitiesPaginator",
     "ListDataSourceRunsPaginator",
     "ListDataSourcesPaginator",
     "ListDomainsPaginator",
     "ListEnvironmentBlueprintConfigurationsPaginator",
@@ -139,15 +138,14 @@
     "SearchPaginator",
     "SearchGroupProfilesPaginator",
     "SearchListingsPaginator",
     "SearchTypesPaginator",
     "SearchUserProfilesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -161,15 +159,15 @@
     """
 
     def paginate(
         self,
         *,
         domainIdentifier: str,
         identifier: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAssetRevisionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListAssetRevisions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/paginators/#listassetrevisionspaginator)
         """
 
 
@@ -181,15 +179,15 @@
 
     def paginate(
         self,
         *,
         domainIdentifier: str,
         identifier: str,
         status: DataAssetActivityStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDataSourceRunActivitiesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListDataSourceRunActivities.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/paginators/#listdatasourcerunactivitiespaginator)
         """
 
 
@@ -201,15 +199,15 @@
 
     def paginate(
         self,
         *,
         dataSourceIdentifier: str,
         domainIdentifier: str,
         status: DataSourceRunStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDataSourceRunsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListDataSourceRuns.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/paginators/#listdatasourcerunspaginator)
         """
 
 
@@ -224,15 +222,15 @@
         *,
         domainIdentifier: str,
         projectIdentifier: str,
         environmentIdentifier: str = ...,
         name: str = ...,
         status: DataSourceStatusType = ...,
         type: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDataSourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListDataSources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/paginators/#listdatasourcespaginator)
         """
 
 
@@ -274,15 +272,15 @@
 
     def paginate(
         self,
         *,
         domainIdentifier: str,
         managed: bool = ...,
         name: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEnvironmentBlueprintsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListEnvironmentBlueprints.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/paginators/#listenvironmentblueprintspaginator)
         """
 
 
@@ -297,15 +295,15 @@
         *,
         domainIdentifier: str,
         awsAccountId: str = ...,
         awsAccountRegion: str = ...,
         environmentBlueprintIdentifier: str = ...,
         name: str = ...,
         projectIdentifier: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEnvironmentProfilesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListEnvironmentProfiles.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/paginators/#listenvironmentprofilespaginator)
         """
 
 
@@ -323,15 +321,15 @@
         awsAccountId: str = ...,
         awsAccountRegion: str = ...,
         environmentBlueprintIdentifier: str = ...,
         environmentProfileIdentifier: str = ...,
         name: str = ...,
         provider: str = ...,
         status: EnvironmentStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEnvironmentsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListEnvironments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/paginators/#listenvironmentspaginator)
         """
 
 
@@ -346,15 +344,15 @@
         *,
         domainIdentifier: str,
         type: NotificationTypeType,
         afterTimestamp: TimestampTypeDef = ...,
         beforeTimestamp: TimestampTypeDef = ...,
         subjects: Sequence[str] = ...,
         taskStatus: TaskStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListNotificationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListNotifications.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/paginators/#listnotificationspaginator)
         """
 
 
@@ -367,15 +365,15 @@
     def paginate(
         self,
         *,
         domainIdentifier: str,
         projectIdentifier: str,
         sortBy: Literal["NAME"] = ...,
         sortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListProjectMembershipsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListProjectMemberships.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/paginators/#listprojectmembershipspaginator)
         """
 
 
@@ -388,15 +386,15 @@
     def paginate(
         self,
         *,
         domainIdentifier: str,
         groupIdentifier: str = ...,
         name: str = ...,
         userIdentifier: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListProjectsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListProjects.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/paginators/#listprojectspaginator)
         """
 
 
@@ -412,15 +410,15 @@
         domainIdentifier: str,
         environmentId: str = ...,
         sortBy: SortKeyType = ...,
         sortOrder: SortOrderType = ...,
         subscribedListingId: str = ...,
         subscriptionId: str = ...,
         subscriptionTargetId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSubscriptionGrantsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListSubscriptionGrants.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/paginators/#listsubscriptiongrantspaginator)
         """
 
 
@@ -436,15 +434,15 @@
         domainIdentifier: str,
         approverProjectId: str = ...,
         owningProjectId: str = ...,
         sortBy: SortKeyType = ...,
         sortOrder: SortOrderType = ...,
         status: SubscriptionRequestStatusType = ...,
         subscribedListingId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSubscriptionRequestsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListSubscriptionRequests.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/paginators/#listsubscriptionrequestspaginator)
         """
 
 
@@ -457,15 +455,15 @@
     def paginate(
         self,
         *,
         domainIdentifier: str,
         environmentIdentifier: str,
         sortBy: SortKeyType = ...,
         sortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSubscriptionTargetsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListSubscriptionTargets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/paginators/#listsubscriptiontargetspaginator)
         """
 
 
@@ -482,15 +480,15 @@
         approverProjectId: str = ...,
         owningProjectId: str = ...,
         sortBy: SortKeyType = ...,
         sortOrder: SortOrderType = ...,
         status: SubscriptionStatusType = ...,
         subscribedListingId: str = ...,
         subscriptionRequestIdentifier: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSubscriptionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListSubscriptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/paginators/#listsubscriptionspaginator)
         """
 
 
@@ -507,15 +505,15 @@
         searchScope: InventorySearchScopeType,
         additionalAttributes: Sequence[Literal["FORMS"]] = ...,
         filters: FilterClauseTypeDef = ...,
         owningProjectIdentifier: str = ...,
         searchIn: Sequence[SearchInItemTypeDef] = ...,
         searchText: str = ...,
         sort: SearchSortTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchOutputPaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.Search.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/paginators/#searchpaginator)
         """
 
 
@@ -527,15 +525,15 @@
 
     def paginate(
         self,
         *,
         domainIdentifier: str,
         groupType: GroupSearchTypeType,
         searchText: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchGroupProfilesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.SearchGroupProfiles.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/paginators/#searchgroupprofilespaginator)
         """
 
 
@@ -550,15 +548,15 @@
         *,
         domainIdentifier: str,
         additionalAttributes: Sequence[Literal["FORMS"]] = ...,
         filters: FilterClauseTypeDef = ...,
         searchIn: Sequence[SearchInItemTypeDef] = ...,
         searchText: str = ...,
         sort: SearchSortTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchListingsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.SearchListings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/paginators/#searchlistingspaginator)
         """
 
 
@@ -574,15 +572,15 @@
         domainIdentifier: str,
         managed: bool,
         searchScope: TypesSearchScopeType,
         filters: FilterClauseTypeDef = ...,
         searchIn: Sequence[SearchInItemTypeDef] = ...,
         searchText: str = ...,
         sort: SearchSortTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchTypesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.SearchTypes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/paginators/#searchtypespaginator)
         """
 
 
@@ -594,13 +592,13 @@
 
     def paginate(
         self,
         *,
         domainIdentifier: str,
         userType: UserSearchTypeType,
         searchText: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchUserProfilesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.SearchUserProfiles.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/paginators/#searchuserprofilespaginator)
         """
```

### Comparing `types-aiobotocore-datazone-2.9.0/types_aiobotocore_datazone/paginator.pyi` & `types-aiobotocore-datazone-2.9.1/types_aiobotocore_datazone/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -157,15 +157,15 @@
     """
 
     def paginate(
         self,
         *,
         domainIdentifier: str,
         identifier: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAssetRevisionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListAssetRevisions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/paginators/#listassetrevisionspaginator)
         """
 
 class ListDataSourceRunActivitiesPaginator(AioPaginator):
@@ -176,15 +176,15 @@
 
     def paginate(
         self,
         *,
         domainIdentifier: str,
         identifier: str,
         status: DataAssetActivityStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDataSourceRunActivitiesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListDataSourceRunActivities.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/paginators/#listdatasourcerunactivitiespaginator)
         """
 
 class ListDataSourceRunsPaginator(AioPaginator):
@@ -195,15 +195,15 @@
 
     def paginate(
         self,
         *,
         dataSourceIdentifier: str,
         domainIdentifier: str,
         status: DataSourceRunStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDataSourceRunsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListDataSourceRuns.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/paginators/#listdatasourcerunspaginator)
         """
 
 class ListDataSourcesPaginator(AioPaginator):
@@ -217,15 +217,15 @@
         *,
         domainIdentifier: str,
         projectIdentifier: str,
         environmentIdentifier: str = ...,
         name: str = ...,
         status: DataSourceStatusType = ...,
         type: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDataSourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListDataSources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/paginators/#listdatasourcespaginator)
         """
 
 class ListDomainsPaginator(AioPaginator):
@@ -264,15 +264,15 @@
 
     def paginate(
         self,
         *,
         domainIdentifier: str,
         managed: bool = ...,
         name: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEnvironmentBlueprintsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListEnvironmentBlueprints.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/paginators/#listenvironmentblueprintspaginator)
         """
 
 class ListEnvironmentProfilesPaginator(AioPaginator):
@@ -286,15 +286,15 @@
         *,
         domainIdentifier: str,
         awsAccountId: str = ...,
         awsAccountRegion: str = ...,
         environmentBlueprintIdentifier: str = ...,
         name: str = ...,
         projectIdentifier: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEnvironmentProfilesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListEnvironmentProfiles.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/paginators/#listenvironmentprofilespaginator)
         """
 
 class ListEnvironmentsPaginator(AioPaginator):
@@ -311,15 +311,15 @@
         awsAccountId: str = ...,
         awsAccountRegion: str = ...,
         environmentBlueprintIdentifier: str = ...,
         environmentProfileIdentifier: str = ...,
         name: str = ...,
         provider: str = ...,
         status: EnvironmentStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEnvironmentsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListEnvironments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/paginators/#listenvironmentspaginator)
         """
 
 class ListNotificationsPaginator(AioPaginator):
@@ -333,15 +333,15 @@
         *,
         domainIdentifier: str,
         type: NotificationTypeType,
         afterTimestamp: TimestampTypeDef = ...,
         beforeTimestamp: TimestampTypeDef = ...,
         subjects: Sequence[str] = ...,
         taskStatus: TaskStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListNotificationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListNotifications.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/paginators/#listnotificationspaginator)
         """
 
 class ListProjectMembershipsPaginator(AioPaginator):
@@ -353,15 +353,15 @@
     def paginate(
         self,
         *,
         domainIdentifier: str,
         projectIdentifier: str,
         sortBy: Literal["NAME"] = ...,
         sortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListProjectMembershipsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListProjectMemberships.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/paginators/#listprojectmembershipspaginator)
         """
 
 class ListProjectsPaginator(AioPaginator):
@@ -373,15 +373,15 @@
     def paginate(
         self,
         *,
         domainIdentifier: str,
         groupIdentifier: str = ...,
         name: str = ...,
         userIdentifier: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListProjectsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListProjects.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/paginators/#listprojectspaginator)
         """
 
 class ListSubscriptionGrantsPaginator(AioPaginator):
@@ -396,15 +396,15 @@
         domainIdentifier: str,
         environmentId: str = ...,
         sortBy: SortKeyType = ...,
         sortOrder: SortOrderType = ...,
         subscribedListingId: str = ...,
         subscriptionId: str = ...,
         subscriptionTargetId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSubscriptionGrantsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListSubscriptionGrants.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/paginators/#listsubscriptiongrantspaginator)
         """
 
 class ListSubscriptionRequestsPaginator(AioPaginator):
@@ -419,15 +419,15 @@
         domainIdentifier: str,
         approverProjectId: str = ...,
         owningProjectId: str = ...,
         sortBy: SortKeyType = ...,
         sortOrder: SortOrderType = ...,
         status: SubscriptionRequestStatusType = ...,
         subscribedListingId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSubscriptionRequestsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListSubscriptionRequests.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/paginators/#listsubscriptionrequestspaginator)
         """
 
 class ListSubscriptionTargetsPaginator(AioPaginator):
@@ -439,15 +439,15 @@
     def paginate(
         self,
         *,
         domainIdentifier: str,
         environmentIdentifier: str,
         sortBy: SortKeyType = ...,
         sortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSubscriptionTargetsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListSubscriptionTargets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/paginators/#listsubscriptiontargetspaginator)
         """
 
 class ListSubscriptionsPaginator(AioPaginator):
@@ -463,15 +463,15 @@
         approverProjectId: str = ...,
         owningProjectId: str = ...,
         sortBy: SortKeyType = ...,
         sortOrder: SortOrderType = ...,
         status: SubscriptionStatusType = ...,
         subscribedListingId: str = ...,
         subscriptionRequestIdentifier: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSubscriptionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListSubscriptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/paginators/#listsubscriptionspaginator)
         """
 
 class SearchPaginator(AioPaginator):
@@ -487,15 +487,15 @@
         searchScope: InventorySearchScopeType,
         additionalAttributes: Sequence[Literal["FORMS"]] = ...,
         filters: FilterClauseTypeDef = ...,
         owningProjectIdentifier: str = ...,
         searchIn: Sequence[SearchInItemTypeDef] = ...,
         searchText: str = ...,
         sort: SearchSortTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchOutputPaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.Search.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/paginators/#searchpaginator)
         """
 
 class SearchGroupProfilesPaginator(AioPaginator):
@@ -506,15 +506,15 @@
 
     def paginate(
         self,
         *,
         domainIdentifier: str,
         groupType: GroupSearchTypeType,
         searchText: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchGroupProfilesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.SearchGroupProfiles.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/paginators/#searchgroupprofilespaginator)
         """
 
 class SearchListingsPaginator(AioPaginator):
@@ -528,15 +528,15 @@
         *,
         domainIdentifier: str,
         additionalAttributes: Sequence[Literal["FORMS"]] = ...,
         filters: FilterClauseTypeDef = ...,
         searchIn: Sequence[SearchInItemTypeDef] = ...,
         searchText: str = ...,
         sort: SearchSortTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchListingsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.SearchListings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/paginators/#searchlistingspaginator)
         """
 
 class SearchTypesPaginator(AioPaginator):
@@ -551,15 +551,15 @@
         domainIdentifier: str,
         managed: bool,
         searchScope: TypesSearchScopeType,
         filters: FilterClauseTypeDef = ...,
         searchIn: Sequence[SearchInItemTypeDef] = ...,
         searchText: str = ...,
         sort: SearchSortTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchTypesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.SearchTypes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/paginators/#searchtypespaginator)
         """
 
 class SearchUserProfilesPaginator(AioPaginator):
@@ -570,13 +570,13 @@
 
     def paginate(
         self,
         *,
         domainIdentifier: str,
         userType: UserSearchTypeType,
         searchText: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchUserProfilesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.SearchUserProfiles.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/paginators/#searchuserprofilespaginator)
         """
```

### Comparing `types-aiobotocore-datazone-2.9.0/types_aiobotocore_datazone/type_defs.py` & `types-aiobotocore-datazone-2.9.1/types_aiobotocore_datazone/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AcceptChoiceTypeDef",
     "AcceptRuleTypeDef",
     "ResponseMetadataTypeDef",
     "AcceptSubscriptionRequestInputRequestTypeDef",
     "FormOutputTypeDef",
     "AssetListingDetailsTypeDef",
```

### Comparing `types-aiobotocore-datazone-2.9.0/types_aiobotocore_datazone/type_defs.pyi` & `types-aiobotocore-datazone-2.9.1/types_aiobotocore_datazone/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-datazone-2.9.0/types_aiobotocore_datazone.egg-info/PKG-INFO` & `types-aiobotocore-datazone-2.9.1/types_aiobotocore_datazone.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-datazone
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.DataZone 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.DataZone 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/
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
 
 <a id="types-aiobotocore-datazone"></a>
 
 # types-aiobotocore-datazone
 
 [![PyPI - types-aiobotocore-datazone](https://img.shields.io/pypi/v/types-aiobotocore-datazone.svg?color=blue)](https://pypi.org/project/types-aiobotocore-datazone)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-datazone.svg?color=blue)](https://pypi.org/project/types-aiobotocore-datazone)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-datazone)](https://pepy.tech/project/types-aiobotocore-datazone)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DataZone 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone)
+[aiobotocore.DataZone 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone)
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
 [types-aiobotocore-datazone docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datazone/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-datazone-2.9.0/types_aiobotocore_datazone.egg-info/SOURCES.txt` & `types-aiobotocore-datazone-2.9.1/types_aiobotocore_datazone.egg-info/SOURCES.txt`

 * *Files identical despite different names*

