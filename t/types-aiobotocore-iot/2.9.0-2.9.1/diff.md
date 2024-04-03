# Comparing `tmp/types-aiobotocore-iot-2.9.0.tar.gz` & `tmp/types-aiobotocore-iot-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iot-2.9.0.tar", last modified: Wed Dec 13 19:59:31 2023, max compression
+gzip compressed data, was "types-aiobotocore-iot-2.9.1.tar", last modified: Thu Jan 18 01:20:54 2024, max compression
```

## Comparing `types-aiobotocore-iot-2.9.0.tar` & `types-aiobotocore-iot-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:31.381661 types-aiobotocore-iot-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:47:38.000000 types-aiobotocore-iot-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    22441 2023-12-13 19:59:31.381661 types-aiobotocore-iot-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20894 2023-12-13 19:47:38.000000 types-aiobotocore-iot-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:31.381661 types-aiobotocore-iot-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2023-12-13 19:47:38.000000 types-aiobotocore-iot-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:31.377661 types-aiobotocore-iot-2.9.0/types_aiobotocore_iot/
--rw-r--r--   0 runner    (1001) docker     (127)    14186 2023-12-13 19:47:38.000000 types-aiobotocore-iot-2.9.0/types_aiobotocore_iot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14185 2023-12-13 19:47:38.000000 types-aiobotocore-iot-2.9.0/types_aiobotocore_iot/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      905 2023-12-13 19:47:38.000000 types-aiobotocore-iot-2.9.0/types_aiobotocore_iot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)   190349 2023-12-13 19:47:39.000000 types-aiobotocore-iot-2.9.0/types_aiobotocore_iot/client.py
--rw-r--r--   0 runner    (1001) docker     (127)   190345 2023-12-13 19:47:39.000000 types-aiobotocore-iot-2.9.0/types_aiobotocore_iot/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    25673 2023-12-13 19:47:40.000000 types-aiobotocore-iot-2.9.0/types_aiobotocore_iot/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    25671 2023-12-13 19:47:40.000000 types-aiobotocore-iot-2.9.0/types_aiobotocore_iot/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    71761 2023-12-13 19:47:39.000000 types-aiobotocore-iot-2.9.0/types_aiobotocore_iot/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    71700 2023-12-13 19:47:39.000000 types-aiobotocore-iot-2.9.0/types_aiobotocore_iot/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:47:38.000000 types-aiobotocore-iot-2.9.0/types_aiobotocore_iot/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   220551 2023-12-13 19:47:46.000000 types-aiobotocore-iot-2.9.0/types_aiobotocore_iot/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   220550 2023-12-13 19:47:43.000000 types-aiobotocore-iot-2.9.0/types_aiobotocore_iot/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:47:38.000000 types-aiobotocore-iot-2.9.0/types_aiobotocore_iot/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:31.381661 types-aiobotocore-iot-2.9.0/types_aiobotocore_iot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22441 2023-12-13 19:59:31.000000 types-aiobotocore-iot-2.9.0/types_aiobotocore_iot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      737 2023-12-13 19:59:31.000000 types-aiobotocore-iot-2.9.0/types_aiobotocore_iot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:31.000000 types-aiobotocore-iot-2.9.0/types_aiobotocore_iot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:31.000000 types-aiobotocore-iot-2.9.0/types_aiobotocore_iot.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:31.000000 types-aiobotocore-iot-2.9.0/types_aiobotocore_iot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-13 19:59:31.000000 types-aiobotocore-iot-2.9.0/types_aiobotocore_iot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:54.945277 types-aiobotocore-iot-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:09:28.000000 types-aiobotocore-iot-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    22461 2024-01-18 01:20:54.945277 types-aiobotocore-iot-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20894 2024-01-18 01:09:28.000000 types-aiobotocore-iot-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:54.945277 types-aiobotocore-iot-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-01-18 01:09:28.000000 types-aiobotocore-iot-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:54.941277 types-aiobotocore-iot-2.9.1/types_aiobotocore_iot/
+-rw-r--r--   0 runner    (1001) docker     (127)    14185 2024-01-18 01:09:28.000000 types-aiobotocore-iot-2.9.1/types_aiobotocore_iot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14185 2024-01-18 01:09:28.000000 types-aiobotocore-iot-2.9.1/types_aiobotocore_iot/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-01-18 01:09:28.000000 types-aiobotocore-iot-2.9.1/types_aiobotocore_iot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   190435 2024-01-18 01:09:31.000000 types-aiobotocore-iot-2.9.1/types_aiobotocore_iot/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   190432 2024-01-18 01:09:30.000000 types-aiobotocore-iot-2.9.1/types_aiobotocore_iot/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    25671 2024-01-18 01:09:32.000000 types-aiobotocore-iot-2.9.1/types_aiobotocore_iot/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25671 2024-01-18 01:09:32.000000 types-aiobotocore-iot-2.9.1/types_aiobotocore_iot/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    71788 2024-01-18 01:09:32.000000 types-aiobotocore-iot-2.9.1/types_aiobotocore_iot/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71728 2024-01-18 01:09:31.000000 types-aiobotocore-iot-2.9.1/types_aiobotocore_iot/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:09:28.000000 types-aiobotocore-iot-2.9.1/types_aiobotocore_iot/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   220550 2024-01-18 01:09:37.000000 types-aiobotocore-iot-2.9.1/types_aiobotocore_iot/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   220550 2024-01-18 01:09:36.000000 types-aiobotocore-iot-2.9.1/types_aiobotocore_iot/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:09:28.000000 types-aiobotocore-iot-2.9.1/types_aiobotocore_iot/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:54.945277 types-aiobotocore-iot-2.9.1/types_aiobotocore_iot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22461 2024-01-18 01:20:54.000000 types-aiobotocore-iot-2.9.1/types_aiobotocore_iot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-01-18 01:20:54.000000 types-aiobotocore-iot-2.9.1/types_aiobotocore_iot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:54.000000 types-aiobotocore-iot-2.9.1/types_aiobotocore_iot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:54.000000 types-aiobotocore-iot-2.9.1/types_aiobotocore_iot.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:54.000000 types-aiobotocore-iot-2.9.1/types_aiobotocore_iot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-18 01:20:54.000000 types-aiobotocore-iot-2.9.1/types_aiobotocore_iot.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iot-2.9.0/LICENSE` & `types-aiobotocore-iot-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-iot-2.9.0/PKG-INFO` & `types-aiobotocore-iot-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iot
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.IoT 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.IoT 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/
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
 
 <a id="types-aiobotocore-iot"></a>
 
 # types-aiobotocore-iot
 
 [![PyPI - types-aiobotocore-iot](https://img.shields.io/pypi/v/types-aiobotocore-iot.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iot.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iot)](https://pepy.tech/project/types-aiobotocore-iot)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoT 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT)
+[aiobotocore.IoT 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT)
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
 [types-aiobotocore-iot docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-iot-2.9.0/README.md` & `types-aiobotocore-iot-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iot.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iot)](https://pepy.tech/project/types-aiobotocore-iot)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoT 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT)
+[aiobotocore.IoT 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT)
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
 [types-aiobotocore-iot docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-iot-2.9.0/setup.py` & `types-aiobotocore-iot-2.9.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iot",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_iot"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.IoT 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.IoT 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore iot type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_iot": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-iot-2.9.0/types_aiobotocore_iot/__init__.py` & `types-aiobotocore-iot-2.9.1/types_aiobotocore_iot/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,15 +198,14 @@
     ListTopicRulesPaginator,
     ListV2LoggingLevelsPaginator,
     ListViolationEventsPaginator,
 )
 
 Client = IoTClient
 
-
 __all__ = (
     "Client",
     "GetBehaviorModelTrainingSummariesPaginator",
     "IoTClient",
     "ListActiveViolationsPaginator",
     "ListAttachedPoliciesPaginator",
     "ListAuditFindingsPaginator",
```

### Comparing `types-aiobotocore-iot-2.9.0/types_aiobotocore_iot/__init__.pyi` & `types-aiobotocore-iot-2.9.1/types_aiobotocore_iot/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-2.9.0/types_aiobotocore_iot/__main__.py` & `types-aiobotocore-iot-2.9.1/types_aiobotocore_iot/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IoT 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.IoT 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT\nOther"
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

### Comparing `types-aiobotocore-iot-2.9.0/types_aiobotocore_iot/client.py` & `types-aiobotocore-iot-2.9.1/types_aiobotocore_iot/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -337,15 +337,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("IoTClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -419,15 +418,15 @@
 
     async def add_thing_to_billing_group(
         self,
         *,
         billingGroupName: str = ...,
         billingGroupArn: str = ...,
         thingName: str = ...,
-        thingArn: str = ...
+        thingArn: str = ...,
     ) -> Dict[str, Any]:
         """
         Adds a thing to a billing group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.add_thing_to_billing_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#add_thing_to_billing_group)
         """
@@ -435,15 +434,15 @@
     async def add_thing_to_thing_group(
         self,
         *,
         thingGroupName: str = ...,
         thingGroupArn: str = ...,
         thingName: str = ...,
         thingArn: str = ...,
-        overrideDynamicGroups: bool = ...
+        overrideDynamicGroups: bool = ...,
     ) -> Dict[str, Any]:
         """
         Adds a thing to a thing group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.add_thing_to_thing_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#add_thing_to_thing_group)
         """
@@ -552,15 +551,15 @@
     async def cancel_job_execution(
         self,
         *,
         jobId: str,
         thingName: str,
         force: bool = ...,
         expectedVersion: int = ...,
-        statusDetails: Mapping[str, str] = ...
+        statusDetails: Mapping[str, str] = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Cancels the execution of a job for a given thing.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.cancel_job_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#cancel_job_execution)
         """
@@ -593,15 +592,15 @@
         self,
         *,
         checkName: str,
         resourceIdentifier: ResourceIdentifierTypeDef,
         clientRequestToken: str,
         expirationDate: TimestampTypeDef = ...,
         suppressIndefinitely: bool = ...,
-        description: str = ...
+        description: str = ...,
     ) -> Dict[str, Any]:
         """
         Creates a Device Defender audit suppression.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_audit_suppression)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_audit_suppression)
         """
@@ -612,29 +611,29 @@
         authorizerName: str,
         authorizerFunctionArn: str,
         tokenKeyName: str = ...,
         tokenSigningPublicKeys: Mapping[str, str] = ...,
         status: AuthorizerStatusType = ...,
         tags: Sequence[TagTypeDef] = ...,
         signingDisabled: bool = ...,
-        enableCachingForHttp: bool = ...
+        enableCachingForHttp: bool = ...,
     ) -> CreateAuthorizerResponseTypeDef:
         """
         Creates an authorizer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_authorizer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_authorizer)
         """
 
     async def create_billing_group(
         self,
         *,
         billingGroupName: str,
         billingGroupProperties: BillingGroupPropertiesTypeDef = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateBillingGroupResponseTypeDef:
         """
         Creates a billing group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_billing_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_billing_group)
         """
@@ -652,15 +651,15 @@
     async def create_custom_metric(
         self,
         *,
         metricName: str,
         metricType: CustomMetricTypeType,
         clientRequestToken: str,
         displayName: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateCustomMetricResponseTypeDef:
         """
         Use this API to define a Custom Metric published by your devices to Device
         Defender.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_custom_metric)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_custom_metric)
