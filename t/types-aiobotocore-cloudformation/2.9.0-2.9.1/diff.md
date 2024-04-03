# Comparing `tmp/types-aiobotocore-cloudformation-2.9.0.tar.gz` & `tmp/types-aiobotocore-cloudformation-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cloudformation-2.9.0.tar", last modified: Wed Dec 13 19:58:48 2023, max compression
+gzip compressed data, was "types-aiobotocore-cloudformation-2.9.1.tar", last modified: Thu Jan 18 01:20:15 2024, max compression
```

## Comparing `types-aiobotocore-cloudformation-2.9.0.tar` & `types-aiobotocore-cloudformation-2.9.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:48.837978 types-aiobotocore-cloudformation-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:42:18.000000 types-aiobotocore-cloudformation-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    19473 2023-12-13 19:58:48.837978 types-aiobotocore-cloudformation-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17882 2023-12-13 19:42:18.000000 types-aiobotocore-cloudformation-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:48.837978 types-aiobotocore-cloudformation-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2023-12-13 19:42:18.000000 types-aiobotocore-cloudformation-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:48.837978 types-aiobotocore-cloudformation-2.9.0/types_aiobotocore_cloudformation/
--rw-r--r--   0 runner    (1001) docker     (127)     5305 2023-12-13 19:42:18.000000 types-aiobotocore-cloudformation-2.9.0/types_aiobotocore_cloudformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5303 2023-12-13 19:42:18.000000 types-aiobotocore-cloudformation-2.9.0/types_aiobotocore_cloudformation/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      960 2023-12-13 19:42:18.000000 types-aiobotocore-cloudformation-2.9.0/types_aiobotocore_cloudformation/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    69790 2023-12-13 19:42:19.000000 types-aiobotocore-cloudformation-2.9.0/types_aiobotocore_cloudformation/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    69786 2023-12-13 19:42:19.000000 types-aiobotocore-cloudformation-2.9.0/types_aiobotocore_cloudformation/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    19189 2023-12-13 19:42:20.000000 types-aiobotocore-cloudformation-2.9.0/types_aiobotocore_cloudformation/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    19187 2023-12-13 19:42:20.000000 types-aiobotocore-cloudformation-2.9.0/types_aiobotocore_cloudformation/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    18085 2023-12-13 19:42:20.000000 types-aiobotocore-cloudformation-2.9.0/types_aiobotocore_cloudformation/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    18069 2023-12-13 19:42:19.000000 types-aiobotocore-cloudformation-2.9.0/types_aiobotocore_cloudformation/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:42:18.000000 types-aiobotocore-cloudformation-2.9.0/types_aiobotocore_cloudformation/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    25585 2023-12-13 19:42:19.000000 types-aiobotocore-cloudformation-2.9.0/types_aiobotocore_cloudformation/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    25571 2023-12-13 19:42:19.000000 types-aiobotocore-cloudformation-2.9.0/types_aiobotocore_cloudformation/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    85249 2023-12-13 19:42:22.000000 types-aiobotocore-cloudformation-2.9.0/types_aiobotocore_cloudformation/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    85248 2023-12-13 19:42:21.000000 types-aiobotocore-cloudformation-2.9.0/types_aiobotocore_cloudformation/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:42:18.000000 types-aiobotocore-cloudformation-2.9.0/types_aiobotocore_cloudformation/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     9292 2023-12-13 19:42:20.000000 types-aiobotocore-cloudformation-2.9.0/types_aiobotocore_cloudformation/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9284 2023-12-13 19:42:20.000000 types-aiobotocore-cloudformation-2.9.0/types_aiobotocore_cloudformation/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:48.837978 types-aiobotocore-cloudformation-2.9.0/types_aiobotocore_cloudformation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19473 2023-12-13 19:58:48.000000 types-aiobotocore-cloudformation-2.9.0/types_aiobotocore_cloudformation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2023-12-13 19:58:48.000000 types-aiobotocore-cloudformation-2.9.0/types_aiobotocore_cloudformation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:48.000000 types-aiobotocore-cloudformation-2.9.0/types_aiobotocore_cloudformation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:48.000000 types-aiobotocore-cloudformation-2.9.0/types_aiobotocore_cloudformation.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:48.000000 types-aiobotocore-cloudformation-2.9.0/types_aiobotocore_cloudformation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-13 19:58:48.000000 types-aiobotocore-cloudformation-2.9.0/types_aiobotocore_cloudformation.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:15.653465 types-aiobotocore-cloudformation-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:04:15.000000 types-aiobotocore-cloudformation-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    19493 2024-01-18 01:20:15.653465 types-aiobotocore-cloudformation-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17882 2024-01-18 01:04:15.000000 types-aiobotocore-cloudformation-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:15.653465 types-aiobotocore-cloudformation-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-01-18 01:04:15.000000 types-aiobotocore-cloudformation-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:15.653465 types-aiobotocore-cloudformation-2.9.1/types_aiobotocore_cloudformation/
+-rw-r--r--   0 runner    (1001) docker     (127)     5303 2024-01-18 01:04:15.000000 types-aiobotocore-cloudformation-2.9.1/types_aiobotocore_cloudformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5303 2024-01-18 01:04:15.000000 types-aiobotocore-cloudformation-2.9.1/types_aiobotocore_cloudformation/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-01-18 01:04:15.000000 types-aiobotocore-cloudformation-2.9.1/types_aiobotocore_cloudformation/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69827 2024-01-18 01:04:16.000000 types-aiobotocore-cloudformation-2.9.1/types_aiobotocore_cloudformation/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69824 2024-01-18 01:04:15.000000 types-aiobotocore-cloudformation-2.9.1/types_aiobotocore_cloudformation/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    19187 2024-01-18 01:04:17.000000 types-aiobotocore-cloudformation-2.9.1/types_aiobotocore_cloudformation/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19187 2024-01-18 01:04:17.000000 types-aiobotocore-cloudformation-2.9.1/types_aiobotocore_cloudformation/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    18091 2024-01-18 01:04:17.000000 types-aiobotocore-cloudformation-2.9.1/types_aiobotocore_cloudformation/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18076 2024-01-18 01:04:17.000000 types-aiobotocore-cloudformation-2.9.1/types_aiobotocore_cloudformation/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:04:15.000000 types-aiobotocore-cloudformation-2.9.1/types_aiobotocore_cloudformation/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    25815 2024-01-18 01:04:16.000000 types-aiobotocore-cloudformation-2.9.1/types_aiobotocore_cloudformation/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25802 2024-01-18 01:04:16.000000 types-aiobotocore-cloudformation-2.9.1/types_aiobotocore_cloudformation/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    85248 2024-01-18 01:04:19.000000 types-aiobotocore-cloudformation-2.9.1/types_aiobotocore_cloudformation/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85248 2024-01-18 01:04:18.000000 types-aiobotocore-cloudformation-2.9.1/types_aiobotocore_cloudformation/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:04:15.000000 types-aiobotocore-cloudformation-2.9.1/types_aiobotocore_cloudformation/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9293 2024-01-18 01:04:17.000000 types-aiobotocore-cloudformation-2.9.1/types_aiobotocore_cloudformation/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9285 2024-01-18 01:04:17.000000 types-aiobotocore-cloudformation-2.9.1/types_aiobotocore_cloudformation/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:15.653465 types-aiobotocore-cloudformation-2.9.1/types_aiobotocore_cloudformation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19493 2024-01-18 01:20:15.000000 types-aiobotocore-cloudformation-2.9.1/types_aiobotocore_cloudformation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-01-18 01:20:15.000000 types-aiobotocore-cloudformation-2.9.1/types_aiobotocore_cloudformation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:15.000000 types-aiobotocore-cloudformation-2.9.1/types_aiobotocore_cloudformation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:15.000000 types-aiobotocore-cloudformation-2.9.1/types_aiobotocore_cloudformation.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:15.000000 types-aiobotocore-cloudformation-2.9.1/types_aiobotocore_cloudformation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-18 01:20:15.000000 types-aiobotocore-cloudformation-2.9.1/types_aiobotocore_cloudformation.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cloudformation-2.9.0/LICENSE` & `types-aiobotocore-cloudformation-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-cloudformation-2.9.0/PKG-INFO` & `types-aiobotocore-cloudformation-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudformation
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CloudFormation 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CloudFormation 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/
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
 
 <a id="types-aiobotocore-cloudformation"></a>
 
 # types-aiobotocore-cloudformation
 
 [![PyPI - types-aiobotocore-cloudformation](https://img.shields.io/pypi/v/types-aiobotocore-cloudformation.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudformation)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudformation.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudformation)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudformation)](https://pepy.tech/project/types-aiobotocore-cloudformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudFormation 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation)
+[aiobotocore.CloudFormation 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation)
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
 [types-aiobotocore-cloudformation docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-cloudformation-2.9.0/README.md` & `types-aiobotocore-cloudformation-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudformation.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudformation)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudformation)](https://pepy.tech/project/types-aiobotocore-cloudformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudFormation 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation)
+[aiobotocore.CloudFormation 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation)
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
 [types-aiobotocore-cloudformation docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-cloudformation-2.9.0/setup.py` & `types-aiobotocore-cloudformation-2.9.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cloudformation",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_cloudformation"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CloudFormation 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.CloudFormation 2.9.1 service generated with"
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
     keywords="aiobotocore cloudformation type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_cloudformation": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-cloudformation-2.9.0/types_aiobotocore_cloudformation/__init__.py` & `types-aiobotocore-cloudformation-2.9.1/types_aiobotocore_cloudformation/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,18 +93,16 @@
     StackRollbackCompleteWaiter,
     StackUpdateCompleteWaiter,
     TypeRegistrationCompleteWaiter,
 )
 
 Client = CloudFormationClient
 
-
 ServiceResource = CloudFormationServiceResource
 
-
 __all__ = (
     "ChangeSetCreateCompleteWaiter",
     "Client",
     "CloudFormationClient",
     "CloudFormationServiceResource",
     "DescribeAccountLimitsPaginator",
     "DescribeChangeSetPaginator",
```

### Comparing `types-aiobotocore-cloudformation-2.9.0/types_aiobotocore_cloudformation/__init__.pyi` & `types-aiobotocore-cloudformation-2.9.1/types_aiobotocore_cloudformation/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudformation-2.9.0/types_aiobotocore_cloudformation/__main__.py` & `types-aiobotocore-cloudformation-2.9.1/types_aiobotocore_cloudformation/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CloudFormation 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.CloudFormation 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation\nOther"
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

### Comparing `types-aiobotocore-cloudformation-2.9.0/types_aiobotocore_cloudformation/client.py` & `types-aiobotocore-cloudformation-2.9.1/types_aiobotocore_cloudformation/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("CloudFormationClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -218,15 +217,15 @@
         PublisherId: str = ...,
         TypeName: str = ...,
         TypeNameAlias: str = ...,
         AutoUpdate: bool = ...,
         LoggingConfig: LoggingConfigTypeDef = ...,
         ExecutionRoleArn: str = ...,
         VersionBump: VersionBumpType = ...,
-        MajorVersion: int = ...
+        MajorVersion: int = ...,
     ) -> ActivateTypeOutputTypeDef:
         """
         Activates a public third-party extension, making it available for use in stack
         templates.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.activate_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#activate_type)
@@ -272,15 +271,15 @@
 
     async def continue_update_rollback(
         self,
         *,
         StackName: str,
         RoleARN: str = ...,
         ResourcesToSkip: Sequence[str] = ...,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
     ) -> Dict[str, Any]:
         """
         For a specified stack that's in the `UPDATE_ROLLBACK_FAILED` state, continues
         rolling it back to the `UPDATE_ROLLBACK_COMPLETE`
         state.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.continue_update_rollback)
