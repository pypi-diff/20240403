# Comparing `tmp/types-aiobotocore-firehose-2.9.0.tar.gz` & `tmp/types-aiobotocore-firehose-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-firehose-2.9.0.tar", last modified: Wed Dec 13 19:59:19 2023, max compression
+gzip compressed data, was "types-aiobotocore-firehose-2.9.1.tar", last modified: Thu Jan 18 01:20:43 2024, max compression
```

## Comparing `types-aiobotocore-firehose-2.9.0.tar` & `types-aiobotocore-firehose-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:19.409746 types-aiobotocore-firehose-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:46:15.000000 types-aiobotocore-firehose-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12382 2023-12-13 19:59:19.409746 types-aiobotocore-firehose-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10815 2023-12-13 19:46:15.000000 types-aiobotocore-firehose-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:19.409746 types-aiobotocore-firehose-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2023-12-13 19:46:15.000000 types-aiobotocore-firehose-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:19.409746 types-aiobotocore-firehose-2.9.0/types_aiobotocore_firehose/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2023-12-13 19:46:15.000000 types-aiobotocore-firehose-2.9.0/types_aiobotocore_firehose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2023-12-13 19:46:15.000000 types-aiobotocore-firehose-2.9.0/types_aiobotocore_firehose/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      936 2023-12-13 19:46:15.000000 types-aiobotocore-firehose-2.9.0/types_aiobotocore_firehose/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14222 2023-12-13 19:46:15.000000 types-aiobotocore-firehose-2.9.0/types_aiobotocore_firehose/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14219 2023-12-13 19:46:15.000000 types-aiobotocore-firehose-2.9.0/types_aiobotocore_firehose/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12153 2023-12-13 19:46:15.000000 types-aiobotocore-firehose-2.9.0/types_aiobotocore_firehose/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    12151 2023-12-13 19:46:15.000000 types-aiobotocore-firehose-2.9.0/types_aiobotocore_firehose/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:46:15.000000 types-aiobotocore-firehose-2.9.0/types_aiobotocore_firehose/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    42660 2023-12-13 19:46:16.000000 types-aiobotocore-firehose-2.9.0/types_aiobotocore_firehose/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    42659 2023-12-13 19:46:15.000000 types-aiobotocore-firehose-2.9.0/types_aiobotocore_firehose/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:46:15.000000 types-aiobotocore-firehose-2.9.0/types_aiobotocore_firehose/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:19.409746 types-aiobotocore-firehose-2.9.0/types_aiobotocore_firehose.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12382 2023-12-13 19:59:19.000000 types-aiobotocore-firehose-2.9.0/types_aiobotocore_firehose.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      751 2023-12-13 19:59:19.000000 types-aiobotocore-firehose-2.9.0/types_aiobotocore_firehose.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:19.000000 types-aiobotocore-firehose-2.9.0/types_aiobotocore_firehose.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:19.000000 types-aiobotocore-firehose-2.9.0/types_aiobotocore_firehose.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:19.000000 types-aiobotocore-firehose-2.9.0/types_aiobotocore_firehose.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-13 19:59:19.000000 types-aiobotocore-firehose-2.9.0/types_aiobotocore_firehose.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:43.865328 types-aiobotocore-firehose-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:08:09.000000 types-aiobotocore-firehose-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12402 2024-01-18 01:20:43.865328 types-aiobotocore-firehose-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10815 2024-01-18 01:08:09.000000 types-aiobotocore-firehose-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:43.865328 types-aiobotocore-firehose-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-01-18 01:08:09.000000 types-aiobotocore-firehose-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:43.861328 types-aiobotocore-firehose-2.9.1/types_aiobotocore_firehose/
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-01-18 01:08:09.000000 types-aiobotocore-firehose-2.9.1/types_aiobotocore_firehose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-01-18 01:08:09.000000 types-aiobotocore-firehose-2.9.1/types_aiobotocore_firehose/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-01-18 01:08:09.000000 types-aiobotocore-firehose-2.9.1/types_aiobotocore_firehose/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14226 2024-01-18 01:08:09.000000 types-aiobotocore-firehose-2.9.1/types_aiobotocore_firehose/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14223 2024-01-18 01:08:09.000000 types-aiobotocore-firehose-2.9.1/types_aiobotocore_firehose/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12151 2024-01-18 01:08:09.000000 types-aiobotocore-firehose-2.9.1/types_aiobotocore_firehose/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12151 2024-01-18 01:08:09.000000 types-aiobotocore-firehose-2.9.1/types_aiobotocore_firehose/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:08:09.000000 types-aiobotocore-firehose-2.9.1/types_aiobotocore_firehose/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    42659 2024-01-18 01:08:10.000000 types-aiobotocore-firehose-2.9.1/types_aiobotocore_firehose/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42659 2024-01-18 01:08:09.000000 types-aiobotocore-firehose-2.9.1/types_aiobotocore_firehose/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:08:09.000000 types-aiobotocore-firehose-2.9.1/types_aiobotocore_firehose/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:43.865328 types-aiobotocore-firehose-2.9.1/types_aiobotocore_firehose.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12402 2024-01-18 01:20:43.000000 types-aiobotocore-firehose-2.9.1/types_aiobotocore_firehose.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-01-18 01:20:43.000000 types-aiobotocore-firehose-2.9.1/types_aiobotocore_firehose.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:43.000000 types-aiobotocore-firehose-2.9.1/types_aiobotocore_firehose.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:43.000000 types-aiobotocore-firehose-2.9.1/types_aiobotocore_firehose.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:43.000000 types-aiobotocore-firehose-2.9.1/types_aiobotocore_firehose.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-18 01:20:43.000000 types-aiobotocore-firehose-2.9.1/types_aiobotocore_firehose.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-firehose-2.9.0/LICENSE` & `types-aiobotocore-firehose-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-firehose-2.9.0/PKG-INFO` & `types-aiobotocore-firehose-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-firehose
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Firehose 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Firehose 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/
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
 
 <a id="types-aiobotocore-firehose"></a>
 
 # types-aiobotocore-firehose
 
 [![PyPI - types-aiobotocore-firehose](https://img.shields.io/pypi/v/types-aiobotocore-firehose.svg?color=blue)](https://pypi.org/project/types-aiobotocore-firehose)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-firehose.svg?color=blue)](https://pypi.org/project/types-aiobotocore-firehose)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-firehose)](https://pepy.tech/project/types-aiobotocore-firehose)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Firehose 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose)
+[aiobotocore.Firehose 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose)
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
 [types-aiobotocore-firehose docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-firehose-2.9.0/README.md` & `types-aiobotocore-firehose-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-firehose.svg?color=blue)](https://pypi.org/project/types-aiobotocore-firehose)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-firehose)](https://pepy.tech/project/types-aiobotocore-firehose)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Firehose 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose)
+[aiobotocore.Firehose 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose)
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
 [types-aiobotocore-firehose docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-firehose-2.9.0/setup.py` & `types-aiobotocore-firehose-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-firehose",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_firehose"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Firehose 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.Firehose 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore firehose type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_firehose": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-firehose-2.9.0/types_aiobotocore_firehose/__main__.py` & `types-aiobotocore-firehose-2.9.1/types_aiobotocore_firehose/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Firehose 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Firehose 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose\nOther"
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

### Comparing `types-aiobotocore-firehose-2.9.0/types_aiobotocore_firehose/client.py` & `types-aiobotocore-firehose-2.9.1/types_aiobotocore_firehose/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
         RedshiftDestinationConfiguration: RedshiftDestinationConfigurationTypeDef = ...,
         ElasticsearchDestinationConfiguration: ElasticsearchDestinationConfigurationTypeDef = ...,
         AmazonopensearchserviceDestinationConfiguration: AmazonopensearchserviceDestinationConfigurationTypeDef = ...,
         SplunkDestinationConfiguration: SplunkDestinationConfigurationTypeDef = ...,
         HttpEndpointDestinationConfiguration: HttpEndpointDestinationConfigurationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         AmazonOpenSearchServerlessDestinationConfiguration: AmazonOpenSearchServerlessDestinationConfigurationTypeDef = ...,
-        MSKSourceConfiguration: MSKSourceConfigurationTypeDef = ...
+        MSKSourceConfiguration: MSKSourceConfigurationTypeDef = ...,
     ) -> CreateDeliveryStreamOutputTypeDef:
         """
         Creates a Kinesis Data Firehose delivery stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose.Client.create_delivery_stream)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/client/#create_delivery_stream)
         """
@@ -166,15 +166,15 @@
         """
 
     async def list_delivery_streams(
         self,
         *,
         Limit: int = ...,
         DeliveryStreamType: DeliveryStreamTypeType = ...,
-        ExclusiveStartDeliveryStreamName: str = ...
+        ExclusiveStartDeliveryStreamName: str = ...,
     ) -> ListDeliveryStreamsOutputTypeDef:
         """
         Lists your delivery streams in alphabetical order of their names.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose.Client.list_delivery_streams)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/client/#list_delivery_streams)
         """
@@ -212,15 +212,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/client/#put_record_batch)
         """
 
     async def start_delivery_stream_encryption(
         self,
         *,
         DeliveryStreamName: str,
-        DeliveryStreamEncryptionConfigurationInput: DeliveryStreamEncryptionConfigurationInputTypeDef = ...
+        DeliveryStreamEncryptionConfigurationInput: DeliveryStreamEncryptionConfigurationInputTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Enables server-side encryption (SSE) for the delivery stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose.Client.start_delivery_stream_encryption)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/client/#start_delivery_stream_encryption)
         """
@@ -262,15 +262,15 @@
         S3DestinationUpdate: S3DestinationUpdateTypeDef = ...,
         ExtendedS3DestinationUpdate: ExtendedS3DestinationUpdateTypeDef = ...,
         RedshiftDestinationUpdate: RedshiftDestinationUpdateTypeDef = ...,
         ElasticsearchDestinationUpdate: ElasticsearchDestinationUpdateTypeDef = ...,
         AmazonopensearchserviceDestinationUpdate: AmazonopensearchserviceDestinationUpdateTypeDef = ...,
         SplunkDestinationUpdate: SplunkDestinationUpdateTypeDef = ...,
         HttpEndpointDestinationUpdate: HttpEndpointDestinationUpdateTypeDef = ...,
-        AmazonOpenSearchServerlessDestinationUpdate: AmazonOpenSearchServerlessDestinationUpdateTypeDef = ...
+        AmazonOpenSearchServerlessDestinationUpdate: AmazonOpenSearchServerlessDestinationUpdateTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates the specified destination of the specified delivery stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose.Client.update_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/client/#update_destination)
         """
```

### Comparing `types-aiobotocore-firehose-2.9.0/types_aiobotocore_firehose/client.pyi` & `types-aiobotocore-firehose-2.9.1/types_aiobotocore_firehose/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
         RedshiftDestinationConfiguration: RedshiftDestinationConfigurationTypeDef = ...,
         ElasticsearchDestinationConfiguration: ElasticsearchDestinationConfigurationTypeDef = ...,
         AmazonopensearchserviceDestinationConfiguration: AmazonopensearchserviceDestinationConfigurationTypeDef = ...,
         SplunkDestinationConfiguration: SplunkDestinationConfigurationTypeDef = ...,
         HttpEndpointDestinationConfiguration: HttpEndpointDestinationConfigurationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         AmazonOpenSearchServerlessDestinationConfiguration: AmazonOpenSearchServerlessDestinationConfigurationTypeDef = ...,
-        MSKSourceConfiguration: MSKSourceConfigurationTypeDef = ...
+        MSKSourceConfiguration: MSKSourceConfigurationTypeDef = ...,
     ) -> CreateDeliveryStreamOutputTypeDef:
         """
         Creates a Kinesis Data Firehose delivery stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose.Client.create_delivery_stream)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/client/#create_delivery_stream)
         """
