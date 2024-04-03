# Comparing `tmp/types-aiobotocore-healthlake-2.9.0.tar.gz` & `tmp/types-aiobotocore-healthlake-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-healthlake-2.9.0.tar", last modified: Wed Dec 13 19:59:26 2023, max compression
+gzip compressed data, was "types-aiobotocore-healthlake-2.9.1.tar", last modified: Thu Jan 18 01:20:50 2024, max compression
```

## Comparing `types-aiobotocore-healthlake-2.9.0.tar` & `types-aiobotocore-healthlake-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:26.181705 types-aiobotocore-healthlake-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:47:11.000000 types-aiobotocore-healthlake-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12432 2023-12-13 19:59:26.181705 types-aiobotocore-healthlake-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10857 2023-12-13 19:47:11.000000 types-aiobotocore-healthlake-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:26.181705 types-aiobotocore-healthlake-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2023-12-13 19:47:11.000000 types-aiobotocore-healthlake-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:26.181705 types-aiobotocore-healthlake-2.9.0/types_aiobotocore_healthlake/
--rw-r--r--   0 runner    (1001) docker     (127)      467 2023-12-13 19:47:11.000000 types-aiobotocore-healthlake-2.9.0/types_aiobotocore_healthlake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2023-12-13 19:47:11.000000 types-aiobotocore-healthlake-2.9.0/types_aiobotocore_healthlake/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      944 2023-12-13 19:47:11.000000 types-aiobotocore-healthlake-2.9.0/types_aiobotocore_healthlake/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13460 2023-12-13 19:47:11.000000 types-aiobotocore-healthlake-2.9.0/types_aiobotocore_healthlake/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13456 2023-12-13 19:47:11.000000 types-aiobotocore-healthlake-2.9.0/types_aiobotocore_healthlake/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8868 2023-12-13 19:47:12.000000 types-aiobotocore-healthlake-2.9.0/types_aiobotocore_healthlake/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8866 2023-12-13 19:47:12.000000 types-aiobotocore-healthlake-2.9.0/types_aiobotocore_healthlake/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:47:11.000000 types-aiobotocore-healthlake-2.9.0/types_aiobotocore_healthlake/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    11785 2023-12-13 19:47:12.000000 types-aiobotocore-healthlake-2.9.0/types_aiobotocore_healthlake/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11784 2023-12-13 19:47:12.000000 types-aiobotocore-healthlake-2.9.0/types_aiobotocore_healthlake/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:47:11.000000 types-aiobotocore-healthlake-2.9.0/types_aiobotocore_healthlake/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:26.181705 types-aiobotocore-healthlake-2.9.0/types_aiobotocore_healthlake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12432 2023-12-13 19:59:26.000000 types-aiobotocore-healthlake-2.9.0/types_aiobotocore_healthlake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      785 2023-12-13 19:59:26.000000 types-aiobotocore-healthlake-2.9.0/types_aiobotocore_healthlake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:26.000000 types-aiobotocore-healthlake-2.9.0/types_aiobotocore_healthlake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:26.000000 types-aiobotocore-healthlake-2.9.0/types_aiobotocore_healthlake.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:26.000000 types-aiobotocore-healthlake-2.9.0/types_aiobotocore_healthlake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-13 19:59:26.000000 types-aiobotocore-healthlake-2.9.0/types_aiobotocore_healthlake.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:50.109299 types-aiobotocore-healthlake-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:09:04.000000 types-aiobotocore-healthlake-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12452 2024-01-18 01:20:50.109299 types-aiobotocore-healthlake-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10857 2024-01-18 01:09:04.000000 types-aiobotocore-healthlake-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:50.109299 types-aiobotocore-healthlake-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-01-18 01:09:03.000000 types-aiobotocore-healthlake-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:50.109299 types-aiobotocore-healthlake-2.9.1/types_aiobotocore_healthlake/
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-01-18 01:09:04.000000 types-aiobotocore-healthlake-2.9.1/types_aiobotocore_healthlake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-01-18 01:09:04.000000 types-aiobotocore-healthlake-2.9.1/types_aiobotocore_healthlake/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-01-18 01:09:04.000000 types-aiobotocore-healthlake-2.9.1/types_aiobotocore_healthlake/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13464 2024-01-18 01:09:04.000000 types-aiobotocore-healthlake-2.9.1/types_aiobotocore_healthlake/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13461 2024-01-18 01:09:04.000000 types-aiobotocore-healthlake-2.9.1/types_aiobotocore_healthlake/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8866 2024-01-18 01:09:04.000000 types-aiobotocore-healthlake-2.9.1/types_aiobotocore_healthlake/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8866 2024-01-18 01:09:04.000000 types-aiobotocore-healthlake-2.9.1/types_aiobotocore_healthlake/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:09:04.000000 types-aiobotocore-healthlake-2.9.1/types_aiobotocore_healthlake/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    11784 2024-01-18 01:09:04.000000 types-aiobotocore-healthlake-2.9.1/types_aiobotocore_healthlake/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11784 2024-01-18 01:09:04.000000 types-aiobotocore-healthlake-2.9.1/types_aiobotocore_healthlake/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:09:04.000000 types-aiobotocore-healthlake-2.9.1/types_aiobotocore_healthlake/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:50.109299 types-aiobotocore-healthlake-2.9.1/types_aiobotocore_healthlake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12452 2024-01-18 01:20:50.000000 types-aiobotocore-healthlake-2.9.1/types_aiobotocore_healthlake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-01-18 01:20:50.000000 types-aiobotocore-healthlake-2.9.1/types_aiobotocore_healthlake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:50.000000 types-aiobotocore-healthlake-2.9.1/types_aiobotocore_healthlake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:50.000000 types-aiobotocore-healthlake-2.9.1/types_aiobotocore_healthlake.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:50.000000 types-aiobotocore-healthlake-2.9.1/types_aiobotocore_healthlake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-01-18 01:20:50.000000 types-aiobotocore-healthlake-2.9.1/types_aiobotocore_healthlake.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-healthlake-2.9.0/LICENSE` & `types-aiobotocore-healthlake-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-healthlake-2.9.0/PKG-INFO` & `types-aiobotocore-healthlake-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-healthlake
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.HealthLake 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.HealthLake 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/
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
 
 <a id="types-aiobotocore-healthlake"></a>
 
 # types-aiobotocore-healthlake
 
 [![PyPI - types-aiobotocore-healthlake](https://img.shields.io/pypi/v/types-aiobotocore-healthlake.svg?color=blue)](https://pypi.org/project/types-aiobotocore-healthlake)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-healthlake.svg?color=blue)](https://pypi.org/project/types-aiobotocore-healthlake)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-healthlake)](https://pepy.tech/project/types-aiobotocore-healthlake)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.HealthLake 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake)
+[aiobotocore.HealthLake 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake)
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
 [types-aiobotocore-healthlake docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-healthlake-2.9.0/README.md` & `types-aiobotocore-healthlake-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-healthlake.svg?color=blue)](https://pypi.org/project/types-aiobotocore-healthlake)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-healthlake)](https://pepy.tech/project/types-aiobotocore-healthlake)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.HealthLake 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake)
+[aiobotocore.HealthLake 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake)
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
 [types-aiobotocore-healthlake docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-healthlake-2.9.0/setup.py` & `types-aiobotocore-healthlake-2.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-healthlake",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_healthlake"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.HealthLake 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.HealthLake 2.9.1 service generated with"
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
     keywords="aiobotocore healthlake type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_healthlake": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-healthlake-2.9.0/types_aiobotocore_healthlake/__main__.py` & `types-aiobotocore-healthlake-2.9.1/types_aiobotocore_healthlake/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.HealthLake 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.HealthLake 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake\nOther"
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

### Comparing `types-aiobotocore-healthlake-2.9.0/types_aiobotocore_healthlake/client.py` & `types-aiobotocore-healthlake-2.9.1/types_aiobotocore_healthlake/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("HealthLakeClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -109,15 +108,15 @@
         *,
         DatastoreTypeVersion: Literal["R4"],
         DatastoreName: str = ...,
         SseConfiguration: SseConfigurationTypeDef = ...,
         PreloadDataConfig: PreloadDataConfigTypeDef = ...,
         ClientToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        IdentityProviderConfiguration: IdentityProviderConfigurationTypeDef = ...
+        IdentityProviderConfiguration: IdentityProviderConfigurationTypeDef = ...,
     ) -> CreateFHIRDatastoreResponseTypeDef:
         """
         Creates a data store that can ingest and export FHIR formatted data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.create_fhir_datastore)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/client/#create_fhir_datastore)
         """
@@ -200,15 +199,15 @@
         *,
         DatastoreId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         JobName: str = ...,
         JobStatus: JobStatusType = ...,
         SubmittedBefore: TimestampTypeDef = ...,
-        SubmittedAfter: TimestampTypeDef = ...
+        SubmittedAfter: TimestampTypeDef = ...,
     ) -> ListFHIRExportJobsResponseTypeDef:
         """
         Lists all FHIR export jobs associated with an account and their statuses.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.list_fhir_export_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/client/#list_fhir_export_jobs)
         """
@@ -218,15 +217,15 @@
         *,
         DatastoreId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         JobName: str = ...,
         JobStatus: JobStatusType = ...,
         SubmittedBefore: TimestampTypeDef = ...,
-        SubmittedAfter: TimestampTypeDef = ...
+        SubmittedAfter: TimestampTypeDef = ...,
     ) -> ListFHIRImportJobsResponseTypeDef:
         """
         Lists all FHIR import jobs associated with an account and their statuses.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.list_fhir_import_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/client/#list_fhir_import_jobs)
         """
