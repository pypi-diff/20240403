# Comparing `tmp/types-aiobotocore-batch-2.9.0.tar.gz` & `tmp/types-aiobotocore-batch-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-batch-2.9.0.tar", last modified: Wed Dec 13 19:58:40 2023, max compression
+gzip compressed data, was "types-aiobotocore-batch-2.9.1.tar", last modified: Thu Jan 18 01:20:08 2024, max compression
```

## Comparing `types-aiobotocore-batch-2.9.0.tar` & `types-aiobotocore-batch-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:40.978042 types-aiobotocore-batch-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:41:38.000000 types-aiobotocore-batch-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13525 2023-12-13 19:58:40.978042 types-aiobotocore-batch-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11970 2023-12-13 19:41:38.000000 types-aiobotocore-batch-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:40.978042 types-aiobotocore-batch-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2023-12-13 19:41:38.000000 types-aiobotocore-batch-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:40.978042 types-aiobotocore-batch-2.9.0/types_aiobotocore_batch/
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2023-12-13 19:41:38.000000 types-aiobotocore-batch-2.9.0/types_aiobotocore_batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2023-12-13 19:41:38.000000 types-aiobotocore-batch-2.9.0/types_aiobotocore_batch/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      913 2023-12-13 19:41:38.000000 types-aiobotocore-batch-2.9.0/types_aiobotocore_batch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22151 2023-12-13 19:41:39.000000 types-aiobotocore-batch-2.9.0/types_aiobotocore_batch/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    22147 2023-12-13 19:41:38.000000 types-aiobotocore-batch-2.9.0/types_aiobotocore_batch/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11313 2023-12-13 19:41:39.000000 types-aiobotocore-batch-2.9.0/types_aiobotocore_batch/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11311 2023-12-13 19:41:39.000000 types-aiobotocore-batch-2.9.0/types_aiobotocore_batch/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6997 2023-12-13 19:41:39.000000 types-aiobotocore-batch-2.9.0/types_aiobotocore_batch/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6990 2023-12-13 19:41:39.000000 types-aiobotocore-batch-2.9.0/types_aiobotocore_batch/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:41:38.000000 types-aiobotocore-batch-2.9.0/types_aiobotocore_batch/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    42912 2023-12-13 19:41:40.000000 types-aiobotocore-batch-2.9.0/types_aiobotocore_batch/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    42911 2023-12-13 19:41:39.000000 types-aiobotocore-batch-2.9.0/types_aiobotocore_batch/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:41:38.000000 types-aiobotocore-batch-2.9.0/types_aiobotocore_batch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:40.978042 types-aiobotocore-batch-2.9.0/types_aiobotocore_batch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13525 2023-12-13 19:58:40.000000 types-aiobotocore-batch-2.9.0/types_aiobotocore_batch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      775 2023-12-13 19:58:40.000000 types-aiobotocore-batch-2.9.0/types_aiobotocore_batch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:40.000000 types-aiobotocore-batch-2.9.0/types_aiobotocore_batch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:40.000000 types-aiobotocore-batch-2.9.0/types_aiobotocore_batch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:40.000000 types-aiobotocore-batch-2.9.0/types_aiobotocore_batch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-13 19:58:40.000000 types-aiobotocore-batch-2.9.0/types_aiobotocore_batch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:08.517494 types-aiobotocore-batch-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:03:36.000000 types-aiobotocore-batch-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13545 2024-01-18 01:20:08.517494 types-aiobotocore-batch-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11970 2024-01-18 01:03:36.000000 types-aiobotocore-batch-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:08.517494 types-aiobotocore-batch-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-01-18 01:03:36.000000 types-aiobotocore-batch-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:08.517494 types-aiobotocore-batch-2.9.1/types_aiobotocore_batch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-01-18 01:03:36.000000 types-aiobotocore-batch-2.9.1/types_aiobotocore_batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-01-18 01:03:36.000000 types-aiobotocore-batch-2.9.1/types_aiobotocore_batch/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-01-18 01:03:36.000000 types-aiobotocore-batch-2.9.1/types_aiobotocore_batch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22160 2024-01-18 01:03:37.000000 types-aiobotocore-batch-2.9.1/types_aiobotocore_batch/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22157 2024-01-18 01:03:36.000000 types-aiobotocore-batch-2.9.1/types_aiobotocore_batch/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11311 2024-01-18 01:03:37.000000 types-aiobotocore-batch-2.9.1/types_aiobotocore_batch/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11311 2024-01-18 01:03:37.000000 types-aiobotocore-batch-2.9.1/types_aiobotocore_batch/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6999 2024-01-18 01:03:37.000000 types-aiobotocore-batch-2.9.1/types_aiobotocore_batch/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-01-18 01:03:37.000000 types-aiobotocore-batch-2.9.1/types_aiobotocore_batch/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:03:36.000000 types-aiobotocore-batch-2.9.1/types_aiobotocore_batch/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    42911 2024-01-18 01:03:38.000000 types-aiobotocore-batch-2.9.1/types_aiobotocore_batch/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42911 2024-01-18 01:03:37.000000 types-aiobotocore-batch-2.9.1/types_aiobotocore_batch/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:03:36.000000 types-aiobotocore-batch-2.9.1/types_aiobotocore_batch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:08.517494 types-aiobotocore-batch-2.9.1/types_aiobotocore_batch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13545 2024-01-18 01:20:08.000000 types-aiobotocore-batch-2.9.1/types_aiobotocore_batch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-01-18 01:20:08.000000 types-aiobotocore-batch-2.9.1/types_aiobotocore_batch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:08.000000 types-aiobotocore-batch-2.9.1/types_aiobotocore_batch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:08.000000 types-aiobotocore-batch-2.9.1/types_aiobotocore_batch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:08.000000 types-aiobotocore-batch-2.9.1/types_aiobotocore_batch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-01-18 01:20:08.000000 types-aiobotocore-batch-2.9.1/types_aiobotocore_batch.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-batch-2.9.0/LICENSE` & `types-aiobotocore-batch-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-batch-2.9.0/PKG-INFO` & `types-aiobotocore-batch-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-batch
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Batch 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Batch 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/
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
 
 <a id="types-aiobotocore-batch"></a>
 
 # types-aiobotocore-batch
 
 [![PyPI - types-aiobotocore-batch](https://img.shields.io/pypi/v/types-aiobotocore-batch.svg?color=blue)](https://pypi.org/project/types-aiobotocore-batch)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-batch.svg?color=blue)](https://pypi.org/project/types-aiobotocore-batch)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-batch)](https://pepy.tech/project/types-aiobotocore-batch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Batch 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
+[aiobotocore.Batch 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
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
 [types-aiobotocore-batch docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-batch-2.9.0/README.md` & `types-aiobotocore-batch-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-batch.svg?color=blue)](https://pypi.org/project/types-aiobotocore-batch)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-batch)](https://pepy.tech/project/types-aiobotocore-batch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Batch 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
+[aiobotocore.Batch 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
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
 [types-aiobotocore-batch docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-batch-2.9.0/setup.py` & `types-aiobotocore-batch-2.9.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-batch",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_batch"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Batch 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.Batch 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore batch type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_batch": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-batch-2.9.0/types_aiobotocore_batch/__init__.py` & `types-aiobotocore-batch-2.9.1/types_aiobotocore_batch/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     DescribeJobQueuesPaginator,
     ListJobsPaginator,
     ListSchedulingPoliciesPaginator,
 )
 
 Client = BatchClient
 
-
 __all__ = (
     "BatchClient",
     "Client",
     "DescribeComputeEnvironmentsPaginator",
     "DescribeJobDefinitionsPaginator",
     "DescribeJobQueuesPaginator",
     "ListJobsPaginator",
```

### Comparing `types-aiobotocore-batch-2.9.0/types_aiobotocore_batch/__init__.pyi` & `types-aiobotocore-batch-2.9.1/types_aiobotocore_batch/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-batch-2.9.0/types_aiobotocore_batch/__main__.py` & `types-aiobotocore-batch-2.9.1/types_aiobotocore_batch/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Batch 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Batch 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch\nOther"
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

### Comparing `types-aiobotocore-batch-2.9.0/types_aiobotocore_batch/client.py` & `types-aiobotocore-batch-2.9.1/types_aiobotocore_batch/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("BatchClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -141,15 +140,15 @@
         computeEnvironmentName: str,
         type: CETypeType,
         state: CEStateType = ...,
         unmanagedvCpus: int = ...,
         computeResources: ComputeResourceTypeDef = ...,
         serviceRole: str = ...,
         tags: Mapping[str, str] = ...,
-        eksConfiguration: EksConfigurationTypeDef = ...
+        eksConfiguration: EksConfigurationTypeDef = ...,
     ) -> CreateComputeEnvironmentResponseTypeDef:
         """
         Creates an Batch compute environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.create_compute_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/client/#create_compute_environment)
         """
@@ -158,29 +157,29 @@
         self,
         *,
         jobQueueName: str,
         priority: int,
         computeEnvironmentOrder: Sequence[ComputeEnvironmentOrderTypeDef],
         state: JQStateType = ...,
         schedulingPolicyArn: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateJobQueueResponseTypeDef:
         """
         Creates an Batch job queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.create_job_queue)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/client/#create_job_queue)
         """
 
     async def create_scheduling_policy(
         self,
         *,
         name: str,
         fairsharePolicy: FairsharePolicyTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateSchedulingPolicyResponseTypeDef:
         """
         Creates an Batch scheduling policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.create_scheduling_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/client/#create_scheduling_policy)
         """
@@ -218,15 +217,15 @@
         """
 
     async def describe_compute_environments(
         self,
         *,
         computeEnvironments: Sequence[str] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeComputeEnvironmentsResponseTypeDef:
         """
         Describes one or more of your compute environments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.describe_compute_environments)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/client/#describe_compute_environments)
         """
@@ -234,15 +233,15 @@
     async def describe_job_definitions(
         self,
         *,
         jobDefinitions: Sequence[str] = ...,
         maxResults: int = ...,
         jobDefinitionName: str = ...,
         status: str = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeJobDefinitionsResponseTypeDef:
         """
         Describes a list of job definitions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.describe_job_definitions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/client/#describe_job_definitions)
         """
@@ -294,15 +293,15 @@
         *,
         jobQueue: str = ...,
         arrayJobId: str = ...,
         multiNodeJobId: str = ...,
         jobStatus: JobStatusType = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        filters: Sequence[KeyValuesPairTypeDef] = ...
+        filters: Sequence[KeyValuesPairTypeDef] = ...,
     ) -> ListJobsResponseTypeDef:
         """
         Returns a list of Batch jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.list_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/client/#list_jobs)
         """
@@ -337,15 +336,15 @@
         containerProperties: ContainerPropertiesTypeDef = ...,
         nodeProperties: NodePropertiesTypeDef = ...,
         retryStrategy: RetryStrategyTypeDef = ...,
         propagateTags: bool = ...,
         timeout: JobTimeoutTypeDef = ...,
         tags: Mapping[str, str] = ...,
         platformCapabilities: Sequence[PlatformCapabilityType] = ...,
-        eksProperties: EksPropertiesTypeDef = ...
+        eksProperties: EksPropertiesTypeDef = ...,
     ) -> RegisterJobDefinitionResponseTypeDef:
         """
         Registers an Batch job definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.register_job_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/client/#register_job_definition)
         """
@@ -363,15 +362,15 @@
         parameters: Mapping[str, str] = ...,
         containerOverrides: ContainerOverridesTypeDef = ...,
         nodeOverrides: NodeOverridesTypeDef = ...,
         retryStrategy: RetryStrategyTypeDef = ...,
         propagateTags: bool = ...,
         timeout: JobTimeoutTypeDef = ...,
         tags: Mapping[str, str] = ...,
-        eksPropertiesOverride: EksPropertiesOverrideTypeDef = ...
+        eksPropertiesOverride: EksPropertiesOverrideTypeDef = ...,
     ) -> SubmitJobResponseTypeDef:
         """
         Submits an Batch job from a job definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.submit_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/client/#submit_job)
         """
@@ -404,15 +403,15 @@
         self,
         *,
         computeEnvironment: str,
         state: CEStateType = ...,
         unmanagedvCpus: int = ...,
         computeResources: ComputeResourceUpdateTypeDef = ...,
         serviceRole: str = ...,
-        updatePolicy: UpdatePolicyTypeDef = ...
+        updatePolicy: UpdatePolicyTypeDef = ...,
     ) -> UpdateComputeEnvironmentResponseTypeDef:
         """
         Updates an Batch compute environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.update_compute_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/client/#update_compute_environment)
         """
@@ -420,15 +419,15 @@
     async def update_job_queue(
         self,
         *,
         jobQueue: str,
         state: JQStateType = ...,
         schedulingPolicyArn: str = ...,
         priority: int = ...,
-        computeEnvironmentOrder: Sequence[ComputeEnvironmentOrderTypeDef] = ...
+        computeEnvironmentOrder: Sequence[ComputeEnvironmentOrderTypeDef] = ...,
     ) -> UpdateJobQueueResponseTypeDef:
         """
         Updates a job queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.update_job_queue)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/client/#update_job_queue)
         """
```

### Comparing `types-aiobotocore-batch-2.9.0/types_aiobotocore_batch/client.pyi` & `types-aiobotocore-batch-2.9.1/types_aiobotocore_batch/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,15 @@
         computeEnvironmentName: str,
         type: CETypeType,
         state: CEStateType = ...,
         unmanagedvCpus: int = ...,
         computeResources: ComputeResourceTypeDef = ...,
         serviceRole: str = ...,
         tags: Mapping[str, str] = ...,
-        eksConfiguration: EksConfigurationTypeDef = ...
+        eksConfiguration: EksConfigurationTypeDef = ...,
     ) -> CreateComputeEnvironmentResponseTypeDef:
         """
         Creates an Batch compute environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.create_compute_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/client/#create_compute_environment)
         """
@@ -154,29 +154,29 @@
         self,
         *,
         jobQueueName: str,
         priority: int,
         computeEnvironmentOrder: Sequence[ComputeEnvironmentOrderTypeDef],
         state: JQStateType = ...,
         schedulingPolicyArn: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateJobQueueResponseTypeDef:
         """
         Creates an Batch job queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.create_job_queue)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/client/#create_job_queue)
         """
 
     async def create_scheduling_policy(
         self,
         *,
         name: str,
         fairsharePolicy: FairsharePolicyTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateSchedulingPolicyResponseTypeDef:
         """
         Creates an Batch scheduling policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.create_scheduling_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/client/#create_scheduling_policy)
         """
@@ -214,15 +214,15 @@
         """
 
     async def describe_compute_environments(
         self,
         *,
         computeEnvironments: Sequence[str] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeComputeEnvironmentsResponseTypeDef:
         """
         Describes one or more of your compute environments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.describe_compute_environments)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/client/#describe_compute_environments)
         """
@@ -230,15 +230,15 @@
     async def describe_job_definitions(
         self,
         *,
         jobDefinitions: Sequence[str] = ...,
         maxResults: int = ...,
         jobDefinitionName: str = ...,
         status: str = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeJobDefinitionsResponseTypeDef:
         """
         Describes a list of job definitions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.describe_job_definitions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/client/#describe_job_definitions)
         """
@@ -290,15 +290,15 @@
         *,
         jobQueue: str = ...,
         arrayJobId: str = ...,
         multiNodeJobId: str = ...,
         jobStatus: JobStatusType = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        filters: Sequence[KeyValuesPairTypeDef] = ...
+        filters: Sequence[KeyValuesPairTypeDef] = ...,
     ) -> ListJobsResponseTypeDef:
         """
         Returns a list of Batch jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.list_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/client/#list_jobs)
         """
@@ -333,15 +333,15 @@
         containerProperties: ContainerPropertiesTypeDef = ...,
         nodeProperties: NodePropertiesTypeDef = ...,
         retryStrategy: RetryStrategyTypeDef = ...,
         propagateTags: bool = ...,
         timeout: JobTimeoutTypeDef = ...,
         tags: Mapping[str, str] = ...,
         platformCapabilities: Sequence[PlatformCapabilityType] = ...,
-        eksProperties: EksPropertiesTypeDef = ...
+        eksProperties: EksPropertiesTypeDef = ...,
     ) -> RegisterJobDefinitionResponseTypeDef:
         """
         Registers an Batch job definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.register_job_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/client/#register_job_definition)
         """
@@ -359,15 +359,15 @@
         parameters: Mapping[str, str] = ...,
         containerOverrides: ContainerOverridesTypeDef = ...,
         nodeOverrides: NodeOverridesTypeDef = ...,
         retryStrategy: RetryStrategyTypeDef = ...,
         propagateTags: bool = ...,
         timeout: JobTimeoutTypeDef = ...,
         tags: Mapping[str, str] = ...,
-        eksPropertiesOverride: EksPropertiesOverrideTypeDef = ...
+        eksPropertiesOverride: EksPropertiesOverrideTypeDef = ...,
     ) -> SubmitJobResponseTypeDef:
         """
         Submits an Batch job from a job definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.submit_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/client/#submit_job)
         """
@@ -400,15 +400,15 @@
         self,
         *,
         computeEnvironment: str,
         state: CEStateType = ...,
         unmanagedvCpus: int = ...,
         computeResources: ComputeResourceUpdateTypeDef = ...,
         serviceRole: str = ...,
-        updatePolicy: UpdatePolicyTypeDef = ...
+        updatePolicy: UpdatePolicyTypeDef = ...,
     ) -> UpdateComputeEnvironmentResponseTypeDef:
         """
         Updates an Batch compute environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.update_compute_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/client/#update_compute_environment)
         """