@@ -163,15 +163,15 @@
         """
 
     async def list_delivery_streams(
         self,
         *,
         Limit: int = ...,
         DeliveryStreamType: DeliveryStreamTypeType = ...,
-        ExclusiveStartDeliveryStreamName: str = ...
+        ExclusiveStartDeliveryStreamName: str = ...,
     ) -> ListDeliveryStreamsOutputTypeDef:
         """
         Lists your delivery streams in alphabetical order of their names.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose.Client.list_delivery_streams)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/client/#list_delivery_streams)
         """
@@ -209,15 +209,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/client/#put_record_batch)
         """
 
     async def start_delivery_stream_encryption(
         self,
         *,
         DeliveryStreamName: str,
-        DeliveryStreamEncryptionConfigurationInput: DeliveryStreamEncryptionConfigurationInputTypeDef = ...
+        DeliveryStreamEncryptionConfigurationInput: DeliveryStreamEncryptionConfigurationInputTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Enables server-side encryption (SSE) for the delivery stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose.Client.start_delivery_stream_encryption)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/client/#start_delivery_stream_encryption)
         """
@@ -259,15 +259,15 @@
         S3DestinationUpdate: S3DestinationUpdateTypeDef = ...,
         ExtendedS3DestinationUpdate: ExtendedS3DestinationUpdateTypeDef = ...,
         RedshiftDestinationUpdate: RedshiftDestinationUpdateTypeDef = ...,
         ElasticsearchDestinationUpdate: ElasticsearchDestinationUpdateTypeDef = ...,
         AmazonopensearchserviceDestinationUpdate: AmazonopensearchserviceDestinationUpdateTypeDef = ...,
         SplunkDestinationUpdate: SplunkDestinationUpdateTypeDef = ...,
         HttpEndpointDestinationUpdate: HttpEndpointDestinationUpdateTypeDef = ...,
-        AmazonOpenSearchServerlessDestinationUpdate: AmazonOpenSearchServerlessDestinationUpdateTypeDef = ...
+        AmazonOpenSearchServerlessDestinationUpdate: AmazonOpenSearchServerlessDestinationUpdateTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates the specified destination of the specified delivery stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose.Client.update_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/client/#update_destination)
         """
