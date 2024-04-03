# Comparing `tmp/types-aiobotocore-cloudtrail-2.9.0.tar.gz` & `tmp/types-aiobotocore-cloudtrail-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cloudtrail-2.9.0.tar", last modified: Wed Dec 13 19:58:51 2023, max compression
+gzip compressed data, was "types-aiobotocore-cloudtrail-2.9.1.tar", last modified: Thu Jan 18 01:20:18 2024, max compression
```

## Comparing `types-aiobotocore-cloudtrail-2.9.0.tar` & `types-aiobotocore-cloudtrail-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:51.825955 types-aiobotocore-cloudtrail-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:42:34.000000 types-aiobotocore-cloudtrail-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13702 2023-12-13 19:58:51.825955 types-aiobotocore-cloudtrail-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12127 2023-12-13 19:42:34.000000 types-aiobotocore-cloudtrail-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:51.825955 types-aiobotocore-cloudtrail-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2023-12-13 19:42:34.000000 types-aiobotocore-cloudtrail-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:51.821955 types-aiobotocore-cloudtrail-2.9.0/types_aiobotocore_cloudtrail/
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2023-12-13 19:42:34.000000 types-aiobotocore-cloudtrail-2.9.0/types_aiobotocore_cloudtrail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2023-12-13 19:42:34.000000 types-aiobotocore-cloudtrail-2.9.0/types_aiobotocore_cloudtrail/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      944 2023-12-13 19:42:34.000000 types-aiobotocore-cloudtrail-2.9.0/types_aiobotocore_cloudtrail/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43232 2023-12-13 19:42:34.000000 types-aiobotocore-cloudtrail-2.9.0/types_aiobotocore_cloudtrail/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    43228 2023-12-13 19:42:34.000000 types-aiobotocore-cloudtrail-2.9.0/types_aiobotocore_cloudtrail/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10926 2023-12-13 19:42:34.000000 types-aiobotocore-cloudtrail-2.9.0/types_aiobotocore_cloudtrail/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10924 2023-12-13 19:42:34.000000 types-aiobotocore-cloudtrail-2.9.0/types_aiobotocore_cloudtrail/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7968 2023-12-13 19:42:34.000000 types-aiobotocore-cloudtrail-2.9.0/types_aiobotocore_cloudtrail/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7959 2023-12-13 19:42:34.000000 types-aiobotocore-cloudtrail-2.9.0/types_aiobotocore_cloudtrail/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:42:34.000000 types-aiobotocore-cloudtrail-2.9.0/types_aiobotocore_cloudtrail/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    38272 2023-12-13 19:42:36.000000 types-aiobotocore-cloudtrail-2.9.0/types_aiobotocore_cloudtrail/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    38271 2023-12-13 19:42:35.000000 types-aiobotocore-cloudtrail-2.9.0/types_aiobotocore_cloudtrail/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:42:34.000000 types-aiobotocore-cloudtrail-2.9.0/types_aiobotocore_cloudtrail/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:51.825955 types-aiobotocore-cloudtrail-2.9.0/types_aiobotocore_cloudtrail.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13702 2023-12-13 19:58:51.000000 types-aiobotocore-cloudtrail-2.9.0/types_aiobotocore_cloudtrail.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      870 2023-12-13 19:58:51.000000 types-aiobotocore-cloudtrail-2.9.0/types_aiobotocore_cloudtrail.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:51.000000 types-aiobotocore-cloudtrail-2.9.0/types_aiobotocore_cloudtrail.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:51.000000 types-aiobotocore-cloudtrail-2.9.0/types_aiobotocore_cloudtrail.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:51.000000 types-aiobotocore-cloudtrail-2.9.0/types_aiobotocore_cloudtrail.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-13 19:58:51.000000 types-aiobotocore-cloudtrail-2.9.0/types_aiobotocore_cloudtrail.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:18.397452 types-aiobotocore-cloudtrail-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:04:31.000000 types-aiobotocore-cloudtrail-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13722 2024-01-18 01:20:18.397452 types-aiobotocore-cloudtrail-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12127 2024-01-18 01:04:31.000000 types-aiobotocore-cloudtrail-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:18.397452 types-aiobotocore-cloudtrail-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-01-18 01:04:30.000000 types-aiobotocore-cloudtrail-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:18.397452 types-aiobotocore-cloudtrail-2.9.1/types_aiobotocore_cloudtrail/
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-01-18 01:04:31.000000 types-aiobotocore-cloudtrail-2.9.1/types_aiobotocore_cloudtrail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-01-18 01:04:31.000000 types-aiobotocore-cloudtrail-2.9.1/types_aiobotocore_cloudtrail/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-01-18 01:04:31.000000 types-aiobotocore-cloudtrail-2.9.1/types_aiobotocore_cloudtrail/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43245 2024-01-18 01:04:31.000000 types-aiobotocore-cloudtrail-2.9.1/types_aiobotocore_cloudtrail/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43242 2024-01-18 01:04:31.000000 types-aiobotocore-cloudtrail-2.9.1/types_aiobotocore_cloudtrail/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10924 2024-01-18 01:04:31.000000 types-aiobotocore-cloudtrail-2.9.1/types_aiobotocore_cloudtrail/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10924 2024-01-18 01:04:31.000000 types-aiobotocore-cloudtrail-2.9.1/types_aiobotocore_cloudtrail/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-01-18 01:04:31.000000 types-aiobotocore-cloudtrail-2.9.1/types_aiobotocore_cloudtrail/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7962 2024-01-18 01:04:31.000000 types-aiobotocore-cloudtrail-2.9.1/types_aiobotocore_cloudtrail/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:04:31.000000 types-aiobotocore-cloudtrail-2.9.1/types_aiobotocore_cloudtrail/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    38271 2024-01-18 01:04:32.000000 types-aiobotocore-cloudtrail-2.9.1/types_aiobotocore_cloudtrail/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38271 2024-01-18 01:04:32.000000 types-aiobotocore-cloudtrail-2.9.1/types_aiobotocore_cloudtrail/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:04:31.000000 types-aiobotocore-cloudtrail-2.9.1/types_aiobotocore_cloudtrail/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:18.397452 types-aiobotocore-cloudtrail-2.9.1/types_aiobotocore_cloudtrail.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13722 2024-01-18 01:20:18.000000 types-aiobotocore-cloudtrail-2.9.1/types_aiobotocore_cloudtrail.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-01-18 01:20:18.000000 types-aiobotocore-cloudtrail-2.9.1/types_aiobotocore_cloudtrail.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:18.000000 types-aiobotocore-cloudtrail-2.9.1/types_aiobotocore_cloudtrail.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:18.000000 types-aiobotocore-cloudtrail-2.9.1/types_aiobotocore_cloudtrail.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:18.000000 types-aiobotocore-cloudtrail-2.9.1/types_aiobotocore_cloudtrail.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-01-18 01:20:18.000000 types-aiobotocore-cloudtrail-2.9.1/types_aiobotocore_cloudtrail.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cloudtrail-2.9.0/LICENSE` & `types-aiobotocore-cloudtrail-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-cloudtrail-2.9.0/PKG-INFO` & `types-aiobotocore-cloudtrail-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudtrail
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CloudTrail 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CloudTrail 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/
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
 
 <a id="types-aiobotocore-cloudtrail"></a>
 
 # types-aiobotocore-cloudtrail
 
 [![PyPI - types-aiobotocore-cloudtrail](https://img.shields.io/pypi/v/types-aiobotocore-cloudtrail.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudtrail)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudtrail.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudtrail)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudtrail)](https://pepy.tech/project/types-aiobotocore-cloudtrail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudTrail 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
+[aiobotocore.CloudTrail 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
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
 [types-aiobotocore-cloudtrail docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-cloudtrail-2.9.0/README.md` & `types-aiobotocore-cloudtrail-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudtrail.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudtrail)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudtrail)](https://pepy.tech/project/types-aiobotocore-cloudtrail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudTrail 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
+[aiobotocore.CloudTrail 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
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
 [types-aiobotocore-cloudtrail docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-cloudtrail-2.9.0/setup.py` & `types-aiobotocore-cloudtrail-2.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cloudtrail",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_cloudtrail"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CloudTrail 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.CloudTrail 2.9.1 service generated with"
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
     keywords="aiobotocore cloudtrail type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_cloudtrail": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-cloudtrail-2.9.0/types_aiobotocore_cloudtrail/__init__.py` & `types-aiobotocore-cloudtrail-2.9.1/types_aiobotocore_cloudtrail/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,14 @@
     ListTagsPaginator,
     ListTrailsPaginator,
     LookupEventsPaginator,
 )
 
 Client = CloudTrailClient
 
-
 __all__ = (
     "Client",
     "CloudTrailClient",
     "ListImportFailuresPaginator",
     "ListImportsPaginator",
     "ListPublicKeysPaginator",
     "ListTagsPaginator",
```

### Comparing `types-aiobotocore-cloudtrail-2.9.0/types_aiobotocore_cloudtrail/__init__.pyi` & `types-aiobotocore-cloudtrail-2.9.1/types_aiobotocore_cloudtrail/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudtrail-2.9.0/types_aiobotocore_cloudtrail/__main__.py` & `types-aiobotocore-cloudtrail-2.9.1/types_aiobotocore_cloudtrail/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CloudTrail 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.CloudTrail 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail\nOther"
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

### Comparing `types-aiobotocore-cloudtrail-2.9.0/types_aiobotocore_cloudtrail/client.py` & `types-aiobotocore-cloudtrail-2.9.1/types_aiobotocore_cloudtrail/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("CloudTrailClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -238,15 +237,15 @@
 
     async def create_channel(
         self,
         *,
         Name: str,
         Source: str,
         Destinations: Sequence[DestinationTypeDef],
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateChannelResponseTypeDef:
         """
         Creates a channel for CloudTrail to ingest events from a partner or external
         source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.create_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/client/#create_channel)
@@ -260,15 +259,15 @@
         MultiRegionEnabled: bool = ...,
         OrganizationEnabled: bool = ...,
         RetentionPeriod: int = ...,
         TerminationProtectionEnabled: bool = ...,
         TagsList: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...,
         StartIngestion: bool = ...,
-        BillingMode: BillingModeType = ...
+        BillingMode: BillingModeType = ...,
     ) -> CreateEventDataStoreResponseTypeDef:
         """
         Creates a new event data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.create_event_data_store)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/client/#create_event_data_store)
         """
@@ -283,15 +282,15 @@
         IncludeGlobalServiceEvents: bool = ...,
         IsMultiRegionTrail: bool = ...,
         EnableLogFileValidation: bool = ...,
         CloudWatchLogsLogGroupArn: str = ...,
         CloudWatchLogsRoleArn: str = ...,
         KmsKeyId: str = ...,
         IsOrganizationTrail: bool = ...,
-        TagsList: Sequence[TagTypeDef] = ...
+        TagsList: Sequence[TagTypeDef] = ...,
     ) -> CreateTrailResponseTypeDef:
         """
         Creates a trail that specifies the settings for delivery of log data to an
         Amazon S3
         bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.create_trail)
@@ -451,15 +450,15 @@
 
     async def get_query_results(
         self,
         *,
         QueryId: str,
         EventDataStore: str = ...,
         NextToken: str = ...,
-        MaxQueryResults: int = ...
+        MaxQueryResults: int = ...,
     ) -> GetQueryResultsResponseTypeDef:
         """
         Gets event data results of a query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.get_query_results)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/client/#get_query_results)
         """
@@ -523,15 +522,15 @@
 
     async def list_imports(
         self,
         *,
         MaxResults: int = ...,
         Destination: str = ...,
         ImportStatus: ImportStatusType = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListImportsResponseTypeDef:
         """
         Returns information on all imports, or a select set of imports by
         `ImportStatus` or
         `Destination`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.list_imports)
@@ -539,15 +538,15 @@
         """
 
     async def list_public_keys(
         self,
         *,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListPublicKeysResponseTypeDef:
         """
         Returns all public keys whose private keys were used to sign the digest files
         within the specified time
         range.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.list_public_keys)
@@ -558,15 +557,15 @@
         self,
         *,
         EventDataStore: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
-        QueryStatus: QueryStatusType = ...
+        QueryStatus: QueryStatusType = ...,
     ) -> ListQueriesResponseTypeDef:
         """
         Returns a list of queries and query statuses for the past seven days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.list_queries)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/client/#list_queries)
         """
@@ -595,15 +594,15 @@
         self,
         *,
         LookupAttributes: Sequence[LookupAttributeTypeDef] = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         EventCategory: Literal["insight"] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> LookupEventsResponseTypeDef:
         """
         Looks up [management
         events](https://docs.aws.amazon.com/awscloudtrail/latest/userguide/cloudtrail-concepts.html#cloudtrail-concepts-management-events)
         or `CloudTrail Insights events
         <https://docs.aws.amazon.com/awscloudtrail/latest/userguide/cloudtrail-concepts.html#cloudtrail-concepts-insigh...`.
 
@@ -612,30 +611,30 @@
         """
 
     async def put_event_selectors(
         self,
         *,
         TrailName: str,
         EventSelectors: Sequence[EventSelectorTypeDef] = ...,
-        AdvancedEventSelectors: Sequence[AdvancedEventSelectorTypeDef] = ...
+        AdvancedEventSelectors: Sequence[AdvancedEventSelectorTypeDef] = ...,
     ) -> PutEventSelectorsResponseTypeDef:
         """
         Configures an event selector or advanced event selectors for your trail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.put_event_selectors)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/client/#put_event_selectors)
         """
 
     async def put_insight_selectors(
         self,
         *,
         InsightSelectors: Sequence[InsightSelectorTypeDef],
         TrailName: str = ...,
         EventDataStore: str = ...,
-        InsightsDestination: str = ...
+        InsightsDestination: str = ...,
     ) -> PutInsightSelectorsResponseTypeDef:
         """
         Lets you enable Insights event logging by specifying the Insights selectors
         that you want to enable on an existing trail or event data
         store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.put_insight_selectors)
@@ -700,15 +699,15 @@
     async def start_import(
         self,
         *,
         Destinations: Sequence[str] = ...,
         ImportSource: ImportSourceTypeDef = ...,
         StartEventTime: TimestampTypeDef = ...,
         EndEventTime: TimestampTypeDef = ...,
-        ImportId: str = ...
+        ImportId: str = ...,
     ) -> StartImportResponseTypeDef:
         """
         Starts an import of logged trail events from a source S3 bucket to a
         destination event data
         store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.start_import)
@@ -727,15 +726,15 @@
 
     async def start_query(
         self,
         *,
         QueryStatement: str = ...,
         DeliveryS3Uri: str = ...,
         QueryAlias: str = ...,
-        QueryParameters: Sequence[str] = ...
+        QueryParameters: Sequence[str] = ...,
     ) -> StartQueryResponseTypeDef:
         """
         Starts a CloudTrail Lake query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.start_query)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/client/#start_query)
         """
@@ -785,15 +784,15 @@
         Name: str = ...,
         AdvancedEventSelectors: Sequence[AdvancedEventSelectorTypeDef] = ...,
         MultiRegionEnabled: bool = ...,
         OrganizationEnabled: bool = ...,
         RetentionPeriod: int = ...,
         TerminationProtectionEnabled: bool = ...,
         KmsKeyId: str = ...,
-        BillingMode: BillingModeType = ...
+        BillingMode: BillingModeType = ...,
     ) -> UpdateEventDataStoreResponseTypeDef:
         """
         Updates an event data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.update_event_data_store)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/client/#update_event_data_store)
         """
@@ -807,15 +806,15 @@
         SnsTopicName: str = ...,
         IncludeGlobalServiceEvents: bool = ...,
         IsMultiRegionTrail: bool = ...,
         EnableLogFileValidation: bool = ...,
         CloudWatchLogsLogGroupArn: str = ...,
         CloudWatchLogsRoleArn: str = ...,
         KmsKeyId: str = ...,
-        IsOrganizationTrail: bool = ...
+        IsOrganizationTrail: bool = ...,
     ) -> UpdateTrailResponseTypeDef:
         """
         Updates trail settings that control what events you are logging, and how to
         handle log
         files.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.update_trail)
