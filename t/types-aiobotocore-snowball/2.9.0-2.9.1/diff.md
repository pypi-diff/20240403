# Comparing `tmp/types-aiobotocore-snowball-2.9.0.tar.gz` & `tmp/types-aiobotocore-snowball-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-snowball-2.9.0.tar", last modified: Wed Dec 13 20:00:33 2023, max compression
+gzip compressed data, was "types-aiobotocore-snowball-2.9.1.tar", last modified: Thu Jan 18 01:21:52 2024, max compression
```

## Comparing `types-aiobotocore-snowball-2.9.0.tar` & `types-aiobotocore-snowball-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:33.965108 types-aiobotocore-snowball-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:56:37.000000 types-aiobotocore-snowball-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13710 2023-12-13 20:00:33.965108 types-aiobotocore-snowball-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12143 2023-12-13 19:56:37.000000 types-aiobotocore-snowball-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:33.969108 types-aiobotocore-snowball-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2023-12-13 19:56:37.000000 types-aiobotocore-snowball-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:33.965108 types-aiobotocore-snowball-2.9.0/types_aiobotocore_snowball/
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2023-12-13 19:56:37.000000 types-aiobotocore-snowball-2.9.0/types_aiobotocore_snowball/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2023-12-13 19:56:37.000000 types-aiobotocore-snowball-2.9.0/types_aiobotocore_snowball/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      936 2023-12-13 19:56:37.000000 types-aiobotocore-snowball-2.9.0/types_aiobotocore_snowball/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26121 2023-12-13 19:56:38.000000 types-aiobotocore-snowball-2.9.0/types_aiobotocore_snowball/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    26117 2023-12-13 19:56:38.000000 types-aiobotocore-snowball-2.9.0/types_aiobotocore_snowball/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11171 2023-12-13 19:56:38.000000 types-aiobotocore-snowball-2.9.0/types_aiobotocore_snowball/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11169 2023-12-13 19:56:38.000000 types-aiobotocore-snowball-2.9.0/types_aiobotocore_snowball/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7416 2023-12-13 19:56:38.000000 types-aiobotocore-snowball-2.9.0/types_aiobotocore_snowball/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7408 2023-12-13 19:56:38.000000 types-aiobotocore-snowball-2.9.0/types_aiobotocore_snowball/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:56:37.000000 types-aiobotocore-snowball-2.9.0/types_aiobotocore_snowball/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    27694 2023-12-13 19:56:38.000000 types-aiobotocore-snowball-2.9.0/types_aiobotocore_snowball/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    27693 2023-12-13 19:56:38.000000 types-aiobotocore-snowball-2.9.0/types_aiobotocore_snowball/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:56:37.000000 types-aiobotocore-snowball-2.9.0/types_aiobotocore_snowball/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:33.965108 types-aiobotocore-snowball-2.9.0/types_aiobotocore_snowball.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13710 2023-12-13 20:00:33.000000 types-aiobotocore-snowball-2.9.0/types_aiobotocore_snowball.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      832 2023-12-13 20:00:33.000000 types-aiobotocore-snowball-2.9.0/types_aiobotocore_snowball.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:33.000000 types-aiobotocore-snowball-2.9.0/types_aiobotocore_snowball.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:33.000000 types-aiobotocore-snowball-2.9.0/types_aiobotocore_snowball.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:33.000000 types-aiobotocore-snowball-2.9.0/types_aiobotocore_snowball.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-13 20:00:33.000000 types-aiobotocore-snowball-2.9.0/types_aiobotocore_snowball.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:52.045020 types-aiobotocore-snowball-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:18:09.000000 types-aiobotocore-snowball-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13730 2024-01-18 01:21:52.045020 types-aiobotocore-snowball-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12143 2024-01-18 01:18:09.000000 types-aiobotocore-snowball-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:52.045020 types-aiobotocore-snowball-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-01-18 01:18:09.000000 types-aiobotocore-snowball-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:52.045020 types-aiobotocore-snowball-2.9.1/types_aiobotocore_snowball/
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-01-18 01:18:09.000000 types-aiobotocore-snowball-2.9.1/types_aiobotocore_snowball/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-01-18 01:18:09.000000 types-aiobotocore-snowball-2.9.1/types_aiobotocore_snowball/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-01-18 01:18:09.000000 types-aiobotocore-snowball-2.9.1/types_aiobotocore_snowball/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26127 2024-01-18 01:18:09.000000 types-aiobotocore-snowball-2.9.1/types_aiobotocore_snowball/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26124 2024-01-18 01:18:09.000000 types-aiobotocore-snowball-2.9.1/types_aiobotocore_snowball/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11169 2024-01-18 01:18:09.000000 types-aiobotocore-snowball-2.9.1/types_aiobotocore_snowball/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11169 2024-01-18 01:18:09.000000 types-aiobotocore-snowball-2.9.1/types_aiobotocore_snowball/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7415 2024-01-18 01:18:09.000000 types-aiobotocore-snowball-2.9.1/types_aiobotocore_snowball/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7408 2024-01-18 01:18:09.000000 types-aiobotocore-snowball-2.9.1/types_aiobotocore_snowball/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:18:09.000000 types-aiobotocore-snowball-2.9.1/types_aiobotocore_snowball/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    27693 2024-01-18 01:18:10.000000 types-aiobotocore-snowball-2.9.1/types_aiobotocore_snowball/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27693 2024-01-18 01:18:10.000000 types-aiobotocore-snowball-2.9.1/types_aiobotocore_snowball/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:18:09.000000 types-aiobotocore-snowball-2.9.1/types_aiobotocore_snowball/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:52.045020 types-aiobotocore-snowball-2.9.1/types_aiobotocore_snowball.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13730 2024-01-18 01:21:52.000000 types-aiobotocore-snowball-2.9.1/types_aiobotocore_snowball.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-01-18 01:21:52.000000 types-aiobotocore-snowball-2.9.1/types_aiobotocore_snowball.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:52.000000 types-aiobotocore-snowball-2.9.1/types_aiobotocore_snowball.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:52.000000 types-aiobotocore-snowball-2.9.1/types_aiobotocore_snowball.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:52.000000 types-aiobotocore-snowball-2.9.1/types_aiobotocore_snowball.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-18 01:21:52.000000 types-aiobotocore-snowball-2.9.1/types_aiobotocore_snowball.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-snowball-2.9.0/LICENSE` & `types-aiobotocore-snowball-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-snowball-2.9.0/PKG-INFO` & `types-aiobotocore-snowball-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-snowball
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Snowball 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Snowball 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/
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
 
 <a id="types-aiobotocore-snowball"></a>
 
 # types-aiobotocore-snowball
 
 [![PyPI - types-aiobotocore-snowball](https://img.shields.io/pypi/v/types-aiobotocore-snowball.svg?color=blue)](https://pypi.org/project/types-aiobotocore-snowball)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-snowball.svg?color=blue)](https://pypi.org/project/types-aiobotocore-snowball)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-snowball)](https://pepy.tech/project/types-aiobotocore-snowball)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Snowball 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball)
+[aiobotocore.Snowball 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball)
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
 [types-aiobotocore-snowball docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-snowball-2.9.0/README.md` & `types-aiobotocore-snowball-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-snowball.svg?color=blue)](https://pypi.org/project/types-aiobotocore-snowball)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-snowball)](https://pepy.tech/project/types-aiobotocore-snowball)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Snowball 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball)
+[aiobotocore.Snowball 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball)
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
 [types-aiobotocore-snowball docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-snowball-2.9.0/setup.py` & `types-aiobotocore-snowball-2.9.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-snowball",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_snowball"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Snowball 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.Snowball 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore snowball type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_snowball": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-snowball-2.9.0/types_aiobotocore_snowball/__init__.py` & `types-aiobotocore-snowball-2.9.1/types_aiobotocore_snowball/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,14 @@
     ListCompatibleImagesPaginator,
     ListJobsPaginator,
     ListLongTermPricingPaginator,
 )
 
 Client = SnowballClient
 
-
 __all__ = (
     "Client",
     "DescribeAddressesPaginator",
     "ListClusterJobsPaginator",
     "ListClustersPaginator",
     "ListCompatibleImagesPaginator",
     "ListJobsPaginator",
```

### Comparing `types-aiobotocore-snowball-2.9.0/types_aiobotocore_snowball/__init__.pyi` & `types-aiobotocore-snowball-2.9.1/types_aiobotocore_snowball/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-snowball-2.9.0/types_aiobotocore_snowball/__main__.py` & `types-aiobotocore-snowball-2.9.1/types_aiobotocore_snowball/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Snowball 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Snowball 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball\nOther"
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

### Comparing `types-aiobotocore-snowball-2.9.0/types_aiobotocore_snowball/client.py` & `types-aiobotocore-snowball-2.9.1/types_aiobotocore_snowball/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("SnowballClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -176,15 +175,15 @@
         Notification: NotificationTypeDef = ...,
         ForwardingAddressId: str = ...,
         TaxDocuments: TaxDocumentsTypeDef = ...,
         RemoteManagement: RemoteManagementType = ...,
         InitialClusterSize: int = ...,
         ForceCreateJobs: bool = ...,
         LongTermPricingIds: Sequence[str] = ...,
-        SnowballCapacityPreference: SnowballCapacityType = ...
+        SnowballCapacityPreference: SnowballCapacityType = ...,
     ) -> CreateClusterResultTypeDef:
         """
         Creates an empty cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.create_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/client/#create_cluster)
         """
@@ -206,15 +205,15 @@
         SnowballType: SnowballTypeType = ...,
         ForwardingAddressId: str = ...,
         TaxDocuments: TaxDocumentsTypeDef = ...,
         DeviceConfiguration: DeviceConfigurationTypeDef = ...,
         RemoteManagement: RemoteManagementType = ...,
         LongTermPricingId: str = ...,
         ImpactLevel: ImpactLevelType = ...,
-        PickupDetails: PickupDetailsTypeDef = ...
+        PickupDetails: PickupDetailsTypeDef = ...,
     ) -> CreateJobResultTypeDef:
         """
         Creates a job to import or export data between Amazon S3 and your on-premises
         data
         center.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.create_job)
@@ -222,15 +221,15 @@
         """
 
     async def create_long_term_pricing(
         self,
         *,
         LongTermPricingType: LongTermPricingTypeType,
         SnowballType: SnowballTypeType,
-        IsLongTermPricingAutoRenew: bool = ...
+        IsLongTermPricingAutoRenew: bool = ...,
     ) -> CreateLongTermPricingResultTypeDef:
         """
         Creates a job with the long-term usage option for a device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.create_long_term_pricing)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/client/#create_long_term_pricing)
         """
@@ -416,15 +415,15 @@
 
     async def list_service_versions(
         self,
         *,
         ServiceName: ServiceNameType,
         DependentServices: Sequence[DependentServiceTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListServiceVersionsResultTypeDef:
         """
         Lists all supported versions for Snow on-device services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.list_service_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/client/#list_service_versions)
         """
@@ -436,15 +435,15 @@
         RoleARN: str = ...,
         Description: str = ...,
         Resources: JobResourceTypeDef = ...,
         OnDeviceServiceConfiguration: OnDeviceServiceConfigurationTypeDef = ...,
         AddressId: str = ...,
         ShippingOption: ShippingOptionType = ...,
         Notification: NotificationTypeDef = ...,
-        ForwardingAddressId: str = ...
+        ForwardingAddressId: str = ...,
     ) -> Dict[str, Any]:
         """
         While a cluster's `ClusterState` value is in the `AwaitingQuorum` state, you
         can update some of the information associated with a
         cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.update_cluster)
@@ -460,15 +459,15 @@
         Resources: JobResourceTypeDef = ...,
         OnDeviceServiceConfiguration: OnDeviceServiceConfigurationTypeDef = ...,
         AddressId: str = ...,
         ShippingOption: ShippingOptionType = ...,
         Description: str = ...,
         SnowballCapacityPreference: SnowballCapacityType = ...,
         ForwardingAddressId: str = ...,
-        PickupDetails: PickupDetailsTypeDef = ...
+        PickupDetails: PickupDetailsTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         While a job's `JobState` value is `New`, you can update some of the information
         associated with a
         job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.update_job)
@@ -486,15 +485,15 @@
         """
 
     async def update_long_term_pricing(
         self,
         *,
         LongTermPricingId: str,
         ReplacementJob: str = ...,
-        IsLongTermPricingAutoRenew: bool = ...
+        IsLongTermPricingAutoRenew: bool = ...,
     ) -> Dict[str, Any]:
         """
         Updates the long-term pricing type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.update_long_term_pricing)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/client/#update_long_term_pricing)
         """
```

### Comparing `types-aiobotocore-snowball-2.9.0/types_aiobotocore_snowball/client.pyi` & `types-aiobotocore-snowball-2.9.1/types_aiobotocore_snowball/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,15 @@
         Notification: NotificationTypeDef = ...,
         ForwardingAddressId: str = ...,
         TaxDocuments: TaxDocumentsTypeDef = ...,
         RemoteManagement: RemoteManagementType = ...,
         InitialClusterSize: int = ...,
         ForceCreateJobs: bool = ...,
         LongTermPricingIds: Sequence[str] = ...,
-        SnowballCapacityPreference: SnowballCapacityType = ...
+        SnowballCapacityPreference: SnowballCapacityType = ...,
     ) -> CreateClusterResultTypeDef:
         """
         Creates an empty cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.create_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/client/#create_cluster)
         """
@@ -202,15 +202,15 @@
         SnowballType: SnowballTypeType = ...,
         ForwardingAddressId: str = ...,
         TaxDocuments: TaxDocumentsTypeDef = ...,
         DeviceConfiguration: DeviceConfigurationTypeDef = ...,
         RemoteManagement: RemoteManagementType = ...,
         LongTermPricingId: str = ...,
         ImpactLevel: ImpactLevelType = ...,
-        PickupDetails: PickupDetailsTypeDef = ...
+        PickupDetails: PickupDetailsTypeDef = ...,
     ) -> CreateJobResultTypeDef:
         """
         Creates a job to import or export data between Amazon S3 and your on-premises
         data
         center.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.create_job)
@@ -218,15 +218,15 @@
         """
 
     async def create_long_term_pricing(
         self,
         *,
         LongTermPricingType: LongTermPricingTypeType,
         SnowballType: SnowballTypeType,
-        IsLongTermPricingAutoRenew: bool = ...
+        IsLongTermPricingAutoRenew: bool = ...,
     ) -> CreateLongTermPricingResultTypeDef:
         """
         Creates a job with the long-term usage option for a device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.create_long_term_pricing)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/client/#create_long_term_pricing)
         """