```

### Comparing `types-aiobotocore-firehose-2.9.0/types_aiobotocore_firehose/literals.py` & `types-aiobotocore-firehose-2.9.1/types_aiobotocore_firehose/literals.py`

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
     "AmazonOpenSearchServerlessS3BackupModeType",
     "AmazonopensearchserviceIndexRotationPeriodType",
     "AmazonopensearchserviceS3BackupModeType",
     "CompressionFormatType",
     "ConnectivityType",
     "ContentEncodingType",
@@ -49,15 +48,14 @@
     "SplunkS3BackupModeType",
     "FirehoseServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 AmazonOpenSearchServerlessS3BackupModeType = Literal["AllDocuments", "FailedDocumentsOnly"]
 AmazonopensearchserviceIndexRotationPeriodType = Literal[
     "NoRotation", "OneDay", "OneHour", "OneMonth", "OneWeek"
 ]
 AmazonopensearchserviceS3BackupModeType = Literal["AllDocuments", "FailedDocumentsOnly"]
 CompressionFormatType = Literal["GZIP", "HADOOP_SNAPPY", "Snappy", "UNCOMPRESSED", "ZIP"]
 ConnectivityType = Literal["PRIVATE", "PUBLIC"]
```

### Comparing `types-aiobotocore-firehose-2.9.0/types_aiobotocore_firehose/literals.pyi` & `types-aiobotocore-firehose-2.9.1/types_aiobotocore_firehose/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-firehose-2.9.0/types_aiobotocore_firehose/type_defs.py` & `types-aiobotocore-firehose-2.9.1/types_aiobotocore_firehose/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AmazonOpenSearchServerlessBufferingHintsTypeDef",
     "AmazonOpenSearchServerlessRetryOptionsTypeDef",
     "CloudWatchLoggingOptionsTypeDef",
     "VpcConfigurationTypeDef",
     "VpcConfigurationDescriptionTypeDef",
     "AmazonopensearchserviceBufferingHintsTypeDef",
