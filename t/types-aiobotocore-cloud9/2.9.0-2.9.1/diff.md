# Comparing `tmp/types-aiobotocore-cloud9-2.9.0.tar.gz` & `tmp/types-aiobotocore-cloud9-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cloud9-2.9.0.tar", last modified: Wed Dec 13 19:58:47 2023, max compression
+gzip compressed data, was "types-aiobotocore-cloud9-2.9.1.tar", last modified: Thu Jan 18 01:20:14 2024, max compression
```

## Comparing `types-aiobotocore-cloud9-2.9.0.tar` & `types-aiobotocore-cloud9-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:47.717987 types-aiobotocore-cloud9-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:42:12.000000 types-aiobotocore-cloud9-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13098 2023-12-13 19:58:47.717987 types-aiobotocore-cloud9-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11539 2023-12-13 19:42:12.000000 types-aiobotocore-cloud9-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:47.717987 types-aiobotocore-cloud9-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2023-12-13 19:42:12.000000 types-aiobotocore-cloud9-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:47.717987 types-aiobotocore-cloud9-2.9.0/types_aiobotocore_cloud9/
--rw-r--r--   0 runner    (1001) docker     (127)      951 2023-12-13 19:42:12.000000 types-aiobotocore-cloud9-2.9.0/types_aiobotocore_cloud9/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2023-12-13 19:42:12.000000 types-aiobotocore-cloud9-2.9.0/types_aiobotocore_cloud9/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      917 2023-12-13 19:42:12.000000 types-aiobotocore-cloud9-2.9.0/types_aiobotocore_cloud9/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13609 2023-12-13 19:42:12.000000 types-aiobotocore-cloud9-2.9.0/types_aiobotocore_cloud9/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13605 2023-12-13 19:42:12.000000 types-aiobotocore-cloud9-2.9.0/types_aiobotocore_cloud9/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10041 2023-12-13 19:42:12.000000 types-aiobotocore-cloud9-2.9.0/types_aiobotocore_cloud9/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10039 2023-12-13 19:42:12.000000 types-aiobotocore-cloud9-2.9.0/types_aiobotocore_cloud9/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2023-12-13 19:42:12.000000 types-aiobotocore-cloud9-2.9.0/types_aiobotocore_cloud9/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3413 2023-12-13 19:42:12.000000 types-aiobotocore-cloud9-2.9.0/types_aiobotocore_cloud9/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:42:12.000000 types-aiobotocore-cloud9-2.9.0/types_aiobotocore_cloud9/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9020 2023-12-13 19:42:13.000000 types-aiobotocore-cloud9-2.9.0/types_aiobotocore_cloud9/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9019 2023-12-13 19:42:12.000000 types-aiobotocore-cloud9-2.9.0/types_aiobotocore_cloud9/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:42:12.000000 types-aiobotocore-cloud9-2.9.0/types_aiobotocore_cloud9/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:47.717987 types-aiobotocore-cloud9-2.9.0/types_aiobotocore_cloud9.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13098 2023-12-13 19:58:47.000000 types-aiobotocore-cloud9-2.9.0/types_aiobotocore_cloud9.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      794 2023-12-13 19:58:47.000000 types-aiobotocore-cloud9-2.9.0/types_aiobotocore_cloud9.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:47.000000 types-aiobotocore-cloud9-2.9.0/types_aiobotocore_cloud9.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:47.000000 types-aiobotocore-cloud9-2.9.0/types_aiobotocore_cloud9.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:47.000000 types-aiobotocore-cloud9-2.9.0/types_aiobotocore_cloud9.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-13 19:58:47.000000 types-aiobotocore-cloud9-2.9.0/types_aiobotocore_cloud9.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:14.625469 types-aiobotocore-cloud9-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:04:09.000000 types-aiobotocore-cloud9-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13118 2024-01-18 01:20:14.625469 types-aiobotocore-cloud9-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11539 2024-01-18 01:04:09.000000 types-aiobotocore-cloud9-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:14.625469 types-aiobotocore-cloud9-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-01-18 01:04:09.000000 types-aiobotocore-cloud9-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:14.621469 types-aiobotocore-cloud9-2.9.1/types_aiobotocore_cloud9/
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-01-18 01:04:09.000000 types-aiobotocore-cloud9-2.9.1/types_aiobotocore_cloud9/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-01-18 01:04:09.000000 types-aiobotocore-cloud9-2.9.1/types_aiobotocore_cloud9/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-01-18 01:04:09.000000 types-aiobotocore-cloud9-2.9.1/types_aiobotocore_cloud9/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13611 2024-01-18 01:04:09.000000 types-aiobotocore-cloud9-2.9.1/types_aiobotocore_cloud9/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13608 2024-01-18 01:04:09.000000 types-aiobotocore-cloud9-2.9.1/types_aiobotocore_cloud9/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10039 2024-01-18 01:04:10.000000 types-aiobotocore-cloud9-2.9.1/types_aiobotocore_cloud9/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10039 2024-01-18 01:04:10.000000 types-aiobotocore-cloud9-2.9.1/types_aiobotocore_cloud9/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-01-18 01:04:09.000000 types-aiobotocore-cloud9-2.9.1/types_aiobotocore_cloud9/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-01-18 01:04:09.000000 types-aiobotocore-cloud9-2.9.1/types_aiobotocore_cloud9/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:04:09.000000 types-aiobotocore-cloud9-2.9.1/types_aiobotocore_cloud9/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9019 2024-01-18 01:04:10.000000 types-aiobotocore-cloud9-2.9.1/types_aiobotocore_cloud9/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9019 2024-01-18 01:04:10.000000 types-aiobotocore-cloud9-2.9.1/types_aiobotocore_cloud9/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:04:09.000000 types-aiobotocore-cloud9-2.9.1/types_aiobotocore_cloud9/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:14.621469 types-aiobotocore-cloud9-2.9.1/types_aiobotocore_cloud9.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13118 2024-01-18 01:20:14.000000 types-aiobotocore-cloud9-2.9.1/types_aiobotocore_cloud9.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-01-18 01:20:14.000000 types-aiobotocore-cloud9-2.9.1/types_aiobotocore_cloud9.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:14.000000 types-aiobotocore-cloud9-2.9.1/types_aiobotocore_cloud9.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:14.000000 types-aiobotocore-cloud9-2.9.1/types_aiobotocore_cloud9.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:14.000000 types-aiobotocore-cloud9-2.9.1/types_aiobotocore_cloud9.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-01-18 01:20:14.000000 types-aiobotocore-cloud9-2.9.1/types_aiobotocore_cloud9.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cloud9-2.9.0/LICENSE` & `types-aiobotocore-cloud9-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-cloud9-2.9.0/PKG-INFO` & `types-aiobotocore-cloud9-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloud9
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Cloud9 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Cloud9 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloud9/
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
 
 <a id="types-aiobotocore-cloud9"></a>
 
 # types-aiobotocore-cloud9
 
 [![PyPI - types-aiobotocore-cloud9](https://img.shields.io/pypi/v/types-aiobotocore-cloud9.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloud9)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloud9.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloud9)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloud9/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloud9)](https://pepy.tech/project/types-aiobotocore-cloud9)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Cloud9 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9)
+[aiobotocore.Cloud9 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9)
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
 [types-aiobotocore-cloud9 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloud9/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-cloud9-2.9.0/README.md` & `types-aiobotocore-cloud9-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloud9.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloud9)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloud9/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloud9)](https://pepy.tech/project/types-aiobotocore-cloud9)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Cloud9 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9)
+[aiobotocore.Cloud9 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9)
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
 [types-aiobotocore-cloud9 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloud9/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-cloud9-2.9.0/setup.py` & `types-aiobotocore-cloud9-2.9.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cloud9",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_cloud9"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Cloud9 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.Cloud9 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore cloud9 type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_cloud9": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloud9/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-cloud9-2.9.0/types_aiobotocore_cloud9/__init__.py` & `types-aiobotocore-cloud9-2.9.1/types_aiobotocore_cloud9/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,13 @@
 """
 
 from .client import Cloud9Client
 from .paginator import DescribeEnvironmentMembershipsPaginator, ListEnvironmentsPaginator
 
 Client = Cloud9Client
 
-
 __all__ = (
     "Client",
     "Cloud9Client",
     "DescribeEnvironmentMembershipsPaginator",
     "ListEnvironmentsPaginator",
 )
```

### Comparing `types-aiobotocore-cloud9-2.9.0/types_aiobotocore_cloud9/__init__.pyi` & `types-aiobotocore-cloud9-2.9.1/types_aiobotocore_cloud9/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloud9-2.9.0/types_aiobotocore_cloud9/__main__.py` & `types-aiobotocore-cloud9-2.9.1/types_aiobotocore_cloud9/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Cloud9 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Cloud9 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloud9//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9\nOther"
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

### Comparing `types-aiobotocore-cloud9-2.9.0/types_aiobotocore_cloud9/client.py` & `types-aiobotocore-cloud9-2.9.1/types_aiobotocore_cloud9/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("Cloud9Client",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -111,15 +110,15 @@
         description: str = ...,
         clientRequestToken: str = ...,
         subnetId: str = ...,
         automaticStopTimeMinutes: int = ...,
         ownerArn: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         connectionType: ConnectionTypeType = ...,
-        dryRun: bool = ...
+        dryRun: bool = ...,
     ) -> CreateEnvironmentEC2ResultTypeDef:
         """
         Creates an Cloud9 development environment, launches an Amazon Elastic Compute
         Cloud (Amazon EC2) instance, and then connects from the instance to the
         environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9.Client.create_environment_ec2)
@@ -157,15 +156,15 @@
     async def describe_environment_memberships(
         self,
         *,
         userArn: str = ...,
         environmentId: str = ...,
         permissions: Sequence[PermissionsType] = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> DescribeEnvironmentMembershipsResultTypeDef:
         """
         Gets information about environment members for an Cloud9 development
         environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9.Client.describe_environment_memberships)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloud9/client/#describe_environment_memberships)
@@ -243,15 +242,15 @@
 
     async def update_environment(
         self,
         *,
         environmentId: str,
         name: str = ...,
         description: str = ...,
-        managedCredentialsAction: ManagedCredentialsActionType = ...
+        managedCredentialsAction: ManagedCredentialsActionType = ...,
     ) -> Dict[str, Any]:
         """
         Changes the settings of an existing Cloud9 development environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9.Client.update_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloud9/client/#update_environment)
         """
```

### Comparing `types-aiobotocore-cloud9-2.9.0/types_aiobotocore_cloud9/client.pyi` & `types-aiobotocore-cloud9-2.9.1/types_aiobotocore_cloud9/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         description: str = ...,
         clientRequestToken: str = ...,
         subnetId: str = ...,
         automaticStopTimeMinutes: int = ...,
         ownerArn: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         connectionType: ConnectionTypeType = ...,
-        dryRun: bool = ...
+        dryRun: bool = ...,
     ) -> CreateEnvironmentEC2ResultTypeDef:
         """
         Creates an Cloud9 development environment, launches an Amazon Elastic Compute
         Cloud (Amazon EC2) instance, and then connects from the instance to the
         environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9.Client.create_environment_ec2)
@@ -153,15 +153,15 @@
     async def describe_environment_memberships(
         self,
         *,
         userArn: str = ...,
         environmentId: str = ...,
         permissions: Sequence[PermissionsType] = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> DescribeEnvironmentMembershipsResultTypeDef:
         """
         Gets information about environment members for an Cloud9 development
         environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9.Client.describe_environment_memberships)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloud9/client/#describe_environment_memberships)
@@ -239,15 +239,15 @@
 
     async def update_environment(
         self,
         *,
         environmentId: str,
         name: str = ...,
         description: str = ...,
-        managedCredentialsAction: ManagedCredentialsActionType = ...
+        managedCredentialsAction: ManagedCredentialsActionType = ...,
     ) -> Dict[str, Any]:
         """
         Changes the settings of an existing Cloud9 development environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9.Client.update_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloud9/client/#update_environment)
         """
```

### Comparing `types-aiobotocore-cloud9-2.9.0/types_aiobotocore_cloud9/literals.py` & `types-aiobotocore-cloud9-2.9.1/types_aiobotocore_cloud9/literals.py`

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
     "ConnectionTypeType",
     "DescribeEnvironmentMembershipsPaginatorName",
     "EnvironmentLifecycleStatusType",
     "EnvironmentStatusType",
     "EnvironmentTypeType",
     "ListEnvironmentsPaginatorName",
@@ -34,15 +33,14 @@
     "Cloud9ServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ConnectionTypeType = Literal["CONNECT_SSH", "CONNECT_SSM"]
 DescribeEnvironmentMembershipsPaginatorName = Literal["describe_environment_memberships"]
 EnvironmentLifecycleStatusType = Literal[
     "CREATED", "CREATE_FAILED", "CREATING", "DELETE_FAILED", "DELETING"
 ]
 EnvironmentStatusType = Literal[
     "connecting", "creating", "deleting", "error", "ready", "stopped", "stopping"
```

### Comparing `types-aiobotocore-cloud9-2.9.0/types_aiobotocore_cloud9/literals.pyi` & `types-aiobotocore-cloud9-2.9.1/types_aiobotocore_cloud9/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloud9-2.9.0/types_aiobotocore_cloud9/paginator.py` & `types-aiobotocore-cloud9-2.9.1/types_aiobotocore_cloud9/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     DescribeEnvironmentMembershipsResultTypeDef,
     ListEnvironmentsResultTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("DescribeEnvironmentMembershipsPaginator", "ListEnvironmentsPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -56,15 +55,15 @@
 
     def paginate(
         self,
         *,
         userArn: str = ...,
         environmentId: str = ...,
         permissions: Sequence[PermissionsType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeEnvironmentMembershipsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9.Paginator.DescribeEnvironmentMemberships.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloud9/paginators/#describeenvironmentmembershipspaginator)
         """
```

### Comparing `types-aiobotocore-cloud9-2.9.0/types_aiobotocore_cloud9/paginator.pyi` & `types-aiobotocore-cloud9-2.9.1/types_aiobotocore_cloud9/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
     def paginate(
         self,
         *,
         userArn: str = ...,
         environmentId: str = ...,
         permissions: Sequence[PermissionsType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeEnvironmentMembershipsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9.Paginator.DescribeEnvironmentMemberships.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloud9/paginators/#describeenvironmentmembershipspaginator)
         """
 
 class ListEnvironmentsPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-cloud9-2.9.0/types_aiobotocore_cloud9/type_defs.py` & `types-aiobotocore-cloud9-2.9.1/types_aiobotocore_cloud9/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "CreateEnvironmentMembershipRequestRequestTypeDef",
     "EnvironmentMemberTypeDef",
     "DeleteEnvironmentMembershipRequestRequestTypeDef",
     "DeleteEnvironmentRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-cloud9-2.9.0/types_aiobotocore_cloud9/type_defs.pyi` & `types-aiobotocore-cloud9-2.9.1/types_aiobotocore_cloud9/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloud9-2.9.0/types_aiobotocore_cloud9.egg-info/PKG-INFO` & `types-aiobotocore-cloud9-2.9.1/types_aiobotocore_cloud9.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloud9
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Cloud9 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Cloud9 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloud9/
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
 
 <a id="types-aiobotocore-cloud9"></a>
 
 # types-aiobotocore-cloud9
 
 [![PyPI - types-aiobotocore-cloud9](https://img.shields.io/pypi/v/types-aiobotocore-cloud9.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloud9)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloud9.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloud9)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloud9/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloud9)](https://pepy.tech/project/types-aiobotocore-cloud9)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Cloud9 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9)
+[aiobotocore.Cloud9 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9)
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
 [types-aiobotocore-cloud9 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloud9/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-cloud9-2.9.0/types_aiobotocore_cloud9.egg-info/SOURCES.txt` & `types-aiobotocore-cloud9-2.9.1/types_aiobotocore_cloud9.egg-info/SOURCES.txt`

 * *Files identical despite different names*

