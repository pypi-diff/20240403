# Comparing `tmp/types-aiobotocore-cognito-sync-2.9.0.tar.gz` & `tmp/types-aiobotocore-cognito-sync-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cognito-sync-2.9.0.tar", last modified: Wed Dec 13 19:58:57 2023, max compression
+gzip compressed data, was "types-aiobotocore-cognito-sync-2.9.1.tar", last modified: Thu Jan 18 01:20:23 2024, max compression
```

## Comparing `types-aiobotocore-cognito-sync-2.9.0.tar` & `types-aiobotocore-cognito-sync-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:57.821906 types-aiobotocore-cognito-sync-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:43:07.000000 types-aiobotocore-cognito-sync-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12513 2023-12-13 19:58:57.821906 types-aiobotocore-cognito-sync-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10931 2023-12-13 19:43:07.000000 types-aiobotocore-cognito-sync-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:57.821906 types-aiobotocore-cognito-sync-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2023-12-13 19:43:07.000000 types-aiobotocore-cognito-sync-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:57.821906 types-aiobotocore-cognito-sync-2.9.0/types_aiobotocore_cognito_sync/
--rw-r--r--   0 runner    (1001) docker     (127)      478 2023-12-13 19:43:07.000000 types-aiobotocore-cognito-sync-2.9.0/types_aiobotocore_cognito_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2023-12-13 19:43:07.000000 types-aiobotocore-cognito-sync-2.9.0/types_aiobotocore_cognito_sync/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      950 2023-12-13 19:43:07.000000 types-aiobotocore-cognito-sync-2.9.0/types_aiobotocore_cognito_sync/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15536 2023-12-13 19:43:08.000000 types-aiobotocore-cognito-sync-2.9.0/types_aiobotocore_cognito_sync/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    15533 2023-12-13 19:43:07.000000 types-aiobotocore-cognito-sync-2.9.0/types_aiobotocore_cognito_sync/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8715 2023-12-13 19:43:08.000000 types-aiobotocore-cognito-sync-2.9.0/types_aiobotocore_cognito_sync/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8713 2023-12-13 19:43:08.000000 types-aiobotocore-cognito-sync-2.9.0/types_aiobotocore_cognito_sync/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:43:07.000000 types-aiobotocore-cognito-sync-2.9.0/types_aiobotocore_cognito_sync/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    11809 2023-12-13 19:43:08.000000 types-aiobotocore-cognito-sync-2.9.0/types_aiobotocore_cognito_sync/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11808 2023-12-13 19:43:08.000000 types-aiobotocore-cognito-sync-2.9.0/types_aiobotocore_cognito_sync/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:43:07.000000 types-aiobotocore-cognito-sync-2.9.0/types_aiobotocore_cognito_sync/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:57.821906 types-aiobotocore-cognito-sync-2.9.0/types_aiobotocore_cognito_sync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12513 2023-12-13 19:58:57.000000 types-aiobotocore-cognito-sync-2.9.0/types_aiobotocore_cognito_sync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      819 2023-12-13 19:58:57.000000 types-aiobotocore-cognito-sync-2.9.0/types_aiobotocore_cognito_sync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:57.000000 types-aiobotocore-cognito-sync-2.9.0/types_aiobotocore_cognito_sync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:57.000000 types-aiobotocore-cognito-sync-2.9.0/types_aiobotocore_cognito_sync.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:57.000000 types-aiobotocore-cognito-sync-2.9.0/types_aiobotocore_cognito_sync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-13 19:58:57.000000 types-aiobotocore-cognito-sync-2.9.0/types_aiobotocore_cognito_sync.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:23.897427 types-aiobotocore-cognito-sync-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:05:03.000000 types-aiobotocore-cognito-sync-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12533 2024-01-18 01:20:23.897427 types-aiobotocore-cognito-sync-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10931 2024-01-18 01:05:03.000000 types-aiobotocore-cognito-sync-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:23.897427 types-aiobotocore-cognito-sync-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-01-18 01:05:03.000000 types-aiobotocore-cognito-sync-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:23.893427 types-aiobotocore-cognito-sync-2.9.1/types_aiobotocore_cognito_sync/
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-01-18 01:05:03.000000 types-aiobotocore-cognito-sync-2.9.1/types_aiobotocore_cognito_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-01-18 01:05:03.000000 types-aiobotocore-cognito-sync-2.9.1/types_aiobotocore_cognito_sync/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-01-18 01:05:03.000000 types-aiobotocore-cognito-sync-2.9.1/types_aiobotocore_cognito_sync/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15539 2024-01-18 01:05:04.000000 types-aiobotocore-cognito-sync-2.9.1/types_aiobotocore_cognito_sync/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15536 2024-01-18 01:05:03.000000 types-aiobotocore-cognito-sync-2.9.1/types_aiobotocore_cognito_sync/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8713 2024-01-18 01:05:04.000000 types-aiobotocore-cognito-sync-2.9.1/types_aiobotocore_cognito_sync/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8713 2024-01-18 01:05:04.000000 types-aiobotocore-cognito-sync-2.9.1/types_aiobotocore_cognito_sync/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:05:03.000000 types-aiobotocore-cognito-sync-2.9.1/types_aiobotocore_cognito_sync/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    11808 2024-01-18 01:05:04.000000 types-aiobotocore-cognito-sync-2.9.1/types_aiobotocore_cognito_sync/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11808 2024-01-18 01:05:04.000000 types-aiobotocore-cognito-sync-2.9.1/types_aiobotocore_cognito_sync/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:05:03.000000 types-aiobotocore-cognito-sync-2.9.1/types_aiobotocore_cognito_sync/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:23.893427 types-aiobotocore-cognito-sync-2.9.1/types_aiobotocore_cognito_sync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12533 2024-01-18 01:20:23.000000 types-aiobotocore-cognito-sync-2.9.1/types_aiobotocore_cognito_sync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-01-18 01:20:23.000000 types-aiobotocore-cognito-sync-2.9.1/types_aiobotocore_cognito_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:23.000000 types-aiobotocore-cognito-sync-2.9.1/types_aiobotocore_cognito_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:23.000000 types-aiobotocore-cognito-sync-2.9.1/types_aiobotocore_cognito_sync.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:23.000000 types-aiobotocore-cognito-sync-2.9.1/types_aiobotocore_cognito_sync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-01-18 01:20:23.000000 types-aiobotocore-cognito-sync-2.9.1/types_aiobotocore_cognito_sync.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cognito-sync-2.9.0/LICENSE` & `types-aiobotocore-cognito-sync-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-cognito-sync-2.9.0/PKG-INFO` & `types-aiobotocore-cognito-sync-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cognito-sync
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CognitoSync 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CognitoSync 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_sync/
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
 
 <a id="types-aiobotocore-cognito-sync"></a>
 
 # types-aiobotocore-cognito-sync
 
 [![PyPI - types-aiobotocore-cognito-sync](https://img.shields.io/pypi/v/types-aiobotocore-cognito-sync.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cognito-sync)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cognito-sync.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cognito-sync)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_sync/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cognito-sync)](https://pepy.tech/project/types-aiobotocore-cognito-sync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CognitoSync 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync)
+[aiobotocore.CognitoSync 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync)
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
 [types-aiobotocore-cognito-sync docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_sync/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-cognito-sync-2.9.0/README.md` & `types-aiobotocore-cognito-sync-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cognito-sync.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cognito-sync)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_sync/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cognito-sync)](https://pepy.tech/project/types-aiobotocore-cognito-sync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CognitoSync 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync)
+[aiobotocore.CognitoSync 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync)
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
 [types-aiobotocore-cognito-sync docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_sync/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-cognito-sync-2.9.0/setup.py` & `types-aiobotocore-cognito-sync-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cognito-sync",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_cognito_sync"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CognitoSync 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.CognitoSync 2.9.1 service generated with"
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
     keywords="aiobotocore cognito-sync type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_cognito_sync": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_sync/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-cognito-sync-2.9.0/types_aiobotocore_cognito_sync/__main__.py` & `types-aiobotocore-cognito-sync-2.9.1/types_aiobotocore_cognito_sync/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CognitoSync 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.CognitoSync 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_sync//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync\nOther"
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

### Comparing `types-aiobotocore-cognito-sync-2.9.0/types_aiobotocore_cognito_sync/client.py` & `types-aiobotocore-cognito-sync-2.9.1/types_aiobotocore_cognito_sync/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -223,15 +223,15 @@
         *,
         IdentityPoolId: str,
         IdentityId: str,
         DatasetName: str,
         LastSyncCount: int = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        SyncSessionToken: str = ...
+        SyncSessionToken: str = ...,
     ) -> ListRecordsResponseTypeDef:
         """
         Gets paginated records, optionally changed after a particular sync count for a
         dataset and
         identity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync.Client.list_records)
@@ -259,15 +259,15 @@
         """
 
     async def set_identity_pool_configuration(
         self,
         *,
         IdentityPoolId: str,
         PushSync: PushSyncTypeDef = ...,
-        CognitoStreams: CognitoStreamsTypeDef = ...
+        CognitoStreams: CognitoStreamsTypeDef = ...,
     ) -> SetIdentityPoolConfigurationResponseTypeDef:
         """
         Sets the necessary configuration for push sync.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync.Client.set_identity_pool_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_sync/client/#set_identity_pool_configuration)
         """
@@ -299,15 +299,15 @@
         *,
         IdentityPoolId: str,
         IdentityId: str,
         DatasetName: str,
         SyncSessionToken: str,
         DeviceId: str = ...,
         RecordPatches: Sequence[RecordPatchTypeDef] = ...,
-        ClientContext: str = ...
+        ClientContext: str = ...,
     ) -> UpdateRecordsResponseTypeDef:
         """
         Posts updates to records and adds and deletes records for a dataset and user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync.Client.update_records)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_sync/client/#update_records)
         """