@@ -669,15 +668,15 @@
     async def create_dimension(
         self,
         *,
         name: str,
         type: Literal["TOPIC_FILTER"],
         stringValues: Sequence[str],
         clientRequestToken: str,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDimensionResponseTypeDef:
         """
         Create a dimension that you can use to limit the scope of a metric used in a
         security profile for IoT Device
         Defender.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_dimension)
@@ -690,15 +689,15 @@
         domainConfigurationName: str,
         domainName: str = ...,
         serverCertificateArns: Sequence[str] = ...,
         validationCertificateArn: str = ...,
         authorizerConfig: AuthorizerConfigTypeDef = ...,
         serviceType: ServiceTypeType = ...,
         tags: Sequence[TagTypeDef] = ...,
-        tlsConfig: TlsConfigTypeDef = ...
+        tlsConfig: TlsConfigTypeDef = ...,
     ) -> CreateDomainConfigurationResponseTypeDef:
         """
         Creates a domain configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_domain_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_domain_configuration)
         """
@@ -707,15 +706,15 @@
         self,
         *,
         thingGroupName: str,
         queryString: str,
         thingGroupProperties: ThingGroupPropertiesTypeDef = ...,
         indexName: str = ...,
         queryVersion: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDynamicThingGroupResponseTypeDef:
         """
         Creates a dynamic thing group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_dynamic_thing_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_dynamic_thing_group)
         """
@@ -728,15 +727,15 @@
         aggregationType: AggregationTypeTypeDef,
         period: int,
         aggregationField: str,
         description: str = ...,
         queryVersion: str = ...,
         indexName: str = ...,
         unit: FleetMetricUnitType = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateFleetMetricResponseTypeDef:
         """
         Creates a fleet metric.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_fleet_metric)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_fleet_metric)
         """
@@ -756,15 +755,15 @@
         timeoutConfig: TimeoutConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         namespaceId: str = ...,
         jobTemplateArn: str = ...,
         jobExecutionsRetryConfig: JobExecutionsRetryConfigTypeDef = ...,
         documentParameters: Mapping[str, str] = ...,
         schedulingConfig: SchedulingConfigTypeDef = ...,
-        destinationPackageVersions: Sequence[str] = ...
+        destinationPackageVersions: Sequence[str] = ...,
     ) -> CreateJobResponseTypeDef:
         """
         Creates a job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_job)
         """
@@ -780,15 +779,15 @@
         presignedUrlConfig: PresignedUrlConfigTypeDef = ...,
         jobExecutionsRolloutConfig: JobExecutionsRolloutConfigTypeDef = ...,
         abortConfig: AbortConfigTypeDef = ...,
         timeoutConfig: TimeoutConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         jobExecutionsRetryConfig: JobExecutionsRetryConfigTypeDef = ...,
         maintenanceWindows: Sequence[MaintenanceWindowTypeDef] = ...,
-        destinationPackageVersions: Sequence[str] = ...
+        destinationPackageVersions: Sequence[str] = ...,
     ) -> CreateJobTemplateResponseTypeDef:
         """
         Creates a job template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_job_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_job_template)
         """
@@ -807,15 +806,15 @@
 
     async def create_mitigation_action(
         self,
         *,
         actionName: str,
         roleArn: str,
         actionParams: MitigationActionParamsTypeDef,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateMitigationActionResponseTypeDef:
         """
         Defines an action that can be applied to audit findings by using
         StartAuditMitigationActionsTask.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_mitigation_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_mitigation_action)
@@ -832,30 +831,30 @@
         protocols: Sequence[ProtocolType] = ...,
         targetSelection: TargetSelectionType = ...,
         awsJobExecutionsRolloutConfig: AwsJobExecutionsRolloutConfigTypeDef = ...,
         awsJobPresignedUrlConfig: AwsJobPresignedUrlConfigTypeDef = ...,
         awsJobAbortConfig: AwsJobAbortConfigTypeDef = ...,
         awsJobTimeoutConfig: AwsJobTimeoutConfigTypeDef = ...,
         additionalParameters: Mapping[str, str] = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateOTAUpdateResponseTypeDef:
         """
         Creates an IoT OTA update on a target group of things or groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_ota_update)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_ota_update)
         """
 
     async def create_package(
         self,
         *,
         packageName: str,
         description: str = ...,
         tags: Mapping[str, str] = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> CreatePackageResponseTypeDef:
         """
         Creates an IoT software package that can be deployed to your fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_package)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_package)
         """
@@ -864,15 +863,15 @@
         self,
         *,
         packageName: str,
         versionName: str,
         description: str = ...,
         attributes: Mapping[str, str] = ...,
         tags: Mapping[str, str] = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> CreatePackageVersionResponseTypeDef:
         """
         Creates a new version for an existing IoT software package.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_package_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_package_version)
         """
@@ -913,15 +912,15 @@
         templateName: str,
         templateBody: str,
         provisioningRoleArn: str,
         description: str = ...,
         enabled: bool = ...,
         preProvisioningHook: ProvisioningHookTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
-        type: TemplateTypeType = ...
+        type: TemplateTypeType = ...,
     ) -> CreateProvisioningTemplateResponseTypeDef:
         """
         Creates a provisioning template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_provisioning_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_provisioning_template)
         """
@@ -938,15 +937,15 @@
 
     async def create_role_alias(
         self,
         *,
         roleAlias: str,
         roleArn: str,
         credentialDurationSeconds: int = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateRoleAliasResponseTypeDef:
         """
         Creates a role alias.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_role_alias)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_role_alias)
         """
@@ -955,15 +954,15 @@
         self,
         *,
         frequency: AuditFrequencyType,
         targetCheckNames: Sequence[str],
         scheduledAuditName: str,
         dayOfMonth: str = ...,
         dayOfWeek: DayOfWeekType = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateScheduledAuditResponseTypeDef:
         """
         Creates a scheduled audit that is run at a specified time interval.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_scheduled_audit)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_scheduled_audit)
         """
@@ -974,15 +973,15 @@
         securityProfileName: str,
         securityProfileDescription: str = ...,
         behaviors: Sequence[BehaviorTypeDef] = ...,
         alertTargets: Mapping[Literal["SNS"], AlertTargetTypeDef] = ...,
         additionalMetricsToRetain: Sequence[str] = ...,
         additionalMetricsToRetainV2: Sequence[MetricToRetainTypeDef] = ...,
         tags: Sequence[TagTypeDef] = ...,
-        metricsExportConfig: MetricsExportConfigTypeDef = ...
+        metricsExportConfig: MetricsExportConfigTypeDef = ...,
     ) -> CreateSecurityProfileResponseTypeDef:
         """
         Creates a Device Defender security profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_security_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_security_profile)
         """
@@ -990,59 +989,59 @@
     async def create_stream(
         self,
         *,
         streamId: str,
         files: Sequence[StreamFileTypeDef],
         roleArn: str,
         description: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateStreamResponseTypeDef:
         """
         Creates a stream for delivering one or more large files in chunks over MQTT.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_stream)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_stream)
         """
 
     async def create_thing(
         self,
         *,
         thingName: str,
         thingTypeName: str = ...,
         attributePayload: AttributePayloadTypeDef = ...,
-        billingGroupName: str = ...
+        billingGroupName: str = ...,
     ) -> CreateThingResponseTypeDef:
         """
         Creates a thing record in the registry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_thing)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_thing)
         """
 
     async def create_thing_group(
         self,
         *,
         thingGroupName: str,
         parentGroupName: str = ...,
         thingGroupProperties: ThingGroupPropertiesTypeDef = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateThingGroupResponseTypeDef:
         """
         Create a thing group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_thing_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_thing_group)
         """
 
     async def create_thing_type(
         self,
         *,
         thingTypeName: str,
         thingTypeProperties: ThingTypePropertiesTypeDef = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateThingTypeResponseTypeDef:
         """
         Creates a new thing type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_thing_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_thing_type)
         """
@@ -1180,15 +1179,15 @@
     async def delete_job_execution(
         self,
         *,
         jobId: str,
         thingName: str,
         executionNumber: int,
         force: bool = ...,
-        namespaceId: str = ...
+        namespaceId: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a job execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.delete_job_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#delete_job_execution)
         """
@@ -1773,30 +1772,30 @@
     async def get_buckets_aggregation(
         self,
         *,
         queryString: str,
         aggregationField: str,
         bucketsAggregationType: BucketsAggregationTypeTypeDef,
         indexName: str = ...,
-        queryVersion: str = ...
+        queryVersion: str = ...,
     ) -> GetBucketsAggregationResponseTypeDef:
         """
         Aggregates on indexed data with search queries pertaining to particular fields.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.get_buckets_aggregation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#get_buckets_aggregation)
         """
 
     async def get_cardinality(
         self,
         *,
         queryString: str,
         indexName: str = ...,
         aggregationField: str = ...,
-        queryVersion: str = ...
+        queryVersion: str = ...,
     ) -> GetCardinalityResponseTypeDef:
         """
         Returns the approximate count of unique values that match the query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.get_cardinality)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#get_cardinality)
         """
@@ -1874,15 +1873,15 @@
     async def get_percentiles(
         self,
         *,
         queryString: str,
         indexName: str = ...,
         aggregationField: str = ...,
         queryVersion: str = ...,
-        percents: Sequence[float] = ...
+        percents: Sequence[float] = ...,
     ) -> GetPercentilesResponseTypeDef:
         """
         Groups the aggregated values that match the query into percentile groupings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.get_percentiles)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#get_percentiles)
         """
@@ -1917,15 +1916,15 @@
 
     async def get_statistics(
         self,
         *,
         queryString: str,
         indexName: str = ...,
         aggregationField: str = ...,
-        queryVersion: str = ...
+        queryVersion: str = ...,
     ) -> GetStatisticsResponseTypeDef:
         """
         Returns the count, average, sum, minimum, maximum, sum of squares, variance,
         and standard deviation for the specified aggregated
         field.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.get_statistics)
@@ -1963,15 +1962,15 @@
         *,
         thingName: str = ...,
         securityProfileName: str = ...,
         behaviorCriteriaType: BehaviorCriteriaTypeType = ...,
         listSuppressedAlerts: bool = ...,
         verificationState: VerificationStateType = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListActiveViolationsResponseTypeDef:
         """
         Lists the active violations for a given Device Defender security profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_active_violations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_active_violations)
         """
@@ -1992,15 +1991,15 @@
         taskId: str = ...,
         checkName: str = ...,
         resourceIdentifier: ResourceIdentifierTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         startTime: TimestampTypeDef = ...,
         endTime: TimestampTypeDef = ...,
-        listSuppressedFindings: bool = ...
+        listSuppressedFindings: bool = ...,
     ) -> ListAuditFindingsResponseTypeDef:
         """
         Lists the findings (results) of a Device Defender audit or of the audits
         performed during a specified time
         period.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_audit_findings)
@@ -2010,15 +2009,15 @@
     async def list_audit_mitigation_actions_executions(
         self,
         *,
         taskId: str,
         findingId: str,
         actionStatus: AuditMitigationActionsExecutionStatusType = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListAuditMitigationActionsExecutionsResponseTypeDef:
         """
         Gets the status of audit mitigation action tasks that were executed.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_audit_mitigation_actions_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_audit_mitigation_actions_executions)
         """
@@ -2028,15 +2027,15 @@
         *,
         startTime: TimestampTypeDef,
         endTime: TimestampTypeDef,
         auditTaskId: str = ...,
         findingId: str = ...,
         taskStatus: AuditMitigationActionsTaskStatusType = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListAuditMitigationActionsTasksResponseTypeDef:
         """
         Gets a list of audit mitigation action tasks that match the specified filters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_audit_mitigation_actions_tasks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_audit_mitigation_actions_tasks)
         """
@@ -2044,15 +2043,15 @@
     async def list_audit_suppressions(
         self,
         *,
         checkName: str = ...,
         resourceIdentifier: ResourceIdentifierTypeDef = ...,
         ascendingOrder: bool = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListAuditSuppressionsResponseTypeDef:
         """
         Lists your Device Defender audit listings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_audit_suppressions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_audit_suppressions)
         """
@@ -2061,15 +2060,15 @@
         self,
         *,
         startTime: TimestampTypeDef,
         endTime: TimestampTypeDef,
         taskType: AuditTaskTypeType = ...,
         taskStatus: AuditTaskStatusType = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListAuditTasksResponseTypeDef:
         """
         Lists the Device Defender audits that have been performed during a given time
         period.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_audit_tasks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_audit_tasks)
@@ -2077,15 +2076,15 @@
 
     async def list_authorizers(
         self,
         *,
         pageSize: int = ...,
         marker: str = ...,
         ascendingOrder: bool = ...,
-        status: AuthorizerStatusType = ...
+        status: AuthorizerStatusType = ...,
     ) -> ListAuthorizersResponseTypeDef:
         """
         Lists the authorizers registered in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_authorizers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_authorizers)
         """
@@ -2102,15 +2101,15 @@
 
     async def list_ca_certificates(
         self,
         *,
         pageSize: int = ...,
         marker: str = ...,
         ascendingOrder: bool = ...,
-        templateName: str = ...
+        templateName: str = ...,
     ) -> ListCACertificatesResponseTypeDef:
         """
         Lists the CA certificates registered for your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_ca_certificates)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_ca_certificates)
         """
@@ -2127,15 +2126,15 @@
 
     async def list_certificates_by_ca(
         self,
         *,
         caCertificateId: str,
         pageSize: int = ...,
         marker: str = ...,
-        ascendingOrder: bool = ...
+        ascendingOrder: bool = ...,
     ) -> ListCertificatesByCAResponseTypeDef:
         """
         List the device certificates signed by the specified CA certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_certificates_by_ca)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_certificates_by_ca)
         """