@@ -304,15 +303,15 @@
         Tags: Sequence[TagTypeDef] = ...,
         ClientToken: str = ...,
         Description: str = ...,
         ChangeSetType: ChangeSetTypeType = ...,
         ResourcesToImport: Sequence[ResourceToImportTypeDef] = ...,
         IncludeNestedStacks: bool = ...,
         OnStackFailure: OnStackFailureType = ...,
-        ImportExistingResources: bool = ...
+        ImportExistingResources: bool = ...,
     ) -> CreateChangeSetOutputTypeDef:
         """
         Creates a list of changes that will be applied to a stack so that you can
         review the changes before executing
         them.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.create_change_set)
@@ -335,15 +334,15 @@
         RoleARN: str = ...,
         OnFailure: OnFailureType = ...,
         StackPolicyBody: str = ...,
         StackPolicyURL: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...,
         EnableTerminationProtection: bool = ...,
-        RetainExceptOnCreate: bool = ...
+        RetainExceptOnCreate: bool = ...,
     ) -> CreateStackOutputTypeDef:
         """
         Creates a stack as specified in the template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.create_stack)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#create_stack)
         """
@@ -354,15 +353,15 @@
         StackSetName: str,
         Regions: Sequence[str],
         Accounts: Sequence[str] = ...,
         DeploymentTargets: DeploymentTargetsTypeDef = ...,
         ParameterOverrides: Sequence[ParameterTypeDef] = ...,
         OperationPreferences: StackSetOperationPreferencesTypeDef = ...,
         OperationId: str = ...,
-        CallAs: CallAsType = ...
+        CallAs: CallAsType = ...,
     ) -> CreateStackInstancesOutputTypeDef:
         """
         Creates stack instances for the specified accounts, within the specified Amazon
         Web Services
         Regions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.create_stack_instances)
@@ -382,15 +381,15 @@
         Tags: Sequence[TagTypeDef] = ...,
         AdministrationRoleARN: str = ...,
         ExecutionRoleName: str = ...,
         PermissionModel: PermissionModelsType = ...,
         AutoDeployment: AutoDeploymentTypeDef = ...,
         CallAs: CallAsType = ...,
         ClientRequestToken: str = ...,
-        ManagedExecution: ManagedExecutionTypeDef = ...
+        ManagedExecution: ManagedExecutionTypeDef = ...,
     ) -> CreateStackSetOutputTypeDef:
         """
         Creates a stack set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.create_stack_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#create_stack_set)
         """
@@ -427,15 +426,15 @@
 
     async def delete_stack(
         self,
         *,
         StackName: str,
         RetainResources: Sequence[str] = ...,
         RoleARN: str = ...,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a specified stack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.delete_stack)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#delete_stack)
         """
@@ -446,15 +445,15 @@
         StackSetName: str,
         Regions: Sequence[str],
         RetainStacks: bool,
         Accounts: Sequence[str] = ...,
         DeploymentTargets: DeploymentTargetsTypeDef = ...,
         OperationPreferences: StackSetOperationPreferencesTypeDef = ...,
         OperationId: str = ...,
-        CallAs: CallAsType = ...
+        CallAs: CallAsType = ...,
     ) -> DeleteStackInstancesOutputTypeDef:
         """
         Deletes stack instances for the specified accounts, in the specified Amazon Web
         Services
         Regions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.delete_stack_instances)
@@ -473,15 +472,15 @@
 
     async def deregister_type(
         self,
         *,
         Arn: str = ...,
         Type: RegistryTypeType = ...,
         TypeName: str = ...,
-        VersionId: str = ...
+        VersionId: str = ...,
     ) -> Dict[str, Any]:
         """
         Marks an extension or extension version as `DEPRECATED` in the CloudFormation
         registry, removing it from active
         use.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.deregister_type)
@@ -514,15 +513,15 @@
 
     async def describe_change_set_hooks(
         self,
         *,
         ChangeSetName: str,
         StackName: str = ...,
         NextToken: str = ...,
-        LogicalResourceId: str = ...
+        LogicalResourceId: str = ...,
     ) -> DescribeChangeSetHooksOutputTypeDef:
         """
         Returns hook-related information for the change set and a list of changes that
         CloudFormation makes when you run the change
         set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.describe_change_set_hooks)
@@ -570,15 +569,15 @@
 
     async def describe_stack_instance(
         self,
         *,
         StackSetName: str,
         StackInstanceAccount: str,
         StackInstanceRegion: str,
-        CallAs: CallAsType = ...
+        CallAs: CallAsType = ...,
     ) -> DescribeStackInstanceOutputTypeDef:
         """
         Returns the stack instance that's associated with the specified StackSet,
         Amazon Web Services account, and Amazon Web Services
         Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.describe_stack_instance)
@@ -597,15 +596,15 @@
 
     async def describe_stack_resource_drifts(
         self,
         *,
         StackName: str,
         StackResourceDriftStatusFilters: Sequence[StackResourceDriftStatusType] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeStackResourceDriftsOutputTypeDef:
         """
         Returns drift information for the resources that have been checked for drift in
         the specified
         stack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.describe_stack_resource_drifts)
@@ -659,15 +658,15 @@
         self,
         *,
         Type: RegistryTypeType = ...,
         TypeName: str = ...,
         Arn: str = ...,
         VersionId: str = ...,
         PublisherId: str = ...,
-        PublicVersionNumber: str = ...
+        PublicVersionNumber: str = ...,
     ) -> DescribeTypeOutputTypeDef:
         """
         Returns detailed information about an extension that has been registered.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.describe_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#describe_type)
         """
