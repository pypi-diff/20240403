# Comparing `tmp/types-aiobotocore-cur-2.9.0.tar.gz` & `tmp/types-aiobotocore-cur-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cur-2.9.0.tar", last modified: Wed Dec 13 19:59:02 2023, max compression
+gzip compressed data, was "types-aiobotocore-cur-2.9.1.tar", last modified: Thu Jan 18 01:20:28 2024, max compression
```

## Comparing `types-aiobotocore-cur-2.9.0.tar` & `types-aiobotocore-cur-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:02.345869 types-aiobotocore-cur-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:43:38.000000 types-aiobotocore-cur-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13040 2023-12-13 19:59:02.345869 types-aiobotocore-cur-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11471 2023-12-13 19:43:38.000000 types-aiobotocore-cur-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:02.345869 types-aiobotocore-cur-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2023-12-13 19:43:38.000000 types-aiobotocore-cur-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:02.345869 types-aiobotocore-cur-2.9.0/types_aiobotocore_cur/
--rw-r--r--   0 runner    (1001) docker     (127)      794 2023-12-13 19:43:38.000000 types-aiobotocore-cur-2.9.0/types_aiobotocore_cur/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2023-12-13 19:43:38.000000 types-aiobotocore-cur-2.9.0/types_aiobotocore_cur/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      949 2023-12-13 19:43:38.000000 types-aiobotocore-cur-2.9.0/types_aiobotocore_cur/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8857 2023-12-13 19:43:38.000000 types-aiobotocore-cur-2.9.0/types_aiobotocore_cur/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8853 2023-12-13 19:43:38.000000 types-aiobotocore-cur-2.9.0/types_aiobotocore_cur/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9601 2023-12-13 19:43:38.000000 types-aiobotocore-cur-2.9.0/types_aiobotocore_cur/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9599 2023-12-13 19:43:38.000000 types-aiobotocore-cur-2.9.0/types_aiobotocore_cur/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2023-12-13 19:43:38.000000 types-aiobotocore-cur-2.9.0/types_aiobotocore_cur/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2023-12-13 19:43:38.000000 types-aiobotocore-cur-2.9.0/types_aiobotocore_cur/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:43:38.000000 types-aiobotocore-cur-2.9.0/types_aiobotocore_cur/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5058 2023-12-13 19:43:38.000000 types-aiobotocore-cur-2.9.0/types_aiobotocore_cur/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5057 2023-12-13 19:43:38.000000 types-aiobotocore-cur-2.9.0/types_aiobotocore_cur/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:43:38.000000 types-aiobotocore-cur-2.9.0/types_aiobotocore_cur/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:02.345869 types-aiobotocore-cur-2.9.0/types_aiobotocore_cur.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13040 2023-12-13 19:59:02.000000 types-aiobotocore-cur-2.9.0/types_aiobotocore_cur.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      737 2023-12-13 19:59:02.000000 types-aiobotocore-cur-2.9.0/types_aiobotocore_cur.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:02.000000 types-aiobotocore-cur-2.9.0/types_aiobotocore_cur.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:02.000000 types-aiobotocore-cur-2.9.0/types_aiobotocore_cur.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:02.000000 types-aiobotocore-cur-2.9.0/types_aiobotocore_cur.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-13 19:59:02.000000 types-aiobotocore-cur-2.9.0/types_aiobotocore_cur.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:28.057407 types-aiobotocore-cur-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:05:34.000000 types-aiobotocore-cur-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13060 2024-01-18 01:20:28.057407 types-aiobotocore-cur-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11471 2024-01-18 01:05:34.000000 types-aiobotocore-cur-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:28.057407 types-aiobotocore-cur-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-01-18 01:05:34.000000 types-aiobotocore-cur-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:28.057407 types-aiobotocore-cur-2.9.1/types_aiobotocore_cur/
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-01-18 01:05:34.000000 types-aiobotocore-cur-2.9.1/types_aiobotocore_cur/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-01-18 01:05:34.000000 types-aiobotocore-cur-2.9.1/types_aiobotocore_cur/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-01-18 01:05:34.000000 types-aiobotocore-cur-2.9.1/types_aiobotocore_cur/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8856 2024-01-18 01:05:34.000000 types-aiobotocore-cur-2.9.1/types_aiobotocore_cur/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8853 2024-01-18 01:05:34.000000 types-aiobotocore-cur-2.9.1/types_aiobotocore_cur/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-01-18 01:05:34.000000 types-aiobotocore-cur-2.9.1/types_aiobotocore_cur/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-01-18 01:05:34.000000 types-aiobotocore-cur-2.9.1/types_aiobotocore_cur/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-01-18 01:05:34.000000 types-aiobotocore-cur-2.9.1/types_aiobotocore_cur/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-01-18 01:05:34.000000 types-aiobotocore-cur-2.9.1/types_aiobotocore_cur/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:05:34.000000 types-aiobotocore-cur-2.9.1/types_aiobotocore_cur/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-01-18 01:05:34.000000 types-aiobotocore-cur-2.9.1/types_aiobotocore_cur/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-01-18 01:05:34.000000 types-aiobotocore-cur-2.9.1/types_aiobotocore_cur/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:05:34.000000 types-aiobotocore-cur-2.9.1/types_aiobotocore_cur/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:28.057407 types-aiobotocore-cur-2.9.1/types_aiobotocore_cur.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13060 2024-01-18 01:20:28.000000 types-aiobotocore-cur-2.9.1/types_aiobotocore_cur.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-01-18 01:20:28.000000 types-aiobotocore-cur-2.9.1/types_aiobotocore_cur.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:28.000000 types-aiobotocore-cur-2.9.1/types_aiobotocore_cur.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:28.000000 types-aiobotocore-cur-2.9.1/types_aiobotocore_cur.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:28.000000 types-aiobotocore-cur-2.9.1/types_aiobotocore_cur.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-18 01:20:28.000000 types-aiobotocore-cur-2.9.1/types_aiobotocore_cur.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cur-2.9.0/LICENSE` & `types-aiobotocore-cur-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-cur-2.9.0/PKG-INFO` & `types-aiobotocore-cur-2.9.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cur
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CostandUsageReportService 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CostandUsageReportService 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cur/
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
 
 <a id="types-aiobotocore-cur"></a>
 
 # types-aiobotocore-cur
 
 [![PyPI - types-aiobotocore-cur](https://img.shields.io/pypi/v/types-aiobotocore-cur.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cur)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cur.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cur)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cur/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cur)](https://pepy.tech/project/types-aiobotocore-cur)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CostandUsageReportService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService)
+[aiobotocore.CostandUsageReportService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService)
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
 [types-aiobotocore-cur docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cur/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-cur-2.9.0/README.md` & `types-aiobotocore-cur-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cur.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cur)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cur/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cur)](https://pepy.tech/project/types-aiobotocore-cur)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CostandUsageReportService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService)
+[aiobotocore.CostandUsageReportService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService)
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
 [types-aiobotocore-cur docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cur/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-cur-2.9.0/setup.py` & `types-aiobotocore-cur-2.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cur",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_cur"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CostandUsageReportService 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.CostandUsageReportService 2.9.1 service generated with"
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
     keywords="aiobotocore cur type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_cur": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cur/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-cur-2.9.0/types_aiobotocore_cur/__init__.py` & `types-aiobotocore-cur-2.9.1/types_aiobotocore_cur/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,9 +22,8 @@
 """
 
 from .client import CostandUsageReportServiceClient
 from .paginator import DescribeReportDefinitionsPaginator
 
 Client = CostandUsageReportServiceClient
 
-
 __all__ = ("Client", "CostandUsageReportServiceClient", "DescribeReportDefinitionsPaginator")
```

### Comparing `types-aiobotocore-cur-2.9.0/types_aiobotocore_cur/__init__.pyi` & `types-aiobotocore-cur-2.9.1/types_aiobotocore_cur/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cur-2.9.0/types_aiobotocore_cur/__main__.py` & `types-aiobotocore-cur-2.9.1/types_aiobotocore_cur/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CostandUsageReportService 2.9.0\nVersion:        "
-        " 2.9.0\nBuilder version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.CostandUsageReportService 2.9.1\nVersion:        "
+        " 2.9.1\nBuilder version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cur//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService\nOther"
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

### Comparing `types-aiobotocore-cur-2.9.0/types_aiobotocore_cur/client.py` & `types-aiobotocore-cur-2.9.1/types_aiobotocore_cur/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("CostandUsageReportServiceClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
```

### Comparing `types-aiobotocore-cur-2.9.0/types_aiobotocore_cur/client.pyi` & `types-aiobotocore-cur-2.9.1/types_aiobotocore_cur/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cur-2.9.0/types_aiobotocore_cur/literals.py` & `types-aiobotocore-cur-2.9.1/types_aiobotocore_cur/literals.py`

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
     "AWSRegionType",
     "AdditionalArtifactType",
     "CompressionFormatType",
     "DescribeReportDefinitionsPaginatorName",
     "LastStatusType",
     "ReportFormatType",
@@ -33,15 +32,14 @@
     "CostandUsageReportServiceServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AWSRegionType = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
```

### Comparing `types-aiobotocore-cur-2.9.0/types_aiobotocore_cur/literals.pyi` & `types-aiobotocore-cur-2.9.1/types_aiobotocore_cur/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cur-2.9.0/types_aiobotocore_cur/paginator.py` & `types-aiobotocore-cur-2.9.1/types_aiobotocore_cur/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .type_defs import DescribeReportDefinitionsResponseTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("DescribeReportDefinitionsPaginator",)
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
```

### Comparing `types-aiobotocore-cur-2.9.0/types_aiobotocore_cur/paginator.pyi` & `types-aiobotocore-cur-2.9.1/types_aiobotocore_cur/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cur-2.9.0/types_aiobotocore_cur/type_defs.py` & `types-aiobotocore-cur-2.9.1/types_aiobotocore_cur/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "DeleteReportDefinitionRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeReportDefinitionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagTypeDef",
```

### Comparing `types-aiobotocore-cur-2.9.0/types_aiobotocore_cur/type_defs.pyi` & `types-aiobotocore-cur-2.9.1/types_aiobotocore_cur/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cur-2.9.0/types_aiobotocore_cur.egg-info/PKG-INFO` & `types-aiobotocore-cur-2.9.1/types_aiobotocore_cur.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cur
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CostandUsageReportService 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CostandUsageReportService 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cur/
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
 
 <a id="types-aiobotocore-cur"></a>
 
 # types-aiobotocore-cur
 
 [![PyPI - types-aiobotocore-cur](https://img.shields.io/pypi/v/types-aiobotocore-cur.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cur)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cur.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cur)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cur/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cur)](https://pepy.tech/project/types-aiobotocore-cur)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CostandUsageReportService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService)
+[aiobotocore.CostandUsageReportService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService)
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
 [types-aiobotocore-cur docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cur/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-cur-2.9.0/types_aiobotocore_cur.egg-info/SOURCES.txt` & `types-aiobotocore-cur-2.9.1/types_aiobotocore_cur.egg-info/SOURCES.txt`

 * *Files identical despite different names*

