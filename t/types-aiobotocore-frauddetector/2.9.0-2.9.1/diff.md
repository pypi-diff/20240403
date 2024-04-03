# Comparing `tmp/types-aiobotocore-frauddetector-2.9.0.tar.gz` & `tmp/types-aiobotocore-frauddetector-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-frauddetector-2.9.0.tar", last modified: Wed Dec 13 19:59:21 2023, max compression
+gzip compressed data, was "types-aiobotocore-frauddetector-2.9.1.tar", last modified: Thu Jan 18 01:20:45 2024, max compression
```

## Comparing `types-aiobotocore-frauddetector-2.9.0.tar` & `types-aiobotocore-frauddetector-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:21.261745 types-aiobotocore-frauddetector-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:46:25.000000 types-aiobotocore-frauddetector-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12555 2023-12-13 19:59:21.261745 types-aiobotocore-frauddetector-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10968 2023-12-13 19:46:25.000000 types-aiobotocore-frauddetector-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:21.261745 types-aiobotocore-frauddetector-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2023-12-13 19:46:25.000000 types-aiobotocore-frauddetector-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:21.261745 types-aiobotocore-frauddetector-2.9.0/types_aiobotocore_frauddetector/
--rw-r--r--   0 runner    (1001) docker     (127)      491 2023-12-13 19:46:25.000000 types-aiobotocore-frauddetector-2.9.0/types_aiobotocore_frauddetector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2023-12-13 19:46:25.000000 types-aiobotocore-frauddetector-2.9.0/types_aiobotocore_frauddetector/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      956 2023-12-13 19:46:25.000000 types-aiobotocore-frauddetector-2.9.0/types_aiobotocore_frauddetector/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    49188 2023-12-13 19:46:25.000000 types-aiobotocore-frauddetector-2.9.0/types_aiobotocore_frauddetector/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    49184 2023-12-13 19:46:25.000000 types-aiobotocore-frauddetector-2.9.0/types_aiobotocore_frauddetector/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9885 2023-12-13 19:46:25.000000 types-aiobotocore-frauddetector-2.9.0/types_aiobotocore_frauddetector/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9883 2023-12-13 19:46:25.000000 types-aiobotocore-frauddetector-2.9.0/types_aiobotocore_frauddetector/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:46:25.000000 types-aiobotocore-frauddetector-2.9.0/types_aiobotocore_frauddetector/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    52800 2023-12-13 19:46:26.000000 types-aiobotocore-frauddetector-2.9.0/types_aiobotocore_frauddetector/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    52799 2023-12-13 19:46:26.000000 types-aiobotocore-frauddetector-2.9.0/types_aiobotocore_frauddetector/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:46:25.000000 types-aiobotocore-frauddetector-2.9.0/types_aiobotocore_frauddetector/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:21.261745 types-aiobotocore-frauddetector-2.9.0/types_aiobotocore_frauddetector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12555 2023-12-13 19:59:21.000000 types-aiobotocore-frauddetector-2.9.0/types_aiobotocore_frauddetector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      836 2023-12-13 19:59:21.000000 types-aiobotocore-frauddetector-2.9.0/types_aiobotocore_frauddetector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:21.000000 types-aiobotocore-frauddetector-2.9.0/types_aiobotocore_frauddetector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:21.000000 types-aiobotocore-frauddetector-2.9.0/types_aiobotocore_frauddetector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:21.000000 types-aiobotocore-frauddetector-2.9.0/types_aiobotocore_frauddetector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-13 19:59:21.000000 types-aiobotocore-frauddetector-2.9.0/types_aiobotocore_frauddetector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:45.565320 types-aiobotocore-frauddetector-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:08:18.000000 types-aiobotocore-frauddetector-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12575 2024-01-18 01:20:45.565320 types-aiobotocore-frauddetector-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10968 2024-01-18 01:08:18.000000 types-aiobotocore-frauddetector-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:45.565320 types-aiobotocore-frauddetector-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-01-18 01:08:17.000000 types-aiobotocore-frauddetector-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:45.565320 types-aiobotocore-frauddetector-2.9.1/types_aiobotocore_frauddetector/
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-01-18 01:08:18.000000 types-aiobotocore-frauddetector-2.9.1/types_aiobotocore_frauddetector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-01-18 01:08:18.000000 types-aiobotocore-frauddetector-2.9.1/types_aiobotocore_frauddetector/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-01-18 01:08:18.000000 types-aiobotocore-frauddetector-2.9.1/types_aiobotocore_frauddetector/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49210 2024-01-18 01:08:19.000000 types-aiobotocore-frauddetector-2.9.1/types_aiobotocore_frauddetector/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49207 2024-01-18 01:08:19.000000 types-aiobotocore-frauddetector-2.9.1/types_aiobotocore_frauddetector/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9883 2024-01-18 01:08:19.000000 types-aiobotocore-frauddetector-2.9.1/types_aiobotocore_frauddetector/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9883 2024-01-18 01:08:19.000000 types-aiobotocore-frauddetector-2.9.1/types_aiobotocore_frauddetector/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:08:18.000000 types-aiobotocore-frauddetector-2.9.1/types_aiobotocore_frauddetector/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    52799 2024-01-18 01:08:20.000000 types-aiobotocore-frauddetector-2.9.1/types_aiobotocore_frauddetector/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52799 2024-01-18 01:08:20.000000 types-aiobotocore-frauddetector-2.9.1/types_aiobotocore_frauddetector/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:08:18.000000 types-aiobotocore-frauddetector-2.9.1/types_aiobotocore_frauddetector/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:45.565320 types-aiobotocore-frauddetector-2.9.1/types_aiobotocore_frauddetector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12575 2024-01-18 01:20:45.000000 types-aiobotocore-frauddetector-2.9.1/types_aiobotocore_frauddetector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-01-18 01:20:45.000000 types-aiobotocore-frauddetector-2.9.1/types_aiobotocore_frauddetector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:45.000000 types-aiobotocore-frauddetector-2.9.1/types_aiobotocore_frauddetector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:45.000000 types-aiobotocore-frauddetector-2.9.1/types_aiobotocore_frauddetector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:45.000000 types-aiobotocore-frauddetector-2.9.1/types_aiobotocore_frauddetector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-01-18 01:20:45.000000 types-aiobotocore-frauddetector-2.9.1/types_aiobotocore_frauddetector.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-frauddetector-2.9.0/LICENSE` & `types-aiobotocore-frauddetector-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-frauddetector-2.9.0/PKG-INFO` & `types-aiobotocore-frauddetector-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-frauddetector
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.FraudDetector 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.FraudDetector 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/
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
 
 <a id="types-aiobotocore-frauddetector"></a>
 
 # types-aiobotocore-frauddetector
 
 [![PyPI - types-aiobotocore-frauddetector](https://img.shields.io/pypi/v/types-aiobotocore-frauddetector.svg?color=blue)](https://pypi.org/project/types-aiobotocore-frauddetector)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-frauddetector.svg?color=blue)](https://pypi.org/project/types-aiobotocore-frauddetector)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-frauddetector)](https://pepy.tech/project/types-aiobotocore-frauddetector)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.FraudDetector 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector)
+[aiobotocore.FraudDetector 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector)
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
 [types-aiobotocore-frauddetector docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-frauddetector-2.9.0/README.md` & `types-aiobotocore-frauddetector-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-frauddetector.svg?color=blue)](https://pypi.org/project/types-aiobotocore-frauddetector)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-frauddetector)](https://pepy.tech/project/types-aiobotocore-frauddetector)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.FraudDetector 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector)
+[aiobotocore.FraudDetector 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector)
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
 [types-aiobotocore-frauddetector docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-frauddetector-2.9.0/setup.py` & `types-aiobotocore-frauddetector-2.9.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-frauddetector",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_frauddetector"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.FraudDetector 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.FraudDetector 2.9.1 service generated with"
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
     keywords="aiobotocore frauddetector type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_frauddetector": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-frauddetector-2.9.0/types_aiobotocore_frauddetector/__main__.py` & `types-aiobotocore-frauddetector-2.9.1/types_aiobotocore_frauddetector/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.FraudDetector 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.FraudDetector 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector\nOther"
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

### Comparing `types-aiobotocore-frauddetector-2.9.0/types_aiobotocore_frauddetector/client.py` & `types-aiobotocore-frauddetector-2.9.1/types_aiobotocore_frauddetector/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("FraudDetectorClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -181,15 +180,15 @@
         self,
         *,
         jobId: str,
         inputPath: str,
         outputPath: str,
         eventTypeName: str,
         iamRoleArn: str,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Creates a batch import job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.create_batch_import_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#create_batch_import_job)
         """
@@ -200,15 +199,15 @@
         jobId: str,
         inputPath: str,
         outputPath: str,
         eventTypeName: str,
         detectorName: str,
         iamRoleArn: str,
         detectorVersion: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Creates a batch prediction job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.create_batch_prediction_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#create_batch_prediction_job)
         """
@@ -218,15 +217,15 @@
         *,
         detectorId: str,
         rules: Sequence[RuleTypeDef],
         description: str = ...,
         externalModelEndpoints: Sequence[str] = ...,
         modelVersions: Sequence[ModelVersionTypeDef] = ...,
         ruleExecutionMode: RuleExecutionModeType = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDetectorVersionResultTypeDef:
         """
         Creates a detector version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.create_detector_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#create_detector_version)
         """
@@ -234,15 +233,15 @@
     async def create_list(
         self,
         *,
         name: str,
         elements: Sequence[str] = ...,
         variableType: str = ...,
         description: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Creates a list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.create_list)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#create_list)
         """
@@ -250,15 +249,15 @@
     async def create_model(
         self,
         *,
         modelId: str,
         modelType: ModelTypeEnumType,
         eventTypeName: str,
         description: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Creates a model using the specified model type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.create_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#create_model)
         """
@@ -268,15 +267,15 @@
         *,
         modelId: str,
         modelType: ModelTypeEnumType,
         trainingDataSource: TrainingDataSourceEnumType,
         trainingDataSchema: TrainingDataSchemaTypeDef,
         externalEventsDetail: ExternalEventsDetailTypeDef = ...,
         ingestedEventsDetail: IngestedEventsDetailTypeDef = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateModelVersionResultTypeDef:
         """
         Creates a version of the model using the specified model type and model id.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.create_model_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#create_model_version)
         """
@@ -286,15 +285,15 @@
         *,
         ruleId: str,
         detectorId: str,
         expression: str,
         language: Literal["DETECTORPL"],
         outcomes: Sequence[str],
         description: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateRuleResultTypeDef:
         """
         Creates a rule for use with the specified detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.create_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#create_rule)
         """
@@ -304,15 +303,15 @@
         *,
         name: str,
         dataType: DataTypeType,
         dataSource: DataSourceType,
         defaultValue: str,
         description: str = ...,
         variableType: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Creates a variable.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.create_variable)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#create_variable)
         """
@@ -466,15 +465,15 @@
     async def describe_model_versions(
         self,
         *,
         modelId: str = ...,
         modelVersionNumber: str = ...,
         modelType: ModelTypeEnumType = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> DescribeModelVersionsResultTypeDef:
         """
         Gets all of the model versions for the specified model type or for the
         specified model type and model
         ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.describe_model_versions)
@@ -569,15 +568,15 @@
         detectorId: str,
         eventId: str,
         eventTypeName: str,
         entities: Sequence[EntityTypeDef],
         eventTimestamp: str,
         eventVariables: Mapping[str, str],
         detectorVersionId: str = ...,
-        externalModelEndpointDataBlobs: Mapping[str, ModelEndpointDataBlobTypeDef] = ...
+        externalModelEndpointDataBlobs: Mapping[str, ModelEndpointDataBlobTypeDef] = ...,
     ) -> GetEventPredictionResultTypeDef:
         """
         Evaluates an event against a detector version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_event_prediction)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#get_event_prediction)
         """