@@ -412,15 +412,15 @@
 
     async def list_service_versions(
         self,
         *,
         ServiceName: ServiceNameType,
         DependentServices: Sequence[DependentServiceTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListServiceVersionsResultTypeDef:
         """
         Lists all supported versions for Snow on-device services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.list_service_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/client/#list_service_versions)
         """
@@ -432,15 +432,15 @@
         RoleARN: str = ...,
         Description: str = ...,
         Resources: JobResourceTypeDef = ...,
         OnDeviceServiceConfiguration: OnDeviceServiceConfigurationTypeDef = ...,
         AddressId: str = ...,
         ShippingOption: ShippingOptionType = ...,
         Notification: NotificationTypeDef = ...,
-        ForwardingAddressId: str = ...
+        ForwardingAddressId: str = ...,
     ) -> Dict[str, Any]:
         """
         While a cluster's `ClusterState` value is in the `AwaitingQuorum` state, you
         can update some of the information associated with a
         cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.update_cluster)
@@ -456,15 +456,15 @@
         Resources: JobResourceTypeDef = ...,
         OnDeviceServiceConfiguration: OnDeviceServiceConfigurationTypeDef = ...,
         AddressId: str = ...,
         ShippingOption: ShippingOptionType = ...,
         Description: str = ...,
         SnowballCapacityPreference: SnowballCapacityType = ...,
         ForwardingAddressId: str = ...,
-        PickupDetails: PickupDetailsTypeDef = ...
+        PickupDetails: PickupDetailsTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         While a job's `JobState` value is `New`, you can update some of the information
         associated with a
         job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.update_job)
@@ -482,15 +482,15 @@
         """
 
     async def update_long_term_pricing(
         self,
         *,
         LongTermPricingId: str,
         ReplacementJob: str = ...,
-        IsLongTermPricingAutoRenew: bool = ...
+        IsLongTermPricingAutoRenew: bool = ...,
     ) -> Dict[str, Any]:
         """
         Updates the long-term pricing type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.update_long_term_pricing)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/client/#update_long_term_pricing)
         """
```

### Comparing `types-aiobotocore-snowball-2.9.0/types_aiobotocore_snowball/literals.py` & `types-aiobotocore-snowball-2.9.1/types_aiobotocore_snowball/literals.py`

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
     "AddressTypeType",
     "ClusterStateType",
     "DescribeAddressesPaginatorName",
     "DeviceServiceNameType",
     "ImpactLevelType",
     "JobStateType",
@@ -46,15 +45,14 @@
     "SnowballServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AddressTypeType = Literal["AWS_SHIP", "CUST_PICKUP"]
 ClusterStateType = Literal["AwaitingQuorum", "Cancelled", "Complete", "InUse", "Pending"]
 DescribeAddressesPaginatorName = Literal["describe_addresses"]
 DeviceServiceNameType = Literal["NFS_ON_DEVICE_SERVICE", "S3_ON_DEVICE_SERVICE"]
 ImpactLevelType = Literal["IL2", "IL4", "IL5", "IL6", "IL99"]
 JobStateType = Literal[
     "Cancelled",
```

### Comparing `types-aiobotocore-snowball-2.9.0/types_aiobotocore_snowball/literals.pyi` & `types-aiobotocore-snowball-2.9.1/types_aiobotocore_snowball/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-snowball-2.9.0/types_aiobotocore_snowball/paginator.py` & `types-aiobotocore-snowball-2.9.1/types_aiobotocore_snowball/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,14 @@
     "ListClusterJobsPaginator",
     "ListClustersPaginator",
     "ListCompatibleImagesPaginator",
     "ListJobsPaginator",
     "ListLongTermPricingPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
```

### Comparing `types-aiobotocore-snowball-2.9.0/types_aiobotocore_snowball/paginator.pyi` & `types-aiobotocore-snowball-2.9.1/types_aiobotocore_snowball/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-snowball-2.9.0/types_aiobotocore_snowball/type_defs.py` & `types-aiobotocore-snowball-2.9.1/types_aiobotocore_snowball/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AddressTypeDef",
     "CancelClusterRequestRequestTypeDef",
     "CancelJobRequestRequestTypeDef",
     "ClusterListEntryTypeDef",
     "NotificationTypeDef",
     "CompatibleImageTypeDef",
```

### Comparing `types-aiobotocore-snowball-2.9.0/types_aiobotocore_snowball/type_defs.pyi` & `types-aiobotocore-snowball-2.9.1/types_aiobotocore_snowball/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-snowball-2.9.0/types_aiobotocore_snowball.egg-info/PKG-INFO` & `types-aiobotocore-snowball-2.9.1/types_aiobotocore_snowball.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-snowball
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Snowball 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Snowball 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/
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
 
 <a id="types-aiobotocore-snowball"></a>
 
 # types-aiobotocore-snowball
 
 [![PyPI - types-aiobotocore-snowball](https://img.shields.io/pypi/v/types-aiobotocore-snowball.svg?color=blue)](https://pypi.org/project/types-aiobotocore-snowball)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-snowball.svg?color=blue)](https://pypi.org/project/types-aiobotocore-snowball)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-snowball)](https://pepy.tech/project/types-aiobotocore-snowball)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Snowball 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball)
+[aiobotocore.Snowball 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball)
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
 [types-aiobotocore-snowball docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-snowball-2.9.0/types_aiobotocore_snowball.egg-info/SOURCES.txt` & `types-aiobotocore-snowball-2.9.1/types_aiobotocore_snowball.egg-info/SOURCES.txt`

 * *Files identical despite different names*