@@ -416,15 +416,15 @@
     async def update_job_queue(
         self,
         *,
         jobQueue: str,
         state: JQStateType = ...,
         schedulingPolicyArn: str = ...,
         priority: int = ...,
-        computeEnvironmentOrder: Sequence[ComputeEnvironmentOrderTypeDef] = ...
+        computeEnvironmentOrder: Sequence[ComputeEnvironmentOrderTypeDef] = ...,
     ) -> UpdateJobQueueResponseTypeDef:
         """
         Updates a job queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.update_job_queue)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/client/#update_job_queue)
         """
```

### Comparing `types-aiobotocore-batch-2.9.0/types_aiobotocore_batch/literals.py` & `types-aiobotocore-batch-2.9.1/types_aiobotocore_batch/literals.py`

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
     "ArrayJobDependencyType",
     "AssignPublicIpType",
     "CEStateType",
     "CEStatusType",
     "CETypeType",
     "CRAllocationStrategyType",
@@ -49,15 +48,14 @@
     "BatchServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ArrayJobDependencyType = Literal["N_TO_N", "SEQUENTIAL"]
 AssignPublicIpType = Literal["DISABLED", "ENABLED"]
 CEStateType = Literal["DISABLED", "ENABLED"]
 CEStatusType = Literal["CREATING", "DELETED", "DELETING", "INVALID", "UPDATING", "VALID"]
 CETypeType = Literal["MANAGED", "UNMANAGED"]
 CRAllocationStrategyType = Literal[
     "BEST_FIT", "BEST_FIT_PROGRESSIVE", "SPOT_CAPACITY_OPTIMIZED", "SPOT_PRICE_CAPACITY_OPTIMIZED"
```