@@ -712,29 +711,29 @@
 
     async def detect_stack_set_drift(
         self,
         *,
         StackSetName: str,
         OperationPreferences: StackSetOperationPreferencesTypeDef = ...,
         OperationId: str = ...,
-        CallAs: CallAsType = ...
+        CallAs: CallAsType = ...,
     ) -> DetectStackSetDriftOutputTypeDef:
         """
         Detect drift on a stack set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.detect_stack_set_drift)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#detect_stack_set_drift)
         """
 
     async def estimate_template_cost(
         self,
         *,
         TemplateBody: str = ...,
         TemplateURL: str = ...,
-        Parameters: Sequence[ParameterTypeDef] = ...
+        Parameters: Sequence[ParameterTypeDef] = ...,
     ) -> EstimateTemplateCostOutputTypeDef:
         """
         Returns the estimated monthly cost of a template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.estimate_template_cost)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#estimate_template_cost)
         """
@@ -742,15 +741,15 @@
     async def execute_change_set(
         self,
         *,
         ChangeSetName: str,
         StackName: str = ...,
         ClientRequestToken: str = ...,
         DisableRollback: bool = ...,
-        RetainExceptOnCreate: bool = ...
+        RetainExceptOnCreate: bool = ...,
     ) -> Dict[str, Any]:
         """
         Updates a stack using the input information that was provided when the
         specified change set was
         created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.execute_change_set)
@@ -780,15 +779,15 @@
         """
 
     async def get_template(
         self,
         *,
         StackName: str = ...,
         ChangeSetName: str = ...,
-        TemplateStage: TemplateStageType = ...
+        TemplateStage: TemplateStageType = ...,
     ) -> GetTemplateOutputTypeDef:
         """
         Returns the template body for a specified stack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.get_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#get_template)
         """
@@ -797,15 +796,15 @@
         self,
         *,
         TemplateBody: str = ...,
         TemplateURL: str = ...,
         StackName: str = ...,
         StackSetName: str = ...,
         CallAs: CallAsType = ...,
-        TemplateSummaryConfig: TemplateSummaryConfigTypeDef = ...
+        TemplateSummaryConfig: TemplateSummaryConfigTypeDef = ...,
     ) -> GetTemplateSummaryOutputTypeDef:
         """
         Returns information about a new or existing template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.get_template_summary)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#get_template_summary)
         """
@@ -815,15 +814,15 @@
         *,
         StackSetName: str,
         StackIds: Sequence[str] = ...,
         StackIdsUrl: str = ...,
         OrganizationalUnitIds: Sequence[str] = ...,
         OperationPreferences: StackSetOperationPreferencesTypeDef = ...,
         OperationId: str = ...,
-        CallAs: CallAsType = ...
+        CallAs: CallAsType = ...,
     ) -> ImportStacksToStackSetOutputTypeDef:
         """
         Import existing stacks into a new stack sets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.import_stacks_to_stack_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#import_stacks_to_stack_set)
         """
@@ -864,15 +863,15 @@
         StackSetName: str,
         StackInstanceAccount: str,
         StackInstanceRegion: str,
         OperationId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         StackInstanceResourceDriftStatuses: Sequence[StackResourceDriftStatusType] = ...,
-        CallAs: CallAsType = ...
+        CallAs: CallAsType = ...,
     ) -> ListStackInstanceResourceDriftsOutputTypeDef:
         """
         Returns drift information for resources in a stack instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.list_stack_instance_resource_drifts)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#list_stack_instance_resource_drifts)
         """
@@ -882,15 +881,15 @@
         *,
         StackSetName: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         Filters: Sequence[StackInstanceFilterTypeDef] = ...,
         StackInstanceAccount: str = ...,
         StackInstanceRegion: str = ...,
-        CallAs: CallAsType = ...
+        CallAs: CallAsType = ...,
     ) -> ListStackInstancesOutputTypeDef:
         """
         Returns summary information about stack instances that are associated with the
         specified stack
         set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.list_stack_instances)
@@ -911,45 +910,45 @@
         self,
         *,
         StackSetName: str,
         OperationId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         CallAs: CallAsType = ...,
-        Filters: Sequence[OperationResultFilterTypeDef] = ...
+        Filters: Sequence[OperationResultFilterTypeDef] = ...,
     ) -> ListStackSetOperationResultsOutputTypeDef:
         """
         Returns summary information about the results of a stack set operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.list_stack_set_operation_results)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#list_stack_set_operation_results)
         """
 
     async def list_stack_set_operations(
         self,
         *,
         StackSetName: str,
         NextToken: str = ...,
         MaxResults: int = ...,
-        CallAs: CallAsType = ...
+        CallAs: CallAsType = ...,
     ) -> ListStackSetOperationsOutputTypeDef:
         """
         Returns summary information about operations performed on a stack set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.list_stack_set_operations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#list_stack_set_operations)
         """
 
     async def list_stack_sets(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         Status: StackSetStatusType = ...,
-        CallAs: CallAsType = ...
+        CallAs: CallAsType = ...,
     ) -> ListStackSetsOutputTypeDef:
         """
         Returns summary information about stack sets that are associated with the user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.list_stack_sets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#list_stack_sets)
         """
@@ -969,15 +968,15 @@
         self,
         *,
         Type: RegistryTypeType = ...,
         TypeName: str = ...,
         TypeArn: str = ...,
         RegistrationStatusFilter: RegistrationStatusType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListTypeRegistrationsOutputTypeDef:
         """
         Returns a list of registration tokens for the specified extension(s).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.list_type_registrations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#list_type_registrations)
         """
@@ -987,15 +986,15 @@
         *,
         Type: RegistryTypeType = ...,
         TypeName: str = ...,
         Arn: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         DeprecatedStatus: DeprecatedStatusType = ...,
-        PublisherId: str = ...
+        PublisherId: str = ...,
     ) -> ListTypeVersionsOutputTypeDef:
         """
         Returns summary information about the versions of an extension.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.list_type_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#list_type_versions)
         """
@@ -1005,15 +1004,15 @@
         *,
         Visibility: VisibilityType = ...,
         ProvisioningType: ProvisioningTypeType = ...,
         DeprecatedStatus: DeprecatedStatusType = ...,
         Type: RegistryTypeType = ...,
         Filters: TypeFiltersTypeDef = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListTypesOutputTypeDef:
         """
         Returns summary information about extension that have been registered with
         CloudFormation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.list_types)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#list_types)
@@ -1021,15 +1020,15 @@
 
     async def publish_type(
         self,
         *,
         Type: ThirdPartyTypeType = ...,
         Arn: str = ...,
         TypeName: str = ...,
-        PublicVersionNumber: str = ...
+        PublicVersionNumber: str = ...,
     ) -> PublishTypeOutputTypeDef:
         """
         Publishes the specified extension to the CloudFormation registry as a public
         extension in this
         Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.publish_type)
@@ -1041,15 +1040,15 @@
         *,
         BearerToken: str,
         OperationStatus: OperationStatusType,
         CurrentOperationStatus: OperationStatusType = ...,
         StatusMessage: str = ...,
         ErrorCode: HandlerErrorCodeType = ...,
         ResourceModel: str = ...,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
     ) -> Dict[str, Any]:
         """
         Reports progress of a resource handler to CloudFormation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.record_handler_progress)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#record_handler_progress)
         """
@@ -1070,30 +1069,30 @@
         self,
         *,
         TypeName: str,
         SchemaHandlerPackage: str,
         Type: RegistryTypeType = ...,
         LoggingConfig: LoggingConfigTypeDef = ...,
         ExecutionRoleArn: str = ...,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
     ) -> RegisterTypeOutputTypeDef:
         """
         Registers an extension with the CloudFormation service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.register_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#register_type)
         """
 
     async def rollback_stack(
         self,
         *,
         StackName: str,
         RoleARN: str = ...,
         ClientRequestToken: str = ...,
-        RetainExceptOnCreate: bool = ...
+        RetainExceptOnCreate: bool = ...,
     ) -> RollbackStackOutputTypeDef:
         """
         When specifying `RollbackStack`, you preserve the state of previously
         provisioned resources when an operation
         fails.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.rollback_stack)
@@ -1113,15 +1112,15 @@
     async def set_type_configuration(
         self,
         *,
         Configuration: str,
         TypeArn: str = ...,
         ConfigurationAlias: str = ...,
         TypeName: str = ...,
-        Type: ThirdPartyTypeType = ...
+        Type: ThirdPartyTypeType = ...,
     ) -> SetTypeConfigurationOutputTypeDef:
         """
         Specifies the configuration data for a registered CloudFormation extension, in
         the given account and
         Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.set_type_configuration)
@@ -1130,30 +1129,30 @@
 
     async def set_type_default_version(
         self,
         *,
         Arn: str = ...,
         Type: RegistryTypeType = ...,
         TypeName: str = ...,
-        VersionId: str = ...
+        VersionId: str = ...,
     ) -> Dict[str, Any]:
         """
         Specify the default version of an extension.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.set_type_default_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#set_type_default_version)
         """
 
     async def signal_resource(
         self,
         *,
         StackName: str,
         LogicalResourceId: str,
         UniqueId: str,
-        Status: ResourceSignalStatusType
+        Status: ResourceSignalStatusType,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Sends a signal to the specified resource with a success or failure status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.signal_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#signal_resource)
         """