```

### Comparing `types-aiobotocore-firehose-2.9.0/types_aiobotocore_firehose/type_defs.pyi` & `types-aiobotocore-firehose-2.9.1/types_aiobotocore_firehose/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-firehose-2.9.0/types_aiobotocore_firehose.egg-info/PKG-INFO` & `types-aiobotocore-firehose-2.9.1/types_aiobotocore_firehose.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-firehose
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Firehose 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Firehose 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/
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
 
 <a id="types-aiobotocore-firehose"></a>
 
 # types-aiobotocore-firehose
 
 [![PyPI - types-aiobotocore-firehose](https://img.shields.io/pypi/v/types-aiobotocore-firehose.svg?color=blue)](https://pypi.org/project/types-aiobotocore-firehose)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-firehose.svg?color=blue)](https://pypi.org/project/types-aiobotocore-firehose)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-firehose)](https://pepy.tech/project/types-aiobotocore-firehose)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Firehose 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose)
+[aiobotocore.Firehose 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose)
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
 [types-aiobotocore-firehose docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-firehose-2.9.0/types_aiobotocore_firehose.egg-info/SOURCES.txt` & `types-aiobotocore-firehose-2.9.1/types_aiobotocore_firehose.egg-info/SOURCES.txt`

 * *Files identical despite different names*

