# Comparing `tmp/types-aiobotocore-osis-2.9.0.tar.gz` & `tmp/types-aiobotocore-osis-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-osis-2.9.0.tar", last modified: Wed Dec 13 20:00:05 2023, max compression
+gzip compressed data, was "types-aiobotocore-osis-2.9.1.tar", last modified: Thu Jan 18 01:21:26 2024, max compression
```

## Comparing `types-aiobotocore-osis-2.9.0.tar` & `types-aiobotocore-osis-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:05.177357 types-aiobotocore-osis-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:51:20.000000 types-aiobotocore-osis-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12227 2023-12-13 20:00:05.177357 types-aiobotocore-osis-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10661 2023-12-13 19:51:20.000000 types-aiobotocore-osis-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:05.177357 types-aiobotocore-osis-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2023-12-13 19:51:20.000000 types-aiobotocore-osis-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:05.177357 types-aiobotocore-osis-2.9.0/types_aiobotocore_osis/
--rw-r--r--   0 runner    (1001) docker     (127)      494 2023-12-13 19:51:20.000000 types-aiobotocore-osis-2.9.0/types_aiobotocore_osis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2023-12-13 19:51:20.000000 types-aiobotocore-osis-2.9.0/types_aiobotocore_osis/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      939 2023-12-13 19:51:20.000000 types-aiobotocore-osis-2.9.0/types_aiobotocore_osis/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12740 2023-12-13 19:51:20.000000 types-aiobotocore-osis-2.9.0/types_aiobotocore_osis/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    12737 2023-12-13 19:51:20.000000 types-aiobotocore-osis-2.9.0/types_aiobotocore_osis/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8993 2023-12-13 19:51:20.000000 types-aiobotocore-osis-2.9.0/types_aiobotocore_osis/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8991 2023-12-13 19:51:20.000000 types-aiobotocore-osis-2.9.0/types_aiobotocore_osis/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:51:20.000000 types-aiobotocore-osis-2.9.0/types_aiobotocore_osis/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    11395 2023-12-13 19:51:21.000000 types-aiobotocore-osis-2.9.0/types_aiobotocore_osis/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11394 2023-12-13 19:51:21.000000 types-aiobotocore-osis-2.9.0/types_aiobotocore_osis/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:51:20.000000 types-aiobotocore-osis-2.9.0/types_aiobotocore_osis/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:05.177357 types-aiobotocore-osis-2.9.0/types_aiobotocore_osis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12227 2023-12-13 20:00:05.000000 types-aiobotocore-osis-2.9.0/types_aiobotocore_osis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      683 2023-12-13 20:00:05.000000 types-aiobotocore-osis-2.9.0/types_aiobotocore_osis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:05.000000 types-aiobotocore-osis-2.9.0/types_aiobotocore_osis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:05.000000 types-aiobotocore-osis-2.9.0/types_aiobotocore_osis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:05.000000 types-aiobotocore-osis-2.9.0/types_aiobotocore_osis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-13 20:00:05.000000 types-aiobotocore-osis-2.9.0/types_aiobotocore_osis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:26.001136 types-aiobotocore-osis-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:13:00.000000 types-aiobotocore-osis-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12247 2024-01-18 01:21:26.001136 types-aiobotocore-osis-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10661 2024-01-18 01:13:00.000000 types-aiobotocore-osis-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:26.001136 types-aiobotocore-osis-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-01-18 01:13:00.000000 types-aiobotocore-osis-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:26.001136 types-aiobotocore-osis-2.9.1/types_aiobotocore_osis/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-01-18 01:13:00.000000 types-aiobotocore-osis-2.9.1/types_aiobotocore_osis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-01-18 01:13:00.000000 types-aiobotocore-osis-2.9.1/types_aiobotocore_osis/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-01-18 01:13:00.000000 types-aiobotocore-osis-2.9.1/types_aiobotocore_osis/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12742 2024-01-18 01:13:01.000000 types-aiobotocore-osis-2.9.1/types_aiobotocore_osis/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12739 2024-01-18 01:13:01.000000 types-aiobotocore-osis-2.9.1/types_aiobotocore_osis/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8991 2024-01-18 01:13:01.000000 types-aiobotocore-osis-2.9.1/types_aiobotocore_osis/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8991 2024-01-18 01:13:01.000000 types-aiobotocore-osis-2.9.1/types_aiobotocore_osis/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:13:00.000000 types-aiobotocore-osis-2.9.1/types_aiobotocore_osis/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    11394 2024-01-18 01:13:01.000000 types-aiobotocore-osis-2.9.1/types_aiobotocore_osis/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11394 2024-01-18 01:13:01.000000 types-aiobotocore-osis-2.9.1/types_aiobotocore_osis/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:13:00.000000 types-aiobotocore-osis-2.9.1/types_aiobotocore_osis/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:26.001136 types-aiobotocore-osis-2.9.1/types_aiobotocore_osis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12247 2024-01-18 01:21:25.000000 types-aiobotocore-osis-2.9.1/types_aiobotocore_osis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-01-18 01:21:25.000000 types-aiobotocore-osis-2.9.1/types_aiobotocore_osis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:25.000000 types-aiobotocore-osis-2.9.1/types_aiobotocore_osis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:25.000000 types-aiobotocore-osis-2.9.1/types_aiobotocore_osis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:25.000000 types-aiobotocore-osis-2.9.1/types_aiobotocore_osis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-01-18 01:21:25.000000 types-aiobotocore-osis-2.9.1/types_aiobotocore_osis.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-osis-2.9.0/LICENSE` & `types-aiobotocore-osis-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-osis-2.9.0/PKG-INFO` & `types-aiobotocore-osis-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-osis
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.OpenSearchIngestion 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.OpenSearchIngestion 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_osis/
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
 
 <a id="types-aiobotocore-osis"></a>
 
 # types-aiobotocore-osis
 
 [![PyPI - types-aiobotocore-osis](https://img.shields.io/pypi/v/types-aiobotocore-osis.svg?color=blue)](https://pypi.org/project/types-aiobotocore-osis)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-osis.svg?color=blue)](https://pypi.org/project/types-aiobotocore-osis)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_osis/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-osis)](https://pepy.tech/project/types-aiobotocore-osis)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.OpenSearchIngestion 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion)
+[aiobotocore.OpenSearchIngestion 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion)
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
 [types-aiobotocore-osis docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_osis/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-osis-2.9.0/README.md` & `types-aiobotocore-osis-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-osis.svg?color=blue)](https://pypi.org/project/types-aiobotocore-osis)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_osis/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-osis)](https://pepy.tech/project/types-aiobotocore-osis)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.OpenSearchIngestion 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion)
+[aiobotocore.OpenSearchIngestion 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion)
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
 [types-aiobotocore-osis docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_osis/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-osis-2.9.0/setup.py` & `types-aiobotocore-osis-2.9.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-osis",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_osis"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.OpenSearchIngestion 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.OpenSearchIngestion 2.9.1 service generated with"
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
     keywords="aiobotocore osis type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_osis": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_osis/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-osis-2.9.0/types_aiobotocore_osis/client.py` & `types-aiobotocore-osis-2.9.1/types_aiobotocore_osis/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         MinUnits: int,
         MaxUnits: int,
         PipelineConfigurationBody: str,
         LogPublishingOptions: LogPublishingOptionsTypeDef = ...,
         VpcOptions: VpcOptionsTypeDef = ...,
         BufferOptions: BufferOptionsTypeDef = ...,
         EncryptionAtRestOptions: EncryptionAtRestOptionsTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreatePipelineResponseTypeDef:
         """
         Creates an OpenSearch Ingestion pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion.Client.create_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_osis/client/#create_pipeline)
         """
@@ -232,15 +232,15 @@
         *,
         PipelineName: str,
         MinUnits: int = ...,
         MaxUnits: int = ...,
         PipelineConfigurationBody: str = ...,
         LogPublishingOptions: LogPublishingOptionsTypeDef = ...,
         BufferOptions: BufferOptionsTypeDef = ...,
-        EncryptionAtRestOptions: EncryptionAtRestOptionsTypeDef = ...
+        EncryptionAtRestOptions: EncryptionAtRestOptionsTypeDef = ...,
     ) -> UpdatePipelineResponseTypeDef:
         """
         Updates an OpenSearch Ingestion pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion.Client.update_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_osis/client/#update_pipeline)
         """
```

### Comparing `types-aiobotocore-osis-2.9.0/types_aiobotocore_osis/client.pyi` & `types-aiobotocore-osis-2.9.1/types_aiobotocore_osis/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         MinUnits: int,
         MaxUnits: int,
         PipelineConfigurationBody: str,
         LogPublishingOptions: LogPublishingOptionsTypeDef = ...,
         VpcOptions: VpcOptionsTypeDef = ...,
         BufferOptions: BufferOptionsTypeDef = ...,
         EncryptionAtRestOptions: EncryptionAtRestOptionsTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreatePipelineResponseTypeDef:
         """
         Creates an OpenSearch Ingestion pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion.Client.create_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_osis/client/#create_pipeline)
         """
@@ -229,15 +229,15 @@
         *,
         PipelineName: str,
         MinUnits: int = ...,
         MaxUnits: int = ...,
         PipelineConfigurationBody: str = ...,
         LogPublishingOptions: LogPublishingOptionsTypeDef = ...,
         BufferOptions: BufferOptionsTypeDef = ...,
-        EncryptionAtRestOptions: EncryptionAtRestOptionsTypeDef = ...
+        EncryptionAtRestOptions: EncryptionAtRestOptionsTypeDef = ...,
     ) -> UpdatePipelineResponseTypeDef:
         """
         Updates an OpenSearch Ingestion pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion.Client.update_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_osis/client/#update_pipeline)
         """
```

### Comparing `types-aiobotocore-osis-2.9.0/types_aiobotocore_osis/literals.py` & `types-aiobotocore-osis-2.9.1/types_aiobotocore_osis/literals.py`

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
     "ChangeProgressStageStatusesType",
     "ChangeProgressStatusesType",
     "PipelineStatusType",
     "VpcEndpointServiceNameType",
     "OpenSearchIngestionServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 ChangeProgressStageStatusesType = Literal["COMPLETED", "FAILED", "IN_PROGRESS", "PENDING"]
 ChangeProgressStatusesType = Literal["COMPLETED", "FAILED", "IN_PROGRESS", "PENDING"]
 PipelineStatusType = Literal[
     "ACTIVE",
     "CREATE_FAILED",
     "CREATING",
     "DELETING",
```

### Comparing `types-aiobotocore-osis-2.9.0/types_aiobotocore_osis/literals.pyi` & `types-aiobotocore-osis-2.9.1/types_aiobotocore_osis/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-osis-2.9.0/types_aiobotocore_osis/type_defs.py` & `types-aiobotocore-osis-2.9.1/types_aiobotocore_osis/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "BufferOptionsTypeDef",
     "ChangeProgressStageTypeDef",
     "CloudWatchLogDestinationTypeDef",
     "EncryptionAtRestOptionsTypeDef",
     "TagTypeDef",
     "VpcOptionsTypeDef",
```

### Comparing `types-aiobotocore-osis-2.9.0/types_aiobotocore_osis/type_defs.pyi` & `types-aiobotocore-osis-2.9.1/types_aiobotocore_osis/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-osis-2.9.0/types_aiobotocore_osis.egg-info/PKG-INFO` & `types-aiobotocore-osis-2.9.1/types_aiobotocore_osis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-osis
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.OpenSearchIngestion 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.OpenSearchIngestion 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_osis/
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
 
 <a id="types-aiobotocore-osis"></a>
 
 # types-aiobotocore-osis
 
 [![PyPI - types-aiobotocore-osis](https://img.shields.io/pypi/v/types-aiobotocore-osis.svg?color=blue)](https://pypi.org/project/types-aiobotocore-osis)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-osis.svg?color=blue)](https://pypi.org/project/types-aiobotocore-osis)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_osis/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-osis)](https://pepy.tech/project/types-aiobotocore-osis)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.OpenSearchIngestion 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion)
+[aiobotocore.OpenSearchIngestion 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion)
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
 [types-aiobotocore-osis docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_osis/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-osis-2.9.0/types_aiobotocore_osis.egg-info/SOURCES.txt` & `types-aiobotocore-osis-2.9.1/types_aiobotocore_osis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