@@ -585,15 +584,15 @@
     async def get_event_prediction_metadata(
         self,
         *,
         eventId: str,
         eventTypeName: str,
         detectorId: str,
         detectorVersionId: str,
-        predictionTimestamp: str
+        predictionTimestamp: str,
     ) -> GetEventPredictionMetadataResultTypeDef:
         """
         Gets details of the past fraud predictions for the specified event ID, event
         type, detector ID, and detector version ID that was generated in the specified
         time
         period.
 
@@ -676,15 +675,15 @@
 
     async def get_models(
         self,
         *,
         modelId: str = ...,
         modelType: ModelTypeEnumType = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> GetModelsResultTypeDef:
         """
         Gets one or more models.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_models)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#get_models)
         """
@@ -702,15 +701,15 @@
     async def get_rules(
         self,
         *,
         detectorId: str,
         ruleId: str = ...,
         ruleVersion: str = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> GetRulesResultTypeDef:
         """
         Get all rules for a detector (paginated) if `ruleId` and `ruleVersion` are not
         specified.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_rules)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#get_rules)
@@ -731,15 +730,15 @@
         *,
         eventId: FilterConditionTypeDef = ...,
         eventType: FilterConditionTypeDef = ...,
         detectorId: FilterConditionTypeDef = ...,
         detectorVersionId: FilterConditionTypeDef = ...,
         predictionTimeRange: PredictionTimeRangeTypeDef = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListEventPredictionsResultTypeDef:
         """
         Gets a list of past predictions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.list_event_predictions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#list_event_predictions)
         """
