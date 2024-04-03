# Comparing `tmp/types-aiobotocore-sns-2.9.0.tar.gz` & `tmp/types-aiobotocore-sns-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-sns-2.9.0.tar", last modified: Wed Dec 13 20:00:34 2023, max compression
+gzip compressed data, was "types-aiobotocore-sns-2.9.1.tar", last modified: Thu Jan 18 01:21:52 2024, max compression
```

## Comparing `types-aiobotocore-sns-2.9.0.tar` & `types-aiobotocore-sns-2.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:34.341105 types-aiobotocore-sns-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:56:39.000000 types-aiobotocore-sns-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16582 2023-12-13 20:00:34.341105 types-aiobotocore-sns-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15035 2023-12-13 19:56:39.000000 types-aiobotocore-sns-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:34.341105 types-aiobotocore-sns-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2023-12-13 19:56:39.000000 types-aiobotocore-sns-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:34.341105 types-aiobotocore-sns-2.9.0/types_aiobotocore_sns/
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2023-12-13 19:56:39.000000 types-aiobotocore-sns-2.9.0/types_aiobotocore_sns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2023-12-13 19:56:39.000000 types-aiobotocore-sns-2.9.0/types_aiobotocore_sns/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      905 2023-12-13 19:56:39.000000 types-aiobotocore-sns-2.9.0/types_aiobotocore_sns/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35656 2023-12-13 19:56:39.000000 types-aiobotocore-sns-2.9.0/types_aiobotocore_sns/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    35652 2023-12-13 19:56:39.000000 types-aiobotocore-sns-2.9.0/types_aiobotocore_sns/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10449 2023-12-13 19:56:42.000000 types-aiobotocore-sns-2.9.0/types_aiobotocore_sns/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10447 2023-12-13 19:56:42.000000 types-aiobotocore-sns-2.9.0/types_aiobotocore_sns/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10075 2023-12-13 19:56:42.000000 types-aiobotocore-sns-2.9.0/types_aiobotocore_sns/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10065 2023-12-13 19:56:42.000000 types-aiobotocore-sns-2.9.0/types_aiobotocore_sns/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:56:39.000000 types-aiobotocore-sns-2.9.0/types_aiobotocore_sns/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    37456 2023-12-13 19:56:42.000000 types-aiobotocore-sns-2.9.0/types_aiobotocore_sns/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    37440 2023-12-13 19:56:42.000000 types-aiobotocore-sns-2.9.0/types_aiobotocore_sns/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    27186 2023-12-13 19:56:43.000000 types-aiobotocore-sns-2.9.0/types_aiobotocore_sns/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    27185 2023-12-13 19:56:43.000000 types-aiobotocore-sns-2.9.0/types_aiobotocore_sns/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:56:39.000000 types-aiobotocore-sns-2.9.0/types_aiobotocore_sns/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:34.341105 types-aiobotocore-sns-2.9.0/types_aiobotocore_sns.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16582 2023-12-13 20:00:34.000000 types-aiobotocore-sns-2.9.0/types_aiobotocore_sns.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      822 2023-12-13 20:00:34.000000 types-aiobotocore-sns-2.9.0/types_aiobotocore_sns.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:34.000000 types-aiobotocore-sns-2.9.0/types_aiobotocore_sns.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:34.000000 types-aiobotocore-sns-2.9.0/types_aiobotocore_sns.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:34.000000 types-aiobotocore-sns-2.9.0/types_aiobotocore_sns.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-13 20:00:34.000000 types-aiobotocore-sns-2.9.0/types_aiobotocore_sns.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:52.381018 types-aiobotocore-sns-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:18:10.000000 types-aiobotocore-sns-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16602 2024-01-18 01:21:52.381018 types-aiobotocore-sns-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15035 2024-01-18 01:18:10.000000 types-aiobotocore-sns-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:52.381018 types-aiobotocore-sns-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-01-18 01:18:10.000000 types-aiobotocore-sns-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:52.381018 types-aiobotocore-sns-2.9.1/types_aiobotocore_sns/
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-01-18 01:18:10.000000 types-aiobotocore-sns-2.9.1/types_aiobotocore_sns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-01-18 01:18:10.000000 types-aiobotocore-sns-2.9.1/types_aiobotocore_sns/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-01-18 01:18:10.000000 types-aiobotocore-sns-2.9.1/types_aiobotocore_sns/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35660 2024-01-18 01:18:11.000000 types-aiobotocore-sns-2.9.1/types_aiobotocore_sns/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35657 2024-01-18 01:18:10.000000 types-aiobotocore-sns-2.9.1/types_aiobotocore_sns/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10447 2024-01-18 01:18:11.000000 types-aiobotocore-sns-2.9.1/types_aiobotocore_sns/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10447 2024-01-18 01:18:11.000000 types-aiobotocore-sns-2.9.1/types_aiobotocore_sns/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10074 2024-01-18 01:18:11.000000 types-aiobotocore-sns-2.9.1/types_aiobotocore_sns/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10065 2024-01-18 01:18:11.000000 types-aiobotocore-sns-2.9.1/types_aiobotocore_sns/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:18:10.000000 types-aiobotocore-sns-2.9.1/types_aiobotocore_sns/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    37633 2024-01-18 01:18:11.000000 types-aiobotocore-sns-2.9.1/types_aiobotocore_sns/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37618 2024-01-18 01:18:11.000000 types-aiobotocore-sns-2.9.1/types_aiobotocore_sns/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    27185 2024-01-18 01:18:11.000000 types-aiobotocore-sns-2.9.1/types_aiobotocore_sns/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27185 2024-01-18 01:18:11.000000 types-aiobotocore-sns-2.9.1/types_aiobotocore_sns/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:18:10.000000 types-aiobotocore-sns-2.9.1/types_aiobotocore_sns/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:52.381018 types-aiobotocore-sns-2.9.1/types_aiobotocore_sns.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16602 2024-01-18 01:21:52.000000 types-aiobotocore-sns-2.9.1/types_aiobotocore_sns.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-01-18 01:21:52.000000 types-aiobotocore-sns-2.9.1/types_aiobotocore_sns.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:52.000000 types-aiobotocore-sns-2.9.1/types_aiobotocore_sns.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:52.000000 types-aiobotocore-sns-2.9.1/types_aiobotocore_sns.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:52.000000 types-aiobotocore-sns-2.9.1/types_aiobotocore_sns.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-18 01:21:52.000000 types-aiobotocore-sns-2.9.1/types_aiobotocore_sns.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-sns-2.9.0/LICENSE` & `types-aiobotocore-sns-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-sns-2.9.0/PKG-INFO` & `types-aiobotocore-sns-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sns
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.SNS 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.SNS 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/
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
 
 <a id="types-aiobotocore-sns"></a>
 
 # types-aiobotocore-sns
 
 [![PyPI - types-aiobotocore-sns](https://img.shields.io/pypi/v/types-aiobotocore-sns.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sns)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sns.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sns)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sns)](https://pepy.tech/project/types-aiobotocore-sns)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SNS 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS)
+[aiobotocore.SNS 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS)
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
 [types-aiobotocore-sns docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-sns-2.9.0/README.md` & `types-aiobotocore-sns-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sns.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sns)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sns)](https://pepy.tech/project/types-aiobotocore-sns)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SNS 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS)
+[aiobotocore.SNS 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS)
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
 [types-aiobotocore-sns docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-sns-2.9.0/setup.py` & `types-aiobotocore-sns-2.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-sns",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_sns"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.SNS 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.SNS 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore sns type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_sns": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-sns-2.9.0/types_aiobotocore_sns/__init__.py` & `types-aiobotocore-sns-2.9.1/types_aiobotocore_sns/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,18 +48,16 @@
     ListSubscriptionsPaginator,
     ListTopicsPaginator,
 )
 from .service_resource import SNSServiceResource
 
 Client = SNSClient
 
-
 ServiceResource = SNSServiceResource
 
-
 __all__ = (
     "Client",
     "ListEndpointsByPlatformApplicationPaginator",
     "ListOriginationNumbersPaginator",
     "ListPhoneNumbersOptedOutPaginator",
     "ListPlatformApplicationsPaginator",
     "ListSMSSandboxPhoneNumbersPaginator",
```

### Comparing `types-aiobotocore-sns-2.9.0/types_aiobotocore_sns/__init__.pyi` & `types-aiobotocore-sns-2.9.1/types_aiobotocore_sns/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sns-2.9.0/types_aiobotocore_sns/__main__.py` & `types-aiobotocore-sns-2.9.1/types_aiobotocore_sns/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SNS 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.SNS 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS\nOther"
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

### Comparing `types-aiobotocore-sns-2.9.0/types_aiobotocore_sns/client.py` & `types-aiobotocore-sns-2.9.1/types_aiobotocore_sns/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("SNSClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -202,15 +201,15 @@
 
     async def create_platform_endpoint(
         self,
         *,
         PlatformApplicationArn: str,
         Token: str,
         CustomUserData: str = ...,
-        Attributes: Mapping[str, str] = ...
+        Attributes: Mapping[str, str] = ...,
     ) -> CreateEndpointResponseTypeDef:
         """
         Creates an endpoint for a device and mobile app on one of the supported push
         notification services, such as GCM (Firebase Cloud Messaging) and
         APNS.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Client.create_platform_endpoint)
@@ -231,15 +230,15 @@
 
     async def create_topic(
         self,
         *,
         Name: str,
         Attributes: Mapping[str, str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        DataProtectionPolicy: str = ...
+        DataProtectionPolicy: str = ...,
     ) -> CreateTopicResponseTypeDef:
         """
         Creates a topic to which notifications can be published.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Client.create_topic)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/client/#create_topic)
         """
@@ -484,15 +483,15 @@
         TopicArn: str = ...,
         TargetArn: str = ...,
         PhoneNumber: str = ...,
         Subject: str = ...,
         MessageStructure: str = ...,
         MessageAttributes: Mapping[str, MessageAttributeValueTypeDef] = ...,
         MessageDeduplicationId: str = ...,
-        MessageGroupId: str = ...
+        MessageGroupId: str = ...,
     ) -> PublishResponseTypeDef:
         """
         Sends a message to an Amazon SNS topic, a text message (SMS message) directly
         to a phone number, or a message to a mobile platform endpoint (when you specify
         the
         `TargetArn`).
 
@@ -500,15 +499,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/client/#publish)
         """
 
     async def publish_batch(
         self,
         *,
         TopicArn: str,
-        PublishBatchRequestEntries: Sequence[PublishBatchRequestEntryTypeDef]
+        PublishBatchRequestEntries: Sequence[PublishBatchRequestEntryTypeDef],
     ) -> PublishBatchResponseTypeDef:
         """
         Publishes up to ten messages to the specified topic.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Client.publish_batch)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/client/#publish_batch)
         """
@@ -591,15 +590,15 @@
     async def subscribe(
         self,
         *,
         TopicArn: str,
         Protocol: str,
         Endpoint: str = ...,
         Attributes: Mapping[str, str] = ...,
-        ReturnSubscriptionArn: bool = ...
+        ReturnSubscriptionArn: bool = ...,
     ) -> SubscribeResponseTypeDef:
         """
         Subscribes an endpoint to an Amazon SNS topic.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Client.subscribe)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/client/#subscribe)
         """
```

### Comparing `types-aiobotocore-sns-2.9.0/types_aiobotocore_sns/client.pyi` & `types-aiobotocore-sns-2.9.1/types_aiobotocore_sns/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -198,15 +198,15 @@
 
     async def create_platform_endpoint(
         self,
         *,
         PlatformApplicationArn: str,
         Token: str,
         CustomUserData: str = ...,
-        Attributes: Mapping[str, str] = ...
+        Attributes: Mapping[str, str] = ...,
     ) -> CreateEndpointResponseTypeDef:
         """
         Creates an endpoint for a device and mobile app on one of the supported push
         notification services, such as GCM (Firebase Cloud Messaging) and
         APNS.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Client.create_platform_endpoint)