@@ -1172,15 +1171,15 @@
     async def test_type(
         self,
         *,
         Arn: str = ...,
         Type: ThirdPartyTypeType = ...,
         TypeName: str = ...,
         VersionId: str = ...,
-        LogDeliveryBucket: str = ...
+        LogDeliveryBucket: str = ...,
     ) -> TestTypeOutputTypeDef:
         """
         Tests a registered extension to make sure it meets all necessary requirements
         for being published in the CloudFormation
         registry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.test_type)
@@ -1203,15 +1202,15 @@
         RollbackConfiguration: RollbackConfigurationTypeDef = ...,
         StackPolicyBody: str = ...,
         StackPolicyURL: str = ...,
         NotificationARNs: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DisableRollback: bool = ...,
         ClientRequestToken: str = ...,
-        RetainExceptOnCreate: bool = ...
+        RetainExceptOnCreate: bool = ...,
     ) -> UpdateStackOutputTypeDef:
         """
         Updates a stack as specified in the template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.update_stack)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#update_stack)
         """
@@ -1222,15 +1221,15 @@
         StackSetName: str,
         Regions: Sequence[str],
         Accounts: Sequence[str] = ...,
         DeploymentTargets: DeploymentTargetsTypeDef = ...,
         ParameterOverrides: Sequence[ParameterTypeDef] = ...,
         OperationPreferences: StackSetOperationPreferencesTypeDef = ...,
         OperationId: str = ...,
-        CallAs: CallAsType = ...
+        CallAs: CallAsType = ...,
     ) -> UpdateStackInstancesOutputTypeDef:
         """
         Updates the parameter values for stack instances for the specified accounts,
         within the specified Amazon Web Services
         Regions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.update_stack_instances)
@@ -1254,15 +1253,15 @@
         DeploymentTargets: DeploymentTargetsTypeDef = ...,
         PermissionModel: PermissionModelsType = ...,
         AutoDeployment: AutoDeploymentTypeDef = ...,
         OperationId: str = ...,
         Accounts: Sequence[str] = ...,
         Regions: Sequence[str] = ...,
         CallAs: CallAsType = ...,
-        ManagedExecution: ManagedExecutionTypeDef = ...
+        ManagedExecution: ManagedExecutionTypeDef = ...,
     ) -> UpdateStackSetOutputTypeDef:
         """
         Updates the stack set, and associated stack instances in the specified accounts
         and Amazon Web Services
         Regions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.update_stack_set)
```

### Comparing `types-aiobotocore-cloudformation-2.9.0/types_aiobotocore_cloudformation/client.pyi` & `types-aiobotocore-cloudformation-2.9.1/types_aiobotocore_cloudformation/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -214,15 +214,15 @@
         PublisherId: str = ...,
         TypeName: str = ...,
         TypeNameAlias: str = ...,
         AutoUpdate: bool = ...,
         LoggingConfig: LoggingConfigTypeDef = ...,
         ExecutionRoleArn: str = ...,
         VersionBump: VersionBumpType = ...,
-        MajorVersion: int = ...
+        MajorVersion: int = ...,
     ) -> ActivateTypeOutputTypeDef:
         """
         Activates a public third-party extension, making it available for use in stack
         templates.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.activate_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#activate_type)
@@ -268,15 +268,15 @@
 
     async def continue_update_rollback(
         self,
         *,
         StackName: str,
         RoleARN: str = ...,
         ResourcesToSkip: Sequence[str] = ...,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
     ) -> Dict[str, Any]:
         """
         For a specified stack that's in the `UPDATE_ROLLBACK_FAILED` state, continues
         rolling it back to the `UPDATE_ROLLBACK_COMPLETE`
         state.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.continue_update_rollback)
@@ -300,15 +300,15 @@
         Tags: Sequence[TagTypeDef] = ...,
         ClientToken: str = ...,
         Description: str = ...,
         ChangeSetType: ChangeSetTypeType = ...,
         ResourcesToImport: Sequence[ResourceToImportTypeDef] = ...,
         IncludeNestedStacks: bool = ...,
         OnStackFailure: OnStackFailureType = ...,
-        ImportExistingResources: bool = ...
+        ImportExistingResources: bool = ...,
     ) -> CreateChangeSetOutputTypeDef:
         """
         Creates a list of changes that will be applied to a stack so that you can
         review the changes before executing
         them.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.create_change_set)
@@ -331,15 +331,15 @@
         RoleARN: str = ...,
         OnFailure: OnFailureType = ...,
         StackPolicyBody: str = ...,
         StackPolicyURL: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...,
         EnableTerminationProtection: bool = ...,
-        RetainExceptOnCreate: bool = ...
+        RetainExceptOnCreate: bool = ...,
     ) -> CreateStackOutputTypeDef:
         """
         Creates a stack as specified in the template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.create_stack)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#create_stack)
         """
@@ -350,15 +350,15 @@
         StackSetName: str,
         Regions: Sequence[str],
         Accounts: Sequence[str] = ...,
         DeploymentTargets: DeploymentTargetsTypeDef = ...,
         ParameterOverrides: Sequence[ParameterTypeDef] = ...,
         OperationPreferences: StackSetOperationPreferencesTypeDef = ...,
         OperationId: str = ...,
-        CallAs: CallAsType = ...
+        CallAs: CallAsType = ...,
     ) -> CreateStackInstancesOutputTypeDef:
         """
         Creates stack instances for the specified accounts, within the specified Amazon
         Web Services
         Regions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.create_stack_instances)
@@ -378,15 +378,15 @@
         Tags: Sequence[TagTypeDef] = ...,
         AdministrationRoleARN: str = ...,
         ExecutionRoleName: str = ...,
         PermissionModel: PermissionModelsType = ...,
         AutoDeployment: AutoDeploymentTypeDef = ...,
         CallAs: CallAsType = ...,
         ClientRequestToken: str = ...,
-        ManagedExecution: ManagedExecutionTypeDef = ...
+        ManagedExecution: ManagedExecutionTypeDef = ...,
     ) -> CreateStackSetOutputTypeDef:
         """
         Creates a stack set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.create_stack_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#create_stack_set)
         """
@@ -423,15 +423,15 @@
 
     async def delete_stack(
         self,
         *,
         StackName: str,
         RetainResources: Sequence[str] = ...,
         RoleARN: str = ...,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a specified stack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.delete_stack)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#delete_stack)
         """
@@ -442,15 +442,15 @@
         StackSetName: str,
         Regions: Sequence[str],
         RetainStacks: bool,
         Accounts: Sequence[str] = ...,
         DeploymentTargets: DeploymentTargetsTypeDef = ...,
         OperationPreferences: StackSetOperationPreferencesTypeDef = ...,
         OperationId: str = ...,
-        CallAs: CallAsType = ...
+        CallAs: CallAsType = ...,
     ) -> DeleteStackInstancesOutputTypeDef:
         """
         Deletes stack instances for the specified accounts, in the specified Amazon Web
         Services
         Regions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.delete_stack_instances)
@@ -469,15 +469,15 @@
 
     async def deregister_type(
         self,
         *,
         Arn: str = ...,
         Type: RegistryTypeType = ...,
         TypeName: str = ...,
-        VersionId: str = ...
+        VersionId: str = ...,
     ) -> Dict[str, Any]:
         """
         Marks an extension or extension version as `DEPRECATED` in the CloudFormation
         registry, removing it from active
         use.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.deregister_type)
@@ -510,15 +510,15 @@
 
     async def describe_change_set_hooks(
         self,
         *,
         ChangeSetName: str,
         StackName: str = ...,
         NextToken: str = ...,
-        LogicalResourceId: str = ...
+        LogicalResourceId: str = ...,
     ) -> DescribeChangeSetHooksOutputTypeDef:
         """
         Returns hook-related information for the change set and a list of changes that
         CloudFormation makes when you run the change
         set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.describe_change_set_hooks)
@@ -566,15 +566,15 @@
 
     async def describe_stack_instance(
         self,
         *,
         StackSetName: str,
         StackInstanceAccount: str,
         StackInstanceRegion: str,
-        CallAs: CallAsType = ...
+        CallAs: CallAsType = ...,
     ) -> DescribeStackInstanceOutputTypeDef:
         """
         Returns the stack instance that's associated with the specified StackSet,
         Amazon Web Services account, and Amazon Web Services
         Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.describe_stack_instance)
