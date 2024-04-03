# Comparing `tmp/types-aiobotocore-kafka-2.9.0.tar.gz` & `tmp/types-aiobotocore-kafka-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-kafka-2.9.0.tar", last modified: Wed Dec 13 19:59:37 2023, max compression
+gzip compressed data, was "types-aiobotocore-kafka-2.9.1.tar", last modified: Thu Jan 18 01:21:00 2024, max compression
```

## Comparing `types-aiobotocore-kafka-2.9.0.tar` & `types-aiobotocore-kafka-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:37.377594 types-aiobotocore-kafka-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:48:19.000000 types-aiobotocore-kafka-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14545 2023-12-13 19:59:37.377594 types-aiobotocore-kafka-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12990 2023-12-13 19:48:19.000000 types-aiobotocore-kafka-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:37.377594 types-aiobotocore-kafka-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2023-12-13 19:48:19.000000 types-aiobotocore-kafka-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:37.377594 types-aiobotocore-kafka-2.9.0/types_aiobotocore_kafka/
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2023-12-13 19:48:19.000000 types-aiobotocore-kafka-2.9.0/types_aiobotocore_kafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2023-12-13 19:48:19.000000 types-aiobotocore-kafka-2.9.0/types_aiobotocore_kafka/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      913 2023-12-13 19:48:19.000000 types-aiobotocore-kafka-2.9.0/types_aiobotocore_kafka/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42580 2023-12-13 19:48:20.000000 types-aiobotocore-kafka-2.9.0/types_aiobotocore_kafka/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    42576 2023-12-13 19:48:20.000000 types-aiobotocore-kafka-2.9.0/types_aiobotocore_kafka/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11812 2023-12-13 19:48:20.000000 types-aiobotocore-kafka-2.9.0/types_aiobotocore_kafka/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11810 2023-12-13 19:48:20.000000 types-aiobotocore-kafka-2.9.0/types_aiobotocore_kafka/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14343 2023-12-13 19:48:20.000000 types-aiobotocore-kafka-2.9.0/types_aiobotocore_kafka/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    14329 2023-12-13 19:48:20.000000 types-aiobotocore-kafka-2.9.0/types_aiobotocore_kafka/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:48:19.000000 types-aiobotocore-kafka-2.9.0/types_aiobotocore_kafka/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    65347 2023-12-13 19:48:22.000000 types-aiobotocore-kafka-2.9.0/types_aiobotocore_kafka/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    65346 2023-12-13 19:48:22.000000 types-aiobotocore-kafka-2.9.0/types_aiobotocore_kafka/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:48:19.000000 types-aiobotocore-kafka-2.9.0/types_aiobotocore_kafka/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:37.377594 types-aiobotocore-kafka-2.9.0/types_aiobotocore_kafka.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14545 2023-12-13 19:59:37.000000 types-aiobotocore-kafka-2.9.0/types_aiobotocore_kafka.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      775 2023-12-13 19:59:37.000000 types-aiobotocore-kafka-2.9.0/types_aiobotocore_kafka.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:37.000000 types-aiobotocore-kafka-2.9.0/types_aiobotocore_kafka.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:37.000000 types-aiobotocore-kafka-2.9.0/types_aiobotocore_kafka.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:37.000000 types-aiobotocore-kafka-2.9.0/types_aiobotocore_kafka.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-13 19:59:37.000000 types-aiobotocore-kafka-2.9.0/types_aiobotocore_kafka.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:00.473252 types-aiobotocore-kafka-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:10:09.000000 types-aiobotocore-kafka-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14565 2024-01-18 01:21:00.473252 types-aiobotocore-kafka-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12990 2024-01-18 01:10:09.000000 types-aiobotocore-kafka-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:00.473252 types-aiobotocore-kafka-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-01-18 01:10:09.000000 types-aiobotocore-kafka-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:00.473252 types-aiobotocore-kafka-2.9.1/types_aiobotocore_kafka/
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-01-18 01:10:09.000000 types-aiobotocore-kafka-2.9.1/types_aiobotocore_kafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-01-18 01:10:09.000000 types-aiobotocore-kafka-2.9.1/types_aiobotocore_kafka/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-01-18 01:10:09.000000 types-aiobotocore-kafka-2.9.1/types_aiobotocore_kafka/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42591 2024-01-18 01:10:10.000000 types-aiobotocore-kafka-2.9.1/types_aiobotocore_kafka/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42588 2024-01-18 01:10:09.000000 types-aiobotocore-kafka-2.9.1/types_aiobotocore_kafka/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11810 2024-01-18 01:10:10.000000 types-aiobotocore-kafka-2.9.1/types_aiobotocore_kafka/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11810 2024-01-18 01:10:10.000000 types-aiobotocore-kafka-2.9.1/types_aiobotocore_kafka/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14343 2024-01-18 01:10:10.000000 types-aiobotocore-kafka-2.9.1/types_aiobotocore_kafka/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14330 2024-01-18 01:10:10.000000 types-aiobotocore-kafka-2.9.1/types_aiobotocore_kafka/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:10:09.000000 types-aiobotocore-kafka-2.9.1/types_aiobotocore_kafka/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    65346 2024-01-18 01:10:11.000000 types-aiobotocore-kafka-2.9.1/types_aiobotocore_kafka/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65346 2024-01-18 01:10:11.000000 types-aiobotocore-kafka-2.9.1/types_aiobotocore_kafka/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:10:09.000000 types-aiobotocore-kafka-2.9.1/types_aiobotocore_kafka/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:00.473252 types-aiobotocore-kafka-2.9.1/types_aiobotocore_kafka.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14565 2024-01-18 01:21:00.000000 types-aiobotocore-kafka-2.9.1/types_aiobotocore_kafka.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-01-18 01:21:00.000000 types-aiobotocore-kafka-2.9.1/types_aiobotocore_kafka.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:00.000000 types-aiobotocore-kafka-2.9.1/types_aiobotocore_kafka.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:00.000000 types-aiobotocore-kafka-2.9.1/types_aiobotocore_kafka.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:00.000000 types-aiobotocore-kafka-2.9.1/types_aiobotocore_kafka.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-01-18 01:21:00.000000 types-aiobotocore-kafka-2.9.1/types_aiobotocore_kafka.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-kafka-2.9.0/LICENSE` & `types-aiobotocore-kafka-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-kafka-2.9.0/PKG-INFO` & `types-aiobotocore-kafka-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kafka
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Kafka 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Kafka 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/
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
 
 <a id="types-aiobotocore-kafka"></a>
 
 # types-aiobotocore-kafka
 
 [![PyPI - types-aiobotocore-kafka](https://img.shields.io/pypi/v/types-aiobotocore-kafka.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kafka)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kafka.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kafka)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kafka)](https://pepy.tech/project/types-aiobotocore-kafka)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Kafka 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka)
+[aiobotocore.Kafka 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka)
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
 [types-aiobotocore-kafka docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-kafka-2.9.0/README.md` & `types-aiobotocore-kafka-2.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kafka.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kafka)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kafka)](https://pepy.tech/project/types-aiobotocore-kafka)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Kafka 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka)
+[aiobotocore.Kafka 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka)
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
 [types-aiobotocore-kafka docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-kafka-2.9.0/setup.py` & `types-aiobotocore-kafka-2.9.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-kafka",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_kafka"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Kafka 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.Kafka 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore kafka type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_kafka": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-kafka-2.9.0/types_aiobotocore_kafka/__init__.py` & `types-aiobotocore-kafka-2.9.1/types_aiobotocore_kafka/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,14 @@
     ListReplicatorsPaginator,
     ListScramSecretsPaginator,
     ListVpcConnectionsPaginator,
 )
 
 Client = KafkaClient
 
-
 __all__ = (
     "Client",
     "KafkaClient",
     "ListClientVpcConnectionsPaginator",
     "ListClusterOperationsPaginator",
     "ListClusterOperationsV2Paginator",
     "ListClustersPaginator",
```

### Comparing `types-aiobotocore-kafka-2.9.0/types_aiobotocore_kafka/__init__.pyi` & `types-aiobotocore-kafka-2.9.1/types_aiobotocore_kafka/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kafka-2.9.0/types_aiobotocore_kafka/__main__.py` & `types-aiobotocore-kafka-2.9.1/types_aiobotocore_kafka/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Kafka 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Kafka 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka\nOther"
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

### Comparing `types-aiobotocore-kafka-2.9.0/types_aiobotocore_kafka/client.py` & `types-aiobotocore-kafka-2.9.1/types_aiobotocore_kafka/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("KafkaClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -196,45 +195,45 @@
         ClientAuthentication: ClientAuthenticationTypeDef = ...,
         ConfigurationInfo: ConfigurationInfoTypeDef = ...,
         EncryptionInfo: EncryptionInfoTypeDef = ...,
         EnhancedMonitoring: EnhancedMonitoringType = ...,
         OpenMonitoring: OpenMonitoringInfoTypeDef = ...,
         LoggingInfo: LoggingInfoTypeDef = ...,
         Tags: Mapping[str, str] = ...,
-        StorageMode: StorageModeType = ...
+        StorageMode: StorageModeType = ...,
     ) -> CreateClusterResponseTypeDef:
         """
         Creates a new MSK cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.create_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/client/#create_cluster)
         """
 
     async def create_cluster_v2(
         self,
         *,
         ClusterName: str,
         Tags: Mapping[str, str] = ...,
         Provisioned: ProvisionedRequestTypeDef = ...,
-        Serverless: ServerlessRequestTypeDef = ...
+        Serverless: ServerlessRequestTypeDef = ...,
     ) -> CreateClusterV2ResponseTypeDef:
         """
         Creates a new MSK cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.create_cluster_v2)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/client/#create_cluster_v2)
         """
 
     async def create_configuration(
         self,
         *,
         Name: str,
         ServerProperties: BlobTypeDef,
         Description: str = ...,
-        KafkaVersions: Sequence[str] = ...
+        KafkaVersions: Sequence[str] = ...,
     ) -> CreateConfigurationResponseTypeDef:
         """
         Creates a new MSK configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.create_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/client/#create_configuration)
         """
@@ -243,15 +242,15 @@
         self,
         *,
         KafkaClusters: Sequence[KafkaClusterTypeDef],
         ReplicationInfoList: Sequence[ReplicationInfoTypeDef],
         ReplicatorName: str,
         ServiceExecutionRoleArn: str,
         Description: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateReplicatorResponseTypeDef:
         """
         Creates the replicator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.create_replicator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/client/#create_replicator)
         """
@@ -260,15 +259,15 @@
         self,
         *,
         TargetClusterArn: str,
         Authentication: str,
         VpcId: str,
         ClientSubnets: Sequence[str],
         SecurityGroups: Sequence[str],
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateVpcConnectionResponseTypeDef:
         """
         Creates a new MSK VPC connection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.create_vpc_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/client/#create_vpc_connection)
         """
@@ -481,15 +480,15 @@
 
     async def list_clusters_v2(
         self,
         *,
         ClusterNameFilter: str = ...,
         ClusterTypeFilter: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListClustersV2ResponseTypeDef:
         """
         Returns a list of all the MSK clusters in the current Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.list_clusters_v2)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/client/#list_clusters_v2)
         """
@@ -637,15 +636,15 @@
         """
 
     async def update_broker_storage(
         self,
         *,
         ClusterArn: str,
         CurrentVersion: str,
-        TargetBrokerEBSVolumeInfo: Sequence[BrokerEBSVolumeInfoTypeDef]
+        TargetBrokerEBSVolumeInfo: Sequence[BrokerEBSVolumeInfoTypeDef],
     ) -> UpdateBrokerStorageResponseTypeDef:
         """
         Updates the EBS storage associated with MSK brokers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.update_broker_storage)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/client/#update_broker_storage)
         """
@@ -673,15 +672,15 @@
 
     async def update_cluster_kafka_version(
         self,
         *,
         ClusterArn: str,
         CurrentVersion: str,
         TargetKafkaVersion: str,
-        ConfigurationInfo: ConfigurationInfoTypeDef = ...
+        ConfigurationInfo: ConfigurationInfoTypeDef = ...,
     ) -> UpdateClusterKafkaVersionResponseTypeDef:
         """
         Updates the Apache Kafka version for the cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.update_cluster_kafka_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/client/#update_cluster_kafka_version)
         """
@@ -709,15 +708,15 @@
     async def update_monitoring(
         self,
         *,
         ClusterArn: str,
         CurrentVersion: str,
         EnhancedMonitoring: EnhancedMonitoringType = ...,
         OpenMonitoring: OpenMonitoringInfoTypeDef = ...,
-        LoggingInfo: LoggingInfoTypeDef = ...
+        LoggingInfo: LoggingInfoTypeDef = ...,
     ) -> UpdateMonitoringResponseTypeDef:
         """
         Updates the monitoring settings for the cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.update_monitoring)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/client/#update_monitoring)
         """
@@ -726,30 +725,30 @@
         self,
         *,
         CurrentVersion: str,
         ReplicatorArn: str,
         SourceKafkaClusterArn: str,
         TargetKafkaClusterArn: str,
         ConsumerGroupReplication: ConsumerGroupReplicationUpdateTypeDef = ...,
-        TopicReplication: TopicReplicationUpdateTypeDef = ...
+        TopicReplication: TopicReplicationUpdateTypeDef = ...,
     ) -> UpdateReplicationInfoResponseTypeDef:
         """
         Updates replication info of a replicator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.update_replication_info)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/client/#update_replication_info)
         """
 
     async def update_security(
         self,
         *,
         ClusterArn: str,
         CurrentVersion: str,
         ClientAuthentication: ClientAuthenticationTypeDef = ...,
-        EncryptionInfo: EncryptionInfoTypeDef = ...
+        EncryptionInfo: EncryptionInfoTypeDef = ...,
     ) -> UpdateSecurityResponseTypeDef:
         """
         Updates the security settings for the cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.update_security)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/client/#update_security)
         """
@@ -757,15 +756,15 @@
     async def update_storage(
         self,
         *,
         ClusterArn: str,
         CurrentVersion: str,
         ProvisionedThroughput: ProvisionedThroughputTypeDef = ...,
         StorageMode: StorageModeType = ...,
-        VolumeSizeGB: int = ...
+        VolumeSizeGB: int = ...,
     ) -> UpdateStorageResponseTypeDef:
         """
         Updates cluster broker volume size (or) sets cluster storage mode to TIERED.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.update_storage)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/client/#update_storage)
         """
```

### Comparing `types-aiobotocore-kafka-2.9.0/types_aiobotocore_kafka/client.pyi` & `types-aiobotocore-kafka-2.9.1/types_aiobotocore_kafka/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -192,45 +192,45 @@
         ClientAuthentication: ClientAuthenticationTypeDef = ...,
         ConfigurationInfo: ConfigurationInfoTypeDef = ...,
         EncryptionInfo: EncryptionInfoTypeDef = ...,
         EnhancedMonitoring: EnhancedMonitoringType = ...,
         OpenMonitoring: OpenMonitoringInfoTypeDef = ...,
         LoggingInfo: LoggingInfoTypeDef = ...,
         Tags: Mapping[str, str] = ...,
-        StorageMode: StorageModeType = ...
+        StorageMode: StorageModeType = ...,
     ) -> CreateClusterResponseTypeDef:
         """
         Creates a new MSK cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.create_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/client/#create_cluster)
         """
 
     async def create_cluster_v2(
         self,
         *,
         ClusterName: str,
         Tags: Mapping[str, str] = ...,
         Provisioned: ProvisionedRequestTypeDef = ...,
-        Serverless: ServerlessRequestTypeDef = ...
+        Serverless: ServerlessRequestTypeDef = ...,
     ) -> CreateClusterV2ResponseTypeDef:
         """
         Creates a new MSK cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.create_cluster_v2)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/client/#create_cluster_v2)
         """
 
     async def create_configuration(
         self,
         *,
         Name: str,
         ServerProperties: BlobTypeDef,
         Description: str = ...,
-        KafkaVersions: Sequence[str] = ...
+        KafkaVersions: Sequence[str] = ...,
     ) -> CreateConfigurationResponseTypeDef:
         """
         Creates a new MSK configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.create_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/client/#create_configuration)
         """
@@ -239,15 +239,15 @@
         self,
         *,
         KafkaClusters: Sequence[KafkaClusterTypeDef],
         ReplicationInfoList: Sequence[ReplicationInfoTypeDef],
         ReplicatorName: str,
         ServiceExecutionRoleArn: str,
         Description: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateReplicatorResponseTypeDef:
         """
         Creates the replicator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.create_replicator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/client/#create_replicator)
         """
@@ -256,15 +256,15 @@
         self,
         *,
         TargetClusterArn: str,
         Authentication: str,
         VpcId: str,
         ClientSubnets: Sequence[str],
         SecurityGroups: Sequence[str],
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateVpcConnectionResponseTypeDef:
         """
         Creates a new MSK VPC connection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.create_vpc_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/client/#create_vpc_connection)
         """
@@ -477,15 +477,15 @@
 
     async def list_clusters_v2(
         self,
         *,
         ClusterNameFilter: str = ...,
         ClusterTypeFilter: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListClustersV2ResponseTypeDef:
         """
         Returns a list of all the MSK clusters in the current Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.list_clusters_v2)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/client/#list_clusters_v2)
         """
@@ -633,15 +633,15 @@
         """
 
     async def update_broker_storage(
         self,
         *,
         ClusterArn: str,
         CurrentVersion: str,
-        TargetBrokerEBSVolumeInfo: Sequence[BrokerEBSVolumeInfoTypeDef]
+        TargetBrokerEBSVolumeInfo: Sequence[BrokerEBSVolumeInfoTypeDef],
     ) -> UpdateBrokerStorageResponseTypeDef:
         """
         Updates the EBS storage associated with MSK brokers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.update_broker_storage)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/client/#update_broker_storage)
         """