@@ -227,15 +227,15 @@
 
     async def create_topic(
         self,
         *,
         Name: str,
         Attributes: Mapping[str, str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        DataProtectionPolicy: str = ...
+        DataProtectionPolicy: str = ...,
     ) -> CreateTopicResponseTypeDef:
         """
         Creates a topic to which notifications can be published.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Client.create_topic)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/client/#create_topic)
         """
@@ -480,15 +480,15 @@
         TopicArn: str = ...,
         TargetArn: str = ...,
         PhoneNumber: str = ...,
         Subject: str = ...,
         MessageStructure: str = ...,
         MessageAttributes: Mapping[str, MessageAttributeValueTypeDef] = ...,
         MessageDeduplicationId: str = ...,
-        MessageGroupId: str = ...
+        MessageGroupId: str = ...,
     ) -> PublishResponseTypeDef:
         """
         Sends a message to an Amazon SNS topic, a text message (SMS message) directly
         to a phone number, or a message to a mobile platform endpoint (when you specify
         the
         `TargetArn`).
 
@@ -496,15 +496,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/client/#publish)
         """
 
     async def publish_batch(
         self,
         *,
         TopicArn: str,
-        PublishBatchRequestEntries: Sequence[PublishBatchRequestEntryTypeDef]
+        PublishBatchRequestEntries: Sequence[PublishBatchRequestEntryTypeDef],
     ) -> PublishBatchResponseTypeDef:
         """
         Publishes up to ten messages to the specified topic.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Client.publish_batch)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/client/#publish_batch)
         """