@@ -593,15 +593,15 @@
 
     async def describe_stack_resource_drifts(
         self,
         *,
         StackName: str,
         StackResourceDriftStatusFilters: Sequence[StackResourceDriftStatusType] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeStackResourceDriftsOutputTypeDef:
         """
         Returns drift information for the resources that have been checked for drift in
         the specified
         stack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.describe_stack_resource_drifts)
@@ -655,15 +655,15 @@
         self,
         *,
         Type: RegistryTypeType = ...,
         TypeName: str = ...,
         Arn: str = ...,
         VersionId: str = ...,
         PublisherId: str = ...,
-        PublicVersionNumber: str = ...
+        PublicVersionNumber: str = ...,
     ) -> DescribeTypeOutputTypeDef:
         """
         Returns detailed information about an extension that has been registered.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.describe_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#describe_type)
         """
@@ -708,29 +708,29 @@
 
     async def detect_stack_set_drift(
         self,
         *,
         StackSetName: str,
         OperationPreferences: StackSetOperationPreferencesTypeDef = ...,
         OperationId: str = ...,
-        CallAs: CallAsType = ...
+        CallAs: CallAsType = ...,
     ) -> DetectStackSetDriftOutputTypeDef:
         """
         Detect drift on a stack set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.detect_stack_set_drift)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#detect_stack_set_drift)
         """
 
     async def estimate_template_cost(
         self,
         *,
         TemplateBody: str = ...,
         TemplateURL: str = ...,
-        Parameters: Sequence[ParameterTypeDef] = ...
+        Parameters: Sequence[ParameterTypeDef] = ...,
     ) -> EstimateTemplateCostOutputTypeDef:
         """
         Returns the estimated monthly cost of a template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.estimate_template_cost)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#estimate_template_cost)
         """
@@ -738,15 +738,15 @@
     async def execute_change_set(
         self,
         *,
         ChangeSetName: str,
         StackName: str = ...,
         ClientRequestToken: str = ...,
         DisableRollback: bool = ...,
-        RetainExceptOnCreate: bool = ...
+        RetainExceptOnCreate: bool = ...,
     ) -> Dict[str, Any]:
         """
         Updates a stack using the input information that was provided when the
         specified change set was
         created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.execute_change_set)
@@ -776,15 +776,15 @@
         """
 
     async def get_template(
         self,
         *,
         StackName: str = ...,
         ChangeSetName: str = ...,
-        TemplateStage: TemplateStageType = ...
+        TemplateStage: TemplateStageType = ...,
     ) -> GetTemplateOutputTypeDef:
         """
         Returns the template body for a specified stack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.get_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#get_template)
         """
@@ -793,15 +793,15 @@
         self,
         *,
         TemplateBody: str = ...,
         TemplateURL: str = ...,
         StackName: str = ...,
         StackSetName: str = ...,
         CallAs: CallAsType = ...,
-        TemplateSummaryConfig: TemplateSummaryConfigTypeDef = ...
+        TemplateSummaryConfig: TemplateSummaryConfigTypeDef = ...,
     ) -> GetTemplateSummaryOutputTypeDef:
         """
         Returns information about a new or existing template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.get_template_summary)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#get_template_summary)
         """
@@ -811,15 +811,15 @@
         *,
         StackSetName: str,
         StackIds: Sequence[str] = ...,
         StackIdsUrl: str = ...,
         OrganizationalUnitIds: Sequence[str] = ...,
         OperationPreferences: StackSetOperationPreferencesTypeDef = ...,
         OperationId: str = ...,
-        CallAs: CallAsType = ...
+        CallAs: CallAsType = ...,
     ) -> ImportStacksToStackSetOutputTypeDef:
         """
         Import existing stacks into a new stack sets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.import_stacks_to_stack_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#import_stacks_to_stack_set)
         """
@@ -860,15 +860,15 @@
         StackSetName: str,
         StackInstanceAccount: str,
         StackInstanceRegion: str,
         OperationId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         StackInstanceResourceDriftStatuses: Sequence[StackResourceDriftStatusType] = ...,
-        CallAs: CallAsType = ...
+        CallAs: CallAsType = ...,
     ) -> ListStackInstanceResourceDriftsOutputTypeDef:
         """
         Returns drift information for resources in a stack instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.list_stack_instance_resource_drifts)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#list_stack_instance_resource_drifts)
         """
@@ -878,15 +878,15 @@
         *,
         StackSetName: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         Filters: Sequence[StackInstanceFilterTypeDef] = ...,
         StackInstanceAccount: str = ...,
         StackInstanceRegion: str = ...,
-        CallAs: CallAsType = ...
+        CallAs: CallAsType = ...,
     ) -> ListStackInstancesOutputTypeDef:
         """
         Returns summary information about stack instances that are associated with the
         specified stack
         set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.list_stack_instances)
@@ -907,45 +907,45 @@
         self,
         *,
         StackSetName: str,
         OperationId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         CallAs: CallAsType = ...,
-        Filters: Sequence[OperationResultFilterTypeDef] = ...
+        Filters: Sequence[OperationResultFilterTypeDef] = ...,
     ) -> ListStackSetOperationResultsOutputTypeDef:
         """
         Returns summary information about the results of a stack set operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.list_stack_set_operation_results)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#list_stack_set_operation_results)
         """
 
     async def list_stack_set_operations(
         self,
         *,
         StackSetName: str,
         NextToken: str = ...,
         MaxResults: int = ...,
-        CallAs: CallAsType = ...
+        CallAs: CallAsType = ...,
     ) -> ListStackSetOperationsOutputTypeDef:
         """
         Returns summary information about operations performed on a stack set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.list_stack_set_operations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#list_stack_set_operations)
         """
 
     async def list_stack_sets(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         Status: StackSetStatusType = ...,
-        CallAs: CallAsType = ...
+        CallAs: CallAsType = ...,
     ) -> ListStackSetsOutputTypeDef:
         """
         Returns summary information about stack sets that are associated with the user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.list_stack_sets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#list_stack_sets)
         """
@@ -965,15 +965,15 @@
         self,
         *,
         Type: RegistryTypeType = ...,
         TypeName: str = ...,
         TypeArn: str = ...,
         RegistrationStatusFilter: RegistrationStatusType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListTypeRegistrationsOutputTypeDef:
         """
         Returns a list of registration tokens for the specified extension(s).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.list_type_registrations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#list_type_registrations)
         """
@@ -983,15 +983,15 @@
         *,
         Type: RegistryTypeType = ...,
         TypeName: str = ...,
         Arn: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         DeprecatedStatus: DeprecatedStatusType = ...,
-        PublisherId: str = ...
+        PublisherId: str = ...,
     ) -> ListTypeVersionsOutputTypeDef:
         """
         Returns summary information about the versions of an extension.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.list_type_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#list_type_versions)
         """
@@ -1001,15 +1001,15 @@
         *,
         Visibility: VisibilityType = ...,
         ProvisioningType: ProvisioningTypeType = ...,
         DeprecatedStatus: DeprecatedStatusType = ...,
         Type: RegistryTypeType = ...,
         Filters: TypeFiltersTypeDef = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListTypesOutputTypeDef:
         """
         Returns summary information about extension that have been registered with
         CloudFormation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.list_types)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#list_types)
@@ -1017,15 +1017,15 @@
 
     async def publish_type(
         self,
         *,
         Type: ThirdPartyTypeType = ...,
         Arn: str = ...,
         TypeName: str = ...,
-        PublicVersionNumber: str = ...
+        PublicVersionNumber: str = ...,
     ) -> PublishTypeOutputTypeDef:
         """
         Publishes the specified extension to the CloudFormation registry as a public
         extension in this
         Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.publish_type)
@@ -1037,15 +1037,15 @@
         *,
         BearerToken: str,
         OperationStatus: OperationStatusType,
         CurrentOperationStatus: OperationStatusType = ...,
         StatusMessage: str = ...,
         ErrorCode: HandlerErrorCodeType = ...,
         ResourceModel: str = ...,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
     ) -> Dict[str, Any]:
         """
         Reports progress of a resource handler to CloudFormation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.record_handler_progress)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#record_handler_progress)
         """
@@ -1066,30 +1066,30 @@
         self,
         *,
         TypeName: str,
         SchemaHandlerPackage: str,
         Type: RegistryTypeType = ...,
         LoggingConfig: LoggingConfigTypeDef = ...,
         ExecutionRoleArn: str = ...,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
     ) -> RegisterTypeOutputTypeDef:
         """
         Registers an extension with the CloudFormation service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.register_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#register_type)
         """
 
     async def rollback_stack(
         self,
         *,
         StackName: str,
         RoleARN: str = ...,
         ClientRequestToken: str = ...,
-        RetainExceptOnCreate: bool = ...
+        RetainExceptOnCreate: bool = ...,
     ) -> RollbackStackOutputTypeDef:
         """
         When specifying `RollbackStack`, you preserve the state of previously
         provisioned resources when an operation
         fails.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.rollback_stack)
@@ -1109,15 +1109,15 @@
     async def set_type_configuration(
         self,
         *,
         Configuration: str,
         TypeArn: str = ...,
         ConfigurationAlias: str = ...,
         TypeName: str = ...,
-        Type: ThirdPartyTypeType = ...
+        Type: ThirdPartyTypeType = ...,
     ) -> SetTypeConfigurationOutputTypeDef:
         """
         Specifies the configuration data for a registered CloudFormation extension, in
         the given account and
         Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.set_type_configuration)