@@ -669,15 +669,15 @@
 
     async def update_cluster_kafka_version(
         self,
         *,
         ClusterArn: str,
         CurrentVersion: str,
         TargetKafkaVersion: str,
-        ConfigurationInfo: ConfigurationInfoTypeDef = ...
+        ConfigurationInfo: ConfigurationInfoTypeDef = ...,
     ) -> UpdateClusterKafkaVersionResponseTypeDef:
         """
         Updates the Apache Kafka version for the cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.update_cluster_kafka_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/client/#update_cluster_kafka_version)
         """
@@ -705,15 +705,15 @@
     async def update_monitoring(
         self,
         *,
         ClusterArn: str,
         CurrentVersion: str,
         EnhancedMonitoring: EnhancedMonitoringType = ...,
         OpenMonitoring: OpenMonitoringInfoTypeDef = ...,
-        LoggingInfo: LoggingInfoTypeDef = ...
+        LoggingInfo: LoggingInfoTypeDef = ...,
     ) -> UpdateMonitoringResponseTypeDef:
         """
         Updates the monitoring settings for the cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.update_monitoring)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/client/#update_monitoring)
         """
@@ -722,30 +722,30 @@
         self,
         *,
         CurrentVersion: str,
         ReplicatorArn: str,
         SourceKafkaClusterArn: str,
         TargetKafkaClusterArn: str,
         ConsumerGroupReplication: ConsumerGroupReplicationUpdateTypeDef = ...,