### Comparing `types-aiobotocore-batch-2.9.0/types_aiobotocore_batch/literals.pyi` & `types-aiobotocore-batch-2.9.1/types_aiobotocore_batch/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-batch-2.9.0/types_aiobotocore_batch/paginator.py` & `types-aiobotocore-batch-2.9.1/types_aiobotocore_batch/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,14 @@
     "DescribeComputeEnvironmentsPaginator",
     "DescribeJobDefinitionsPaginator",
     "DescribeJobQueuesPaginator",
     "ListJobsPaginator",
     "ListSchedulingPoliciesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -70,15 +69,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/paginators/#describecomputeenvironmentspaginator)
     """
 
     def paginate(
         self,
         *,
         computeEnvironments: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeComputeEnvironmentsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.DescribeComputeEnvironments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/paginators/#describecomputeenvironmentspaginator)
         """
 
 
@@ -90,15 +89,15 @@
 
     def paginate(
         self,
         *,
         jobDefinitions: Sequence[str] = ...,
         jobDefinitionName: str = ...,
         status: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeJobDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.DescribeJobDefinitions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/paginators/#describejobdefinitionspaginator)
         """
 
 
@@ -127,15 +126,15 @@
         self,
         *,
         jobQueue: str = ...,
         arrayJobId: str = ...,
         multiNodeJobId: str = ...,
         jobStatus: JobStatusType = ...,
         filters: Sequence[KeyValuesPairTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.ListJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/paginators/#listjobspaginator)
         """
```

### Comparing `types-aiobotocore-batch-2.9.0/types_aiobotocore_batch/paginator.pyi` & `types-aiobotocore-batch-2.9.1/types_aiobotocore_batch/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/paginators/#describecomputeenvironmentspaginator)
     """
 
     def paginate(
         self,
         *,
         computeEnvironments: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeComputeEnvironmentsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.DescribeComputeEnvironments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/paginators/#describecomputeenvironmentspaginator)
         """
 
 class DescribeJobDefinitionsPaginator(AioPaginator):
@@ -86,15 +86,15 @@
 
     def paginate(
         self,
         *,
         jobDefinitions: Sequence[str] = ...,
         jobDefinitionName: str = ...,
         status: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeJobDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.DescribeJobDefinitions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/paginators/#describejobdefinitionspaginator)
         """
 
 class DescribeJobQueuesPaginator(AioPaginator):
@@ -121,15 +121,15 @@
         self,
         *,
         jobQueue: str = ...,
         arrayJobId: str = ...,
         multiNodeJobId: str = ...,
         jobStatus: JobStatusType = ...,
         filters: Sequence[KeyValuesPairTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.ListJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/paginators/#listjobspaginator)
         """
 
 class ListSchedulingPoliciesPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-batch-2.9.0/types_aiobotocore_batch/type_defs.py` & `types-aiobotocore-batch-2.9.1/types_aiobotocore_batch/type_defs.py`

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
     "ArrayPropertiesDetailTypeDef",
     "ArrayPropertiesSummaryTypeDef",
     "ArrayPropertiesTypeDef",
     "NetworkInterfaceTypeDef",
     "CancelJobRequestRequestTypeDef",
     "EksConfigurationTypeDef",
```

### Comparing `types-aiobotocore-batch-2.9.0/types_aiobotocore_batch/type_defs.pyi` & `types-aiobotocore-batch-2.9.1/types_aiobotocore_batch/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-batch-2.9.0/types_aiobotocore_batch.egg-info/PKG-INFO` & `types-aiobotocore-batch-2.9.1/types_aiobotocore_batch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-batch
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Batch 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Batch 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/
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
 
 <a id="types-aiobotocore-batch"></a>
 
 # types-aiobotocore-batch
 
 [![PyPI - types-aiobotocore-batch](https://img.shields.io/pypi/v/types-aiobotocore-batch.svg?color=blue)](https://pypi.org/project/types-aiobotocore-batch)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-batch.svg?color=blue)](https://pypi.org/project/types-aiobotocore-batch)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-batch)](https://pepy.tech/project/types-aiobotocore-batch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Batch 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
+[aiobotocore.Batch 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
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
 [types-aiobotocore-batch docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-batch-2.9.0/types_aiobotocore_batch.egg-info/SOURCES.txt` & `types-aiobotocore-batch-2.9.1/types_aiobotocore_batch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