@@ -2155,15 +2154,15 @@
         *,
         taskId: str = ...,
         violationId: str = ...,
         thingName: str = ...,
         startTime: TimestampTypeDef = ...,
         endTime: TimestampTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListDetectMitigationActionsExecutionsResponseTypeDef:
         """
         Lists mitigation actions executions for a Device Defender ML Detect Security
         Profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_detect_mitigation_actions_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_detect_mitigation_actions_executions)
@@ -2171,15 +2170,15 @@
 
     async def list_detect_mitigation_actions_tasks(
         self,
         *,
         startTime: TimestampTypeDef,
         endTime: TimestampTypeDef,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListDetectMitigationActionsTasksResponseTypeDef:
         """
         List of Device Defender ML Detect mitigation actions tasks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_detect_mitigation_actions_tasks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_detect_mitigation_actions_tasks)
         """
@@ -2227,15 +2226,15 @@
 
     async def list_job_executions_for_job(
         self,
         *,
         jobId: str,
         status: JobExecutionStatusType = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListJobExecutionsForJobResponseTypeDef:
         """
         Lists the job executions for a job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_job_executions_for_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_job_executions_for_job)
         """
@@ -2244,15 +2243,15 @@
         self,
         *,
         thingName: str,
         status: JobExecutionStatusType = ...,
         namespaceId: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        jobId: str = ...
+        jobId: str = ...,
     ) -> ListJobExecutionsForThingResponseTypeDef:
         """
         Lists the job executions for the specified thing.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_job_executions_for_thing)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_job_executions_for_thing)
         """
@@ -2272,15 +2271,15 @@
         *,
         status: JobStatusType = ...,
         targetSelection: TargetSelectionType = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         thingGroupName: str = ...,
         thingGroupId: str = ...,
-        namespaceId: str = ...
+        namespaceId: str = ...,
     ) -> ListJobsResponseTypeDef:
         """
         Lists jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_jobs)
         """
@@ -2301,15 +2300,15 @@
         thingName: str,
         metricName: str,
         startTime: TimestampTypeDef,
         endTime: TimestampTypeDef,
         dimensionName: str = ...,
         dimensionValueOperator: DimensionValueOperatorType = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListMetricValuesResponseTypeDef:
         """
         Lists the values reported for an IoT Device Defender metric (device-side
         metric, cloud-side metric, or custom metric) by the given thing during the
         specified time
         period.
 
@@ -2318,29 +2317,29 @@
         """
 
     async def list_mitigation_actions(
         self,
         *,
         actionType: MitigationActionTypeType = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListMitigationActionsResponseTypeDef:
         """
         Gets a list of all mitigation actions that match the specified filter criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_mitigation_actions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_mitigation_actions)
         """
 
     async def list_ota_updates(
         self,
         *,
         maxResults: int = ...,
         nextToken: str = ...,
-        otaUpdateStatus: OTAUpdateStatusType = ...
+        otaUpdateStatus: OTAUpdateStatusType = ...,
     ) -> ListOTAUpdatesResponseTypeDef:
         """
         Lists OTA updates.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_ota_updates)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_ota_updates)
         """
@@ -2357,15 +2356,15 @@
 
     async def list_package_versions(
         self,
         *,
         packageName: str,
         status: PackageVersionStatusType = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListPackageVersionsResponseTypeDef:
         """
         Lists the software package versions associated to the account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_package_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_package_versions)
         """
@@ -2480,30 +2479,30 @@
 
     async def list_security_profiles(
         self,
         *,
         nextToken: str = ...,
         maxResults: int = ...,
         dimensionName: str = ...,
-        metricName: str = ...
+        metricName: str = ...,
     ) -> ListSecurityProfilesResponseTypeDef:
         """
         Lists the Device Defender security profiles you've created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_security_profiles)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_security_profiles)
         """
 
     async def list_security_profiles_for_target(
         self,
         *,
         securityProfileTargetArn: str,
         nextToken: str = ...,
         maxResults: int = ...,
-        recursive: bool = ...
+        recursive: bool = ...,
     ) -> ListSecurityProfilesForTargetResponseTypeDef:
         """
         Lists the Device Defender security profiles attached to a target (thing group).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_security_profiles_for_target)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_security_profiles_for_target)
         """
@@ -2553,15 +2552,15 @@
     async def list_thing_groups(
         self,
         *,
         nextToken: str = ...,
         maxResults: int = ...,
         parentGroup: str = ...,
         namePrefixFilter: str = ...,
-        recursive: bool = ...
+        recursive: bool = ...,
     ) -> ListThingGroupsResponseTypeDef:
         """
         List the thing groups in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_thing_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_thing_groups)
         """
@@ -2588,15 +2587,15 @@
 
     async def list_thing_registration_task_reports(
         self,
         *,
         taskId: str,
         reportType: ReportTypeType,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListThingRegistrationTaskReportsResponseTypeDef:
         """
         Information about the thing registration tasks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_thing_registration_task_reports)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_thing_registration_task_reports)
         """
@@ -2625,15 +2624,15 @@
         self,
         *,
         nextToken: str = ...,
         maxResults: int = ...,
         attributeName: str = ...,
         attributeValue: str = ...,
         thingTypeName: str = ...,
-        usePrefixAttributeValue: bool = ...
+        usePrefixAttributeValue: bool = ...,
     ) -> ListThingsResponseTypeDef:
         """
         Lists your things.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_things)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_things)
         """
@@ -2650,15 +2649,15 @@
 
     async def list_things_in_thing_group(
         self,
         *,
         thingGroupName: str,
         recursive: bool = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListThingsInThingGroupResponseTypeDef:
         """
         Lists the things in the specified group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_things_in_thing_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_things_in_thing_group)
         """
@@ -2675,15 +2674,15 @@
 
     async def list_topic_rules(
         self,
         *,
         topic: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        ruleDisabled: bool = ...
+        ruleDisabled: bool = ...,
     ) -> ListTopicRulesResponseTypeDef:
         """
         Lists the rules for the specific topic.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_topic_rules)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_topic_rules)
         """
@@ -2705,15 +2704,15 @@
         endTime: TimestampTypeDef,
         thingName: str = ...,
         securityProfileName: str = ...,
         behaviorCriteriaType: BehaviorCriteriaTypeType = ...,
         listSuppressedAlerts: bool = ...,
         verificationState: VerificationStateType = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListViolationEventsResponseTypeDef:
         """
         Lists the Device Defender security profile violations discovered during the
         given time
         period.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_violation_events)
@@ -2721,15 +2720,15 @@
         """
 
     async def put_verification_state_on_violation(
         self,
         *,
         violationId: str,
         verificationState: VerificationStateType,
-        verificationStateDescription: str = ...
+        verificationStateDescription: str = ...,
     ) -> Dict[str, Any]:
         """
         Set a verification state and provide a description of that verification state
         on a violation (detect
         alarm).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.put_verification_state_on_violation)
@@ -2741,30 +2740,30 @@
         *,
         caCertificate: str,
         verificationCertificate: str = ...,
         setAsActive: bool = ...,
         allowAutoRegistration: bool = ...,
         registrationConfig: RegistrationConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
-        certificateMode: CertificateModeType = ...
+        certificateMode: CertificateModeType = ...,
     ) -> RegisterCACertificateResponseTypeDef:
         """
         Registers a CA certificate with Amazon Web Services IoT Core.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.register_ca_certificate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#register_ca_certificate)
         """
 
     async def register_certificate(
         self,
         *,
         certificatePem: str,
         caCertificatePem: str = ...,
         setAsActive: bool = ...,
-        status: CertificateStatusType = ...
+        status: CertificateStatusType = ...,
     ) -> RegisterCertificateResponseTypeDef:
         """
         Registers a device certificate with IoT in the same [certificate
         mode](https://docs.aws.amazon.com/iot/latest/apireference/API_CertificateDescription.html#iot-Type-CertificateDescription-certificateMode)
         as the signing
         CA.
 
@@ -2804,30 +2803,30 @@
 
     async def remove_thing_from_billing_group(
         self,
         *,
         billingGroupName: str = ...,
         billingGroupArn: str = ...,
         thingName: str = ...,
-        thingArn: str = ...
+        thingArn: str = ...,
     ) -> Dict[str, Any]:
         """
         Removes the given thing from the billing group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.remove_thing_from_billing_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#remove_thing_from_billing_group)
         """
 
     async def remove_thing_from_thing_group(
         self,
         *,
         thingGroupName: str = ...,
         thingGroupArn: str = ...,
         thingName: str = ...,
-        thingArn: str = ...
+        thingArn: str = ...,
     ) -> Dict[str, Any]:
         """
         Remove the specified thing from the specified group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.remove_thing_from_thing_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#remove_thing_from_thing_group)
         """
@@ -2845,15 +2844,15 @@
     async def search_index(
         self,
         *,
         queryString: str,
         indexName: str = ...,
         nextToken: str = ...,
         maxResults: int = ...,
-        queryVersion: str = ...
+        queryVersion: str = ...,
     ) -> SearchIndexResponseTypeDef:
         """
         The query search index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.search_index)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#search_index)
         """
@@ -2912,15 +2911,15 @@
 
     async def start_audit_mitigation_actions_task(
         self,
         *,
         taskId: str,
         target: AuditMitigationActionsTaskTargetTypeDef,
         auditCheckToActionsMapping: Mapping[str, Sequence[str]],
-        clientRequestToken: str
+        clientRequestToken: str,
     ) -> StartAuditMitigationActionsTaskResponseTypeDef:
         """
         Starts a task that applies a set of mitigation actions to the specified target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.start_audit_mitigation_actions_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#start_audit_mitigation_actions_task)
         """
@@ -2930,15 +2929,15 @@
         *,
         taskId: str,
         target: DetectMitigationActionsTaskTargetTypeDef,
         actions: Sequence[str],
         clientRequestToken: str,
         violationEventOccurrenceRange: ViolationEventOccurrenceRangeTypeDef = ...,
         includeOnlyActiveViolations: bool = ...,
-        includeSuppressedAlerts: bool = ...
+        includeSuppressedAlerts: bool = ...,
     ) -> StartDetectMitigationActionsTaskResponseTypeDef:
         """
         Starts a Device Defender ML Detect mitigation actions task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.start_detect_mitigation_actions_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#start_detect_mitigation_actions_task)
         """
@@ -2983,15 +2982,15 @@
         self,
         *,
         authInfos: Sequence[AuthInfoTypeDef],
         principal: str = ...,
         cognitoIdentityPoolId: str = ...,
         clientId: str = ...,
         policyNamesToAdd: Sequence[str] = ...,
-        policyNamesToSkip: Sequence[str] = ...
+        policyNamesToSkip: Sequence[str] = ...,
     ) -> TestAuthorizationResponseTypeDef:
         """
         Tests if a specified principal is authorized to perform an IoT action on a
         specified
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.test_authorization)
@@ -3002,15 +3001,15 @@
         self,
         *,
         authorizerName: str,
         token: str = ...,
         tokenSignature: str = ...,
         httpContext: HttpContextTypeDef = ...,
         mqttContext: MqttContextTypeDef = ...,
-        tlsContext: TlsContextTypeDef = ...
+        tlsContext: TlsContextTypeDef = ...,
     ) -> TestInvokeAuthorizerResponseTypeDef:
         """
         Tests a custom authorization behavior by invoking a specified custom authorizer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.test_invoke_authorizer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#test_invoke_authorizer)
         """
@@ -3037,15 +3036,15 @@
     async def update_account_audit_configuration(
         self,
         *,
         roleArn: str = ...,
         auditNotificationTargetConfigurations: Mapping[
             Literal["SNS"], AuditNotificationTargetTypeDef
         ] = ...,
-        auditCheckConfigurations: Mapping[str, AuditCheckConfigurationTypeDef] = ...
+        auditCheckConfigurations: Mapping[str, AuditCheckConfigurationTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Configures or reconfigures the Device Defender audit settings for this account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_account_audit_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_account_audit_configuration)
         """
@@ -3053,15 +3052,15 @@
     async def update_audit_suppression(
         self,
         *,
         checkName: str,
         resourceIdentifier: ResourceIdentifierTypeDef,
         expirationDate: TimestampTypeDef = ...,
         suppressIndefinitely: bool = ...,
-        description: str = ...
+        description: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates a Device Defender audit suppression.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_audit_suppression)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_audit_suppression)
         """
@@ -3070,29 +3069,29 @@
         self,
         *,
         authorizerName: str,
         authorizerFunctionArn: str = ...,
         tokenKeyName: str = ...,
         tokenSigningPublicKeys: Mapping[str, str] = ...,
         status: AuthorizerStatusType = ...,
-        enableCachingForHttp: bool = ...
+        enableCachingForHttp: bool = ...,
     ) -> UpdateAuthorizerResponseTypeDef:
         """
         Updates an authorizer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_authorizer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_authorizer)
         """
 
     async def update_billing_group(
         self,
         *,
         billingGroupName: str,
         billingGroupProperties: BillingGroupPropertiesTypeDef,
-        expectedVersion: int = ...
+        expectedVersion: int = ...,
     ) -> UpdateBillingGroupResponseTypeDef:
         """
         Updates information about the billing group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_billing_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_billing_group)
         """