@@ -756,15 +755,15 @@
 
     async def put_detector(
         self,
         *,
         detectorId: str,
         eventTypeName: str,
         description: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Creates or updates a detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.put_detector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#put_detector)
         """
@@ -785,15 +784,15 @@
         name: str,
         eventVariables: Sequence[str],
         entityTypes: Sequence[str],
         description: str = ...,
         labels: Sequence[str] = ...,
         eventIngestion: EventIngestionType = ...,
         tags: Sequence[TagTypeDef] = ...,
-        eventOrchestration: EventOrchestrationTypeDef = ...
+        eventOrchestration: EventOrchestrationTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Creates or updates an event type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.put_event_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#put_event_type)
         """
@@ -803,15 +802,15 @@
         *,
         modelEndpoint: str,
         modelSource: Literal["SAGEMAKER"],
         invokeModelEndpointRoleArn: str,
         inputConfiguration: ModelInputConfigurationTypeDef,
         outputConfiguration: ModelOutputConfigurationTypeDef,
         modelEndpointStatus: ModelEndpointStatusType,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Creates or updates an Amazon SageMaker model endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.put_external_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#put_external_model)
         """
@@ -849,15 +848,15 @@
         *,
         eventId: str,
         eventTypeName: str,
         eventTimestamp: str,
         eventVariables: Mapping[str, str],
         entities: Sequence[EntityTypeDef],
         assignedLabel: str = ...,
-        labelTimestamp: str = ...
+        labelTimestamp: str = ...,
     ) -> Dict[str, Any]:
         """
         Stores events in Amazon Fraud Detector without generating fraud predictions for
         those
         events.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.send_event)