```

### Comparing `types-aiobotocore-cloudtrail-2.9.0/types_aiobotocore_cloudtrail/client.pyi` & `types-aiobotocore-cloudtrail-2.9.1/types_aiobotocore_cloudtrail/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -234,15 +234,15 @@
 
     async def create_channel(
         self,
         *,
         Name: str,
         Source: str,
         Destinations: Sequence[DestinationTypeDef],
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateChannelResponseTypeDef:
         """
         Creates a channel for CloudTrail to ingest events from a partner or external
         source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.create_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/client/#create_channel)
@@ -256,15 +256,15 @@
         MultiRegionEnabled: bool = ...,
         OrganizationEnabled: bool = ...,
         RetentionPeriod: int = ...,
         TerminationProtectionEnabled: bool = ...,
         TagsList: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...,
         StartIngestion: bool = ...,
-        BillingMode: BillingModeType = ...
+        BillingMode: BillingModeType = ...,
     ) -> CreateEventDataStoreResponseTypeDef:
         """
         Creates a new event data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.create_event_data_store)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/client/#create_event_data_store)
         """
@@ -279,15 +279,15 @@
         IncludeGlobalServiceEvents: bool = ...,
         IsMultiRegionTrail: bool = ...,
         EnableLogFileValidation: bool = ...,
         CloudWatchLogsLogGroupArn: str = ...,
         CloudWatchLogsRoleArn: str = ...,
         KmsKeyId: str = ...,
         IsOrganizationTrail: bool = ...,
-        TagsList: Sequence[TagTypeDef] = ...
+        TagsList: Sequence[TagTypeDef] = ...,
     ) -> CreateTrailResponseTypeDef:
         """
         Creates a trail that specifies the settings for delivery of log data to an
         Amazon S3
         bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.create_trail)