@@ -587,15 +587,15 @@
     async def subscribe(
         self,
         *,
         TopicArn: str,
         Protocol: str,
         Endpoint: str = ...,
         Attributes: Mapping[str, str] = ...,
-        ReturnSubscriptionArn: bool = ...
+        ReturnSubscriptionArn: bool = ...,
     ) -> SubscribeResponseTypeDef:
         """
         Subscribes an endpoint to an Amazon SNS topic.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Client.subscribe)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/client/#subscribe)
         """
```

### Comparing `types-aiobotocore-sns-2.9.0/types_aiobotocore_sns/literals.py` & `types-aiobotocore-sns-2.9.1/types_aiobotocore_sns/literals.py`

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
     "LanguageCodeStringType",
     "ListEndpointsByPlatformApplicationPaginatorName",
     "ListOriginationNumbersPaginatorName",
     "ListPhoneNumbersOptedOutPaginatorName",
     "ListPlatformApplicationsPaginatorName",
     "ListSMSSandboxPhoneNumbersPaginatorName",
@@ -36,15 +35,14 @@
     "SNSServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 LanguageCodeStringType = Literal[
     "de-DE",
     "en-GB",
     "en-US",
     "es-419",
     "es-ES",
     "fr-CA",
```

### Comparing `types-aiobotocore-sns-2.9.0/types_aiobotocore_sns/literals.pyi` & `types-aiobotocore-sns-2.9.1/types_aiobotocore_sns/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sns-2.9.0/types_aiobotocore_sns/paginator.py` & `types-aiobotocore-sns-2.9.1/types_aiobotocore_sns/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,14 @@
     "ListPlatformApplicationsPaginator",
     "ListSMSSandboxPhoneNumbersPaginator",
     "ListSubscriptionsPaginator",
     "ListSubscriptionsByTopicPaginator",
     "ListTopicsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
