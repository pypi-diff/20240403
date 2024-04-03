# Comparing `tmp/types-aiobotocore-timestream-write-2.9.0.tar.gz` & `tmp/types-aiobotocore-timestream-write-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-timestream-write-2.9.0.tar", last modified: Wed Dec 13 20:00:41 2023, max compression
+gzip compressed data, was "types-aiobotocore-timestream-write-2.9.1.tar", last modified: Thu Jan 18 01:21:58 2024, max compression
```

## Comparing `types-aiobotocore-timestream-write-2.9.0.tar` & `types-aiobotocore-timestream-write-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:41.117047 types-aiobotocore-timestream-write-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:57:21.000000 types-aiobotocore-timestream-write-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12725 2023-12-13 20:00:41.117047 types-aiobotocore-timestream-write-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11127 2023-12-13 19:57:21.000000 types-aiobotocore-timestream-write-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:41.117047 types-aiobotocore-timestream-write-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2023-12-13 19:57:21.000000 types-aiobotocore-timestream-write-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:41.117047 types-aiobotocore-timestream-write-2.9.0/types_aiobotocore_timestream_write/
--rw-r--r--   0 runner    (1001) docker     (127)      510 2023-12-13 19:57:21.000000 types-aiobotocore-timestream-write-2.9.0/types_aiobotocore_timestream_write/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2023-12-13 19:57:21.000000 types-aiobotocore-timestream-write-2.9.0/types_aiobotocore_timestream_write/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      966 2023-12-13 19:57:21.000000 types-aiobotocore-timestream-write-2.9.0/types_aiobotocore_timestream_write/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16922 2023-12-13 19:57:21.000000 types-aiobotocore-timestream-write-2.9.0/types_aiobotocore_timestream_write/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    16919 2023-12-13 19:57:21.000000 types-aiobotocore-timestream-write-2.9.0/types_aiobotocore_timestream_write/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9324 2023-12-13 19:57:21.000000 types-aiobotocore-timestream-write-2.9.0/types_aiobotocore_timestream_write/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9322 2023-12-13 19:57:21.000000 types-aiobotocore-timestream-write-2.9.0/types_aiobotocore_timestream_write/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:57:21.000000 types-aiobotocore-timestream-write-2.9.0/types_aiobotocore_timestream_write/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    18300 2023-12-13 19:57:21.000000 types-aiobotocore-timestream-write-2.9.0/types_aiobotocore_timestream_write/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18299 2023-12-13 19:57:21.000000 types-aiobotocore-timestream-write-2.9.0/types_aiobotocore_timestream_write/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:57:21.000000 types-aiobotocore-timestream-write-2.9.0/types_aiobotocore_timestream_write/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:41.117047 types-aiobotocore-timestream-write-2.9.0/types_aiobotocore_timestream_write.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12725 2023-12-13 20:00:41.000000 types-aiobotocore-timestream-write-2.9.0/types_aiobotocore_timestream_write.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      887 2023-12-13 20:00:41.000000 types-aiobotocore-timestream-write-2.9.0/types_aiobotocore_timestream_write.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:41.000000 types-aiobotocore-timestream-write-2.9.0/types_aiobotocore_timestream_write.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:41.000000 types-aiobotocore-timestream-write-2.9.0/types_aiobotocore_timestream_write.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:41.000000 types-aiobotocore-timestream-write-2.9.0/types_aiobotocore_timestream_write.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-13 20:00:41.000000 types-aiobotocore-timestream-write-2.9.0/types_aiobotocore_timestream_write.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:58.516990 types-aiobotocore-timestream-write-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:18:49.000000 types-aiobotocore-timestream-write-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12745 2024-01-18 01:21:58.516990 types-aiobotocore-timestream-write-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11127 2024-01-18 01:18:49.000000 types-aiobotocore-timestream-write-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:58.516990 types-aiobotocore-timestream-write-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-01-18 01:18:49.000000 types-aiobotocore-timestream-write-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:58.512990 types-aiobotocore-timestream-write-2.9.1/types_aiobotocore_timestream_write/
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-01-18 01:18:49.000000 types-aiobotocore-timestream-write-2.9.1/types_aiobotocore_timestream_write/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-01-18 01:18:49.000000 types-aiobotocore-timestream-write-2.9.1/types_aiobotocore_timestream_write/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-01-18 01:18:49.000000 types-aiobotocore-timestream-write-2.9.1/types_aiobotocore_timestream_write/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16926 2024-01-18 01:18:49.000000 types-aiobotocore-timestream-write-2.9.1/types_aiobotocore_timestream_write/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16923 2024-01-18 01:18:49.000000 types-aiobotocore-timestream-write-2.9.1/types_aiobotocore_timestream_write/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9322 2024-01-18 01:18:49.000000 types-aiobotocore-timestream-write-2.9.1/types_aiobotocore_timestream_write/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9322 2024-01-18 01:18:49.000000 types-aiobotocore-timestream-write-2.9.1/types_aiobotocore_timestream_write/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:18:49.000000 types-aiobotocore-timestream-write-2.9.1/types_aiobotocore_timestream_write/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    18299 2024-01-18 01:18:50.000000 types-aiobotocore-timestream-write-2.9.1/types_aiobotocore_timestream_write/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18299 2024-01-18 01:18:50.000000 types-aiobotocore-timestream-write-2.9.1/types_aiobotocore_timestream_write/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:18:49.000000 types-aiobotocore-timestream-write-2.9.1/types_aiobotocore_timestream_write/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:58.512990 types-aiobotocore-timestream-write-2.9.1/types_aiobotocore_timestream_write.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12745 2024-01-18 01:21:58.000000 types-aiobotocore-timestream-write-2.9.1/types_aiobotocore_timestream_write.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-01-18 01:21:58.000000 types-aiobotocore-timestream-write-2.9.1/types_aiobotocore_timestream_write.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:58.000000 types-aiobotocore-timestream-write-2.9.1/types_aiobotocore_timestream_write.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:58.000000 types-aiobotocore-timestream-write-2.9.1/types_aiobotocore_timestream_write.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:58.000000 types-aiobotocore-timestream-write-2.9.1/types_aiobotocore_timestream_write.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-18 01:21:58.000000 types-aiobotocore-timestream-write-2.9.1/types_aiobotocore_timestream_write.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-timestream-write-2.9.0/LICENSE` & `types-aiobotocore-timestream-write-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-timestream-write-2.9.0/PKG-INFO` & `types-aiobotocore-timestream-write-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-timestream-write
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.TimestreamWrite 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.TimestreamWrite 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_write/
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
 
 <a id="types-aiobotocore-timestream-write"></a>
 
 # types-aiobotocore-timestream-write
 
 [![PyPI - types-aiobotocore-timestream-write](https://img.shields.io/pypi/v/types-aiobotocore-timestream-write.svg?color=blue)](https://pypi.org/project/types-aiobotocore-timestream-write)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-timestream-write.svg?color=blue)](https://pypi.org/project/types-aiobotocore-timestream-write)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_write/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-timestream-write)](https://pepy.tech/project/types-aiobotocore-timestream-write)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.TimestreamWrite 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite)
+[aiobotocore.TimestreamWrite 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite)
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
 [types-aiobotocore-timestream-write docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_write/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-timestream-write-2.9.0/README.md` & `types-aiobotocore-timestream-write-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-timestream-write.svg?color=blue)](https://pypi.org/project/types-aiobotocore-timestream-write)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_write/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-timestream-write)](https://pepy.tech/project/types-aiobotocore-timestream-write)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.TimestreamWrite 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite)
+[aiobotocore.TimestreamWrite 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite)
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
 [types-aiobotocore-timestream-write docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_write/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-timestream-write-2.9.0/setup.py` & `types-aiobotocore-timestream-write-2.9.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-timestream-write",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_timestream_write"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.TimestreamWrite 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.TimestreamWrite 2.9.1 service generated with"
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
     keywords="aiobotocore timestream-write type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_timestream_write": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_write/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-timestream-write-2.9.0/types_aiobotocore_timestream_write/__main__.py` & `types-aiobotocore-timestream-write-2.9.1/types_aiobotocore_timestream_write/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.TimestreamWrite 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.TimestreamWrite 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_write//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite\nOther"
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

### Comparing `types-aiobotocore-timestream-write-2.9.0/types_aiobotocore_timestream_write/client.py` & `types-aiobotocore-timestream-write-2.9.1/types_aiobotocore_timestream_write/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         *,
         DataSourceConfiguration: DataSourceConfigurationTypeDef,
         ReportConfiguration: ReportConfigurationTypeDef,
         TargetDatabaseName: str,
         TargetTableName: str,
         ClientToken: str = ...,
         DataModelConfiguration: DataModelConfigurationTypeDef = ...,
-        RecordVersion: int = ...
+        RecordVersion: int = ...,
     ) -> CreateBatchLoadTaskResponseTypeDef:
         """
         Creates a new Timestream batch load task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.create_batch_load_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_write/client/#create_batch_load_task)
         """
@@ -136,15 +136,15 @@
         self,
         *,
         DatabaseName: str,
         TableName: str,
         RetentionProperties: RetentionPropertiesTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         MagneticStoreWriteProperties: MagneticStoreWritePropertiesTypeDef = ...,
-        Schema: SchemaTypeDef = ...
+        Schema: SchemaTypeDef = ...,
     ) -> CreateTableResponseTypeDef:
         """
         Adds a new table to an existing database in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.create_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_write/client/#create_table)
         """
@@ -305,15 +305,15 @@
     async def update_table(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         RetentionProperties: RetentionPropertiesTypeDef = ...,
         MagneticStoreWriteProperties: MagneticStoreWritePropertiesTypeDef = ...,
-        Schema: SchemaTypeDef = ...
+        Schema: SchemaTypeDef = ...,
     ) -> UpdateTableResponseTypeDef:
         """
         Modifies the retention duration of the memory store and magnetic store for your
         Timestream
         table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.update_table)
@@ -322,15 +322,15 @@
 
     async def write_records(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         Records: Sequence[RecordTypeDef],
-        CommonAttributes: RecordTypeDef = ...
+        CommonAttributes: RecordTypeDef = ...,
     ) -> WriteRecordsResponseTypeDef:
         """
         Enables you to write your time-series data into Timestream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.write_records)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_write/client/#write_records)
         """
```

### Comparing `types-aiobotocore-timestream-write-2.9.0/types_aiobotocore_timestream_write/client.pyi` & `types-aiobotocore-timestream-write-2.9.1/types_aiobotocore_timestream_write/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         *,
         DataSourceConfiguration: DataSourceConfigurationTypeDef,
         ReportConfiguration: ReportConfigurationTypeDef,
         TargetDatabaseName: str,
         TargetTableName: str,
         ClientToken: str = ...,
         DataModelConfiguration: DataModelConfigurationTypeDef = ...,
-        RecordVersion: int = ...
+        RecordVersion: int = ...,
     ) -> CreateBatchLoadTaskResponseTypeDef:
         """
         Creates a new Timestream batch load task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.create_batch_load_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_write/client/#create_batch_load_task)
         """
@@ -133,15 +133,15 @@
         self,
         *,
         DatabaseName: str,
         TableName: str,
         RetentionProperties: RetentionPropertiesTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         MagneticStoreWriteProperties: MagneticStoreWritePropertiesTypeDef = ...,
-        Schema: SchemaTypeDef = ...
+        Schema: SchemaTypeDef = ...,
     ) -> CreateTableResponseTypeDef:
         """
         Adds a new table to an existing database in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.create_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_write/client/#create_table)
         """
@@ -302,15 +302,15 @@
     async def update_table(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         RetentionProperties: RetentionPropertiesTypeDef = ...,
         MagneticStoreWriteProperties: MagneticStoreWritePropertiesTypeDef = ...,
-        Schema: SchemaTypeDef = ...
+        Schema: SchemaTypeDef = ...,
     ) -> UpdateTableResponseTypeDef:
         """
         Modifies the retention duration of the memory store and magnetic store for your
         Timestream
         table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.update_table)
