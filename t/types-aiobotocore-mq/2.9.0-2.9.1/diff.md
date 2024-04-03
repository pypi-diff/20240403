# Comparing `tmp/types-aiobotocore-mq-2.9.0.tar.gz` & `tmp/types-aiobotocore-mq-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-mq-2.9.0.tar", last modified: Wed Dec 13 19:59:59 2023, max compression
+gzip compressed data, was "types-aiobotocore-mq-2.9.1.tar", last modified: Thu Jan 18 01:21:20 2024, max compression
```

## Comparing `types-aiobotocore-mq-2.9.0.tar` & `types-aiobotocore-mq-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:59.453406 types-aiobotocore-mq-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:50:39.000000 types-aiobotocore-mq-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12647 2023-12-13 19:59:59.453406 types-aiobotocore-mq-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11104 2023-12-13 19:50:39.000000 types-aiobotocore-mq-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:59.453406 types-aiobotocore-mq-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2023-12-13 19:50:39.000000 types-aiobotocore-mq-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:59.453406 types-aiobotocore-mq-2.9.0/types_aiobotocore_mq/
--rw-r--r--   0 runner    (1001) docker     (127)      590 2023-12-13 19:50:39.000000 types-aiobotocore-mq-2.9.0/types_aiobotocore_mq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2023-12-13 19:50:39.000000 types-aiobotocore-mq-2.9.0/types_aiobotocore_mq/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      901 2023-12-13 19:50:39.000000 types-aiobotocore-mq-2.9.0/types_aiobotocore_mq/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18728 2023-12-13 19:50:39.000000 types-aiobotocore-mq-2.9.0/types_aiobotocore_mq/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    18724 2023-12-13 19:50:39.000000 types-aiobotocore-mq-2.9.0/types_aiobotocore_mq/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9887 2023-12-13 19:50:40.000000 types-aiobotocore-mq-2.9.0/types_aiobotocore_mq/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9885 2023-12-13 19:50:40.000000 types-aiobotocore-mq-2.9.0/types_aiobotocore_mq/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2023-12-13 19:50:39.000000 types-aiobotocore-mq-2.9.0/types_aiobotocore_mq/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2023-12-13 19:50:39.000000 types-aiobotocore-mq-2.9.0/types_aiobotocore_mq/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:50:39.000000 types-aiobotocore-mq-2.9.0/types_aiobotocore_mq/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    22845 2023-12-13 19:50:40.000000 types-aiobotocore-mq-2.9.0/types_aiobotocore_mq/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    22844 2023-12-13 19:50:40.000000 types-aiobotocore-mq-2.9.0/types_aiobotocore_mq/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:50:39.000000 types-aiobotocore-mq-2.9.0/types_aiobotocore_mq/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:59.453406 types-aiobotocore-mq-2.9.0/types_aiobotocore_mq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12647 2023-12-13 19:59:59.000000 types-aiobotocore-mq-2.9.0/types_aiobotocore_mq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      718 2023-12-13 19:59:59.000000 types-aiobotocore-mq-2.9.0/types_aiobotocore_mq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:59.000000 types-aiobotocore-mq-2.9.0/types_aiobotocore_mq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:59.000000 types-aiobotocore-mq-2.9.0/types_aiobotocore_mq.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:59.000000 types-aiobotocore-mq-2.9.0/types_aiobotocore_mq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-12-13 19:59:59.000000 types-aiobotocore-mq-2.9.0/types_aiobotocore_mq.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:20.805160 types-aiobotocore-mq-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:12:21.000000 types-aiobotocore-mq-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12667 2024-01-18 01:21:20.805160 types-aiobotocore-mq-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11104 2024-01-18 01:12:21.000000 types-aiobotocore-mq-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:20.805160 types-aiobotocore-mq-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-01-18 01:12:21.000000 types-aiobotocore-mq-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:20.801160 types-aiobotocore-mq-2.9.1/types_aiobotocore_mq/
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-01-18 01:12:21.000000 types-aiobotocore-mq-2.9.1/types_aiobotocore_mq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-01-18 01:12:21.000000 types-aiobotocore-mq-2.9.1/types_aiobotocore_mq/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-01-18 01:12:21.000000 types-aiobotocore-mq-2.9.1/types_aiobotocore_mq/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18733 2024-01-18 01:12:21.000000 types-aiobotocore-mq-2.9.1/types_aiobotocore_mq/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18730 2024-01-18 01:12:21.000000 types-aiobotocore-mq-2.9.1/types_aiobotocore_mq/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9885 2024-01-18 01:12:21.000000 types-aiobotocore-mq-2.9.1/types_aiobotocore_mq/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9885 2024-01-18 01:12:21.000000 types-aiobotocore-mq-2.9.1/types_aiobotocore_mq/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-01-18 01:12:21.000000 types-aiobotocore-mq-2.9.1/types_aiobotocore_mq/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-01-18 01:12:21.000000 types-aiobotocore-mq-2.9.1/types_aiobotocore_mq/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:12:21.000000 types-aiobotocore-mq-2.9.1/types_aiobotocore_mq/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    22844 2024-01-18 01:12:22.000000 types-aiobotocore-mq-2.9.1/types_aiobotocore_mq/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22844 2024-01-18 01:12:22.000000 types-aiobotocore-mq-2.9.1/types_aiobotocore_mq/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:12:21.000000 types-aiobotocore-mq-2.9.1/types_aiobotocore_mq/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:20.805160 types-aiobotocore-mq-2.9.1/types_aiobotocore_mq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12667 2024-01-18 01:21:20.000000 types-aiobotocore-mq-2.9.1/types_aiobotocore_mq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-01-18 01:21:20.000000 types-aiobotocore-mq-2.9.1/types_aiobotocore_mq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:20.000000 types-aiobotocore-mq-2.9.1/types_aiobotocore_mq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:20.000000 types-aiobotocore-mq-2.9.1/types_aiobotocore_mq.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:20.000000 types-aiobotocore-mq-2.9.1/types_aiobotocore_mq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-18 01:21:20.000000 types-aiobotocore-mq-2.9.1/types_aiobotocore_mq.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-mq-2.9.0/LICENSE` & `types-aiobotocore-mq-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-mq-2.9.0/PKG-INFO` & `types-aiobotocore-mq-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mq
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.MQ 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.MQ 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mq/
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
 
 <a id="types-aiobotocore-mq"></a>
 
 # types-aiobotocore-mq
 
 [![PyPI - types-aiobotocore-mq](https://img.shields.io/pypi/v/types-aiobotocore-mq.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mq)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mq.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mq)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mq/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mq)](https://pepy.tech/project/types-aiobotocore-mq)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MQ 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ)
+[aiobotocore.MQ 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ)
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
 [types-aiobotocore-mq docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mq/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-mq-2.9.0/README.md` & `types-aiobotocore-mq-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mq.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mq)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mq/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mq)](https://pepy.tech/project/types-aiobotocore-mq)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MQ 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ)
+[aiobotocore.MQ 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ)
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
 [types-aiobotocore-mq docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mq/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-mq-2.9.0/setup.py` & `types-aiobotocore-mq-2.9.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,47 +7,46 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-mq",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_mq"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.MQ 2.9.0 service generated with mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.MQ 2.9.1 service generated with mypy-boto3-builder 7.23.1"
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
     keywords="aiobotocore mq type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_mq": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mq/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-mq-2.9.0/types_aiobotocore_mq/__init__.py` & `types-aiobotocore-mq-2.9.1/types_aiobotocore_mq/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,9 +22,8 @@
 """
 
 from .client import MQClient
 from .paginator import ListBrokersPaginator
 
 Client = MQClient
 
-
 __all__ = ("Client", "ListBrokersPaginator", "MQClient")
```

### Comparing `types-aiobotocore-mq-2.9.0/types_aiobotocore_mq/__init__.pyi` & `types-aiobotocore-mq-2.9.1/types_aiobotocore_mq/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mq-2.9.0/types_aiobotocore_mq/__main__.py` & `types-aiobotocore-mq-2.9.1/types_aiobotocore_mq/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.MQ 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.MQ 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mq//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ\nOther"
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

### Comparing `types-aiobotocore-mq-2.9.0/types_aiobotocore_mq/client.py` & `types-aiobotocore-mq-2.9.1/types_aiobotocore_mq/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("MQClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -136,15 +135,15 @@
         Logs: LogsTypeDef = ...,
         MaintenanceWindowStartTime: WeeklyStartTimeTypeDef = ...,
         SecurityGroups: Sequence[str] = ...,
         StorageType: BrokerStorageTypeType = ...,
         SubnetIds: Sequence[str] = ...,
         Tags: Mapping[str, str] = ...,
         DataReplicationMode: DataReplicationModeType = ...,
-        DataReplicationPrimaryBrokerArn: str = ...
+        DataReplicationPrimaryBrokerArn: str = ...,
     ) -> CreateBrokerResponseTypeDef:
         """
         Creates a broker.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client.create_broker)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mq/client/#create_broker)
         """
@@ -152,15 +151,15 @@
     async def create_configuration(
         self,
         *,
         EngineType: EngineTypeType,
         EngineVersion: str,
         Name: str,
         AuthenticationStrategy: AuthenticationStrategyType = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateConfigurationResponseTypeDef:
         """
         Creates a new configuration for the specified configuration name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client.create_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mq/client/#create_configuration)
         """
@@ -179,15 +178,15 @@
         self,
         *,
         BrokerId: str,
         Password: str,
         Username: str,
         ConsoleAccess: bool = ...,
         Groups: Sequence[str] = ...,
-        ReplicationUser: bool = ...
+        ReplicationUser: bool = ...,
     ) -> Dict[str, Any]:
         """
         Creates an ActiveMQ user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client.create_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mq/client/#create_user)
         """
@@ -239,15 +238,15 @@
     async def describe_broker_instance_options(
         self,
         *,
         EngineType: str = ...,
         HostInstanceType: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        StorageType: str = ...
+        StorageType: str = ...,
     ) -> DescribeBrokerInstanceOptionsResponseTypeDef:
         """
         Describe available broker instance options.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client.describe_broker_instance_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mq/client/#describe_broker_instance_options)
         """
@@ -367,15 +366,15 @@
         Configuration: ConfigurationIdTypeDef = ...,
         EngineVersion: str = ...,
         HostInstanceType: str = ...,
         LdapServerMetadata: LdapServerMetadataInputTypeDef = ...,
         Logs: LogsTypeDef = ...,
         MaintenanceWindowStartTime: WeeklyStartTimeTypeDef = ...,
         SecurityGroups: Sequence[str] = ...,
-        DataReplicationMode: DataReplicationModeType = ...
+        DataReplicationMode: DataReplicationModeType = ...,
     ) -> UpdateBrokerResponseTypeDef:
         """
         Adds a pending configuration change to a broker.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client.update_broker)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mq/client/#update_broker)
         """
@@ -394,15 +393,15 @@
         self,
         *,
         BrokerId: str,
         Username: str,
         ConsoleAccess: bool = ...,
         Groups: Sequence[str] = ...,
         Password: str = ...,
-        ReplicationUser: bool = ...
+        ReplicationUser: bool = ...,
     ) -> Dict[str, Any]:
         """
         Updates the information for an ActiveMQ user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client.update_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mq/client/#update_user)
         """
```

### Comparing `types-aiobotocore-mq-2.9.0/types_aiobotocore_mq/client.pyi` & `types-aiobotocore-mq-2.9.1/types_aiobotocore_mq/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,15 @@
         Logs: LogsTypeDef = ...,
         MaintenanceWindowStartTime: WeeklyStartTimeTypeDef = ...,
         SecurityGroups: Sequence[str] = ...,
         StorageType: BrokerStorageTypeType = ...,
         SubnetIds: Sequence[str] = ...,
         Tags: Mapping[str, str] = ...,
         DataReplicationMode: DataReplicationModeType = ...,
-        DataReplicationPrimaryBrokerArn: str = ...
+        DataReplicationPrimaryBrokerArn: str = ...,
     ) -> CreateBrokerResponseTypeDef:
         """
         Creates a broker.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client.create_broker)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mq/client/#create_broker)
         """
@@ -148,15 +148,15 @@
     async def create_configuration(
         self,
         *,
         EngineType: EngineTypeType,
         EngineVersion: str,
         Name: str,
         AuthenticationStrategy: AuthenticationStrategyType = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateConfigurationResponseTypeDef:
         """
         Creates a new configuration for the specified configuration name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client.create_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mq/client/#create_configuration)
         """
@@ -175,15 +175,15 @@
         self,
         *,
         BrokerId: str,
         Password: str,
         Username: str,
         ConsoleAccess: bool = ...,
         Groups: Sequence[str] = ...,
-        ReplicationUser: bool = ...
+        ReplicationUser: bool = ...,
     ) -> Dict[str, Any]:
         """
         Creates an ActiveMQ user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client.create_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mq/client/#create_user)
         """
@@ -235,15 +235,15 @@
     async def describe_broker_instance_options(
         self,
         *,
         EngineType: str = ...,
         HostInstanceType: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        StorageType: str = ...
+        StorageType: str = ...,
     ) -> DescribeBrokerInstanceOptionsResponseTypeDef:
         """
         Describe available broker instance options.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client.describe_broker_instance_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mq/client/#describe_broker_instance_options)
         """
@@ -363,15 +363,15 @@
         Configuration: ConfigurationIdTypeDef = ...,
         EngineVersion: str = ...,
         HostInstanceType: str = ...,
         LdapServerMetadata: LdapServerMetadataInputTypeDef = ...,
         Logs: LogsTypeDef = ...,
         MaintenanceWindowStartTime: WeeklyStartTimeTypeDef = ...,
         SecurityGroups: Sequence[str] = ...,
-        DataReplicationMode: DataReplicationModeType = ...
+        DataReplicationMode: DataReplicationModeType = ...,
     ) -> UpdateBrokerResponseTypeDef:
         """
         Adds a pending configuration change to a broker.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client.update_broker)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mq/client/#update_broker)
         """
@@ -390,15 +390,15 @@
         self,
         *,
         BrokerId: str,
         Username: str,
         ConsoleAccess: bool = ...,
         Groups: Sequence[str] = ...,
         Password: str = ...,
-        ReplicationUser: bool = ...
+        ReplicationUser: bool = ...,
     ) -> Dict[str, Any]:
         """
         Updates the information for an ActiveMQ user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client.update_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mq/client/#update_user)
         """
```

### Comparing `types-aiobotocore-mq-2.9.0/types_aiobotocore_mq/literals.py` & `types-aiobotocore-mq-2.9.1/types_aiobotocore_mq/literals.py`

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
     "AuthenticationStrategyType",
     "BrokerStateType",
     "BrokerStorageTypeType",
     "ChangeTypeType",
     "DataReplicationModeType",
     "DayOfWeekType",
@@ -35,15 +34,14 @@
     "MQServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AuthenticationStrategyType = Literal["LDAP", "SIMPLE"]
 BrokerStateType = Literal[
     "CREATION_FAILED",
     "CREATION_IN_PROGRESS",
     "CRITICAL_ACTION_REQUIRED",
     "DELETION_IN_PROGRESS",
     "REBOOT_IN_PROGRESS",
```

### Comparing `types-aiobotocore-mq-2.9.0/types_aiobotocore_mq/literals.pyi` & `types-aiobotocore-mq-2.9.1/types_aiobotocore_mq/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mq-2.9.0/types_aiobotocore_mq/paginator.py` & `types-aiobotocore-mq-2.9.1/types_aiobotocore_mq/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .type_defs import ListBrokersResponseTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListBrokersPaginator",)
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
```

### Comparing `types-aiobotocore-mq-2.9.0/types_aiobotocore_mq/paginator.pyi` & `types-aiobotocore-mq-2.9.1/types_aiobotocore_mq/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mq-2.9.0/types_aiobotocore_mq/type_defs.py` & `types-aiobotocore-mq-2.9.1/types_aiobotocore_mq/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ActionRequiredTypeDef",
     "AvailabilityZoneTypeDef",
     "EngineVersionTypeDef",
     "BrokerInstanceTypeDef",
     "BrokerSummaryTypeDef",
     "ConfigurationIdTypeDef",
```

### Comparing `types-aiobotocore-mq-2.9.0/types_aiobotocore_mq/type_defs.pyi` & `types-aiobotocore-mq-2.9.1/types_aiobotocore_mq/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mq-2.9.0/types_aiobotocore_mq.egg-info/PKG-INFO` & `types-aiobotocore-mq-2.9.1/types_aiobotocore_mq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mq
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.MQ 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.MQ 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mq/
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
 
 <a id="types-aiobotocore-mq"></a>
 
 # types-aiobotocore-mq
 
 [![PyPI - types-aiobotocore-mq](https://img.shields.io/pypi/v/types-aiobotocore-mq.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mq)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mq.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mq)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mq/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mq)](https://pepy.tech/project/types-aiobotocore-mq)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MQ 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ)
+[aiobotocore.MQ 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ)
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
 [types-aiobotocore-mq docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mq/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-mq-2.9.0/types_aiobotocore_mq.egg-info/SOURCES.txt` & `types-aiobotocore-mq-2.9.1/types_aiobotocore_mq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