```

### Comparing `types-aiobotocore-sns-2.9.0/types_aiobotocore_sns/paginator.pyi` & `types-aiobotocore-sns-2.9.1/types_aiobotocore_sns/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sns-2.9.0/types_aiobotocore_sns/service_resource.py` & `types-aiobotocore-sns-2.9.1/types_aiobotocore_sns/service_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,14 @@
 except ImportError:
     from builtins import object as AIOResourceCollection
 try:
     from boto3.resources.base import ResourceMeta
 except ImportError:
     from builtins import object as ResourceMeta
 
-
 __all__ = (
     "SNSServiceResource",
     "PlatformApplication",
     "PlatformEndpoint",
     "Subscription",
     "Topic",
     "ServiceResourcePlatformApplicationsCollection",
@@ -328,14 +327,15 @@
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.ServiceResource.PlatformEndpoint)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/service_resource/#platformendpoint)
     """
 
     attributes: Awaitable[Dict[str, str]]
     arn: str
+    meta: Awaitable["SNSResourceMeta"]
 
     async def delete(self) -> None:
         """
         Deletes the endpoint for a device and mobile app from Amazon SNS.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.PlatformEndpoint.delete)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/service_resource/#platformendpointdelete-method)
@@ -365,15 +365,15 @@
         Message: str,
         TopicArn: str = ...,
         PhoneNumber: str = ...,
         Subject: str = ...,
         MessageStructure: str = ...,
         MessageAttributes: Mapping[str, MessageAttributeValueTypeDef] = ...,
         MessageDeduplicationId: str = ...,