@@ -319,15 +319,15 @@
 
     async def write_records(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         Records: Sequence[RecordTypeDef],
-        CommonAttributes: RecordTypeDef = ...
+        CommonAttributes: RecordTypeDef = ...,
     ) -> WriteRecordsResponseTypeDef:
         """
         Enables you to write your time-series data into Timestream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.write_records)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_write/client/#write_records)
         """
```

### Comparing `types-aiobotocore-timestream-write-2.9.0/types_aiobotocore_timestream_write/literals.py` & `types-aiobotocore-timestream-write-2.9.1/types_aiobotocore_timestream_write/literals.py`

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
     "BatchLoadDataFormatType",
     "BatchLoadStatusType",
     "DimensionValueTypeType",
     "MeasureValueTypeType",
     "PartitionKeyEnforcementLevelType",
     "PartitionKeyTypeType",
@@ -33,15 +32,14 @@
     "TimeUnitType",
     "TimestreamWriteServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 BatchLoadDataFormatType = Literal["CSV"]
 BatchLoadStatusType = Literal[
     "CREATED", "FAILED", "IN_PROGRESS", "PENDING_RESUME", "PROGRESS_STOPPED", "SUCCEEDED"
 ]
 DimensionValueTypeType = Literal["VARCHAR"]
 MeasureValueTypeType = Literal["BIGINT", "BOOLEAN", "DOUBLE", "MULTI", "TIMESTAMP", "VARCHAR"]
 PartitionKeyEnforcementLevelType = Literal["OPTIONAL", "REQUIRED"]
```