@@ -1126,30 +1126,30 @@
 
     async def set_type_default_version(
         self,
         *,
         Arn: str = ...,
         Type: RegistryTypeType = ...,
         TypeName: str = ...,
-        VersionId: str = ...
+        VersionId: str = ...,
     ) -> Dict[str, Any]:
         """
         Specify the default version of an extension.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.set_type_default_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#set_type_default_version)
         """
 
     async def signal_resource(
         self,
         *,
         StackName: str,
         LogicalResourceId: str,
         UniqueId: str,
-        Status: ResourceSignalStatusType
+        Status: ResourceSignalStatusType,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Sends a signal to the specified resource with a success or failure status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.signal_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#signal_resource)
         """
@@ -1168,15 +1168,15 @@
     async def test_type(
         self,
         *,
         Arn: str = ...,
         Type: ThirdPartyTypeType = ...,
         TypeName: str = ...,
         VersionId: str = ...,
-        LogDeliveryBucket: str = ...
+        LogDeliveryBucket: str = ...,
     ) -> TestTypeOutputTypeDef:
         """
         Tests a registered extension to make sure it meets all necessary requirements
         for being published in the CloudFormation
         registry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.test_type)
@@ -1199,15 +1199,15 @@
         RollbackConfiguration: RollbackConfigurationTypeDef = ...,
         StackPolicyBody: str = ...,
         StackPolicyURL: str = ...,
         NotificationARNs: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DisableRollback: bool = ...,
         ClientRequestToken: str = ...,
-        RetainExceptOnCreate: bool = ...
+        RetainExceptOnCreate: bool = ...,
     ) -> UpdateStackOutputTypeDef:
         """
         Updates a stack as specified in the template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.update_stack)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#update_stack)
         """
@@ -1218,15 +1218,15 @@
         StackSetName: str,
         Regions: Sequence[str],
         Accounts: Sequence[str] = ...,
         DeploymentTargets: DeploymentTargetsTypeDef = ...,
         ParameterOverrides: Sequence[ParameterTypeDef] = ...,
         OperationPreferences: StackSetOperationPreferencesTypeDef = ...,
         OperationId: str = ...,
-        CallAs: CallAsType = ...
+        CallAs: CallAsType = ...,
     ) -> UpdateStackInstancesOutputTypeDef:
         """
         Updates the parameter values for stack instances for the specified accounts,
         within the specified Amazon Web Services
         Regions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.update_stack_instances)
@@ -1250,15 +1250,15 @@
         DeploymentTargets: DeploymentTargetsTypeDef = ...,
         PermissionModel: PermissionModelsType = ...,
         AutoDeployment: AutoDeploymentTypeDef = ...,
         OperationId: str = ...,
         Accounts: Sequence[str] = ...,
         Regions: Sequence[str] = ...,
         CallAs: CallAsType = ...,
-        ManagedExecution: ManagedExecutionTypeDef = ...
+        ManagedExecution: ManagedExecutionTypeDef = ...,
     ) -> UpdateStackSetOutputTypeDef:
         """
         Updates the stack set, and associated stack instances in the specified accounts
         and Amazon Web Services
         Regions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.update_stack_set)
```

### Comparing `types-aiobotocore-cloudformation-2.9.0/types_aiobotocore_cloudformation/literals.py` & `types-aiobotocore-cloudformation-2.9.1/types_aiobotocore_cloudformation/literals.py`

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
     "AccountFilterTypeType",
     "AccountGateStatusType",
     "CallAsType",
     "CapabilityType",
     "CategoryType",
     "ChangeActionType",
@@ -103,15 +102,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 AccountFilterTypeType = Literal["DIFFERENCE", "INTERSECTION", "NONE", "UNION"]
 AccountGateStatusType = Literal["FAILED", "SKIPPED", "SUCCEEDED"]
 CallAsType = Literal["DELEGATED_ADMIN", "SELF"]
 CapabilityType = Literal["CAPABILITY_AUTO_EXPAND", "CAPABILITY_IAM", "CAPABILITY_NAMED_IAM"]
 CategoryType = Literal["ACTIVATED", "AWS_TYPES", "REGISTERED", "THIRD_PARTY"]
 ChangeActionType = Literal["Add", "Dynamic", "Import", "Modify", "Remove"]
 ChangeSetCreateCompleteWaiterName = Literal["change_set_create_complete"]
```

### Comparing `types-aiobotocore-cloudformation-2.9.0/types_aiobotocore_cloudformation/literals.pyi` & `types-aiobotocore-cloudformation-2.9.1/types_aiobotocore_cloudformation/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudformation-2.9.0/types_aiobotocore_cloudformation/paginator.py` & `types-aiobotocore-cloudformation-2.9.1/types_aiobotocore_cloudformation/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -95,261 +95,245 @@
     "ListStackSetOperationResultsPaginator",
     "ListStackSetOperationsPaginator",
     "ListStackSetsPaginator",
     "ListStacksPaginator",
     "ListTypesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class DescribeAccountLimitsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeAccountLimits)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#describeaccountlimitspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeAccountLimitsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeAccountLimits.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#describeaccountlimitspaginator)
         """
 
-
 class DescribeChangeSetPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeChangeSet)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#describechangesetpaginator)
     """
 
     def paginate(
         self,
         *,
         ChangeSetName: str,
         StackName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeChangeSetOutputPaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeChangeSet.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#describechangesetpaginator)
         """
 
-
 class DescribeStackEventsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeStackEvents)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#describestackeventspaginator)
     """
 
     def paginate(
         self, *, StackName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeStackEventsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeStackEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#describestackeventspaginator)
         """
 
-
 class DescribeStacksPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeStacks)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#describestackspaginator)
     """
 
     def paginate(
         self, *, StackName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeStacksOutputPaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeStacks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#describestackspaginator)
         """
 
-
 class ListChangeSetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListChangeSets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#listchangesetspaginator)
     """
 
     def paginate(
         self, *, StackName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListChangeSetsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListChangeSets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#listchangesetspaginator)
         """
 
-
 class ListExportsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListExports)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#listexportspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListExportsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListExports.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#listexportspaginator)
         """
 
-
 class ListImportsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListImports)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#listimportspaginator)
     """
 
     def paginate(
         self, *, ExportName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListImportsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListImports.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#listimportspaginator)
         """
 
-
 class ListStackInstancesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackInstances)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#liststackinstancespaginator)
     """
 
     def paginate(
         self,
         *,
         StackSetName: str,
         Filters: Sequence[StackInstanceFilterTypeDef] = ...,
         StackInstanceAccount: str = ...,
         StackInstanceRegion: str = ...,
         CallAs: CallAsType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListStackInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#liststackinstancespaginator)
         """
 
-
 class ListStackResourcesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackResources)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#liststackresourcespaginator)
     """
 
     def paginate(
         self, *, StackName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListStackResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#liststackresourcespaginator)
         """
 
-
 class ListStackSetOperationResultsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSetOperationResults)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#liststacksetoperationresultspaginator)
     """
 
     def paginate(
         self,
         *,
         StackSetName: str,
         OperationId: str,
         CallAs: CallAsType = ...,
         Filters: Sequence[OperationResultFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListStackSetOperationResultsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSetOperationResults.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#liststacksetoperationresultspaginator)
         """
 
-
 class ListStackSetOperationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSetOperations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#liststacksetoperationspaginator)
     """
 
     def paginate(
         self,
         *,
         StackSetName: str,
         CallAs: CallAsType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListStackSetOperationsOutputPaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSetOperations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#liststacksetoperationspaginator)
         """
 
-
 class ListStackSetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#liststacksetspaginator)
     """
 
     def paginate(
         self,
         *,
         Status: StackSetStatusType = ...,
         CallAs: CallAsType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListStackSetsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#liststacksetspaginator)
         """
 
-
 class ListStacksPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStacks)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#liststackspaginator)
     """
 
     def paginate(
         self,
         *,
         StackStatusFilter: Sequence[StackStatusType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListStacksOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStacks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#liststackspaginator)
         """
 
-
 class ListTypesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListTypes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#listtypespaginator)
     """
 
     def paginate(
         self,
         *,
         Visibility: VisibilityType = ...,
         ProvisioningType: ProvisioningTypeType = ...,
         DeprecatedStatus: DeprecatedStatusType = ...,
         Type: RegistryTypeType = ...,
         Filters: TypeFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTypesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListTypes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#listtypespaginator)
         """