@@ -447,15 +447,15 @@
 
     async def get_query_results(
         self,
         *,
         QueryId: str,
         EventDataStore: str = ...,
         NextToken: str = ...,
-        MaxQueryResults: int = ...
+        MaxQueryResults: int = ...,
     ) -> GetQueryResultsResponseTypeDef:
         """
         Gets event data results of a query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.get_query_results)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/client/#get_query_results)
         """
@@ -519,15 +519,15 @@
 
     async def list_imports(
         self,
         *,
         MaxResults: int = ...,
         Destination: str = ...,
         ImportStatus: ImportStatusType = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListImportsResponseTypeDef:
         """
         Returns information on all imports, or a select set of imports by
         `ImportStatus` or
         `Destination`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.list_imports)
@@ -535,15 +535,15 @@
         """
 
     async def list_public_keys(
         self,
         *,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListPublicKeysResponseTypeDef:
         """
         Returns all public keys whose private keys were used to sign the digest files
         within the specified time
         range.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.list_public_keys)
@@ -554,15 +554,15 @@
         self,
         *,
         EventDataStore: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
-        QueryStatus: QueryStatusType = ...
+        QueryStatus: QueryStatusType = ...,
     ) -> ListQueriesResponseTypeDef:
         """
         Returns a list of queries and query statuses for the past seven days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.list_queries)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/client/#list_queries)
         """
@@ -591,15 +591,15 @@
         self,
         *,
         LookupAttributes: Sequence[LookupAttributeTypeDef] = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         EventCategory: Literal["insight"] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> LookupEventsResponseTypeDef:
         """
         Looks up [management
         events](https://docs.aws.amazon.com/awscloudtrail/latest/userguide/cloudtrail-concepts.html#cloudtrail-concepts-management-events)
         or `CloudTrail Insights events
         <https://docs.aws.amazon.com/awscloudtrail/latest/userguide/cloudtrail-concepts.html#cloudtrail-concepts-insigh...`.
 
@@ -608,30 +608,30 @@
         """
 
     async def put_event_selectors(
         self,
         *,
         TrailName: str,
         EventSelectors: Sequence[EventSelectorTypeDef] = ...,
-        AdvancedEventSelectors: Sequence[AdvancedEventSelectorTypeDef] = ...
+        AdvancedEventSelectors: Sequence[AdvancedEventSelectorTypeDef] = ...,
     ) -> PutEventSelectorsResponseTypeDef:
         """
         Configures an event selector or advanced event selectors for your trail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.put_event_selectors)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/client/#put_event_selectors)
         """
 
     async def put_insight_selectors(
         self,
         *,
         InsightSelectors: Sequence[InsightSelectorTypeDef],
         TrailName: str = ...,
         EventDataStore: str = ...,
-        InsightsDestination: str = ...
+        InsightsDestination: str = ...,
     ) -> PutInsightSelectorsResponseTypeDef:
         """
         Lets you enable Insights event logging by specifying the Insights selectors
         that you want to enable on an existing trail or event data
         store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.put_insight_selectors)