### Comparing `types-aiobotocore-timestream-write-2.9.0/types_aiobotocore_timestream_write/literals.pyi` & `types-aiobotocore-timestream-write-2.9.1/types_aiobotocore_timestream_write/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-timestream-write-2.9.0/types_aiobotocore_timestream_write/type_defs.py` & `types-aiobotocore-timestream-write-2.9.1/types_aiobotocore_timestream_write/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "BatchLoadProgressReportTypeDef",
     "BatchLoadTaskTypeDef",
     "ResponseMetadataTypeDef",
     "TagTypeDef",
     "DatabaseTypeDef",
     "RetentionPropertiesTypeDef",
```

### Comparing `types-aiobotocore-timestream-write-2.9.0/types_aiobotocore_timestream_write/type_defs.pyi` & `types-aiobotocore-timestream-write-2.9.1/types_aiobotocore_timestream_write/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-timestream-write-2.9.0/types_aiobotocore_timestream_write.egg-info/PKG-INFO` & `types-aiobotocore-timestream-write-2.9.1/types_aiobotocore_timestream_write.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-timestream-write
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.TimestreamWrite 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.TimestreamWrite 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_write/
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
 
 <a id="types-aiobotocore-timestream-write"></a>
 
 # types-aiobotocore-timestream-write
 
 [![PyPI - types-aiobotocore-timestream-write](https://img.shields.io/pypi/v/types-aiobotocore-timestream-write.svg?color=blue)](https://pypi.org/project/types-aiobotocore-timestream-write)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-timestream-write.svg?color=blue)](https://pypi.org/project/types-aiobotocore-timestream-write)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_write/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-timestream-write)](https://pepy.tech/project/types-aiobotocore-timestream-write)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.TimestreamWrite 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite)
+[aiobotocore.TimestreamWrite 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite)
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
 [types-aiobotocore-timestream-write docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_write/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-timestream-write-2.9.0/types_aiobotocore_timestream_write.egg-info/SOURCES.txt` & `types-aiobotocore-timestream-write-2.9.1/types_aiobotocore_timestream_write.egg-info/SOURCES.txt`

 * *Files identical despite different names*