@@ -244,15 +243,15 @@
     async def start_fhir_export_job(
         self,
         *,
         OutputDataConfig: OutputDataConfigTypeDef,
         DatastoreId: str,
         DataAccessRoleArn: str,
         ClientToken: str,
-        JobName: str = ...
+        JobName: str = ...,
     ) -> StartFHIRExportJobResponseTypeDef:
         """
         Begins a FHIR export job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.start_fhir_export_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/client/#start_fhir_export_job)
         """
@@ -261,15 +260,15 @@
         self,
         *,
         InputDataConfig: InputDataConfigTypeDef,
         JobOutputDataConfig: OutputDataConfigTypeDef,
         DatastoreId: str,
         DataAccessRoleArn: str,
         ClientToken: str,
-        JobName: str = ...
+        JobName: str = ...,
     ) -> StartFHIRImportJobResponseTypeDef:
         """
         Begins a FHIR Import job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.start_fhir_import_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/client/#start_fhir_import_job)
         """
```

### Comparing `types-aiobotocore-healthlake-2.9.0/types_aiobotocore_healthlake/client.pyi` & `types-aiobotocore-healthlake-2.9.1/types_aiobotocore_healthlake/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         *,
         DatastoreTypeVersion: Literal["R4"],
         DatastoreName: str = ...,
         SseConfiguration: SseConfigurationTypeDef = ...,
         PreloadDataConfig: PreloadDataConfigTypeDef = ...,
         ClientToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        IdentityProviderConfiguration: IdentityProviderConfigurationTypeDef = ...
