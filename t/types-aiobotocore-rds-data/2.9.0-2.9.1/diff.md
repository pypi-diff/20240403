# Comparing `tmp/types-aiobotocore-rds-data-2.9.0.tar.gz` & `tmp/types-aiobotocore-rds-data-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-rds-data-2.9.0.tar", last modified: Wed Dec 13 20:00:15 2023, max compression
+gzip compressed data, was "types-aiobotocore-rds-data-2.9.1.tar", last modified: Thu Jan 18 01:21:34 2024, max compression
```

## Comparing `types-aiobotocore-rds-data-2.9.0.tar` & `types-aiobotocore-rds-data-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:15.069271 types-aiobotocore-rds-data-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:54:17.000000 types-aiobotocore-rds-data-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12334 2023-12-13 20:00:15.069271 types-aiobotocore-rds-data-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10761 2023-12-13 19:54:17.000000 types-aiobotocore-rds-data-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:15.069271 types-aiobotocore-rds-data-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2023-12-13 19:54:17.000000 types-aiobotocore-rds-data-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:15.065271 types-aiobotocore-rds-data-2.9.0/types_aiobotocore_rds_data/
--rw-r--r--   0 runner    (1001) docker     (127)      481 2023-12-13 19:54:17.000000 types-aiobotocore-rds-data-2.9.0/types_aiobotocore_rds_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2023-12-13 19:54:17.000000 types-aiobotocore-rds-data-2.9.0/types_aiobotocore_rds_data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      948 2023-12-13 19:54:17.000000 types-aiobotocore-rds-data-2.9.0/types_aiobotocore_rds_data/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8558 2023-12-13 19:54:17.000000 types-aiobotocore-rds-data-2.9.0/types_aiobotocore_rds_data/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8555 2023-12-13 19:54:17.000000 types-aiobotocore-rds-data-2.9.0/types_aiobotocore_rds_data/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8764 2023-12-13 19:54:17.000000 types-aiobotocore-rds-data-2.9.0/types_aiobotocore_rds_data/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8762 2023-12-13 19:54:17.000000 types-aiobotocore-rds-data-2.9.0/types_aiobotocore_rds_data/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:54:17.000000 types-aiobotocore-rds-data-2.9.0/types_aiobotocore_rds_data/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     8407 2023-12-13 19:54:17.000000 types-aiobotocore-rds-data-2.9.0/types_aiobotocore_rds_data/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8406 2023-12-13 19:54:17.000000 types-aiobotocore-rds-data-2.9.0/types_aiobotocore_rds_data/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:54:17.000000 types-aiobotocore-rds-data-2.9.0/types_aiobotocore_rds_data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:15.069271 types-aiobotocore-rds-data-2.9.0/types_aiobotocore_rds_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12334 2023-12-13 20:00:15.000000 types-aiobotocore-rds-data-2.9.0/types_aiobotocore_rds_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      751 2023-12-13 20:00:15.000000 types-aiobotocore-rds-data-2.9.0/types_aiobotocore_rds_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:15.000000 types-aiobotocore-rds-data-2.9.0/types_aiobotocore_rds_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:15.000000 types-aiobotocore-rds-data-2.9.0/types_aiobotocore_rds_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:15.000000 types-aiobotocore-rds-data-2.9.0/types_aiobotocore_rds_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-13 20:00:15.000000 types-aiobotocore-rds-data-2.9.0/types_aiobotocore_rds_data.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:34.869096 types-aiobotocore-rds-data-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:15:54.000000 types-aiobotocore-rds-data-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12354 2024-01-18 01:21:34.869096 types-aiobotocore-rds-data-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10761 2024-01-18 01:15:54.000000 types-aiobotocore-rds-data-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:34.869096 types-aiobotocore-rds-data-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-01-18 01:15:54.000000 types-aiobotocore-rds-data-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:34.869096 types-aiobotocore-rds-data-2.9.1/types_aiobotocore_rds_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-01-18 01:15:54.000000 types-aiobotocore-rds-data-2.9.1/types_aiobotocore_rds_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-01-18 01:15:54.000000 types-aiobotocore-rds-data-2.9.1/types_aiobotocore_rds_data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-01-18 01:15:54.000000 types-aiobotocore-rds-data-2.9.1/types_aiobotocore_rds_data/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8561 2024-01-18 01:15:54.000000 types-aiobotocore-rds-data-2.9.1/types_aiobotocore_rds_data/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8558 2024-01-18 01:15:54.000000 types-aiobotocore-rds-data-2.9.1/types_aiobotocore_rds_data/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8762 2024-01-18 01:15:54.000000 types-aiobotocore-rds-data-2.9.1/types_aiobotocore_rds_data/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8762 2024-01-18 01:15:54.000000 types-aiobotocore-rds-data-2.9.1/types_aiobotocore_rds_data/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:15:54.000000 types-aiobotocore-rds-data-2.9.1/types_aiobotocore_rds_data/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     8406 2024-01-18 01:15:54.000000 types-aiobotocore-rds-data-2.9.1/types_aiobotocore_rds_data/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8406 2024-01-18 01:15:54.000000 types-aiobotocore-rds-data-2.9.1/types_aiobotocore_rds_data/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:15:54.000000 types-aiobotocore-rds-data-2.9.1/types_aiobotocore_rds_data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:34.869096 types-aiobotocore-rds-data-2.9.1/types_aiobotocore_rds_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12354 2024-01-18 01:21:34.000000 types-aiobotocore-rds-data-2.9.1/types_aiobotocore_rds_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-01-18 01:21:34.000000 types-aiobotocore-rds-data-2.9.1/types_aiobotocore_rds_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:34.000000 types-aiobotocore-rds-data-2.9.1/types_aiobotocore_rds_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:34.000000 types-aiobotocore-rds-data-2.9.1/types_aiobotocore_rds_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:34.000000 types-aiobotocore-rds-data-2.9.1/types_aiobotocore_rds_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-18 01:21:34.000000 types-aiobotocore-rds-data-2.9.1/types_aiobotocore_rds_data.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-rds-data-2.9.0/LICENSE` & `types-aiobotocore-rds-data-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-rds-data-2.9.0/PKG-INFO` & `types-aiobotocore-rds-data-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-rds-data
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.RDSDataService 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.RDSDataService 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds_data/
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
 
 <a id="types-aiobotocore-rds-data"></a>
 
 # types-aiobotocore-rds-data
 
 [![PyPI - types-aiobotocore-rds-data](https://img.shields.io/pypi/v/types-aiobotocore-rds-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rds-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-rds-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rds-data)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-rds-data)](https://pepy.tech/project/types-aiobotocore-rds-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.RDSDataService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService)
+[aiobotocore.RDSDataService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService)
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
 [types-aiobotocore-rds-data docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds_data/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-rds-data-2.9.0/README.md` & `types-aiobotocore-rds-data-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-rds-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rds-data)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-rds-data)](https://pepy.tech/project/types-aiobotocore-rds-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.RDSDataService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService)
+[aiobotocore.RDSDataService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService)
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
 [types-aiobotocore-rds-data docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds_data/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-rds-data-2.9.0/setup.py` & `types-aiobotocore-rds-data-2.9.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-rds-data",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_rds_data"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.RDSDataService 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.RDSDataService 2.9.1 service generated with"
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
     keywords="aiobotocore rds-data type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_rds_data": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds_data/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-rds-data-2.9.0/types_aiobotocore_rds_data/__main__.py` & `types-aiobotocore-rds-data-2.9.1/types_aiobotocore_rds_data/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.RDSDataService 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.RDSDataService 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds_data//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService\nOther"
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

### Comparing `types-aiobotocore-rds-data-2.9.0/types_aiobotocore_rds_data/client.py` & `types-aiobotocore-rds-data-2.9.1/types_aiobotocore_rds_data/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         *,
         resourceArn: str,
         secretArn: str,
         sql: str,
         database: str = ...,
         schema: str = ...,
         parameterSets: Sequence[Sequence[SqlParameterTypeDef]] = ...,
-        transactionId: str = ...
+        transactionId: str = ...,
     ) -> BatchExecuteStatementResponseTypeDef:
         """
         Runs a batch SQL statement over an array of data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService.Client.batch_execute_statement)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds_data/client/#batch_execute_statement)
         """
@@ -130,15 +130,15 @@
     async def execute_sql(
         self,
         *,
         dbClusterOrInstanceArn: str,
         awsSecretStoreArn: str,
         sqlStatements: str,
         database: str = ...,
-        schema: str = ...
+        schema: str = ...,
     ) -> ExecuteSqlResponseTypeDef:
         """
         Runs one or more SQL statements.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService.Client.execute_sql)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds_data/client/#execute_sql)
         """
@@ -152,15 +152,15 @@
         database: str = ...,
         schema: str = ...,
         parameters: Sequence[SqlParameterTypeDef] = ...,
         transactionId: str = ...,
         includeResultMetadata: bool = ...,
         continueAfterTimeout: bool = ...,
         resultSetOptions: ResultSetOptionsTypeDef = ...,
-        formatRecordsAs: RecordsFormatTypeType = ...
+        formatRecordsAs: RecordsFormatTypeType = ...,
     ) -> ExecuteStatementResponseTypeDef:
         """
         Runs a SQL statement against a database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService.Client.execute_statement)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds_data/client/#execute_statement)
         """