-        MessageGroupId: str = ...
+        MessageGroupId: str = ...,
     ) -> PublishResponseTypeDef:
         """
         Sends a message to an Amazon SNS topic, a text message (SMS message) directly
         to a phone number, or a message to a mobile platform endpoint (when you specify
         the
         `TargetArn`).
 
@@ -409,14 +409,15 @@
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.ServiceResource.Subscription)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/service_resource/#subscription)
     """
 
     attributes: Awaitable[Dict[str, str]]
     arn: str
+    meta: Awaitable["SNSResourceMeta"]
 
     async def delete(self) -> None:
         """
         Deletes a subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Subscription.delete)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/service_resource/#subscriptiondelete-method)
@@ -468,18 +469,19 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.ServiceResource.PlatformApplication)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/service_resource/#platformapplication)
     """
 
     attributes: Awaitable[Dict[str, str]]
     arn: str
     endpoints: PlatformApplicationEndpointsCollection
+    meta: Awaitable["SNSResourceMeta"]
 
     async def create_platform_endpoint(
         self, *, Token: str, CustomUserData: str = ..., Attributes: Mapping[str, str] = ...
-    ) -> _PlatformEndpoint:
+    ) -> "_PlatformEndpoint":
         """
         Creates an endpoint for a device and mobile app on one of the supported push
         notification services, such as GCM (Firebase Cloud Messaging) and
         APNS.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.PlatformApplication.create_platform_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/service_resource/#platformapplicationcreate_platform_endpoint-method)
@@ -542,14 +544,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.ServiceResource.Topic)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/service_resource/#topic)
     """
 
     attributes: Awaitable[Dict[str, str]]
     arn: str
     subscriptions: TopicSubscriptionsCollection
+    meta: Awaitable["SNSResourceMeta"]
 
     async def add_permission(
         self, *, Label: str, AWSAccountId: Sequence[str], ActionName: Sequence[str]
     ) -> None:
         """
         Adds a statement to a topic's access control policy, granting access for the
         specified Amazon Web Services accounts to the specified
@@ -557,15 +560,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Topic.add_permission)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/service_resource/#topicadd_permission-method)
         """
 
     async def confirm_subscription(
         self, *, Token: str, AuthenticateOnUnsubscribe: str = ...
-    ) -> _Subscription:
+    ) -> "_Subscription":
         """
         Verifies an endpoint owner's intent to receive messages by validating the token
         sent to the endpoint by an earlier `Subscribe`
         action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Topic.confirm_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/service_resource/#topicconfirm_subscription-method)
@@ -603,15 +606,15 @@
         Message: str,
         TargetArn: str = ...,
         PhoneNumber: str = ...,
         Subject: str = ...,
         MessageStructure: str = ...,
         MessageAttributes: Mapping[str, MessageAttributeValueTypeDef] = ...,
         MessageDeduplicationId: str = ...,
-        MessageGroupId: str = ...
+        MessageGroupId: str = ...,
     ) -> PublishResponseTypeDef:
         """
         Sends a message to an Amazon SNS topic, a text message (SMS message) directly
         to a phone number, or a message to a mobile platform endpoint (when you specify
         the
         `TargetArn`).
 