```

### Comparing `types-aiobotocore-cloudformation-2.9.0/types_aiobotocore_cloudformation/paginator.pyi` & `types-aiobotocore-cloudformation-2.9.1/types_aiobotocore_cloudformation/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,243 +97,258 @@
     "ListStackSetsPaginator",
     "ListStacksPaginator",
     "ListTypesPaginator",
 )
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class DescribeAccountLimitsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeAccountLimits)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#describeaccountlimitspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeAccountLimitsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeAccountLimits.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#describeaccountlimitspaginator)
         """
 
+
 class DescribeChangeSetPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeChangeSet)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#describechangesetpaginator)
     """
 
     def paginate(
         self,
         *,
         ChangeSetName: str,
         StackName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeChangeSetOutputPaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeChangeSet.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#describechangesetpaginator)
         """
 
+
 class DescribeStackEventsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeStackEvents)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#describestackeventspaginator)
     """
 
     def paginate(
         self, *, StackName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeStackEventsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeStackEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#describestackeventspaginator)
         """
 
+
 class DescribeStacksPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeStacks)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#describestackspaginator)
     """
 
     def paginate(
         self, *, StackName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeStacksOutputPaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeStacks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#describestackspaginator)
         """
 
+
 class ListChangeSetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListChangeSets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#listchangesetspaginator)
     """
 
     def paginate(
         self, *, StackName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListChangeSetsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListChangeSets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#listchangesetspaginator)
         """
 
+
 class ListExportsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListExports)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#listexportspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListExportsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListExports.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#listexportspaginator)
         """
 
+
 class ListImportsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListImports)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#listimportspaginator)
     """
 
     def paginate(
         self, *, ExportName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListImportsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListImports.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#listimportspaginator)
         """
 
+
 class ListStackInstancesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackInstances)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#liststackinstancespaginator)
     """
 
     def paginate(
         self,
         *,
         StackSetName: str,
         Filters: Sequence[StackInstanceFilterTypeDef] = ...,
         StackInstanceAccount: str = ...,
         StackInstanceRegion: str = ...,
         CallAs: CallAsType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListStackInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#liststackinstancespaginator)
         """
 
+
 class ListStackResourcesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackResources)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#liststackresourcespaginator)
     """
 
     def paginate(
         self, *, StackName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListStackResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#liststackresourcespaginator)
         """
 
+
 class ListStackSetOperationResultsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSetOperationResults)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#liststacksetoperationresultspaginator)
     """
 
     def paginate(
         self,
         *,
         StackSetName: str,
         OperationId: str,
         CallAs: CallAsType = ...,
         Filters: Sequence[OperationResultFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListStackSetOperationResultsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSetOperationResults.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#liststacksetoperationresultspaginator)
         """
 
+
 class ListStackSetOperationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSetOperations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#liststacksetoperationspaginator)
     """
 
     def paginate(
         self,
         *,
         StackSetName: str,
         CallAs: CallAsType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListStackSetOperationsOutputPaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSetOperations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#liststacksetoperationspaginator)
         """
 
+
 class ListStackSetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#liststacksetspaginator)
     """
 
     def paginate(
         self,
         *,
         Status: StackSetStatusType = ...,
         CallAs: CallAsType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListStackSetsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#liststacksetspaginator)
         """
 
+
 class ListStacksPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStacks)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#liststackspaginator)
     """
 
     def paginate(
         self,
         *,
         StackStatusFilter: Sequence[StackStatusType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListStacksOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStacks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#liststackspaginator)
         """
 
+
 class ListTypesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListTypes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#listtypespaginator)
     """
 
     def paginate(
         self,
         *,
         Visibility: VisibilityType = ...,
         ProvisioningType: ProvisioningTypeType = ...,
         DeprecatedStatus: DeprecatedStatusType = ...,
         Type: RegistryTypeType = ...,
         Filters: TypeFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTypesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListTypes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#listtypespaginator)
         """
```

### Comparing `types-aiobotocore-cloudformation-2.9.0/types_aiobotocore_cloudformation/service_resource.py` & `types-aiobotocore-cloudformation-2.9.1/types_aiobotocore_cloudformation/service_resource.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,15 +62,14 @@
 else:
     from typing_extensions import Literal
 try:
     from boto3.resources.base import ResourceMeta
 except ImportError:
     from builtins import object as ResourceMeta
 
-
 __all__ = (
     "CloudFormationServiceResource",
     "Event",
     "Stack",
     "StackResource",
     "StackResourceSummary",
     "ServiceResourceStacksCollection",
@@ -239,14 +238,15 @@
     client_request_token: Awaitable[str]
     hook_type: Awaitable[str]
     hook_status: Awaitable[HookStatusType]
     hook_status_reason: Awaitable[str]
     hook_invocation_point: Awaitable[Literal["PRE_PROVISION"]]
     hook_failure_mode: Awaitable[HookFailureModeType]
     id: str
+    meta: Awaitable["CloudFormationResourceMeta"]
 
     async def get_available_subresources(self) -> Sequence[str]:
         """
         Returns a list of all the available sub-resources for this Resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Event.get_available_subresources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/service_resource/#eventget_available_subresources-method)
@@ -284,14 +284,15 @@
     parent_id: Awaitable[str]
     root_id: Awaitable[str]
     drift_information: Awaitable[StackDriftInformationResponseTypeDef]
     retain_except_on_create: Awaitable[bool]
     name: str
     events: StackEventsCollection
     resource_summaries: StackResourceSummariesCollection
+    meta: Awaitable["CloudFormationResourceMeta"]
 
     async def Resource(self, logical_id: str) -> "_StackResource":
         """
         Creates a StackResource resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Stack.Resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/service_resource/#stackresource-method)
@@ -306,15 +307,15 @@
         """
 
     async def delete(
         self,
         *,
         RetainResources: Sequence[str] = ...,
         RoleARN: str = ...,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
     ) -> None:
         """
         Deletes a specified stack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Stack.delete)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/service_resource/#stackdelete-method)
         """
@@ -362,15 +363,15 @@
         RollbackConfiguration: RollbackConfigurationTypeDef = ...,
         StackPolicyBody: str = ...,
         StackPolicyURL: str = ...,
         NotificationARNs: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DisableRollback: bool = ...,
         ClientRequestToken: str = ...,
-        RetainExceptOnCreate: bool = ...
+        RetainExceptOnCreate: bool = ...,
     ) -> UpdateStackOutputTypeDef:
         """
         Updates a stack as specified in the template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Stack.update)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/service_resource/#stackupdate-method)
         """
@@ -394,16 +395,17 @@
     resource_status_reason: Awaitable[str]
     description: Awaitable[str]
     metadata: Awaitable[str]
     drift_information: Awaitable[StackResourceDriftInformationResponseTypeDef]
     module_info: Awaitable[ModuleInfoTypeDef]
     stack_name: str
     logical_id: str
+    meta: Awaitable["CloudFormationResourceMeta"]
 
-    async def Stack(self) -> _Stack:
+    async def Stack(self) -> "_Stack":
         """
         Creates a Stack resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.StackResource.Stack)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/service_resource/#stackresourcestack-method)
         """
 
@@ -451,16 +453,17 @@
     last_updated_timestamp: Awaitable[datetime]
     resource_status: Awaitable[ResourceStatusType]
     resource_status_reason: Awaitable[str]
     drift_information: Awaitable[StackResourceDriftInformationSummaryResponseTypeDef]
     module_info: Awaitable[ModuleInfoResponseTypeDef]
     stack_name: str
     logical_id: str
+    meta: Awaitable["CloudFormationResourceMeta"]
 
-    async def Resource(self) -> _StackResource:
+    async def Resource(self) -> "_StackResource":
         """
         Creates a StackResource resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.StackResourceSummary.Resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/service_resource/#stackresourcesummaryresource-method)
         """
 
@@ -485,39 +488,41 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.ServiceResource)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/service_resource/)
     """
 
     meta: "CloudFormationResourceMeta"
     stacks: ServiceResourceStacksCollection
 
-    async def Event(self, id: str) -> _Event:
+    async def Event(self, id: str) -> "_Event":
         """
         Creates a Event resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.ServiceResource.Event)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/service_resource/#cloudformationserviceresourceevent-method)
         """
 
-    async def Stack(self, name: str) -> _Stack:
+    async def Stack(self, name: str) -> "_Stack":
         """
         Creates a Stack resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.ServiceResource.Stack)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/service_resource/#cloudformationserviceresourcestack-method)
         """
 
-    async def StackResource(self, stack_name: str, logical_id: str) -> _StackResource:
+    async def StackResource(self, stack_name: str, logical_id: str) -> "_StackResource":
         """
         Creates a StackResource resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.ServiceResource.StackResource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/service_resource/#cloudformationserviceresourcestackresource-method)
         """
 
-    async def StackResourceSummary(self, stack_name: str, logical_id: str) -> _StackResourceSummary:
+    async def StackResourceSummary(
+        self, stack_name: str, logical_id: str
+    ) -> "_StackResourceSummary":
         """
         Creates a StackResourceSummary resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.ServiceResource.StackResourceSummary)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/service_resource/#cloudformationserviceresourcestackresourcesummary-method)
         """
 