```

### Comparing `types-aiobotocore-rds-data-2.9.0/types_aiobotocore_rds_data/client.pyi` & `types-aiobotocore-rds-data-2.9.1/types_aiobotocore_rds_data/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         *,
         resourceArn: str,
         secretArn: str,
         sql: str,
         database: str = ...,
         schema: str = ...,
         parameterSets: Sequence[Sequence[SqlParameterTypeDef]] = ...,
-        transactionId: str = ...
+        transactionId: str = ...,
     ) -> BatchExecuteStatementResponseTypeDef:
         """
         Runs a batch SQL statement over an array of data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService.Client.batch_execute_statement)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds_data/client/#batch_execute_statement)
         """
@@ -127,15 +127,15 @@
     async def execute_sql(
         self,
         *,
         dbClusterOrInstanceArn: str,
         awsSecretStoreArn: str,
         sqlStatements: str,
         database: str = ...,
-        schema: str = ...
+        schema: str = ...,
     ) -> ExecuteSqlResponseTypeDef:
         """
         Runs one or more SQL statements.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService.Client.execute_sql)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds_data/client/#execute_sql)
         """
@@ -149,15 +149,15 @@
         database: str = ...,
         schema: str = ...,
         parameters: Sequence[SqlParameterTypeDef] = ...,
         transactionId: str = ...,
         includeResultMetadata: bool = ...,
         continueAfterTimeout: bool = ...,
         resultSetOptions: ResultSetOptionsTypeDef = ...,