@@ -647,16 +650,16 @@
 
     async def subscribe(
         self,
         *,
         Protocol: str,
         Endpoint: str = ...,
         Attributes: Mapping[str, str] = ...,
-        ReturnSubscriptionArn: bool = ...
-    ) -> _Subscription:
+        ReturnSubscriptionArn: bool = ...,
+    ) -> "_Subscription":
         """
         Subscribes an endpoint to an Amazon SNS topic.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Topic.subscribe)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/service_resource/#topicsubscribe-method)
         """
 
@@ -675,49 +678,49 @@
     """
 
     meta: "SNSResourceMeta"
     platform_applications: ServiceResourcePlatformApplicationsCollection
     subscriptions: ServiceResourceSubscriptionsCollection
     topics: ServiceResourceTopicsCollection
 
-    async def PlatformApplication(self, arn: str) -> _PlatformApplication:
+    async def PlatformApplication(self, arn: str) -> "_PlatformApplication":
         """
         Creates a PlatformApplication resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.ServiceResource.PlatformApplication)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/service_resource/#snsserviceresourceplatformapplication-method)
         """
 
-    async def PlatformEndpoint(self, arn: str) -> _PlatformEndpoint:
+    async def PlatformEndpoint(self, arn: str) -> "_PlatformEndpoint":
         """
         Creates a PlatformEndpoint resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.ServiceResource.PlatformEndpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/service_resource/#snsserviceresourceplatformendpoint-method)
         """
 
-    async def Subscription(self, arn: str) -> _Subscription:
+    async def Subscription(self, arn: str) -> "_Subscription":
         """
         Creates a Subscription resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.ServiceResource.Subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/service_resource/#snsserviceresourcesubscription-method)
         """
 
-    async def Topic(self, arn: str) -> _Topic:
+    async def Topic(self, arn: str) -> "_Topic":
         """
         Creates a Topic resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.ServiceResource.Topic)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/service_resource/#snsserviceresourcetopic-method)
         """
 
     async def create_platform_application(
         self, *, Name: str, Platform: str, Attributes: Mapping[str, str]
-    ) -> _PlatformApplication:
+    ) -> "_PlatformApplication":
         """
         Creates a platform application object for one of the supported push
         notification services, such as APNS and GCM (Firebase Cloud Messaging), to
         which devices and mobile apps may
         register.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.ServiceResource.create_platform_application)
@@ -726,16 +729,16 @@
 
     async def create_topic(
         self,
         *,
         Name: str,
         Attributes: Mapping[str, str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        DataProtectionPolicy: str = ...
-    ) -> _Topic:
+        DataProtectionPolicy: str = ...,
+    ) -> "_Topic":
         """
         Creates a topic to which notifications can be published.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.ServiceResource.create_topic)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/service_resource/#snsserviceresourcecreate_topic-method)
         """
```

### Comparing `types-aiobotocore-sns-2.9.0/types_aiobotocore_sns/service_resource.pyi` & `types-aiobotocore-sns-2.9.1/types_aiobotocore_sns/service_resource.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -321,14 +321,15 @@
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.ServiceResource.PlatformEndpoint)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/service_resource/#platformendpoint)
     """
 
     attributes: Awaitable[Dict[str, str]]
     arn: str
+    meta: Awaitable["SNSResourceMeta"]
 
     async def delete(self) -> None:
         """
         Deletes the endpoint for a device and mobile app from Amazon SNS.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.PlatformEndpoint.delete)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/service_resource/#platformendpointdelete-method)
