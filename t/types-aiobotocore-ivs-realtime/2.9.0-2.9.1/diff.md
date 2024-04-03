# Comparing `tmp/types-aiobotocore-ivs-realtime-2.9.0.tar.gz` & `tmp/types-aiobotocore-ivs-realtime-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ivs-realtime-2.9.0.tar", last modified: Wed Dec 13 19:59:36 2023, max compression
+gzip compressed data, was "types-aiobotocore-ivs-realtime-2.9.1.tar", last modified: Thu Jan 18 01:20:59 2024, max compression
```

## Comparing `types-aiobotocore-ivs-realtime-2.9.0.tar` & `types-aiobotocore-ivs-realtime-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:36.645600 types-aiobotocore-ivs-realtime-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:48:17.000000 types-aiobotocore-ivs-realtime-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12523 2023-12-13 19:59:36.645600 types-aiobotocore-ivs-realtime-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10941 2023-12-13 19:48:17.000000 types-aiobotocore-ivs-realtime-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:36.645600 types-aiobotocore-ivs-realtime-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2023-12-13 19:48:17.000000 types-aiobotocore-ivs-realtime-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:36.641600 types-aiobotocore-ivs-realtime-2.9.0/types_aiobotocore_ivs_realtime/
--rw-r--r--   0 runner    (1001) docker     (127)      478 2023-12-13 19:48:17.000000 types-aiobotocore-ivs-realtime-2.9.0/types_aiobotocore_ivs_realtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2023-12-13 19:48:17.000000 types-aiobotocore-ivs-realtime-2.9.0/types_aiobotocore_ivs_realtime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      950 2023-12-13 19:48:17.000000 types-aiobotocore-ivs-realtime-2.9.0/types_aiobotocore_ivs_realtime/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21100 2023-12-13 19:48:17.000000 types-aiobotocore-ivs-realtime-2.9.0/types_aiobotocore_ivs_realtime/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    21097 2023-12-13 19:48:17.000000 types-aiobotocore-ivs-realtime-2.9.0/types_aiobotocore_ivs_realtime/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9182 2023-12-13 19:48:18.000000 types-aiobotocore-ivs-realtime-2.9.0/types_aiobotocore_ivs_realtime/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9180 2023-12-13 19:48:17.000000 types-aiobotocore-ivs-realtime-2.9.0/types_aiobotocore_ivs_realtime/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:48:17.000000 types-aiobotocore-ivs-realtime-2.9.0/types_aiobotocore_ivs_realtime/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    20891 2023-12-13 19:48:18.000000 types-aiobotocore-ivs-realtime-2.9.0/types_aiobotocore_ivs_realtime/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    20890 2023-12-13 19:48:18.000000 types-aiobotocore-ivs-realtime-2.9.0/types_aiobotocore_ivs_realtime/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:48:17.000000 types-aiobotocore-ivs-realtime-2.9.0/types_aiobotocore_ivs_realtime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:36.641600 types-aiobotocore-ivs-realtime-2.9.0/types_aiobotocore_ivs_realtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12523 2023-12-13 19:59:36.000000 types-aiobotocore-ivs-realtime-2.9.0/types_aiobotocore_ivs_realtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      819 2023-12-13 19:59:36.000000 types-aiobotocore-ivs-realtime-2.9.0/types_aiobotocore_ivs_realtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:36.000000 types-aiobotocore-ivs-realtime-2.9.0/types_aiobotocore_ivs_realtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:36.000000 types-aiobotocore-ivs-realtime-2.9.0/types_aiobotocore_ivs_realtime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:36.000000 types-aiobotocore-ivs-realtime-2.9.0/types_aiobotocore_ivs_realtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-13 19:59:36.000000 types-aiobotocore-ivs-realtime-2.9.0/types_aiobotocore_ivs_realtime.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:59.809255 types-aiobotocore-ivs-realtime-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:10:06.000000 types-aiobotocore-ivs-realtime-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12543 2024-01-18 01:20:59.809255 types-aiobotocore-ivs-realtime-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10941 2024-01-18 01:10:06.000000 types-aiobotocore-ivs-realtime-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:59.809255 types-aiobotocore-ivs-realtime-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-01-18 01:10:05.000000 types-aiobotocore-ivs-realtime-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:59.805255 types-aiobotocore-ivs-realtime-2.9.1/types_aiobotocore_ivs_realtime/
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-01-18 01:10:06.000000 types-aiobotocore-ivs-realtime-2.9.1/types_aiobotocore_ivs_realtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-01-18 01:10:06.000000 types-aiobotocore-ivs-realtime-2.9.1/types_aiobotocore_ivs_realtime/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-01-18 01:10:06.000000 types-aiobotocore-ivs-realtime-2.9.1/types_aiobotocore_ivs_realtime/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21106 2024-01-18 01:10:06.000000 types-aiobotocore-ivs-realtime-2.9.1/types_aiobotocore_ivs_realtime/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21103 2024-01-18 01:10:06.000000 types-aiobotocore-ivs-realtime-2.9.1/types_aiobotocore_ivs_realtime/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9180 2024-01-18 01:10:06.000000 types-aiobotocore-ivs-realtime-2.9.1/types_aiobotocore_ivs_realtime/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9180 2024-01-18 01:10:06.000000 types-aiobotocore-ivs-realtime-2.9.1/types_aiobotocore_ivs_realtime/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:10:06.000000 types-aiobotocore-ivs-realtime-2.9.1/types_aiobotocore_ivs_realtime/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    20890 2024-01-18 01:10:06.000000 types-aiobotocore-ivs-realtime-2.9.1/types_aiobotocore_ivs_realtime/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20890 2024-01-18 01:10:06.000000 types-aiobotocore-ivs-realtime-2.9.1/types_aiobotocore_ivs_realtime/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:10:06.000000 types-aiobotocore-ivs-realtime-2.9.1/types_aiobotocore_ivs_realtime/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:59.809255 types-aiobotocore-ivs-realtime-2.9.1/types_aiobotocore_ivs_realtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12543 2024-01-18 01:20:59.000000 types-aiobotocore-ivs-realtime-2.9.1/types_aiobotocore_ivs_realtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-01-18 01:20:59.000000 types-aiobotocore-ivs-realtime-2.9.1/types_aiobotocore_ivs_realtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:59.000000 types-aiobotocore-ivs-realtime-2.9.1/types_aiobotocore_ivs_realtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:59.000000 types-aiobotocore-ivs-realtime-2.9.1/types_aiobotocore_ivs_realtime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:59.000000 types-aiobotocore-ivs-realtime-2.9.1/types_aiobotocore_ivs_realtime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-01-18 01:20:59.000000 types-aiobotocore-ivs-realtime-2.9.1/types_aiobotocore_ivs_realtime.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ivs-realtime-2.9.0/LICENSE` & `types-aiobotocore-ivs-realtime-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-ivs-realtime-2.9.0/PKG-INFO` & `types-aiobotocore-ivs-realtime-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ivs-realtime
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ivsrealtime 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ivsrealtime 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs_realtime/
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
 
 <a id="types-aiobotocore-ivs-realtime"></a>
 
 # types-aiobotocore-ivs-realtime
 
 [![PyPI - types-aiobotocore-ivs-realtime](https://img.shields.io/pypi/v/types-aiobotocore-ivs-realtime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ivs-realtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ivs-realtime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ivs-realtime)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs_realtime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ivs-realtime)](https://pepy.tech/project/types-aiobotocore-ivs-realtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ivsrealtime 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime)
+[aiobotocore.ivsrealtime 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime)
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
 [types-aiobotocore-ivs-realtime docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs_realtime/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-ivs-realtime-2.9.0/README.md` & `types-aiobotocore-ivs-realtime-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ivs-realtime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ivs-realtime)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs_realtime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ivs-realtime)](https://pepy.tech/project/types-aiobotocore-ivs-realtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ivsrealtime 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime)
+[aiobotocore.ivsrealtime 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime)
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
 [types-aiobotocore-ivs-realtime docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs_realtime/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-ivs-realtime-2.9.0/setup.py` & `types-aiobotocore-ivs-realtime-2.9.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ivs-realtime",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_ivs_realtime"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ivsrealtime 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.ivsrealtime 2.9.1 service generated with"
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
     keywords="aiobotocore ivs-realtime type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_ivs_realtime": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs_realtime/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-ivs-realtime-2.9.0/types_aiobotocore_ivs_realtime/__main__.py` & `types-aiobotocore-ivs-realtime-2.9.1/types_aiobotocore_ivs_realtime/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ivsrealtime 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.ivsrealtime 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs_realtime//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime\nOther"
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

### Comparing `types-aiobotocore-ivs-realtime-2.9.0/types_aiobotocore_ivs_realtime/client.py` & `types-aiobotocore-ivs-realtime-2.9.1/types_aiobotocore_ivs_realtime/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,29 +117,29 @@
     async def create_participant_token(
         self,
         *,
         stageArn: str,
         attributes: Mapping[str, str] = ...,
         capabilities: Sequence[ParticipantTokenCapabilityType] = ...,
         duration: int = ...,
-        userId: str = ...
+        userId: str = ...,
     ) -> CreateParticipantTokenResponseTypeDef:
         """
         Creates an additional token for a specified stage.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.create_participant_token)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs_realtime/client/#create_participant_token)
         """
 
     async def create_stage(
         self,
         *,
         name: str = ...,
         participantTokenConfigurations: Sequence[ParticipantTokenConfigurationTypeDef] = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateStageResponseTypeDef:
         """
         Creates a new stage (and optionally participant tokens).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.create_stage)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs_realtime/client/#create_stage)
         """
@@ -262,15 +262,15 @@
 
     async def list_compositions(
         self,
         *,
         filterByEncoderConfigurationArn: str = ...,
         filterByStageArn: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListCompositionsResponseTypeDef:
         """
         Gets summary information about all Compositions in your account, in the AWS
         region where the API request is
         processed.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.list_compositions)
@@ -292,15 +292,15 @@
     async def list_participant_events(
         self,
         *,
         participantId: str,
         sessionId: str,
         stageArn: str,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListParticipantEventsResponseTypeDef:
         """
         Lists events for a specified participant that occurred during a specified stage
         session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.list_participant_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs_realtime/client/#list_participant_events)
@@ -311,15 +311,15 @@
         *,
         sessionId: str,
         stageArn: str,
         filterByPublished: bool = ...,
         filterByState: ParticipantStateType = ...,
         filterByUserId: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListParticipantsResponseTypeDef:
         """
         Lists all participants in a specified stage session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.list_participants)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs_realtime/client/#list_participants)
         """
@@ -371,15 +371,15 @@
     async def start_composition(
         self,
         *,
         destinations: Sequence[DestinationConfigurationTypeDef],
         stageArn: str,
         idempotencyToken: str = ...,
         layout: LayoutConfigurationTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> StartCompositionResponseTypeDef:
         """
         Starts a Composition from a stage based on the configuration provided in the
         request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.start_composition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs_realtime/client/#start_composition)
```

### Comparing `types-aiobotocore-ivs-realtime-2.9.0/types_aiobotocore_ivs_realtime/client.pyi` & `types-aiobotocore-ivs-realtime-2.9.1/types_aiobotocore_ivs_realtime/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -114,29 +114,29 @@
     async def create_participant_token(
         self,
         *,
         stageArn: str,
         attributes: Mapping[str, str] = ...,
         capabilities: Sequence[ParticipantTokenCapabilityType] = ...,
         duration: int = ...,
-        userId: str = ...
+        userId: str = ...,
     ) -> CreateParticipantTokenResponseTypeDef:
         """
         Creates an additional token for a specified stage.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.create_participant_token)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs_realtime/client/#create_participant_token)
         """
 
     async def create_stage(
         self,
         *,
         name: str = ...,
         participantTokenConfigurations: Sequence[ParticipantTokenConfigurationTypeDef] = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateStageResponseTypeDef:
         """
         Creates a new stage (and optionally participant tokens).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.create_stage)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs_realtime/client/#create_stage)
         """
@@ -259,15 +259,15 @@
 
     async def list_compositions(
         self,
         *,
         filterByEncoderConfigurationArn: str = ...,
         filterByStageArn: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListCompositionsResponseTypeDef:
         """
         Gets summary information about all Compositions in your account, in the AWS
         region where the API request is
         processed.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.list_compositions)
@@ -289,15 +289,15 @@
     async def list_participant_events(
         self,
         *,
         participantId: str,
         sessionId: str,
         stageArn: str,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListParticipantEventsResponseTypeDef:
         """
         Lists events for a specified participant that occurred during a specified stage
         session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.list_participant_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs_realtime/client/#list_participant_events)
@@ -308,15 +308,15 @@
         *,
         sessionId: str,
         stageArn: str,
         filterByPublished: bool = ...,
         filterByState: ParticipantStateType = ...,
         filterByUserId: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListParticipantsResponseTypeDef:
         """
         Lists all participants in a specified stage session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.list_participants)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs_realtime/client/#list_participants)
         """
@@ -368,15 +368,15 @@
     async def start_composition(
         self,
         *,
         destinations: Sequence[DestinationConfigurationTypeDef],
         stageArn: str,
         idempotencyToken: str = ...,
         layout: LayoutConfigurationTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> StartCompositionResponseTypeDef:
         """
         Starts a Composition from a stage based on the configuration provided in the
         request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.start_composition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs_realtime/client/#start_composition)
```

### Comparing `types-aiobotocore-ivs-realtime-2.9.0/types_aiobotocore_ivs_realtime/literals.py` & `types-aiobotocore-ivs-realtime-2.9.1/types_aiobotocore_ivs_realtime/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,30 +15,28 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "CompositionStateType",
     "DestinationStateType",
     "EventErrorCodeType",
     "EventNameType",
     "ParticipantStateType",
     "ParticipantTokenCapabilityType",
     "RecordingConfigurationFormatType",
     "ivsrealtimeServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 CompositionStateType = Literal["ACTIVE", "FAILED", "STARTING", "STOPPED", "STOPPING"]
 DestinationStateType = Literal[
     "ACTIVE", "FAILED", "RECONNECTING", "STARTING", "STOPPED", "STOPPING"
 ]
 EventErrorCodeType = Literal["INSUFFICIENT_CAPABILITIES", "PUBLISHER_NOT_FOUND", "QUOTA_EXCEEDED"]
 EventNameType = Literal[
     "JOINED",
```

### Comparing `types-aiobotocore-ivs-realtime-2.9.0/types_aiobotocore_ivs_realtime/literals.pyi` & `types-aiobotocore-ivs-realtime-2.9.1/types_aiobotocore_ivs_realtime/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ivs-realtime-2.9.0/types_aiobotocore_ivs_realtime/type_defs.py` & `types-aiobotocore-ivs-realtime-2.9.1/types_aiobotocore_ivs_realtime/type_defs.py`

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
     "ChannelDestinationConfigurationTypeDef",
     "DestinationSummaryTypeDef",
     "VideoTypeDef",
     "ResponseMetadataTypeDef",
     "CreateParticipantTokenRequestRequestTypeDef",
     "ParticipantTokenTypeDef",
```

### Comparing `types-aiobotocore-ivs-realtime-2.9.0/types_aiobotocore_ivs_realtime/type_defs.pyi` & `types-aiobotocore-ivs-realtime-2.9.1/types_aiobotocore_ivs_realtime/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ivs-realtime-2.9.0/types_aiobotocore_ivs_realtime.egg-info/PKG-INFO` & `types-aiobotocore-ivs-realtime-2.9.1/types_aiobotocore_ivs_realtime.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ivs-realtime
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ivsrealtime 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ivsrealtime 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs_realtime/
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
 
 <a id="types-aiobotocore-ivs-realtime"></a>
 
 # types-aiobotocore-ivs-realtime
 
 [![PyPI - types-aiobotocore-ivs-realtime](https://img.shields.io/pypi/v/types-aiobotocore-ivs-realtime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ivs-realtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ivs-realtime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ivs-realtime)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs_realtime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ivs-realtime)](https://pepy.tech/project/types-aiobotocore-ivs-realtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ivsrealtime 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime)
+[aiobotocore.ivsrealtime 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime)
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
 [types-aiobotocore-ivs-realtime docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs_realtime/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-ivs-realtime-2.9.0/types_aiobotocore_ivs_realtime.egg-info/SOURCES.txt` & `types-aiobotocore-ivs-realtime-2.9.1/types_aiobotocore_ivs_realtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