-        TopicReplication: TopicReplicationUpdateTypeDef = ...
+        TopicReplication: TopicReplicationUpdateTypeDef = ...,
     ) -> UpdateReplicationInfoResponseTypeDef:
         """
         Updates replication info of a replicator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.update_replication_info)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/client/#update_replication_info)
         """
 
     async def update_security(
         self,
         *,
         ClusterArn: str,
         CurrentVersion: str,
         ClientAuthentication: ClientAuthenticationTypeDef = ...,
-        EncryptionInfo: EncryptionInfoTypeDef = ...
+        EncryptionInfo: EncryptionInfoTypeDef = ...,
     ) -> UpdateSecurityResponseTypeDef:
         """
         Updates the security settings for the cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.update_security)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/client/#update_security)
         """
@@ -753,15 +753,15 @@
     async def update_storage(
         self,
         *,
         ClusterArn: str,
         CurrentVersion: str,
         ProvisionedThroughput: ProvisionedThroughputTypeDef = ...,
         StorageMode: StorageModeType = ...,
-        VolumeSizeGB: int = ...
+        VolumeSizeGB: int = ...,
     ) -> UpdateStorageResponseTypeDef:
         """
         Updates cluster broker volume size (or) sets cluster storage mode to TIERED.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.update_storage)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/client/#update_storage)
         """