```

### Comparing `types-aiobotocore-cognito-sync-2.9.0/types_aiobotocore_cognito_sync/client.pyi` & `types-aiobotocore-cognito-sync-2.9.1/types_aiobotocore_cognito_sync/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -220,15 +220,15 @@
         *,
         IdentityPoolId: str,
         IdentityId: str,
         DatasetName: str,
         LastSyncCount: int = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        SyncSessionToken: str = ...
+        SyncSessionToken: str = ...,
     ) -> ListRecordsResponseTypeDef:
         """
         Gets paginated records, optionally changed after a particular sync count for a
         dataset and
         identity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync.Client.list_records)
@@ -256,15 +256,15 @@
         """
 
     async def set_identity_pool_configuration(
         self,
         *,
         IdentityPoolId: str,
         PushSync: PushSyncTypeDef = ...,
-        CognitoStreams: CognitoStreamsTypeDef = ...
+        CognitoStreams: CognitoStreamsTypeDef = ...,
     ) -> SetIdentityPoolConfigurationResponseTypeDef:
         """
         Sets the necessary configuration for push sync.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync.Client.set_identity_pool_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_sync/client/#set_identity_pool_configuration)
         """
@@ -296,15 +296,15 @@
         *,
         IdentityPoolId: str,
         IdentityId: str,
         DatasetName: str,
         SyncSessionToken: str,
         DeviceId: str = ...,
         RecordPatches: Sequence[RecordPatchTypeDef] = ...,