@@ -3100,15 +3099,15 @@
     async def update_ca_certificate(
         self,
         *,
         certificateId: str,
         newStatus: CACertificateStatusType = ...,
         newAutoRegistrationStatus: AutoRegistrationStatusType = ...,
         registrationConfig: RegistrationConfigTypeDef = ...,
-        removeAutoRegistration: bool = ...
+        removeAutoRegistration: bool = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a registered CA certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_ca_certificate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_ca_certificate)
         """
@@ -3146,15 +3145,15 @@
     async def update_domain_configuration(
         self,
         *,
         domainConfigurationName: str,
         authorizerConfig: AuthorizerConfigTypeDef = ...,
         domainConfigurationStatus: DomainConfigurationStatusType = ...,
         removeAuthorizerConfig: bool = ...,
-        tlsConfig: TlsConfigTypeDef = ...
+        tlsConfig: TlsConfigTypeDef = ...,
     ) -> UpdateDomainConfigurationResponseTypeDef:
         """
         Updates values stored in the domain configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_domain_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_domain_configuration)
         """
@@ -3163,15 +3162,15 @@
         self,
         *,
         thingGroupName: str,
         thingGroupProperties: ThingGroupPropertiesTypeDef,
         expectedVersion: int = ...,
         indexName: str = ...,
         queryString: str = ...,
-        queryVersion: str = ...
+        queryVersion: str = ...,
     ) -> UpdateDynamicThingGroupResponseTypeDef:
         """
         Updates a dynamic thing group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_dynamic_thing_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_dynamic_thing_group)
         """
@@ -3194,28 +3193,28 @@
         queryString: str = ...,
         aggregationType: AggregationTypeTypeDef = ...,
         period: int = ...,
         aggregationField: str = ...,
         description: str = ...,
         queryVersion: str = ...,
         unit: FleetMetricUnitType = ...,
-        expectedVersion: int = ...
+        expectedVersion: int = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates the data for a fleet metric.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_fleet_metric)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_fleet_metric)
         """
 
     async def update_indexing_configuration(
         self,
         *,
         thingIndexingConfiguration: ThingIndexingConfigurationTypeDef = ...,
-        thingGroupIndexingConfiguration: ThingGroupIndexingConfigurationTypeDef = ...
+        thingGroupIndexingConfiguration: ThingGroupIndexingConfigurationTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates the search configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_indexing_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_indexing_configuration)
         """
@@ -3226,29 +3225,29 @@
         jobId: str,
         description: str = ...,
         presignedUrlConfig: PresignedUrlConfigTypeDef = ...,
         jobExecutionsRolloutConfig: JobExecutionsRolloutConfigTypeDef = ...,
         abortConfig: AbortConfigTypeDef = ...,
         timeoutConfig: TimeoutConfigTypeDef = ...,
         namespaceId: str = ...,
-        jobExecutionsRetryConfig: JobExecutionsRetryConfigTypeDef = ...
+        jobExecutionsRetryConfig: JobExecutionsRetryConfigTypeDef = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates supported fields of the specified job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_job)
         """
 
     async def update_mitigation_action(
         self,
         *,
         actionName: str,
         roleArn: str = ...,
-        actionParams: MitigationActionParamsTypeDef = ...
+        actionParams: MitigationActionParamsTypeDef = ...,
     ) -> UpdateMitigationActionResponseTypeDef:
         """
         Updates the definition for the specified mitigation action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_mitigation_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_mitigation_action)
         """
@@ -3256,28 +3255,28 @@
     async def update_package(
         self,
         *,
         packageName: str,
         description: str = ...,
         defaultVersionName: str = ...,
         unsetDefaultVersion: bool = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates the supported fields for a specific software package.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_package)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_package)
         """
 
     async def update_package_configuration(
         self,
         *,
         versionUpdateByJobsConfig: VersionUpdateByJobsConfigTypeDef = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates the software package configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_package_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_package_configuration)
         """
@@ -3286,15 +3285,15 @@
         self,
         *,
         packageName: str,
         versionName: str,
         description: str = ...,
         attributes: Mapping[str, str] = ...,
         action: PackageVersionActionType = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates the supported fields for a specific package version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_package_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_package_version)
         """
@@ -3304,15 +3303,15 @@
         *,
         templateName: str,
         description: str = ...,
         enabled: bool = ...,
         defaultVersionId: int = ...,
         provisioningRoleArn: str = ...,
         preProvisioningHook: ProvisioningHookTypeDef = ...,
-        removePreProvisioningHook: bool = ...
+        removePreProvisioningHook: bool = ...,
     ) -> Dict[str, Any]:
         """
         Updates a provisioning template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_provisioning_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_provisioning_template)
         """
@@ -3330,15 +3329,15 @@
     async def update_scheduled_audit(
         self,
         *,
         scheduledAuditName: str,
         frequency: AuditFrequencyType = ...,
         dayOfMonth: str = ...,
         dayOfWeek: DayOfWeekType = ...,
-        targetCheckNames: Sequence[str] = ...
+        targetCheckNames: Sequence[str] = ...,
     ) -> UpdateScheduledAuditResponseTypeDef:
         """
         Updates a scheduled audit, including which checks are performed and how often
         the audit takes
         place.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_scheduled_audit)
@@ -3355,30 +3354,30 @@
         additionalMetricsToRetain: Sequence[str] = ...,
         additionalMetricsToRetainV2: Sequence[MetricToRetainTypeDef] = ...,
         deleteBehaviors: bool = ...,
         deleteAlertTargets: bool = ...,
         deleteAdditionalMetricsToRetain: bool = ...,
         expectedVersion: int = ...,
         metricsExportConfig: MetricsExportConfigTypeDef = ...,
-        deleteMetricsExportConfig: bool = ...
+        deleteMetricsExportConfig: bool = ...,
     ) -> UpdateSecurityProfileResponseTypeDef:
         """
         Updates a Device Defender security profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_security_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_security_profile)
         """
 
     async def update_stream(
         self,
         *,
         streamId: str,
         description: str = ...,
         files: Sequence[StreamFileTypeDef] = ...,
-        roleArn: str = ...
+        roleArn: str = ...,
     ) -> UpdateStreamResponseTypeDef:
         """
         Updates an existing stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_stream)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_stream)
         """
@@ -3386,44 +3385,44 @@
     async def update_thing(
         self,
         *,
         thingName: str,
         thingTypeName: str = ...,
         attributePayload: AttributePayloadTypeDef = ...,
         expectedVersion: int = ...,
-        removeThingType: bool = ...
+        removeThingType: bool = ...,
     ) -> Dict[str, Any]:
         """
         Updates the data for a thing.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_thing)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_thing)
         """
 
     async def update_thing_group(
         self,
         *,
         thingGroupName: str,
         thingGroupProperties: ThingGroupPropertiesTypeDef,
-        expectedVersion: int = ...
+        expectedVersion: int = ...,
     ) -> UpdateThingGroupResponseTypeDef:
         """
         Update a thing group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_thing_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_thing_group)
         """
 
     async def update_thing_groups_for_thing(
         self,
         *,
         thingName: str = ...,
         thingGroupsToAdd: Sequence[str] = ...,
         thingGroupsToRemove: Sequence[str] = ...,
-        overrideDynamicGroups: bool = ...
+        overrideDynamicGroups: bool = ...,
     ) -> Dict[str, Any]:
         """
         Updates the groups to which the thing belongs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_thing_groups_for_thing)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_thing_groups_for_thing)
         """
```

### Comparing `types-aiobotocore-iot-2.9.0/types_aiobotocore_iot/client.pyi` & `types-aiobotocore-iot-2.9.1/types_aiobotocore_iot/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -415,15 +415,15 @@
 
     async def add_thing_to_billing_group(
         self,
         *,
         billingGroupName: str = ...,
         billingGroupArn: str = ...,
         thingName: str = ...,
-        thingArn: str = ...
+        thingArn: str = ...,
     ) -> Dict[str, Any]:
         """
         Adds a thing to a billing group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.add_thing_to_billing_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#add_thing_to_billing_group)
         """
@@ -431,15 +431,15 @@
     async def add_thing_to_thing_group(
         self,
         *,
         thingGroupName: str = ...,
         thingGroupArn: str = ...,
         thingName: str = ...,
         thingArn: str = ...,
-        overrideDynamicGroups: bool = ...
+        overrideDynamicGroups: bool = ...,
     ) -> Dict[str, Any]:
         """
         Adds a thing to a thing group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.add_thing_to_thing_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#add_thing_to_thing_group)
         """
@@ -548,15 +548,15 @@
     async def cancel_job_execution(
         self,
         *,
         jobId: str,
         thingName: str,
         force: bool = ...,
         expectedVersion: int = ...,
-        statusDetails: Mapping[str, str] = ...
+        statusDetails: Mapping[str, str] = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Cancels the execution of a job for a given thing.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.cancel_job_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#cancel_job_execution)
         """
@@ -589,15 +589,15 @@
         self,
         *,
         checkName: str,
         resourceIdentifier: ResourceIdentifierTypeDef,
         clientRequestToken: str,
         expirationDate: TimestampTypeDef = ...,
         suppressIndefinitely: bool = ...,
-        description: str = ...
+        description: str = ...,
     ) -> Dict[str, Any]:
         """
         Creates a Device Defender audit suppression.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_audit_suppression)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_audit_suppression)
         """
@@ -608,29 +608,29 @@
         authorizerName: str,
         authorizerFunctionArn: str,
         tokenKeyName: str = ...,
         tokenSigningPublicKeys: Mapping[str, str] = ...,
         status: AuthorizerStatusType = ...,
         tags: Sequence[TagTypeDef] = ...,
         signingDisabled: bool = ...,
-        enableCachingForHttp: bool = ...
+        enableCachingForHttp: bool = ...,
     ) -> CreateAuthorizerResponseTypeDef:
         """
         Creates an authorizer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_authorizer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_authorizer)
         """
 
     async def create_billing_group(
         self,
         *,
         billingGroupName: str,
         billingGroupProperties: BillingGroupPropertiesTypeDef = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateBillingGroupResponseTypeDef:
         """
         Creates a billing group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_billing_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_billing_group)
         """
@@ -648,15 +648,15 @@
     async def create_custom_metric(
         self,
         *,
         metricName: str,
         metricType: CustomMetricTypeType,
         clientRequestToken: str,
         displayName: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateCustomMetricResponseTypeDef:
         """
         Use this API to define a Custom Metric published by your devices to Device
         Defender.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_custom_metric)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_custom_metric)
@@ -665,15 +665,15 @@
     async def create_dimension(
         self,
         *,
         name: str,
         type: Literal["TOPIC_FILTER"],
         stringValues: Sequence[str],
         clientRequestToken: str,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDimensionResponseTypeDef:
         """
         Create a dimension that you can use to limit the scope of a metric used in a
         security profile for IoT Device
         Defender.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_dimension)
@@ -686,15 +686,15 @@
         domainConfigurationName: str,
         domainName: str = ...,
         serverCertificateArns: Sequence[str] = ...,
         validationCertificateArn: str = ...,
         authorizerConfig: AuthorizerConfigTypeDef = ...,
         serviceType: ServiceTypeType = ...,
         tags: Sequence[TagTypeDef] = ...,
-        tlsConfig: TlsConfigTypeDef = ...
+        tlsConfig: TlsConfigTypeDef = ...,
     ) -> CreateDomainConfigurationResponseTypeDef:
         """
         Creates a domain configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_domain_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_domain_configuration)
         """
@@ -703,15 +703,15 @@
         self,
         *,
         thingGroupName: str,
         queryString: str,
         thingGroupProperties: ThingGroupPropertiesTypeDef = ...,
         indexName: str = ...,
         queryVersion: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDynamicThingGroupResponseTypeDef:
         """
         Creates a dynamic thing group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_dynamic_thing_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_dynamic_thing_group)
         """
@@ -724,15 +724,15 @@
         aggregationType: AggregationTypeTypeDef,
         period: int,
         aggregationField: str,
         description: str = ...,
         queryVersion: str = ...,
         indexName: str = ...,
         unit: FleetMetricUnitType = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateFleetMetricResponseTypeDef:
         """
         Creates a fleet metric.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_fleet_metric)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_fleet_metric)
         """
@@ -752,15 +752,15 @@
         timeoutConfig: TimeoutConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         namespaceId: str = ...,
         jobTemplateArn: str = ...,
         jobExecutionsRetryConfig: JobExecutionsRetryConfigTypeDef = ...,
         documentParameters: Mapping[str, str] = ...,
         schedulingConfig: SchedulingConfigTypeDef = ...,
-        destinationPackageVersions: Sequence[str] = ...
+        destinationPackageVersions: Sequence[str] = ...,
     ) -> CreateJobResponseTypeDef:
         """
         Creates a job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_job)
         """
@@ -776,15 +776,15 @@
         presignedUrlConfig: PresignedUrlConfigTypeDef = ...,
         jobExecutionsRolloutConfig: JobExecutionsRolloutConfigTypeDef = ...,
         abortConfig: AbortConfigTypeDef = ...,
         timeoutConfig: TimeoutConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         jobExecutionsRetryConfig: JobExecutionsRetryConfigTypeDef = ...,
         maintenanceWindows: Sequence[MaintenanceWindowTypeDef] = ...,
-        destinationPackageVersions: Sequence[str] = ...
+        destinationPackageVersions: Sequence[str] = ...,
     ) -> CreateJobTemplateResponseTypeDef:
         """
         Creates a job template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_job_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_job_template)
         """
@@ -803,15 +803,15 @@
 
     async def create_mitigation_action(
         self,
         *,
         actionName: str,
         roleArn: str,
         actionParams: MitigationActionParamsTypeDef,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateMitigationActionResponseTypeDef:
         """
         Defines an action that can be applied to audit findings by using
         StartAuditMitigationActionsTask.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_mitigation_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_mitigation_action)