@@ -358,15 +359,15 @@
         Message: str,
         TopicArn: str = ...,
         PhoneNumber: str = ...,
         Subject: str = ...,
         MessageStructure: str = ...,
         MessageAttributes: Mapping[str, MessageAttributeValueTypeDef] = ...,
         MessageDeduplicationId: str = ...,
-        MessageGroupId: str = ...
+        MessageGroupId: str = ...,
     ) -> PublishResponseTypeDef:
         """
         Sends a message to an Amazon SNS topic, a text message (SMS message) directly
         to a phone number, or a message to a mobile platform endpoint (when you specify
         the
         `TargetArn`).
 
@@ -400,14 +401,15 @@
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.ServiceResource.Subscription)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/service_resource/#subscription)
     """
 
     attributes: Awaitable[Dict[str, str]]
     arn: str
+    meta: Awaitable["SNSResourceMeta"]
 
     async def delete(self) -> None:
         """
         Deletes a subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Subscription.delete)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/service_resource/#subscriptiondelete-method)
@@ -457,18 +459,19 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.ServiceResource.PlatformApplication)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/service_resource/#platformapplication)
     """
 
     attributes: Awaitable[Dict[str, str]]
     arn: str
     endpoints: PlatformApplicationEndpointsCollection
+    meta: Awaitable["SNSResourceMeta"]
 
     async def create_platform_endpoint(
         self, *, Token: str, CustomUserData: str = ..., Attributes: Mapping[str, str] = ...
-    ) -> _PlatformEndpoint:
+    ) -> "_PlatformEndpoint":
         """
         Creates an endpoint for a device and mobile app on one of the supported push
         notification services, such as GCM (Firebase Cloud Messaging) and
         APNS.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.PlatformApplication.create_platform_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/service_resource/#platformapplicationcreate_platform_endpoint-method)
@@ -529,14 +532,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.ServiceResource.Topic)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/service_resource/#topic)
     """
 
     attributes: Awaitable[Dict[str, str]]
     arn: str
     subscriptions: TopicSubscriptionsCollection
+    meta: Awaitable["SNSResourceMeta"]
 
     async def add_permission(
         self, *, Label: str, AWSAccountId: Sequence[str], ActionName: Sequence[str]
     ) -> None:
         """
         Adds a statement to a topic's access control policy, granting access for the
         specified Amazon Web Services accounts to the specified
@@ -544,15 +548,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Topic.add_permission)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/service_resource/#topicadd_permission-method)
         """
 
     async def confirm_subscription(
         self, *, Token: str, AuthenticateOnUnsubscribe: str = ...
-    ) -> _Subscription:
+    ) -> "_Subscription":
         """
         Verifies an endpoint owner's intent to receive messages by validating the token
         sent to the endpoint by an earlier `Subscribe`
         action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Topic.confirm_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/service_resource/#topicconfirm_subscription-method)
@@ -590,15 +594,15 @@
         Message: str,
         TargetArn: str = ...,
         PhoneNumber: str = ...,
         Subject: str = ...,
         MessageStructure: str = ...,
         MessageAttributes: Mapping[str, MessageAttributeValueTypeDef] = ...,
         MessageDeduplicationId: str = ...,
-        MessageGroupId: str = ...
+        MessageGroupId: str = ...,
     ) -> PublishResponseTypeDef:
         """
         Sends a message to an Amazon SNS topic, a text message (SMS message) directly
         to a phone number, or a message to a mobile platform endpoint (when you specify
         the
         `TargetArn`).
 
@@ -634,16 +638,16 @@
 
     async def subscribe(
         self,
         *,
         Protocol: str,
         Endpoint: str = ...,
         Attributes: Mapping[str, str] = ...,
-        ReturnSubscriptionArn: bool = ...
-    ) -> _Subscription:
+        ReturnSubscriptionArn: bool = ...,
+    ) -> "_Subscription":
         """
         Subscribes an endpoint to an Amazon SNS topic.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Topic.subscribe)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/service_resource/#topicsubscribe-method)
         """
 