@@ -696,15 +696,15 @@
     async def start_import(
         self,
         *,
         Destinations: Sequence[str] = ...,
         ImportSource: ImportSourceTypeDef = ...,
         StartEventTime: TimestampTypeDef = ...,
         EndEventTime: TimestampTypeDef = ...,
-        ImportId: str = ...
+        ImportId: str = ...,
     ) -> StartImportResponseTypeDef:
         """
         Starts an import of logged trail events from a source S3 bucket to a
         destination event data
         store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.start_import)
@@ -723,15 +723,15 @@
 
     async def start_query(
         self,
         *,
         QueryStatement: str = ...,
         DeliveryS3Uri: str = ...,
         QueryAlias: str = ...,
-        QueryParameters: Sequence[str] = ...
+        QueryParameters: Sequence[str] = ...,
     ) -> StartQueryResponseTypeDef:
         """
         Starts a CloudTrail Lake query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.start_query)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/client/#start_query)
         """
@@ -781,15 +781,15 @@
         Name: str = ...,
         AdvancedEventSelectors: Sequence[AdvancedEventSelectorTypeDef] = ...,
         MultiRegionEnabled: bool = ...,
         OrganizationEnabled: bool = ...,
         RetentionPeriod: int = ...,
         TerminationProtectionEnabled: bool = ...,
         KmsKeyId: str = ...,
-        BillingMode: BillingModeType = ...
+        BillingMode: BillingModeType = ...,
     ) -> UpdateEventDataStoreResponseTypeDef:
         """
         Updates an event data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.update_event_data_store)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/client/#update_event_data_store)
         """
@@ -803,15 +803,15 @@
         SnsTopicName: str = ...,
         IncludeGlobalServiceEvents: bool = ...,
         IsMultiRegionTrail: bool = ...,
         EnableLogFileValidation: bool = ...,
         CloudWatchLogsLogGroupArn: str = ...,
         CloudWatchLogsRoleArn: str = ...,
         KmsKeyId: str = ...,
-        IsOrganizationTrail: bool = ...
+        IsOrganizationTrail: bool = ...,
     ) -> UpdateTrailResponseTypeDef:
         """
         Updates trail settings that control what events you are logging, and how to
         handle log
         files.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.update_trail)