@@ -828,30 +828,30 @@
         protocols: Sequence[ProtocolType] = ...,
         targetSelection: TargetSelectionType = ...,
         awsJobExecutionsRolloutConfig: AwsJobExecutionsRolloutConfigTypeDef = ...,
         awsJobPresignedUrlConfig: AwsJobPresignedUrlConfigTypeDef = ...,
         awsJobAbortConfig: AwsJobAbortConfigTypeDef = ...,
         awsJobTimeoutConfig: AwsJobTimeoutConfigTypeDef = ...,
         additionalParameters: Mapping[str, str] = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateOTAUpdateResponseTypeDef:
         """
         Creates an IoT OTA update on a target group of things or groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_ota_update)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_ota_update)
         """
 
     async def create_package(
         self,
         *,
         packageName: str,
         description: str = ...,
         tags: Mapping[str, str] = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> CreatePackageResponseTypeDef:
         """
         Creates an IoT software package that can be deployed to your fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_package)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_package)
         """
@@ -860,15 +860,15 @@
         self,
         *,
         packageName: str,
         versionName: str,
         description: str = ...,
         attributes: Mapping[str, str] = ...,
         tags: Mapping[str, str] = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> CreatePackageVersionResponseTypeDef:
         """
         Creates a new version for an existing IoT software package.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_package_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_package_version)
         """
@@ -909,15 +909,15 @@
         templateName: str,
         templateBody: str,
         provisioningRoleArn: str,
         description: str = ...,
         enabled: bool = ...,
         preProvisioningHook: ProvisioningHookTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
-        type: TemplateTypeType = ...
+        type: TemplateTypeType = ...,
     ) -> CreateProvisioningTemplateResponseTypeDef:
         """
         Creates a provisioning template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_provisioning_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_provisioning_template)
         """
@@ -934,15 +934,15 @@
 
     async def create_role_alias(
         self,
         *,
         roleAlias: str,
         roleArn: str,
         credentialDurationSeconds: int = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateRoleAliasResponseTypeDef:
         """
         Creates a role alias.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_role_alias)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_role_alias)
         """
@@ -951,15 +951,15 @@
         self,
         *,
         frequency: AuditFrequencyType,
         targetCheckNames: Sequence[str],
         scheduledAuditName: str,
         dayOfMonth: str = ...,
         dayOfWeek: DayOfWeekType = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateScheduledAuditResponseTypeDef:
         """
         Creates a scheduled audit that is run at a specified time interval.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_scheduled_audit)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_scheduled_audit)
         """
@@ -970,15 +970,15 @@
         securityProfileName: str,
         securityProfileDescription: str = ...,
         behaviors: Sequence[BehaviorTypeDef] = ...,
         alertTargets: Mapping[Literal["SNS"], AlertTargetTypeDef] = ...,
         additionalMetricsToRetain: Sequence[str] = ...,
         additionalMetricsToRetainV2: Sequence[MetricToRetainTypeDef] = ...,
         tags: Sequence[TagTypeDef] = ...,
-        metricsExportConfig: MetricsExportConfigTypeDef = ...
+        metricsExportConfig: MetricsExportConfigTypeDef = ...,
     ) -> CreateSecurityProfileResponseTypeDef:
         """
         Creates a Device Defender security profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_security_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_security_profile)
         """
@@ -986,59 +986,59 @@
     async def create_stream(
         self,
         *,
         streamId: str,
         files: Sequence[StreamFileTypeDef],
         roleArn: str,
         description: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateStreamResponseTypeDef:
         """
         Creates a stream for delivering one or more large files in chunks over MQTT.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_stream)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_stream)
         """
 
     async def create_thing(
         self,
         *,
         thingName: str,
         thingTypeName: str = ...,
         attributePayload: AttributePayloadTypeDef = ...,
-        billingGroupName: str = ...
+        billingGroupName: str = ...,
     ) -> CreateThingResponseTypeDef:
         """
         Creates a thing record in the registry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_thing)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_thing)
         """
 
     async def create_thing_group(
         self,
         *,
         thingGroupName: str,
         parentGroupName: str = ...,
         thingGroupProperties: ThingGroupPropertiesTypeDef = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateThingGroupResponseTypeDef:
         """
         Create a thing group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_thing_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_thing_group)
         """
 
     async def create_thing_type(
         self,
         *,
         thingTypeName: str,
         thingTypeProperties: ThingTypePropertiesTypeDef = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateThingTypeResponseTypeDef:
         """
         Creates a new thing type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_thing_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_thing_type)
         """
@@ -1176,15 +1176,15 @@
     async def delete_job_execution(
         self,
         *,
         jobId: str,
         thingName: str,
         executionNumber: int,
         force: bool = ...,
-        namespaceId: str = ...
+        namespaceId: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a job execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.delete_job_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#delete_job_execution)
         """
@@ -1769,30 +1769,30 @@
     async def get_buckets_aggregation(
         self,
         *,
         queryString: str,
         aggregationField: str,
         bucketsAggregationType: BucketsAggregationTypeTypeDef,
         indexName: str = ...,
-        queryVersion: str = ...
+        queryVersion: str = ...,
     ) -> GetBucketsAggregationResponseTypeDef:
         """
         Aggregates on indexed data with search queries pertaining to particular fields.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.get_buckets_aggregation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#get_buckets_aggregation)
         """
 
     async def get_cardinality(
         self,
         *,
         queryString: str,
         indexName: str = ...,
         aggregationField: str = ...,
-        queryVersion: str = ...
+        queryVersion: str = ...,
     ) -> GetCardinalityResponseTypeDef:
         """
         Returns the approximate count of unique values that match the query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.get_cardinality)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#get_cardinality)
         """
@@ -1870,15 +1870,15 @@
     async def get_percentiles(
         self,
         *,
         queryString: str,
         indexName: str = ...,
         aggregationField: str = ...,
         queryVersion: str = ...,
-        percents: Sequence[float] = ...
+        percents: Sequence[float] = ...,
     ) -> GetPercentilesResponseTypeDef:
         """
         Groups the aggregated values that match the query into percentile groupings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.get_percentiles)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#get_percentiles)
         """
@@ -1913,15 +1913,15 @@
 
     async def get_statistics(
         self,
         *,
         queryString: str,
         indexName: str = ...,
         aggregationField: str = ...,
-        queryVersion: str = ...
+        queryVersion: str = ...,
     ) -> GetStatisticsResponseTypeDef:
         """
         Returns the count, average, sum, minimum, maximum, sum of squares, variance,
         and standard deviation for the specified aggregated
         field.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.get_statistics)
@@ -1959,15 +1959,15 @@
         *,
         thingName: str = ...,
         securityProfileName: str = ...,
         behaviorCriteriaType: BehaviorCriteriaTypeType = ...,
         listSuppressedAlerts: bool = ...,
         verificationState: VerificationStateType = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListActiveViolationsResponseTypeDef:
         """
         Lists the active violations for a given Device Defender security profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_active_violations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_active_violations)
         """
@@ -1988,15 +1988,15 @@
         taskId: str = ...,
         checkName: str = ...,
         resourceIdentifier: ResourceIdentifierTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         startTime: TimestampTypeDef = ...,
         endTime: TimestampTypeDef = ...,
-        listSuppressedFindings: bool = ...
+        listSuppressedFindings: bool = ...,
     ) -> ListAuditFindingsResponseTypeDef:
         """
         Lists the findings (results) of a Device Defender audit or of the audits
         performed during a specified time
         period.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_audit_findings)
@@ -2006,15 +2006,15 @@
     async def list_audit_mitigation_actions_executions(
         self,
         *,
         taskId: str,
         findingId: str,
         actionStatus: AuditMitigationActionsExecutionStatusType = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListAuditMitigationActionsExecutionsResponseTypeDef:
         """
         Gets the status of audit mitigation action tasks that were executed.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_audit_mitigation_actions_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_audit_mitigation_actions_executions)
         """
@@ -2024,15 +2024,15 @@
         *,
         startTime: TimestampTypeDef,
         endTime: TimestampTypeDef,
         auditTaskId: str = ...,
         findingId: str = ...,
         taskStatus: AuditMitigationActionsTaskStatusType = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListAuditMitigationActionsTasksResponseTypeDef:
         """
         Gets a list of audit mitigation action tasks that match the specified filters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_audit_mitigation_actions_tasks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_audit_mitigation_actions_tasks)
         """
@@ -2040,15 +2040,15 @@
     async def list_audit_suppressions(
         self,
         *,
         checkName: str = ...,
         resourceIdentifier: ResourceIdentifierTypeDef = ...,
         ascendingOrder: bool = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListAuditSuppressionsResponseTypeDef:
         """
         Lists your Device Defender audit listings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_audit_suppressions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_audit_suppressions)
         """
@@ -2057,15 +2057,15 @@
         self,
         *,
         startTime: TimestampTypeDef,
         endTime: TimestampTypeDef,
         taskType: AuditTaskTypeType = ...,
         taskStatus: AuditTaskStatusType = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListAuditTasksResponseTypeDef:
         """
         Lists the Device Defender audits that have been performed during a given time
         period.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_audit_tasks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_audit_tasks)
@@ -2073,15 +2073,15 @@
 
     async def list_authorizers(
         self,
         *,
         pageSize: int = ...,
         marker: str = ...,
         ascendingOrder: bool = ...,
-        status: AuthorizerStatusType = ...
+        status: AuthorizerStatusType = ...,
     ) -> ListAuthorizersResponseTypeDef:
         """
         Lists the authorizers registered in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_authorizers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_authorizers)
         """
@@ -2098,15 +2098,15 @@
 
     async def list_ca_certificates(
         self,
         *,
         pageSize: int = ...,
         marker: str = ...,
         ascendingOrder: bool = ...,
-        templateName: str = ...
+        templateName: str = ...,
     ) -> ListCACertificatesResponseTypeDef:
         """
         Lists the CA certificates registered for your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_ca_certificates)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_ca_certificates)
         """
@@ -2123,15 +2123,15 @@
 
     async def list_certificates_by_ca(
         self,
         *,
         caCertificateId: str,
         pageSize: int = ...,
         marker: str = ...,
-        ascendingOrder: bool = ...
+        ascendingOrder: bool = ...,
     ) -> ListCertificatesByCAResponseTypeDef:
         """
         List the device certificates signed by the specified CA certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_certificates_by_ca)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_certificates_by_ca)
         """
@@ -2151,15 +2151,15 @@
         *,
         taskId: str = ...,
         violationId: str = ...,
         thingName: str = ...,
         startTime: TimestampTypeDef = ...,
         endTime: TimestampTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListDetectMitigationActionsExecutionsResponseTypeDef:
         """
         Lists mitigation actions executions for a Device Defender ML Detect Security
         Profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_detect_mitigation_actions_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_detect_mitigation_actions_executions)
@@ -2167,15 +2167,15 @@
 
     async def list_detect_mitigation_actions_tasks(
         self,
         *,
         startTime: TimestampTypeDef,
         endTime: TimestampTypeDef,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListDetectMitigationActionsTasksResponseTypeDef:
         """
         List of Device Defender ML Detect mitigation actions tasks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_detect_mitigation_actions_tasks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_detect_mitigation_actions_tasks)
         """
@@ -2223,15 +2223,15 @@
 
     async def list_job_executions_for_job(
         self,
         *,
         jobId: str,
         status: JobExecutionStatusType = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListJobExecutionsForJobResponseTypeDef:
         """
         Lists the job executions for a job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_job_executions_for_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_job_executions_for_job)
         """
@@ -2240,15 +2240,15 @@
         self,
         *,
         thingName: str,
         status: JobExecutionStatusType = ...,
         namespaceId: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        jobId: str = ...
+        jobId: str = ...,
     ) -> ListJobExecutionsForThingResponseTypeDef:
         """
         Lists the job executions for the specified thing.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_job_executions_for_thing)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_job_executions_for_thing)
         """
@@ -2268,15 +2268,15 @@
         *,
         status: JobStatusType = ...,
         targetSelection: TargetSelectionType = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         thingGroupName: str = ...,
         thingGroupId: str = ...,
-        namespaceId: str = ...
+        namespaceId: str = ...,
     ) -> ListJobsResponseTypeDef:
         """
         Lists jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_jobs)
         """
@@ -2297,15 +2297,15 @@
         thingName: str,
         metricName: str,
         startTime: TimestampTypeDef,
         endTime: TimestampTypeDef,
         dimensionName: str = ...,
         dimensionValueOperator: DimensionValueOperatorType = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListMetricValuesResponseTypeDef:
         """
         Lists the values reported for an IoT Device Defender metric (device-side
         metric, cloud-side metric, or custom metric) by the given thing during the
         specified time
         period.
 