-        formatRecordsAs: RecordsFormatTypeType = ...
+        formatRecordsAs: RecordsFormatTypeType = ...,
     ) -> ExecuteStatementResponseTypeDef:
         """
         Runs a SQL statement against a database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService.Client.execute_statement)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds_data/client/#execute_statement)
         """
```

### Comparing `types-aiobotocore-rds-data-2.9.0/types_aiobotocore_rds_data/literals.py` & `types-aiobotocore-rds-data-2.9.1/types_aiobotocore_rds_data/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,27 +15,25 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "DecimalReturnTypeType",
     "LongReturnTypeType",
     "RecordsFormatTypeType",
     "TypeHintType",
     "RDSDataServiceServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 DecimalReturnTypeType = Literal["DOUBLE_OR_LONG", "STRING"]
 LongReturnTypeType = Literal["LONG", "STRING"]
 RecordsFormatTypeType = Literal["JSON", "NONE"]
 TypeHintType = Literal["DATE", "DECIMAL", "JSON", "TIME", "TIMESTAMP", "UUID"]
 RDSDataServiceServiceName = Literal["rds-data"]
 ServiceName = Literal[
     "accessanalyzer",
```

### Comparing `types-aiobotocore-rds-data-2.9.0/types_aiobotocore_rds_data/literals.pyi` & `types-aiobotocore-rds-data-2.9.1/types_aiobotocore_rds_data/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rds-data-2.9.0/types_aiobotocore_rds_data/type_defs.py` & `types-aiobotocore-rds-data-2.9.1/types_aiobotocore_rds_data/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ArrayValueTypeDef",
     "ResponseMetadataTypeDef",
     "BeginTransactionRequestRequestTypeDef",
     "BlobTypeDef",
     "ColumnMetadataTypeDef",
     "CommitTransactionRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-rds-data-2.9.0/types_aiobotocore_rds_data/type_defs.pyi` & `types-aiobotocore-rds-data-2.9.1/types_aiobotocore_rds_data/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rds-data-2.9.0/types_aiobotocore_rds_data.egg-info/PKG-INFO` & `types-aiobotocore-rds-data-2.9.1/types_aiobotocore_rds_data.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-rds-data
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.RDSDataService 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.RDSDataService 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds_data/
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
 
 <a id="types-aiobotocore-rds-data"></a>
 
 # types-aiobotocore-rds-data
 
 [![PyPI - types-aiobotocore-rds-data](https://img.shields.io/pypi/v/types-aiobotocore-rds-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rds-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-rds-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rds-data)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-rds-data)](https://pepy.tech/project/types-aiobotocore-rds-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.RDSDataService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService)
+[aiobotocore.RDSDataService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService)
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
 [types-aiobotocore-rds-data docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds_data/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-rds-data-2.9.0/types_aiobotocore_rds_data.egg-info/SOURCES.txt` & `types-aiobotocore-rds-data-2.9.1/types_aiobotocore_rds_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