```

### Comparing `types-aiobotocore-kafka-2.9.0/types_aiobotocore_kafka/literals.py` & `types-aiobotocore-kafka-2.9.1/types_aiobotocore_kafka/literals.py`

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
     "BrokerAZDistributionType",
     "ClientBrokerType",
     "ClusterStateType",
     "ClusterTypeType",
     "ConfigurationStateType",
     "CustomerActionStatusType",
@@ -50,15 +49,14 @@
     "KafkaServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 BrokerAZDistributionType = Literal["DEFAULT"]
 ClientBrokerType = Literal["PLAINTEXT", "TLS", "TLS_PLAINTEXT"]
 ClusterStateType = Literal[
     "ACTIVE",
     "CREATING",
     "DELETING",
     "FAILED",
```

### Comparing `types-aiobotocore-kafka-2.9.0/types_aiobotocore_kafka/literals.pyi` & `types-aiobotocore-kafka-2.9.1/types_aiobotocore_kafka/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kafka-2.9.0/types_aiobotocore_kafka/paginator.py` & `types-aiobotocore-kafka-2.9.1/types_aiobotocore_kafka/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,14 @@
     "ListKafkaVersionsPaginator",
     "ListNodesPaginator",
     "ListReplicatorsPaginator",
     "ListScramSecretsPaginator",
     "ListVpcConnectionsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -157,15 +156,15 @@
     """
 
     def paginate(
         self,
         *,
         ClusterNameFilter: str = ...,
         ClusterTypeFilter: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListClustersV2ResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClustersV2.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/paginators/#listclustersv2paginator)
         """