+        IdentityProviderConfiguration: IdentityProviderConfigurationTypeDef = ...,
     ) -> CreateFHIRDatastoreResponseTypeDef:
         """
         Creates a data store that can ingest and export FHIR formatted data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.create_fhir_datastore)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/client/#create_fhir_datastore)
         """
@@ -196,15 +196,15 @@
         *,
         DatastoreId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         JobName: str = ...,
         JobStatus: JobStatusType = ...,
         SubmittedBefore: TimestampTypeDef = ...,
-        SubmittedAfter: TimestampTypeDef = ...
+        SubmittedAfter: TimestampTypeDef = ...,
     ) -> ListFHIRExportJobsResponseTypeDef:
         """
         Lists all FHIR export jobs associated with an account and their statuses.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.list_fhir_export_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/client/#list_fhir_export_jobs)
         """
@@ -214,15 +214,15 @@
         *,
         DatastoreId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         JobName: str = ...,
         JobStatus: JobStatusType = ...,
         SubmittedBefore: TimestampTypeDef = ...,
-        SubmittedAfter: TimestampTypeDef = ...
+        SubmittedAfter: TimestampTypeDef = ...,
     ) -> ListFHIRImportJobsResponseTypeDef:
         """
         Lists all FHIR import jobs associated with an account and their statuses.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.list_fhir_import_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/client/#list_fhir_import_jobs)
         """