@@ -2314,29 +2314,29 @@
         """
 
     async def list_mitigation_actions(
         self,
         *,
         actionType: MitigationActionTypeType = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListMitigationActionsResponseTypeDef:
         """
         Gets a list of all mitigation actions that match the specified filter criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_mitigation_actions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_mitigation_actions)
         """
 
     async def list_ota_updates(
         self,
         *,
         maxResults: int = ...,
         nextToken: str = ...,
-        otaUpdateStatus: OTAUpdateStatusType = ...
+        otaUpdateStatus: OTAUpdateStatusType = ...,
     ) -> ListOTAUpdatesResponseTypeDef:
         """
         Lists OTA updates.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_ota_updates)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_ota_updates)
         """
@@ -2353,15 +2353,15 @@
 
     async def list_package_versions(
         self,
         *,
         packageName: str,
         status: PackageVersionStatusType = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListPackageVersionsResponseTypeDef:
         """
         Lists the software package versions associated to the account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_package_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_package_versions)
         """
@@ -2476,30 +2476,30 @@
 
     async def list_security_profiles(
         self,
         *,
         nextToken: str = ...,
         maxResults: int = ...,
         dimensionName: str = ...,
-        metricName: str = ...
+        metricName: str = ...,
     ) -> ListSecurityProfilesResponseTypeDef:
         """
         Lists the Device Defender security profiles you've created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_security_profiles)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_security_profiles)
         """
 
     async def list_security_profiles_for_target(
         self,
         *,
         securityProfileTargetArn: str,
         nextToken: str = ...,
         maxResults: int = ...,
-        recursive: bool = ...
+        recursive: bool = ...,
     ) -> ListSecurityProfilesForTargetResponseTypeDef:
         """
         Lists the Device Defender security profiles attached to a target (thing group).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_security_profiles_for_target)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_security_profiles_for_target)
         """
@@ -2549,15 +2549,15 @@
     async def list_thing_groups(
         self,
         *,
         nextToken: str = ...,
         maxResults: int = ...,
         parentGroup: str = ...,
         namePrefixFilter: str = ...,
-        recursive: bool = ...
+        recursive: bool = ...,
     ) -> ListThingGroupsResponseTypeDef:
         """
         List the thing groups in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_thing_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_thing_groups)
         """
@@ -2584,15 +2584,15 @@
 
     async def list_thing_registration_task_reports(
         self,
         *,
         taskId: str,
         reportType: ReportTypeType,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListThingRegistrationTaskReportsResponseTypeDef:
         """
         Information about the thing registration tasks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_thing_registration_task_reports)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_thing_registration_task_reports)
         """
@@ -2621,15 +2621,15 @@
         self,
         *,
         nextToken: str = ...,
         maxResults: int = ...,
         attributeName: str = ...,
         attributeValue: str = ...,
         thingTypeName: str = ...,
-        usePrefixAttributeValue: bool = ...
+        usePrefixAttributeValue: bool = ...,
     ) -> ListThingsResponseTypeDef:
         """
         Lists your things.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_things)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_things)
         """
@@ -2646,15 +2646,15 @@
 
     async def list_things_in_thing_group(
         self,
         *,
         thingGroupName: str,
         recursive: bool = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListThingsInThingGroupResponseTypeDef:
         """
         Lists the things in the specified group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_things_in_thing_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_things_in_thing_group)
         """
@@ -2671,15 +2671,15 @@
 
     async def list_topic_rules(
         self,
         *,
         topic: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        ruleDisabled: bool = ...
+        ruleDisabled: bool = ...,
     ) -> ListTopicRulesResponseTypeDef:
         """
         Lists the rules for the specific topic.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_topic_rules)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_topic_rules)
         """
@@ -2701,15 +2701,15 @@
         endTime: TimestampTypeDef,
         thingName: str = ...,
         securityProfileName: str = ...,
         behaviorCriteriaType: BehaviorCriteriaTypeType = ...,
         listSuppressedAlerts: bool = ...,
         verificationState: VerificationStateType = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListViolationEventsResponseTypeDef:
         """
         Lists the Device Defender security profile violations discovered during the
         given time
         period.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_violation_events)
@@ -2717,15 +2717,15 @@
         """
 
     async def put_verification_state_on_violation(
         self,
         *,
         violationId: str,
         verificationState: VerificationStateType,
-        verificationStateDescription: str = ...
+        verificationStateDescription: str = ...,
     ) -> Dict[str, Any]:
         """
         Set a verification state and provide a description of that verification state
         on a violation (detect
         alarm).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.put_verification_state_on_violation)
@@ -2737,30 +2737,30 @@
         *,
         caCertificate: str,
         verificationCertificate: str = ...,
         setAsActive: bool = ...,
         allowAutoRegistration: bool = ...,
         registrationConfig: RegistrationConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
-        certificateMode: CertificateModeType = ...
+        certificateMode: CertificateModeType = ...,
     ) -> RegisterCACertificateResponseTypeDef:
         """
         Registers a CA certificate with Amazon Web Services IoT Core.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.register_ca_certificate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#register_ca_certificate)
         """
 
     async def register_certificate(
         self,
         *,
         certificatePem: str,
         caCertificatePem: str = ...,
         setAsActive: bool = ...,
-        status: CertificateStatusType = ...
+        status: CertificateStatusType = ...,
     ) -> RegisterCertificateResponseTypeDef:
         """
         Registers a device certificate with IoT in the same [certificate
         mode](https://docs.aws.amazon.com/iot/latest/apireference/API_CertificateDescription.html#iot-Type-CertificateDescription-certificateMode)
         as the signing
         CA.
 
@@ -2800,30 +2800,30 @@
 
     async def remove_thing_from_billing_group(
         self,
         *,
         billingGroupName: str = ...,
         billingGroupArn: str = ...,
         thingName: str = ...,
-        thingArn: str = ...
+        thingArn: str = ...,
     ) -> Dict[str, Any]:
         """
         Removes the given thing from the billing group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.remove_thing_from_billing_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#remove_thing_from_billing_group)
         """
 
     async def remove_thing_from_thing_group(
         self,
         *,
         thingGroupName: str = ...,
         thingGroupArn: str = ...,
         thingName: str = ...,
-        thingArn: str = ...
+        thingArn: str = ...,
     ) -> Dict[str, Any]:
         """
         Remove the specified thing from the specified group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.remove_thing_from_thing_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#remove_thing_from_thing_group)
         """
@@ -2841,15 +2841,15 @@
     async def search_index(
         self,
         *,
         queryString: str,
         indexName: str = ...,
         nextToken: str = ...,
         maxResults: int = ...,
-        queryVersion: str = ...
+        queryVersion: str = ...,
     ) -> SearchIndexResponseTypeDef:
         """
         The query search index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.search_index)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#search_index)
         """
@@ -2908,15 +2908,15 @@
 
     async def start_audit_mitigation_actions_task(
         self,
         *,
         taskId: str,
         target: AuditMitigationActionsTaskTargetTypeDef,
         auditCheckToActionsMapping: Mapping[str, Sequence[str]],
-        clientRequestToken: str
+        clientRequestToken: str,
     ) -> StartAuditMitigationActionsTaskResponseTypeDef:
         """
         Starts a task that applies a set of mitigation actions to the specified target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.start_audit_mitigation_actions_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#start_audit_mitigation_actions_task)
         """
@@ -2926,15 +2926,15 @@
         *,
         taskId: str,
         target: DetectMitigationActionsTaskTargetTypeDef,
         actions: Sequence[str],
         clientRequestToken: str,
         violationEventOccurrenceRange: ViolationEventOccurrenceRangeTypeDef = ...,
         includeOnlyActiveViolations: bool = ...,
-        includeSuppressedAlerts: bool = ...
+        includeSuppressedAlerts: bool = ...,
     ) -> StartDetectMitigationActionsTaskResponseTypeDef:
         """
         Starts a Device Defender ML Detect mitigation actions task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.start_detect_mitigation_actions_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#start_detect_mitigation_actions_task)
         """
@@ -2979,15 +2979,15 @@
         self,
         *,
         authInfos: Sequence[AuthInfoTypeDef],
         principal: str = ...,
         cognitoIdentityPoolId: str = ...,
         clientId: str = ...,
         policyNamesToAdd: Sequence[str] = ...,
-        policyNamesToSkip: Sequence[str] = ...
+        policyNamesToSkip: Sequence[str] = ...,
     ) -> TestAuthorizationResponseTypeDef:
         """
         Tests if a specified principal is authorized to perform an IoT action on a
         specified
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.test_authorization)
@@ -2998,15 +2998,15 @@
         self,
         *,
         authorizerName: str,
         token: str = ...,
         tokenSignature: str = ...,
         httpContext: HttpContextTypeDef = ...,
         mqttContext: MqttContextTypeDef = ...,
-        tlsContext: TlsContextTypeDef = ...
+        tlsContext: TlsContextTypeDef = ...,
     ) -> TestInvokeAuthorizerResponseTypeDef:
         """
         Tests a custom authorization behavior by invoking a specified custom authorizer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.test_invoke_authorizer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#test_invoke_authorizer)
         """
@@ -3033,15 +3033,15 @@
     async def update_account_audit_configuration(
         self,
         *,
         roleArn: str = ...,
         auditNotificationTargetConfigurations: Mapping[
             Literal["SNS"], AuditNotificationTargetTypeDef
         ] = ...,
-        auditCheckConfigurations: Mapping[str, AuditCheckConfigurationTypeDef] = ...
+        auditCheckConfigurations: Mapping[str, AuditCheckConfigurationTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Configures or reconfigures the Device Defender audit settings for this account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_account_audit_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_account_audit_configuration)
         """
@@ -3049,15 +3049,15 @@
     async def update_audit_suppression(
         self,
         *,
         checkName: str,
         resourceIdentifier: ResourceIdentifierTypeDef,
         expirationDate: TimestampTypeDef = ...,
         suppressIndefinitely: bool = ...,
-        description: str = ...
+        description: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates a Device Defender audit suppression.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_audit_suppression)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_audit_suppression)
         """
@@ -3066,29 +3066,29 @@
         self,
         *,
         authorizerName: str,
         authorizerFunctionArn: str = ...,
         tokenKeyName: str = ...,
         tokenSigningPublicKeys: Mapping[str, str] = ...,
         status: AuthorizerStatusType = ...,
-        enableCachingForHttp: bool = ...
+        enableCachingForHttp: bool = ...,
     ) -> UpdateAuthorizerResponseTypeDef:
         """
         Updates an authorizer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_authorizer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_authorizer)
         """
 
     async def update_billing_group(
         self,
         *,
         billingGroupName: str,
         billingGroupProperties: BillingGroupPropertiesTypeDef,
-        expectedVersion: int = ...
+        expectedVersion: int = ...,
     ) -> UpdateBillingGroupResponseTypeDef:
         """
         Updates information about the billing group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_billing_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_billing_group)
         """
@@ -3096,15 +3096,15 @@
     async def update_ca_certificate(
         self,
         *,
         certificateId: str,
         newStatus: CACertificateStatusType = ...,
         newAutoRegistrationStatus: AutoRegistrationStatusType = ...,
         registrationConfig: RegistrationConfigTypeDef = ...,
-        removeAutoRegistration: bool = ...
+        removeAutoRegistration: bool = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a registered CA certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_ca_certificate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_ca_certificate)
         """
@@ -3142,15 +3142,15 @@
     async def update_domain_configuration(
         self,
         *,
         domainConfigurationName: str,
         authorizerConfig: AuthorizerConfigTypeDef = ...,
         domainConfigurationStatus: DomainConfigurationStatusType = ...,
         removeAuthorizerConfig: bool = ...,
-        tlsConfig: TlsConfigTypeDef = ...
+        tlsConfig: TlsConfigTypeDef = ...,
     ) -> UpdateDomainConfigurationResponseTypeDef:
         """
         Updates values stored in the domain configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_domain_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_domain_configuration)
         """
@@ -3159,15 +3159,15 @@
         self,
         *,
         thingGroupName: str,
         thingGroupProperties: ThingGroupPropertiesTypeDef,
         expectedVersion: int = ...,
         indexName: str = ...,
         queryString: str = ...,
-        queryVersion: str = ...
+        queryVersion: str = ...,
     ) -> UpdateDynamicThingGroupResponseTypeDef:
         """
         Updates a dynamic thing group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_dynamic_thing_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_dynamic_thing_group)
         """
@@ -3190,28 +3190,28 @@
         queryString: str = ...,
         aggregationType: AggregationTypeTypeDef = ...,
         period: int = ...,
         aggregationField: str = ...,
         description: str = ...,
         queryVersion: str = ...,
         unit: FleetMetricUnitType = ...,
-        expectedVersion: int = ...
+        expectedVersion: int = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates the data for a fleet metric.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_fleet_metric)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_fleet_metric)
         """
 
     async def update_indexing_configuration(
         self,
         *,
         thingIndexingConfiguration: ThingIndexingConfigurationTypeDef = ...,
-        thingGroupIndexingConfiguration: ThingGroupIndexingConfigurationTypeDef = ...
+        thingGroupIndexingConfiguration: ThingGroupIndexingConfigurationTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates the search configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_indexing_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_indexing_configuration)
         """
@@ -3222,29 +3222,29 @@
         jobId: str,
         description: str = ...,
         presignedUrlConfig: PresignedUrlConfigTypeDef = ...,
         jobExecutionsRolloutConfig: JobExecutionsRolloutConfigTypeDef = ...,
         abortConfig: AbortConfigTypeDef = ...,
         timeoutConfig: TimeoutConfigTypeDef = ...,
         namespaceId: str = ...,
-        jobExecutionsRetryConfig: JobExecutionsRetryConfigTypeDef = ...
+        jobExecutionsRetryConfig: JobExecutionsRetryConfigTypeDef = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates supported fields of the specified job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_job)
         """
 
     async def update_mitigation_action(
         self,
         *,
         actionName: str,
         roleArn: str = ...,
-        actionParams: MitigationActionParamsTypeDef = ...
+        actionParams: MitigationActionParamsTypeDef = ...,
     ) -> UpdateMitigationActionResponseTypeDef:
         """
         Updates the definition for the specified mitigation action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_mitigation_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_mitigation_action)
         """