```

### Comparing `types-aiobotocore-kafka-2.9.0/types_aiobotocore_kafka/paginator.pyi` & `types-aiobotocore-kafka-2.9.1/types_aiobotocore_kafka/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,15 @@
     """
 
     def paginate(
         self,
         *,
         ClusterNameFilter: str = ...,
         ClusterTypeFilter: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListClustersV2ResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClustersV2.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/paginators/#listclustersv2paginator)
         """
 
 class ListConfigurationRevisionsPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-kafka-2.9.0/types_aiobotocore_kafka/type_defs.py` & `types-aiobotocore-kafka-2.9.1/types_aiobotocore_kafka/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AmazonMskClusterTypeDef",
     "BatchAssociateScramSecretRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "UnprocessedScramSecretTypeDef",
     "BatchDisassociateScramSecretRequestRequestTypeDef",
     "BlobTypeDef",
```

### Comparing `types-aiobotocore-kafka-2.9.0/types_aiobotocore_kafka/type_defs.pyi` & `types-aiobotocore-kafka-2.9.1/types_aiobotocore_kafka/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kafka-2.9.0/types_aiobotocore_kafka.egg-info/PKG-INFO` & `types-aiobotocore-kafka-2.9.1/types_aiobotocore_kafka.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kafka
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Kafka 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Kafka 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/
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
 
 <a id="types-aiobotocore-kafka"></a>
 
 # types-aiobotocore-kafka
 
 [![PyPI - types-aiobotocore-kafka](https://img.shields.io/pypi/v/types-aiobotocore-kafka.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kafka)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kafka.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kafka)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kafka)](https://pepy.tech/project/types-aiobotocore-kafka)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Kafka 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka)
+[aiobotocore.Kafka 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka)
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
 [types-aiobotocore-kafka docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-kafka-2.9.0/types_aiobotocore_kafka.egg-info/SOURCES.txt` & `types-aiobotocore-kafka-2.9.1/types_aiobotocore_kafka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