@@ -240,15 +240,15 @@
     async def start_fhir_export_job(
         self,
         *,
         OutputDataConfig: OutputDataConfigTypeDef,
         DatastoreId: str,
         DataAccessRoleArn: str,
         ClientToken: str,
-        JobName: str = ...
+        JobName: str = ...,
     ) -> StartFHIRExportJobResponseTypeDef:
         """
         Begins a FHIR export job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.start_fhir_export_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/client/#start_fhir_export_job)
         """
@@ -257,15 +257,15 @@
         self,
         *,
         InputDataConfig: InputDataConfigTypeDef,
         JobOutputDataConfig: OutputDataConfigTypeDef,
         DatastoreId: str,
         DataAccessRoleArn: str,
         ClientToken: str,
-        JobName: str = ...
+        JobName: str = ...,
     ) -> StartFHIRImportJobResponseTypeDef:
         """
         Begins a FHIR Import job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.start_fhir_import_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/client/#start_fhir_import_job)
         """
```

### Comparing `types-aiobotocore-healthlake-2.9.0/types_aiobotocore_healthlake/literals.py` & `types-aiobotocore-healthlake-2.9.1/types_aiobotocore_healthlake/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,29 +15,27 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AuthorizationStrategyType",
     "CmkTypeType",
     "DatastoreStatusType",
     "FHIRVersionType",
     "JobStatusType",
     "PreloadDataTypeType",
     "HealthLakeServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 AuthorizationStrategyType = Literal["AWS_AUTH", "SMART_ON_FHIR_V1"]
 CmkTypeType = Literal["AWS_OWNED_KMS_KEY", "CUSTOMER_MANAGED_KMS_KEY"]
 DatastoreStatusType = Literal["ACTIVE", "CREATING", "DELETED", "DELETING"]
 FHIRVersionType = Literal["R4"]
 JobStatusType = Literal[
     "CANCEL_COMPLETED",
     "CANCEL_FAILED",
```

### Comparing `types-aiobotocore-healthlake-2.9.0/types_aiobotocore_healthlake/literals.pyi` & `types-aiobotocore-healthlake-2.9.1/types_aiobotocore_healthlake/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-healthlake-2.9.0/types_aiobotocore_healthlake/type_defs.py` & `types-aiobotocore-healthlake-2.9.1/types_aiobotocore_healthlake/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "IdentityProviderConfigurationTypeDef",
     "PreloadDataConfigTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "TimestampTypeDef",
     "DeleteFHIRDatastoreRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-healthlake-2.9.0/types_aiobotocore_healthlake/type_defs.pyi` & `types-aiobotocore-healthlake-2.9.1/types_aiobotocore_healthlake/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-healthlake-2.9.0/types_aiobotocore_healthlake.egg-info/PKG-INFO` & `types-aiobotocore-healthlake-2.9.1/types_aiobotocore_healthlake.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-healthlake
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.HealthLake 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.HealthLake 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/
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
 
 <a id="types-aiobotocore-healthlake"></a>
 
 # types-aiobotocore-healthlake
 
 [![PyPI - types-aiobotocore-healthlake](https://img.shields.io/pypi/v/types-aiobotocore-healthlake.svg?color=blue)](https://pypi.org/project/types-aiobotocore-healthlake)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-healthlake.svg?color=blue)](https://pypi.org/project/types-aiobotocore-healthlake)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-healthlake)](https://pepy.tech/project/types-aiobotocore-healthlake)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.HealthLake 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake)
+[aiobotocore.HealthLake 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake)
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
 [types-aiobotocore-healthlake docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-healthlake-2.9.0/types_aiobotocore_healthlake.egg-info/SOURCES.txt` & `types-aiobotocore-healthlake-2.9.1/types_aiobotocore_healthlake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