@@ -3252,28 +3252,28 @@
     async def update_package(
         self,
         *,
         packageName: str,
         description: str = ...,
         defaultVersionName: str = ...,
         unsetDefaultVersion: bool = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates the supported fields for a specific software package.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_package)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_package)
         """
 
     async def update_package_configuration(
         self,
         *,
         versionUpdateByJobsConfig: VersionUpdateByJobsConfigTypeDef = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates the software package configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_package_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_package_configuration)
         """
@@ -3282,15 +3282,15 @@
         self,
         *,
         packageName: str,
         versionName: str,
         description: str = ...,
         attributes: Mapping[str, str] = ...,
         action: PackageVersionActionType = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates the supported fields for a specific package version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_package_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_package_version)
         """
@@ -3300,15 +3300,15 @@
         *,
         templateName: str,
         description: str = ...,
         enabled: bool = ...,
         defaultVersionId: int = ...,
         provisioningRoleArn: str = ...,
         preProvisioningHook: ProvisioningHookTypeDef = ...,
-        removePreProvisioningHook: bool = ...
+        removePreProvisioningHook: bool = ...,
     ) -> Dict[str, Any]:
         """
         Updates a provisioning template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_provisioning_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_provisioning_template)
         """
@@ -3326,15 +3326,15 @@
     async def update_scheduled_audit(
         self,
         *,
         scheduledAuditName: str,
         frequency: AuditFrequencyType = ...,
         dayOfMonth: str = ...,
         dayOfWeek: DayOfWeekType = ...,
-        targetCheckNames: Sequence[str] = ...
+        targetCheckNames: Sequence[str] = ...,
     ) -> UpdateScheduledAuditResponseTypeDef:
         """
         Updates a scheduled audit, including which checks are performed and how often
         the audit takes
         place.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_scheduled_audit)
@@ -3351,30 +3351,30 @@
         additionalMetricsToRetain: Sequence[str] = ...,
         additionalMetricsToRetainV2: Sequence[MetricToRetainTypeDef] = ...,
         deleteBehaviors: bool = ...,
         deleteAlertTargets: bool = ...,
         deleteAdditionalMetricsToRetain: bool = ...,
         expectedVersion: int = ...,
         metricsExportConfig: MetricsExportConfigTypeDef = ...,
-        deleteMetricsExportConfig: bool = ...
+        deleteMetricsExportConfig: bool = ...,
     ) -> UpdateSecurityProfileResponseTypeDef:
         """
         Updates a Device Defender security profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_security_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_security_profile)
         """
 
     async def update_stream(
         self,
         *,
         streamId: str,
         description: str = ...,
         files: Sequence[StreamFileTypeDef] = ...,
-        roleArn: str = ...
+        roleArn: str = ...,
     ) -> UpdateStreamResponseTypeDef:
         """
         Updates an existing stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_stream)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_stream)
         """
@@ -3382,44 +3382,44 @@
     async def update_thing(
         self,
         *,
         thingName: str,
         thingTypeName: str = ...,
         attributePayload: AttributePayloadTypeDef = ...,
         expectedVersion: int = ...,
-        removeThingType: bool = ...
+        removeThingType: bool = ...,
     ) -> Dict[str, Any]:
         """
         Updates the data for a thing.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_thing)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_thing)
         """
 
     async def update_thing_group(
         self,
         *,
         thingGroupName: str,
         thingGroupProperties: ThingGroupPropertiesTypeDef,
-        expectedVersion: int = ...
+        expectedVersion: int = ...,
     ) -> UpdateThingGroupResponseTypeDef:
         """
         Update a thing group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_thing_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_thing_group)
         """
 
     async def update_thing_groups_for_thing(
         self,
         *,
         thingName: str = ...,
         thingGroupsToAdd: Sequence[str] = ...,
         thingGroupsToRemove: Sequence[str] = ...,
-        overrideDynamicGroups: bool = ...
+        overrideDynamicGroups: bool = ...,
     ) -> Dict[str, Any]:
         """
         Updates the groups to which the thing belongs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_thing_groups_for_thing)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_thing_groups_for_thing)
         """
```

### Comparing `types-aiobotocore-iot-2.9.0/types_aiobotocore_iot/literals.py` & `types-aiobotocore-iot-2.9.1/types_aiobotocore_iot/literals.py`

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
     "AbortActionType",
     "ActionTypeType",
     "AggregationTypeNameType",
     "AlertTargetTypeType",
     "AuditCheckRunStatusType",
     "AuditFindingSeverityType",
@@ -154,15 +153,14 @@
     "IoTServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AbortActionType = Literal["CANCEL"]
 ActionTypeType = Literal["CONNECT", "PUBLISH", "RECEIVE", "SUBSCRIBE"]
 AggregationTypeNameType = Literal["Cardinality", "Percentiles", "Statistics"]
 AlertTargetTypeType = Literal["SNS"]
 AuditCheckRunStatusType = Literal[
     "CANCELED",
     "COMPLETED_COMPLIANT",
```

### Comparing `types-aiobotocore-iot-2.9.0/types_aiobotocore_iot/literals.pyi` & `types-aiobotocore-iot-2.9.1/types_aiobotocore_iot/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-2.9.0/types_aiobotocore_iot/paginator.py` & `types-aiobotocore-iot-2.9.1/types_aiobotocore_iot/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -285,15 +285,14 @@
     "ListThingsInThingGroupPaginator",
     "ListTopicRuleDestinationsPaginator",
     "ListTopicRulesPaginator",
     "ListV2LoggingLevelsPaginator",
     "ListViolationEventsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -325,15 +324,15 @@
         self,
         *,
         thingName: str = ...,
         securityProfileName: str = ...,
         behaviorCriteriaType: BehaviorCriteriaTypeType = ...,
         listSuppressedAlerts: bool = ...,
         verificationState: VerificationStateType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListActiveViolationsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListActiveViolations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listactiveviolationspaginator)
         """
 
 
@@ -363,15 +362,15 @@
         *,
         taskId: str = ...,
         checkName: str = ...,
         resourceIdentifier: ResourceIdentifierTypeDef = ...,
         startTime: TimestampTypeDef = ...,
         endTime: TimestampTypeDef = ...,
         listSuppressedFindings: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAuditFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditFindings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listauditfindingspaginator)
         """
 
 
@@ -383,15 +382,15 @@
 
     def paginate(
         self,
         *,
         taskId: str,
         findingId: str,
         actionStatus: AuditMitigationActionsExecutionStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAuditMitigationActionsExecutionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditMitigationActionsExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listauditmitigationactionsexecutionspaginator)
         """
 
 
@@ -405,15 +404,15 @@
         self,
         *,
         startTime: TimestampTypeDef,
         endTime: TimestampTypeDef,
         auditTaskId: str = ...,
         findingId: str = ...,
         taskStatus: AuditMitigationActionsTaskStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAuditMitigationActionsTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditMitigationActionsTasks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listauditmitigationactionstaskspaginator)
         """
 
 
@@ -425,15 +424,15 @@
 
     def paginate(
         self,
         *,
         checkName: str = ...,
         resourceIdentifier: ResourceIdentifierTypeDef = ...,
         ascendingOrder: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAuditSuppressionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditSuppressions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listauditsuppressionspaginator)
         """
 
 
@@ -446,15 +445,15 @@
     def paginate(
         self,
         *,
         startTime: TimestampTypeDef,
         endTime: TimestampTypeDef,
         taskType: AuditTaskTypeType = ...,
         taskStatus: AuditTaskStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAuditTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditTasks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listaudittaskspaginator)
         """
 
 
@@ -465,15 +464,15 @@
     """
 
     def paginate(
         self,
         *,
         ascendingOrder: bool = ...,
         status: AuthorizerStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAuthorizersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuthorizers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listauthorizerspaginator)
         """
 
 
@@ -499,15 +498,15 @@
     """
 
     def paginate(
         self,
         *,
         ascendingOrder: bool = ...,
         templateName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCACertificatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListCACertificates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listcacertificatespaginator)
         """
 
 
@@ -533,15 +532,15 @@
     """
 
     def paginate(
         self,
         *,
         caCertificateId: str,
         ascendingOrder: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCertificatesByCAResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListCertificatesByCA.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listcertificatesbycapaginator)
         """
 
 
@@ -570,15 +569,15 @@
         self,
         *,
         taskId: str = ...,
         violationId: str = ...,
         thingName: str = ...,
         startTime: TimestampTypeDef = ...,
         endTime: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDetectMitigationActionsExecutionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListDetectMitigationActionsExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listdetectmitigationactionsexecutionspaginator)
         """
 
 
@@ -589,15 +588,15 @@
     """
 
     def paginate(
         self,
         *,
         startTime: TimestampTypeDef,
         endTime: TimestampTypeDef,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDetectMitigationActionsTasksResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListDetectMitigationActionsTasks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listdetectmitigationactionstaskspaginator)
         """
 
 
@@ -668,15 +667,15 @@
     """
 
     def paginate(
         self,
         *,
         jobId: str,
         status: JobExecutionStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListJobExecutionsForJobResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListJobExecutionsForJob.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listjobexecutionsforjobpaginator)
         """
 
 
@@ -689,15 +688,15 @@
     def paginate(
         self,
         *,
         thingName: str,
         status: JobExecutionStatusType = ...,
         namespaceId: str = ...,
         jobId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListJobExecutionsForThingResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListJobExecutionsForThing.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listjobexecutionsforthingpaginator)
         """
 
 
@@ -726,15 +725,15 @@
         self,
         *,
         status: JobStatusType = ...,
         targetSelection: TargetSelectionType = ...,
         thingGroupName: str = ...,
         thingGroupId: str = ...,
         namespaceId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listjobspaginator)
         """
 
 
@@ -764,15 +763,15 @@
         *,
         thingName: str,
         metricName: str,
         startTime: TimestampTypeDef,
         endTime: TimestampTypeDef,
         dimensionName: str = ...,
         dimensionValueOperator: DimensionValueOperatorType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListMetricValuesResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListMetricValues.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listmetricvaluespaginator)
         """
 
 
@@ -782,15 +781,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listmitigationactionspaginator)
     """
 
     def paginate(
         self,
         *,
         actionType: MitigationActionTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListMitigationActionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListMitigationActions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listmitigationactionspaginator)
         """
 
 
@@ -800,15 +799,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listotaupdatespaginator)
     """
 
     def paginate(
         self,
         *,
         otaUpdateStatus: OTAUpdateStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListOTAUpdatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListOTAUpdates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listotaupdatespaginator)
         """
 
 
@@ -834,15 +833,15 @@
     """
 
     def paginate(
         self,
         *,
         packageName: str,
         status: PackageVersionStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPackageVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListPackageVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listpackageversionspaginator)
         """
 
 
@@ -883,15 +882,15 @@
     """
 
     def paginate(
         self,
         *,
         policyName: str,
         ascendingOrder: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPolicyPrincipalsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListPolicyPrincipals.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listpolicyprincipalspaginator)
         """
 
 
@@ -902,15 +901,15 @@
     """
 
     def paginate(
         self,
         *,
         principal: str,
         ascendingOrder: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPrincipalPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListPrincipalPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listprincipalpoliciespaginator)
         """
 
 
@@ -1011,15 +1010,15 @@
     """
 
     def paginate(
         self,
         *,
         dimensionName: str = ...,
         metricName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSecurityProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListSecurityProfiles.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listsecurityprofilespaginator)
         """
 
 