@@ -659,49 +663,49 @@
     """
 
     meta: "SNSResourceMeta"
     platform_applications: ServiceResourcePlatformApplicationsCollection
     subscriptions: ServiceResourceSubscriptionsCollection
     topics: ServiceResourceTopicsCollection
 
-    async def PlatformApplication(self, arn: str) -> _PlatformApplication:
+    async def PlatformApplication(self, arn: str) -> "_PlatformApplication":
         """
         Creates a PlatformApplication resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.ServiceResource.PlatformApplication)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/service_resource/#snsserviceresourceplatformapplication-method)
         """
 
-    async def PlatformEndpoint(self, arn: str) -> _PlatformEndpoint:
+    async def PlatformEndpoint(self, arn: str) -> "_PlatformEndpoint":
         """
         Creates a PlatformEndpoint resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.ServiceResource.PlatformEndpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/service_resource/#snsserviceresourceplatformendpoint-method)
         """
 
-    async def Subscription(self, arn: str) -> _Subscription:
+    async def Subscription(self, arn: str) -> "_Subscription":
         """
         Creates a Subscription resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.ServiceResource.Subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/service_resource/#snsserviceresourcesubscription-method)
         """
 
-    async def Topic(self, arn: str) -> _Topic:
+    async def Topic(self, arn: str) -> "_Topic":
         """
         Creates a Topic resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.ServiceResource.Topic)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/service_resource/#snsserviceresourcetopic-method)
         """
 
     async def create_platform_application(
         self, *, Name: str, Platform: str, Attributes: Mapping[str, str]
-    ) -> _PlatformApplication:
+    ) -> "_PlatformApplication":
         """
         Creates a platform application object for one of the supported push
         notification services, such as APNS and GCM (Firebase Cloud Messaging), to
         which devices and mobile apps may
         register.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.ServiceResource.create_platform_application)
@@ -710,16 +714,16 @@
 
     async def create_topic(
         self,
         *,
         Name: str,
         Attributes: Mapping[str, str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        DataProtectionPolicy: str = ...
-    ) -> _Topic:
+        DataProtectionPolicy: str = ...,
+    ) -> "_Topic":
         """
         Creates a topic to which notifications can be published.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.ServiceResource.create_topic)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/service_resource/#snsserviceresourcecreate_topic-method)
         """
```

### Comparing `types-aiobotocore-sns-2.9.0/types_aiobotocore_sns/type_defs.py` & `types-aiobotocore-sns-2.9.1/types_aiobotocore_sns/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AddPermissionInputRequestTypeDef",
     "AddPermissionInputTopicAddPermissionTypeDef",
     "BatchResultErrorEntryTypeDef",
     "BlobTypeDef",
     "CheckIfPhoneNumberIsOptedOutInputRequestTypeDef",
     "ResponseMetadataTypeDef",
```

### Comparing `types-aiobotocore-sns-2.9.0/types_aiobotocore_sns/type_defs.pyi` & `types-aiobotocore-sns-2.9.1/types_aiobotocore_sns/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sns-2.9.0/types_aiobotocore_sns.egg-info/PKG-INFO` & `types-aiobotocore-sns-2.9.1/types_aiobotocore_sns.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sns
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.SNS 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.SNS 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/
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
 
 <a id="types-aiobotocore-sns"></a>
 
 # types-aiobotocore-sns
 
 [![PyPI - types-aiobotocore-sns](https://img.shields.io/pypi/v/types-aiobotocore-sns.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sns)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sns.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sns)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sns)](https://pepy.tech/project/types-aiobotocore-sns)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SNS 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS)
+[aiobotocore.SNS 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS)
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
 [types-aiobotocore-sns docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-sns-2.9.0/types_aiobotocore_sns.egg-info/SOURCES.txt` & `types-aiobotocore-sns-2.9.1/types_aiobotocore_sns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