```

### Comparing `types-aiobotocore-cloudtrail-2.9.0/types_aiobotocore_cloudtrail/literals.py` & `types-aiobotocore-cloudtrail-2.9.1/types_aiobotocore_cloudtrail/literals.py`

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
     "BillingModeType",
     "DeliveryStatusType",
     "DestinationTypeType",
     "EventCategoryType",
     "EventDataStoreStatusType",
     "FederationStatusType",
@@ -42,15 +41,14 @@
     "CloudTrailServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 BillingModeType = Literal["EXTENDABLE_RETENTION_PRICING", "FIXED_RETENTION_PRICING"]
 DeliveryStatusType = Literal[
     "ACCESS_DENIED",
     "ACCESS_DENIED_SIGNING_FILE",
     "CANCELLED",
     "FAILED",
     "FAILED_SIGNING_FILE",
```

### Comparing `types-aiobotocore-cloudtrail-2.9.0/types_aiobotocore_cloudtrail/literals.pyi` & `types-aiobotocore-cloudtrail-2.9.1/types_aiobotocore_cloudtrail/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudtrail-2.9.0/types_aiobotocore_cloudtrail/paginator.py` & `types-aiobotocore-cloudtrail-2.9.1/types_aiobotocore_cloudtrail/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,25 +51,23 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ListImportFailuresPaginator",
     "ListImportsPaginator",
     "ListPublicKeysPaginator",
     "ListTagsPaginator",
     "ListTrailsPaginator",
     "LookupEventsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -98,15 +96,15 @@
     """
 
     def paginate(
         self,
         *,
         Destination: str = ...,
         ImportStatus: ImportStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListImportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListImports.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/paginators/#listimportspaginator)
         """
 
 