@@ -1030,15 +1029,15 @@
     """
 
     def paginate(
         self,
         *,
         securityProfileTargetArn: str,
         recursive: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSecurityProfilesForTargetResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListSecurityProfilesForTarget.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listsecurityprofilesfortargetpaginator)
         """
 
 
@@ -1110,15 +1109,15 @@
 
     def paginate(
         self,
         *,
         parentGroup: str = ...,
         namePrefixFilter: str = ...,
         recursive: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListThingGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listthinggroupspaginator)
         """
 
 
@@ -1159,15 +1158,15 @@
     """
 
     def paginate(
         self,
         *,
         taskId: str,
         reportType: ReportTypeType,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListThingRegistrationTaskReportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingRegistrationTaskReports.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listthingregistrationtaskreportspaginator)
         """
 
 
@@ -1210,15 +1209,15 @@
     def paginate(
         self,
         *,
         attributeName: str = ...,
         attributeValue: str = ...,
         thingTypeName: str = ...,
         usePrefixAttributeValue: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListThingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listthingspaginator)
         """
 
 
@@ -1244,15 +1243,15 @@
     """
 
     def paginate(
         self,
         *,
         thingGroupName: str,
         recursive: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListThingsInThingGroupResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingsInThingGroup.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listthingsinthinggrouppaginator)
         """
 
 
@@ -1278,15 +1277,15 @@
     """
 
     def paginate(
         self,
         *,
         topic: str = ...,
         ruleDisabled: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTopicRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListTopicRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listtopicrulespaginator)
         """
 
 
@@ -1317,13 +1316,13 @@
         startTime: TimestampTypeDef,
         endTime: TimestampTypeDef,
         thingName: str = ...,
         securityProfileName: str = ...,
         behaviorCriteriaType: BehaviorCriteriaTypeType = ...,
         listSuppressedAlerts: bool = ...,
         verificationState: VerificationStateType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListViolationEventsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListViolationEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listviolationeventspaginator)
         """
```

### Comparing `types-aiobotocore-iot-2.9.0/types_aiobotocore_iot/paginator.pyi` & `types-aiobotocore-iot-2.9.1/types_aiobotocore_iot/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -321,15 +321,15 @@
         self,
         *,
         thingName: str = ...,
         securityProfileName: str = ...,
         behaviorCriteriaType: BehaviorCriteriaTypeType = ...,
         listSuppressedAlerts: bool = ...,
         verificationState: VerificationStateType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListActiveViolationsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListActiveViolations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listactiveviolationspaginator)
         """
 
 class ListAttachedPoliciesPaginator(AioPaginator):
@@ -357,15 +357,15 @@
         *,
         taskId: str = ...,
         checkName: str = ...,
         resourceIdentifier: ResourceIdentifierTypeDef = ...,
         startTime: TimestampTypeDef = ...,
         endTime: TimestampTypeDef = ...,
         listSuppressedFindings: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAuditFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditFindings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listauditfindingspaginator)
         """
 
 class ListAuditMitigationActionsExecutionsPaginator(AioPaginator):
@@ -376,15 +376,15 @@
 
     def paginate(
         self,
         *,
         taskId: str,
         findingId: str,
         actionStatus: AuditMitigationActionsExecutionStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAuditMitigationActionsExecutionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditMitigationActionsExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listauditmitigationactionsexecutionspaginator)
         """
 
 class ListAuditMitigationActionsTasksPaginator(AioPaginator):
@@ -397,15 +397,15 @@
         self,
         *,
         startTime: TimestampTypeDef,
         endTime: TimestampTypeDef,
         auditTaskId: str = ...,
         findingId: str = ...,
         taskStatus: AuditMitigationActionsTaskStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAuditMitigationActionsTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditMitigationActionsTasks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listauditmitigationactionstaskspaginator)
         """
 
 class ListAuditSuppressionsPaginator(AioPaginator):
@@ -416,15 +416,15 @@
 
     def paginate(
         self,
         *,
         checkName: str = ...,
         resourceIdentifier: ResourceIdentifierTypeDef = ...,
         ascendingOrder: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAuditSuppressionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditSuppressions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listauditsuppressionspaginator)
         """
 
 class ListAuditTasksPaginator(AioPaginator):
@@ -436,15 +436,15 @@
     def paginate(
         self,
         *,
         startTime: TimestampTypeDef,
         endTime: TimestampTypeDef,
         taskType: AuditTaskTypeType = ...,
         taskStatus: AuditTaskStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAuditTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditTasks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listaudittaskspaginator)
         """
 
 class ListAuthorizersPaginator(AioPaginator):
@@ -454,15 +454,15 @@
     """
 
     def paginate(
         self,
         *,
         ascendingOrder: bool = ...,
         status: AuthorizerStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAuthorizersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuthorizers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listauthorizerspaginator)
         """
 
 class ListBillingGroupsPaginator(AioPaginator):
@@ -486,15 +486,15 @@
     """
 
     def paginate(
         self,
         *,
         ascendingOrder: bool = ...,
         templateName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCACertificatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListCACertificates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listcacertificatespaginator)
         """
 
 class ListCertificatesPaginator(AioPaginator):
@@ -518,15 +518,15 @@
     """
 
     def paginate(
         self,
         *,
         caCertificateId: str,
         ascendingOrder: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCertificatesByCAResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListCertificatesByCA.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listcertificatesbycapaginator)
         """
 
 class ListCustomMetricsPaginator(AioPaginator):
@@ -553,15 +553,15 @@
         self,
         *,
         taskId: str = ...,
         violationId: str = ...,
         thingName: str = ...,
         startTime: TimestampTypeDef = ...,
         endTime: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDetectMitigationActionsExecutionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListDetectMitigationActionsExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listdetectmitigationactionsexecutionspaginator)
         """
 
 class ListDetectMitigationActionsTasksPaginator(AioPaginator):
@@ -571,15 +571,15 @@
     """
 
     def paginate(
         self,
         *,
         startTime: TimestampTypeDef,
         endTime: TimestampTypeDef,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDetectMitigationActionsTasksResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListDetectMitigationActionsTasks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listdetectmitigationactionstaskspaginator)
         """
 
 class ListDimensionsPaginator(AioPaginator):
@@ -645,15 +645,15 @@
     """
 
     def paginate(
         self,
         *,
         jobId: str,
         status: JobExecutionStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListJobExecutionsForJobResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListJobExecutionsForJob.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listjobexecutionsforjobpaginator)
         """
 
 class ListJobExecutionsForThingPaginator(AioPaginator):
@@ -665,15 +665,15 @@
     def paginate(
         self,
         *,
         thingName: str,
         status: JobExecutionStatusType = ...,
         namespaceId: str = ...,
         jobId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListJobExecutionsForThingResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListJobExecutionsForThing.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listjobexecutionsforthingpaginator)
         """
 
 class ListJobTemplatesPaginator(AioPaginator):
@@ -700,15 +700,15 @@
         self,
         *,
         status: JobStatusType = ...,
         targetSelection: TargetSelectionType = ...,
         thingGroupName: str = ...,
         thingGroupId: str = ...,
         namespaceId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listjobspaginator)
         """
 
 class ListManagedJobTemplatesPaginator(AioPaginator):
@@ -736,15 +736,15 @@
         *,
         thingName: str,
         metricName: str,
         startTime: TimestampTypeDef,
         endTime: TimestampTypeDef,
         dimensionName: str = ...,
         dimensionValueOperator: DimensionValueOperatorType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListMetricValuesResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListMetricValues.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listmetricvaluespaginator)
         """
 
 class ListMitigationActionsPaginator(AioPaginator):
@@ -753,15 +753,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listmitigationactionspaginator)
     """
 
     def paginate(
         self,
         *,
         actionType: MitigationActionTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListMitigationActionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListMitigationActions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listmitigationactionspaginator)
         """
 
 class ListOTAUpdatesPaginator(AioPaginator):
@@ -770,15 +770,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listotaupdatespaginator)
     """
 
     def paginate(
         self,
         *,
         otaUpdateStatus: OTAUpdateStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListOTAUpdatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListOTAUpdates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listotaupdatespaginator)
         """
 
 class ListOutgoingCertificatesPaginator(AioPaginator):
@@ -802,15 +802,15 @@
     """
 
     def paginate(
         self,
         *,
         packageName: str,
         status: PackageVersionStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPackageVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListPackageVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listpackageversionspaginator)
         """
 
 class ListPackagesPaginator(AioPaginator):
@@ -848,15 +848,15 @@
     """
 
     def paginate(
         self,
         *,
         policyName: str,
         ascendingOrder: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPolicyPrincipalsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListPolicyPrincipals.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listpolicyprincipalspaginator)
         """
 
 class ListPrincipalPoliciesPaginator(AioPaginator):
@@ -866,15 +866,15 @@
     """
 
     def paginate(
         self,
         *,
         principal: str,
         ascendingOrder: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPrincipalPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListPrincipalPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listprincipalpoliciespaginator)
         """
 
 class ListPrincipalThingsPaginator(AioPaginator):
@@ -968,15 +968,15 @@
     """
 
     def paginate(
         self,
         *,
         dimensionName: str = ...,
         metricName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSecurityProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListSecurityProfiles.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listsecurityprofilespaginator)
         """
 
 class ListSecurityProfilesForTargetPaginator(AioPaginator):
@@ -986,15 +986,15 @@
     """
 
     def paginate(
         self,
         *,
         securityProfileTargetArn: str,
         recursive: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSecurityProfilesForTargetResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListSecurityProfilesForTarget.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listsecurityprofilesfortargetpaginator)
         """
 
 class ListStreamsPaginator(AioPaginator):
@@ -1061,15 +1061,15 @@
 
     def paginate(
         self,
         *,
         parentGroup: str = ...,
         namePrefixFilter: str = ...,
         recursive: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListThingGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listthinggroupspaginator)
         """
 
 class ListThingGroupsForThingPaginator(AioPaginator):
@@ -1107,15 +1107,15 @@
     """
 
     def paginate(
         self,
         *,
         taskId: str,
         reportType: ReportTypeType,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListThingRegistrationTaskReportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingRegistrationTaskReports.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listthingregistrationtaskreportspaginator)
         """
 
 class ListThingRegistrationTasksPaginator(AioPaginator):
@@ -1155,15 +1155,15 @@
     def paginate(
         self,
         *,
         attributeName: str = ...,
         attributeValue: str = ...,
         thingTypeName: str = ...,
         usePrefixAttributeValue: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListThingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listthingspaginator)
         """
 
 class ListThingsInBillingGroupPaginator(AioPaginator):
@@ -1187,15 +1187,15 @@
     """
 
     def paginate(
         self,
         *,
         thingGroupName: str,
         recursive: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListThingsInThingGroupResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingsInThingGroup.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listthingsinthinggrouppaginator)
         """
 
 class ListTopicRuleDestinationsPaginator(AioPaginator):
@@ -1219,15 +1219,15 @@
     """
 
     def paginate(
         self,
         *,
         topic: str = ...,
         ruleDisabled: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTopicRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListTopicRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listtopicrulespaginator)
         """
 
 class ListV2LoggingLevelsPaginator(AioPaginator):
@@ -1256,13 +1256,13 @@
         startTime: TimestampTypeDef,
         endTime: TimestampTypeDef,
         thingName: str = ...,
         securityProfileName: str = ...,
         behaviorCriteriaType: BehaviorCriteriaTypeType = ...,
         listSuppressedAlerts: bool = ...,
         verificationState: VerificationStateType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListViolationEventsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListViolationEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listviolationeventspaginator)
         """
```

### Comparing `types-aiobotocore-iot-2.9.0/types_aiobotocore_iot/type_defs.py` & `types-aiobotocore-iot-2.9.1/types_aiobotocore_iot/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AbortCriteriaTypeDef",
     "AcceptCertificateTransferRequestRequestTypeDef",
     "CloudwatchAlarmActionTypeDef",
     "CloudwatchLogsActionTypeDef",
     "CloudwatchMetricActionTypeDef",
     "DynamoDBActionTypeDef",
```

### Comparing `types-aiobotocore-iot-2.9.0/types_aiobotocore_iot/type_defs.pyi` & `types-aiobotocore-iot-2.9.1/types_aiobotocore_iot/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-2.9.0/types_aiobotocore_iot.egg-info/PKG-INFO` & `types-aiobotocore-iot-2.9.1/types_aiobotocore_iot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iot
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.IoT 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.IoT 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/
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
 
 <a id="types-aiobotocore-iot"></a>
 
 # types-aiobotocore-iot
 
 [![PyPI - types-aiobotocore-iot](https://img.shields.io/pypi/v/types-aiobotocore-iot.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iot.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iot)](https://pepy.tech/project/types-aiobotocore-iot)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoT 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT)
+[aiobotocore.IoT 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT)
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
 [types-aiobotocore-iot docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-iot-2.9.0/types_aiobotocore_iot.egg-info/SOURCES.txt` & `types-aiobotocore-iot-2.9.1/types_aiobotocore_iot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