@@ -537,16 +542,16 @@
         RoleARN: str = ...,
         OnFailure: OnFailureType = ...,
         StackPolicyBody: str = ...,
         StackPolicyURL: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...,
         EnableTerminationProtection: bool = ...,
-        RetainExceptOnCreate: bool = ...
-    ) -> _Stack:
+        RetainExceptOnCreate: bool = ...,
+    ) -> "_Stack":
         """
         Creates a stack as specified in the template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.ServiceResource.create_stack)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/service_resource/#cloudformationserviceresourcecreate_stack-method)
         """
```

### Comparing `types-aiobotocore-cloudformation-2.9.0/types_aiobotocore_cloudformation/service_resource.pyi` & `types-aiobotocore-cloudformation-2.9.1/types_aiobotocore_cloudformation/service_resource.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -234,14 +234,15 @@
     client_request_token: Awaitable[str]
     hook_type: Awaitable[str]
     hook_status: Awaitable[HookStatusType]
     hook_status_reason: Awaitable[str]
     hook_invocation_point: Awaitable[Literal["PRE_PROVISION"]]
     hook_failure_mode: Awaitable[HookFailureModeType]
     id: str
+    meta: Awaitable["CloudFormationResourceMeta"]
 
     async def get_available_subresources(self) -> Sequence[str]:
         """
         Returns a list of all the available sub-resources for this Resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Event.get_available_subresources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/service_resource/#eventget_available_subresources-method)
@@ -277,14 +278,15 @@
     parent_id: Awaitable[str]
     root_id: Awaitable[str]
     drift_information: Awaitable[StackDriftInformationResponseTypeDef]
     retain_except_on_create: Awaitable[bool]
     name: str
     events: StackEventsCollection
     resource_summaries: StackResourceSummariesCollection
+    meta: Awaitable["CloudFormationResourceMeta"]
 
     async def Resource(self, logical_id: str) -> "_StackResource":
         """
         Creates a StackResource resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Stack.Resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/service_resource/#stackresource-method)
@@ -299,15 +301,15 @@
         """
 
     async def delete(
         self,
         *,
         RetainResources: Sequence[str] = ...,
         RoleARN: str = ...,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
     ) -> None:
         """
         Deletes a specified stack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Stack.delete)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/service_resource/#stackdelete-method)
         """
@@ -355,15 +357,15 @@
         RollbackConfiguration: RollbackConfigurationTypeDef = ...,
         StackPolicyBody: str = ...,
         StackPolicyURL: str = ...,
         NotificationARNs: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DisableRollback: bool = ...,
         ClientRequestToken: str = ...,
-        RetainExceptOnCreate: bool = ...
+        RetainExceptOnCreate: bool = ...,
     ) -> UpdateStackOutputTypeDef:
         """
         Updates a stack as specified in the template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Stack.update)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/service_resource/#stackupdate-method)
         """
@@ -385,16 +387,17 @@
     resource_status_reason: Awaitable[str]
     description: Awaitable[str]
     metadata: Awaitable[str]
     drift_information: Awaitable[StackResourceDriftInformationResponseTypeDef]
     module_info: Awaitable[ModuleInfoTypeDef]
     stack_name: str
     logical_id: str
+    meta: Awaitable["CloudFormationResourceMeta"]
 
-    async def Stack(self) -> _Stack:
+    async def Stack(self) -> "_Stack":
         """
         Creates a Stack resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.StackResource.Stack)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/service_resource/#stackresourcestack-method)
         """
 
@@ -440,16 +443,17 @@
     last_updated_timestamp: Awaitable[datetime]
     resource_status: Awaitable[ResourceStatusType]
     resource_status_reason: Awaitable[str]
     drift_information: Awaitable[StackResourceDriftInformationSummaryResponseTypeDef]
     module_info: Awaitable[ModuleInfoResponseTypeDef]
     stack_name: str
     logical_id: str
+    meta: Awaitable["CloudFormationResourceMeta"]
 
-    async def Resource(self) -> _StackResource:
+    async def Resource(self) -> "_StackResource":
         """
         Creates a StackResource resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.StackResourceSummary.Resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/service_resource/#stackresourcesummaryresource-method)
         """
 
@@ -471,39 +475,41 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.ServiceResource)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/service_resource/)
     """
 
     meta: "CloudFormationResourceMeta"
     stacks: ServiceResourceStacksCollection
 
-    async def Event(self, id: str) -> _Event:
+    async def Event(self, id: str) -> "_Event":
         """
         Creates a Event resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.ServiceResource.Event)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/service_resource/#cloudformationserviceresourceevent-method)
         """
 
-    async def Stack(self, name: str) -> _Stack:
+    async def Stack(self, name: str) -> "_Stack":
         """
         Creates a Stack resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.ServiceResource.Stack)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/service_resource/#cloudformationserviceresourcestack-method)
         """
 
-    async def StackResource(self, stack_name: str, logical_id: str) -> _StackResource:
+    async def StackResource(self, stack_name: str, logical_id: str) -> "_StackResource":
         """
         Creates a StackResource resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.ServiceResource.StackResource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/service_resource/#cloudformationserviceresourcestackresource-method)
         """
 
-    async def StackResourceSummary(self, stack_name: str, logical_id: str) -> _StackResourceSummary:
+    async def StackResourceSummary(
+        self, stack_name: str, logical_id: str
+    ) -> "_StackResourceSummary":
         """
         Creates a StackResourceSummary resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.ServiceResource.StackResourceSummary)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/service_resource/#cloudformationserviceresourcestackresourcesummary-method)
         """
 
@@ -523,16 +529,16 @@
         RoleARN: str = ...,
         OnFailure: OnFailureType = ...,
         StackPolicyBody: str = ...,
         StackPolicyURL: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...,
         EnableTerminationProtection: bool = ...,
-        RetainExceptOnCreate: bool = ...
-    ) -> _Stack:
+        RetainExceptOnCreate: bool = ...,
+    ) -> "_Stack":
         """
         Creates a stack as specified in the template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.ServiceResource.create_stack)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/service_resource/#cloudformationserviceresourcecreate_stack-method)
         """
```

### Comparing `types-aiobotocore-cloudformation-2.9.0/types_aiobotocore_cloudformation/type_defs.py` & `types-aiobotocore-cloudformation-2.9.1/types_aiobotocore_cloudformation/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccountGateResultTypeDef",
     "AccountLimitTypeDef",
     "LoggingConfigTypeDef",
     "ResponseMetadataTypeDef",
     "AutoDeploymentTypeDef",
     "TypeConfigurationIdentifierTypeDef",
```

### Comparing `types-aiobotocore-cloudformation-2.9.0/types_aiobotocore_cloudformation/type_defs.pyi` & `types-aiobotocore-cloudformation-2.9.1/types_aiobotocore_cloudformation/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudformation-2.9.0/types_aiobotocore_cloudformation/waiter.py` & `types-aiobotocore-cloudformation-2.9.1/types_aiobotocore_cloudformation/waiter.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
     async def wait(
         self,
         *,
         ChangeSetName: str,
         StackName: str = ...,
         NextToken: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Waiter.ChangeSetCreateComplete.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/waiters/#changesetcreatecompletewaiter)
         """
```

### Comparing `types-aiobotocore-cloudformation-2.9.0/types_aiobotocore_cloudformation/waiter.pyi` & `types-aiobotocore-cloudformation-2.9.1/types_aiobotocore_cloudformation/waiter.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
     async def wait(
         self,
         *,
         ChangeSetName: str,
         StackName: str = ...,
         NextToken: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Waiter.ChangeSetCreateComplete.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/waiters/#changesetcreatecompletewaiter)
         """
 
 class StackCreateCompleteWaiter(AIOWaiter):
```

### Comparing `types-aiobotocore-cloudformation-2.9.0/types_aiobotocore_cloudformation.egg-info/PKG-INFO` & `types-aiobotocore-cloudformation-2.9.1/types_aiobotocore_cloudformation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudformation
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CloudFormation 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CloudFormation 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/
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
 
 <a id="types-aiobotocore-cloudformation"></a>
 
 # types-aiobotocore-cloudformation
 
 [![PyPI - types-aiobotocore-cloudformation](https://img.shields.io/pypi/v/types-aiobotocore-cloudformation.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudformation)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudformation.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudformation)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudformation)](https://pepy.tech/project/types-aiobotocore-cloudformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudFormation 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation)
+[aiobotocore.CloudFormation 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation)
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
 [types-aiobotocore-cloudformation docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-cloudformation-2.9.0/types_aiobotocore_cloudformation.egg-info/SOURCES.txt` & `types-aiobotocore-cloudformation-2.9.1/types_aiobotocore_cloudformation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