@@ -117,15 +115,15 @@
     """
 
     def paginate(
         self,
         *,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPublicKeysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListPublicKeys.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/paginators/#listpublickeyspaginator)
         """
 
 
@@ -168,13 +166,13 @@
     def paginate(
         self,
         *,
         LookupAttributes: Sequence[LookupAttributeTypeDef] = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         EventCategory: Literal["insight"] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[LookupEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.LookupEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/paginators/#lookupeventspaginator)
         """
```

### Comparing `types-aiobotocore-cloudtrail-2.9.0/types_aiobotocore_cloudtrail/paginator.pyi` & `types-aiobotocore-cloudtrail-2.9.1/types_aiobotocore_cloudtrail/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
     """
 
     def paginate(
         self,
         *,
         Destination: str = ...,
         ImportStatus: ImportStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListImportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListImports.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/paginators/#listimportspaginator)
         """
 
 class ListPublicKeysPaginator(AioPaginator):
@@ -111,15 +111,15 @@
     """
 
     def paginate(
         self,
         *,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPublicKeysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListPublicKeys.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/paginators/#listpublickeyspaginator)
         """
 
 class ListTagsPaginator(AioPaginator):
@@ -159,13 +159,13 @@
     def paginate(
         self,
         *,
         LookupAttributes: Sequence[LookupAttributeTypeDef] = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         EventCategory: Literal["insight"] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[LookupEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.LookupEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/paginators/#lookupeventspaginator)
         """
```

### Comparing `types-aiobotocore-cloudtrail-2.9.0/types_aiobotocore_cloudtrail/type_defs.py` & `types-aiobotocore-cloudtrail-2.9.1/types_aiobotocore_cloudtrail/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "TagTypeDef",
     "AdvancedFieldSelectorTypeDef",
     "CancelQueryRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "ChannelTypeDef",
     "DestinationTypeDef",
```

### Comparing `types-aiobotocore-cloudtrail-2.9.0/types_aiobotocore_cloudtrail/type_defs.pyi` & `types-aiobotocore-cloudtrail-2.9.1/types_aiobotocore_cloudtrail/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudtrail-2.9.0/types_aiobotocore_cloudtrail.egg-info/PKG-INFO` & `types-aiobotocore-cloudtrail-2.9.1/types_aiobotocore_cloudtrail.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudtrail
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CloudTrail 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CloudTrail 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/
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
 
 <a id="types-aiobotocore-cloudtrail"></a>
 
 # types-aiobotocore-cloudtrail
 
 [![PyPI - types-aiobotocore-cloudtrail](https://img.shields.io/pypi/v/types-aiobotocore-cloudtrail.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudtrail)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudtrail.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudtrail)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudtrail)](https://pepy.tech/project/types-aiobotocore-cloudtrail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudTrail 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
+[aiobotocore.CloudTrail 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
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
 [types-aiobotocore-cloudtrail docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-cloudtrail-2.9.0/types_aiobotocore_cloudtrail.egg-info/SOURCES.txt` & `types-aiobotocore-cloudtrail-2.9.1/types_aiobotocore_cloudtrail.egg-info/SOURCES.txt`

 * *Files identical despite different names*