-        ClientContext: str = ...
+        ClientContext: str = ...,
     ) -> UpdateRecordsResponseTypeDef:
         """
         Posts updates to records and adds and deletes records for a dataset and user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync.Client.update_records)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_sync/client/#update_records)
         """
```

### Comparing `types-aiobotocore-cognito-sync-2.9.0/types_aiobotocore_cognito_sync/literals.py` & `types-aiobotocore-cognito-sync-2.9.1/types_aiobotocore_cognito_sync/literals.py`

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
     "BulkPublishStatusType",
     "OperationType",
     "PlatformType",
     "StreamingStatusType",
     "CognitoSyncServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 BulkPublishStatusType = Literal["FAILED", "IN_PROGRESS", "NOT_STARTED", "SUCCEEDED"]
 OperationType = Literal["remove", "replace"]
 PlatformType = Literal["ADM", "APNS", "APNS_SANDBOX", "GCM"]
 StreamingStatusType = Literal["DISABLED", "ENABLED"]
 CognitoSyncServiceName = Literal["cognito-sync"]
 ServiceName = Literal[
     "accessanalyzer",
```

### Comparing `types-aiobotocore-cognito-sync-2.9.0/types_aiobotocore_cognito_sync/literals.pyi` & `types-aiobotocore-cognito-sync-2.9.1/types_aiobotocore_cognito_sync/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-sync-2.9.0/types_aiobotocore_cognito_sync/type_defs.py` & `types-aiobotocore-cognito-sync-2.9.1/types_aiobotocore_cognito_sync/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "BulkPublishRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CognitoStreamsTypeDef",
     "DatasetTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-cognito-sync-2.9.0/types_aiobotocore_cognito_sync/type_defs.pyi` & `types-aiobotocore-cognito-sync-2.9.1/types_aiobotocore_cognito_sync/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-sync-2.9.0/types_aiobotocore_cognito_sync.egg-info/PKG-INFO` & `types-aiobotocore-cognito-sync-2.9.1/types_aiobotocore_cognito_sync.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cognito-sync
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CognitoSync 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CognitoSync 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_sync/
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
 
 <a id="types-aiobotocore-cognito-sync"></a>
 
 # types-aiobotocore-cognito-sync
 
 [![PyPI - types-aiobotocore-cognito-sync](https://img.shields.io/pypi/v/types-aiobotocore-cognito-sync.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cognito-sync)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cognito-sync.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cognito-sync)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_sync/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cognito-sync)](https://pepy.tech/project/types-aiobotocore-cognito-sync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CognitoSync 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync)
+[aiobotocore.CognitoSync 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync)
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
 [types-aiobotocore-cognito-sync docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_sync/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-cognito-sync-2.9.0/types_aiobotocore_cognito_sync.egg-info/SOURCES.txt` & `types-aiobotocore-cognito-sync-2.9.1/types_aiobotocore_cognito_sync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