@@ -885,15 +884,15 @@
         *,
         detectorId: str,
         detectorVersionId: str,
         externalModelEndpoints: Sequence[str],
         rules: Sequence[RuleTypeDef],
         description: str = ...,
         modelVersions: Sequence[ModelVersionTypeDef] = ...,
-        ruleExecutionMode: RuleExecutionModeType = ...
+        ruleExecutionMode: RuleExecutionModeType = ...,
     ) -> Dict[str, Any]:
         """
         Updates a detector version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_detector_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#update_detector_version)
         """
@@ -931,15 +930,15 @@
     async def update_list(
         self,
         *,
         name: str,
         elements: Sequence[str] = ...,
         description: str = ...,
         updateMode: ListUpdateModeType = ...,
-        variableType: str = ...
+        variableType: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates a list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_list)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#update_list)
         """
@@ -958,30 +957,30 @@
         self,
         *,
         modelId: str,
         modelType: ModelTypeEnumType,
         majorVersionNumber: str,
         externalEventsDetail: ExternalEventsDetailTypeDef = ...,
         ingestedEventsDetail: IngestedEventsDetailTypeDef = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> UpdateModelVersionResultTypeDef:
         """
         Updates a model version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_model_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#update_model_version)
         """
 
     async def update_model_version_status(
         self,
         *,
         modelId: str,
         modelType: ModelTypeEnumType,
         modelVersionNumber: str,
-        status: ModelVersionStatusType
+        status: ModelVersionStatusType,
     ) -> Dict[str, Any]:
         """
         Updates the status of a model version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_model_version_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#update_model_version_status)
         """
@@ -998,15 +997,15 @@
         self,
         *,
         rule: RuleTypeDef,
         expression: str,
         language: Literal["DETECTORPL"],
         outcomes: Sequence[str],
         description: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> UpdateRuleVersionResultTypeDef:
         """
         Updates a rule version resulting in a new rule version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_rule_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#update_rule_version)
         """
```

### Comparing `types-aiobotocore-frauddetector-2.9.0/types_aiobotocore_frauddetector/client.pyi` & `types-aiobotocore-frauddetector-2.9.1/types_aiobotocore_frauddetector/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,15 @@
         self,
         *,
         jobId: str,
         inputPath: str,
         outputPath: str,
         eventTypeName: str,
         iamRoleArn: str,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Creates a batch import job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.create_batch_import_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#create_batch_import_job)
         """
@@ -196,15 +196,15 @@
         jobId: str,
         inputPath: str,
         outputPath: str,
         eventTypeName: str,
         detectorName: str,
         iamRoleArn: str,
         detectorVersion: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Creates a batch prediction job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.create_batch_prediction_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#create_batch_prediction_job)
         """
@@ -214,15 +214,15 @@
         *,
         detectorId: str,
         rules: Sequence[RuleTypeDef],
         description: str = ...,
         externalModelEndpoints: Sequence[str] = ...,
         modelVersions: Sequence[ModelVersionTypeDef] = ...,
         ruleExecutionMode: RuleExecutionModeType = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDetectorVersionResultTypeDef:
         """
         Creates a detector version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.create_detector_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#create_detector_version)
         """
@@ -230,15 +230,15 @@
     async def create_list(
         self,
         *,
         name: str,
         elements: Sequence[str] = ...,
         variableType: str = ...,
         description: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Creates a list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.create_list)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#create_list)
         """
@@ -246,15 +246,15 @@
     async def create_model(
         self,
         *,
         modelId: str,
         modelType: ModelTypeEnumType,
         eventTypeName: str,
         description: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Creates a model using the specified model type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.create_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#create_model)
         """
@@ -264,15 +264,15 @@
         *,
         modelId: str,
         modelType: ModelTypeEnumType,
         trainingDataSource: TrainingDataSourceEnumType,
         trainingDataSchema: TrainingDataSchemaTypeDef,
         externalEventsDetail: ExternalEventsDetailTypeDef = ...,
         ingestedEventsDetail: IngestedEventsDetailTypeDef = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateModelVersionResultTypeDef:
         """
         Creates a version of the model using the specified model type and model id.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.create_model_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#create_model_version)
         """
@@ -282,15 +282,15 @@
         *,
         ruleId: str,
         detectorId: str,
         expression: str,
         language: Literal["DETECTORPL"],
         outcomes: Sequence[str],
         description: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateRuleResultTypeDef:
         """
         Creates a rule for use with the specified detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.create_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#create_rule)
         """
@@ -300,15 +300,15 @@
         *,
         name: str,
         dataType: DataTypeType,
         dataSource: DataSourceType,
         defaultValue: str,
         description: str = ...,
         variableType: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Creates a variable.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.create_variable)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#create_variable)
         """
@@ -462,15 +462,15 @@
     async def describe_model_versions(
         self,
         *,
         modelId: str = ...,
         modelVersionNumber: str = ...,
         modelType: ModelTypeEnumType = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> DescribeModelVersionsResultTypeDef:
         """
         Gets all of the model versions for the specified model type or for the
         specified model type and model
         ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.describe_model_versions)
@@ -565,15 +565,15 @@
         detectorId: str,
         eventId: str,
         eventTypeName: str,
         entities: Sequence[EntityTypeDef],
         eventTimestamp: str,
         eventVariables: Mapping[str, str],
         detectorVersionId: str = ...,
-        externalModelEndpointDataBlobs: Mapping[str, ModelEndpointDataBlobTypeDef] = ...
+        externalModelEndpointDataBlobs: Mapping[str, ModelEndpointDataBlobTypeDef] = ...,
     ) -> GetEventPredictionResultTypeDef:
         """
         Evaluates an event against a detector version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_event_prediction)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#get_event_prediction)
         """
@@ -581,15 +581,15 @@
     async def get_event_prediction_metadata(
         self,
         *,
         eventId: str,
         eventTypeName: str,
         detectorId: str,
         detectorVersionId: str,
-        predictionTimestamp: str
+        predictionTimestamp: str,
     ) -> GetEventPredictionMetadataResultTypeDef:
         """
         Gets details of the past fraud predictions for the specified event ID, event
         type, detector ID, and detector version ID that was generated in the specified
         time
         period.
 
@@ -672,15 +672,15 @@
 
     async def get_models(
         self,
         *,
         modelId: str = ...,
         modelType: ModelTypeEnumType = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> GetModelsResultTypeDef:
         """
         Gets one or more models.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_models)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#get_models)
         """
@@ -698,15 +698,15 @@
     async def get_rules(
         self,
         *,
         detectorId: str,
         ruleId: str = ...,
         ruleVersion: str = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> GetRulesResultTypeDef:
         """
         Get all rules for a detector (paginated) if `ruleId` and `ruleVersion` are not
         specified.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_rules)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#get_rules)
@@ -727,15 +727,15 @@
         *,
         eventId: FilterConditionTypeDef = ...,
         eventType: FilterConditionTypeDef = ...,
         detectorId: FilterConditionTypeDef = ...,
         detectorVersionId: FilterConditionTypeDef = ...,
         predictionTimeRange: PredictionTimeRangeTypeDef = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListEventPredictionsResultTypeDef:
         """
         Gets a list of past predictions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.list_event_predictions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#list_event_predictions)
         """
@@ -752,15 +752,15 @@
 
     async def put_detector(
         self,
         *,
         detectorId: str,
         eventTypeName: str,
         description: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Creates or updates a detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.put_detector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#put_detector)
         """
@@ -781,15 +781,15 @@
         name: str,
         eventVariables: Sequence[str],
         entityTypes: Sequence[str],
         description: str = ...,
         labels: Sequence[str] = ...,
         eventIngestion: EventIngestionType = ...,
         tags: Sequence[TagTypeDef] = ...,
-        eventOrchestration: EventOrchestrationTypeDef = ...
+        eventOrchestration: EventOrchestrationTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Creates or updates an event type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.put_event_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#put_event_type)
         """
@@ -799,15 +799,15 @@
         *,
         modelEndpoint: str,
         modelSource: Literal["SAGEMAKER"],
         invokeModelEndpointRoleArn: str,
         inputConfiguration: ModelInputConfigurationTypeDef,
         outputConfiguration: ModelOutputConfigurationTypeDef,
         modelEndpointStatus: ModelEndpointStatusType,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Creates or updates an Amazon SageMaker model endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.put_external_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#put_external_model)
         """
@@ -845,15 +845,15 @@
         *,
         eventId: str,
         eventTypeName: str,
         eventTimestamp: str,
         eventVariables: Mapping[str, str],
         entities: Sequence[EntityTypeDef],
         assignedLabel: str = ...,
-        labelTimestamp: str = ...
+        labelTimestamp: str = ...,
     ) -> Dict[str, Any]:
         """
         Stores events in Amazon Fraud Detector without generating fraud predictions for
         those
         events.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.send_event)
@@ -881,15 +881,15 @@
         *,
         detectorId: str,
         detectorVersionId: str,
         externalModelEndpoints: Sequence[str],
         rules: Sequence[RuleTypeDef],
         description: str = ...,
         modelVersions: Sequence[ModelVersionTypeDef] = ...,
-        ruleExecutionMode: RuleExecutionModeType = ...
+        ruleExecutionMode: RuleExecutionModeType = ...,
     ) -> Dict[str, Any]:
         """
         Updates a detector version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_detector_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#update_detector_version)
         """
@@ -927,15 +927,15 @@
     async def update_list(
         self,
         *,
         name: str,
         elements: Sequence[str] = ...,
         description: str = ...,
         updateMode: ListUpdateModeType = ...,
-        variableType: str = ...
+        variableType: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates a list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_list)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#update_list)
         """
@@ -954,30 +954,30 @@
         self,
         *,
         modelId: str,
         modelType: ModelTypeEnumType,
         majorVersionNumber: str,
         externalEventsDetail: ExternalEventsDetailTypeDef = ...,
         ingestedEventsDetail: IngestedEventsDetailTypeDef = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> UpdateModelVersionResultTypeDef:
         """
         Updates a model version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_model_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#update_model_version)
         """
 
     async def update_model_version_status(
         self,
         *,
         modelId: str,
         modelType: ModelTypeEnumType,
         modelVersionNumber: str,
-        status: ModelVersionStatusType
+        status: ModelVersionStatusType,
     ) -> Dict[str, Any]:
         """
         Updates the status of a model version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_model_version_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#update_model_version_status)
         """
@@ -994,15 +994,15 @@
         self,
         *,
         rule: RuleTypeDef,
         expression: str,
         language: Literal["DETECTORPL"],
         outcomes: Sequence[str],
         description: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> UpdateRuleVersionResultTypeDef:
         """
         Updates a rule version resulting in a new rule version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_rule_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#update_rule_version)
         """
```

### Comparing `types-aiobotocore-frauddetector-2.9.0/types_aiobotocore_frauddetector/literals.py` & `types-aiobotocore-frauddetector-2.9.1/types_aiobotocore_frauddetector/literals.py`

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
     "AsyncJobStatusType",
     "DataSourceType",
     "DataTypeType",
     "DetectorVersionStatusType",
     "EventIngestionType",
     "LanguageType",
@@ -39,15 +38,14 @@
     "UnlabeledEventsTreatmentType",
     "FraudDetectorServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 AsyncJobStatusType = Literal[
     "CANCELED",
     "CANCEL_IN_PROGRESS",
     "COMPLETE",
     "FAILED",
     "IN_PROGRESS",
     "IN_PROGRESS_INITIALIZING",
```

### Comparing `types-aiobotocore-frauddetector-2.9.0/types_aiobotocore_frauddetector/literals.pyi` & `types-aiobotocore-frauddetector-2.9.1/types_aiobotocore_frauddetector/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-frauddetector-2.9.0/types_aiobotocore_frauddetector/type_defs.py` & `types-aiobotocore-frauddetector-2.9.1/types_aiobotocore_frauddetector/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ATIMetricDataPointTypeDef",
     "ATIModelPerformanceTypeDef",
     "AggregatedLogOddsMetricTypeDef",
     "AggregatedVariablesImpactExplanationTypeDef",
     "AllowDenyListTypeDef",
     "BatchCreateVariableErrorTypeDef",
```

### Comparing `types-aiobotocore-frauddetector-2.9.0/types_aiobotocore_frauddetector/type_defs.pyi` & `types-aiobotocore-frauddetector-2.9.1/types_aiobotocore_frauddetector/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-frauddetector-2.9.0/types_aiobotocore_frauddetector.egg-info/PKG-INFO` & `types-aiobotocore-frauddetector-2.9.1/types_aiobotocore_frauddetector.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-frauddetector
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.FraudDetector 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.FraudDetector 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/
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
 
 <a id="types-aiobotocore-frauddetector"></a>
 
 # types-aiobotocore-frauddetector
 
 [![PyPI - types-aiobotocore-frauddetector](https://img.shields.io/pypi/v/types-aiobotocore-frauddetector.svg?color=blue)](https://pypi.org/project/types-aiobotocore-frauddetector)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-frauddetector.svg?color=blue)](https://pypi.org/project/types-aiobotocore-frauddetector)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-frauddetector)](https://pepy.tech/project/types-aiobotocore-frauddetector)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.FraudDetector 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector)
+[aiobotocore.FraudDetector 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector)
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
 [types-aiobotocore-frauddetector docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-frauddetector-2.9.0/types_aiobotocore_frauddetector.egg-info/SOURCES.txt` & `types-aiobotocore-frauddetector-2.9.1/types_aiobotocore_frauddetector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

