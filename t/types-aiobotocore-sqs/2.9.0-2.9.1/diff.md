# Comparing `tmp/types-aiobotocore-sqs-2.9.0.tar.gz` & `tmp/types-aiobotocore-sqs-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-sqs-2.9.0.tar", last modified: Wed Dec 13 20:00:34 2023, max compression
+gzip compressed data, was "types-aiobotocore-sqs-2.9.1.tar", last modified: Thu Jan 18 01:21:52 2024, max compression
```

## Comparing `types-aiobotocore-sqs-2.9.0.tar` & `types-aiobotocore-sqs-2.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:34.717101 types-aiobotocore-sqs-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:56:43.000000 types-aiobotocore-sqs-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14943 2023-12-13 20:00:34.717101 types-aiobotocore-sqs-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13396 2023-12-13 19:56:43.000000 types-aiobotocore-sqs-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:34.717101 types-aiobotocore-sqs-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2023-12-13 19:56:43.000000 types-aiobotocore-sqs-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:34.717101 types-aiobotocore-sqs-2.9.0/types_aiobotocore_sqs/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2023-12-13 19:56:43.000000 types-aiobotocore-sqs-2.9.0/types_aiobotocore_sqs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2023-12-13 19:56:43.000000 types-aiobotocore-sqs-2.9.0/types_aiobotocore_sqs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      905 2023-12-13 19:56:43.000000 types-aiobotocore-sqs-2.9.0/types_aiobotocore_sqs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19687 2023-12-13 19:56:43.000000 types-aiobotocore-sqs-2.9.0/types_aiobotocore_sqs/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    19683 2023-12-13 19:56:43.000000 types-aiobotocore-sqs-2.9.0/types_aiobotocore_sqs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10960 2023-12-13 19:56:44.000000 types-aiobotocore-sqs-2.9.0/types_aiobotocore_sqs/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10958 2023-12-13 19:56:44.000000 types-aiobotocore-sqs-2.9.0/types_aiobotocore_sqs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3107 2023-12-13 19:56:43.000000 types-aiobotocore-sqs-2.9.0/types_aiobotocore_sqs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3103 2023-12-13 19:56:43.000000 types-aiobotocore-sqs-2.9.0/types_aiobotocore_sqs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:56:43.000000 types-aiobotocore-sqs-2.9.0/types_aiobotocore_sqs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    20905 2023-12-13 19:56:43.000000 types-aiobotocore-sqs-2.9.0/types_aiobotocore_sqs/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    20896 2023-12-13 19:56:43.000000 types-aiobotocore-sqs-2.9.0/types_aiobotocore_sqs/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    20314 2023-12-13 19:56:44.000000 types-aiobotocore-sqs-2.9.0/types_aiobotocore_sqs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    20313 2023-12-13 19:56:44.000000 types-aiobotocore-sqs-2.9.0/types_aiobotocore_sqs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:56:43.000000 types-aiobotocore-sqs-2.9.0/types_aiobotocore_sqs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:34.717101 types-aiobotocore-sqs-2.9.0/types_aiobotocore_sqs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14943 2023-12-13 20:00:34.000000 types-aiobotocore-sqs-2.9.0/types_aiobotocore_sqs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      822 2023-12-13 20:00:34.000000 types-aiobotocore-sqs-2.9.0/types_aiobotocore_sqs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:34.000000 types-aiobotocore-sqs-2.9.0/types_aiobotocore_sqs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:34.000000 types-aiobotocore-sqs-2.9.0/types_aiobotocore_sqs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:34.000000 types-aiobotocore-sqs-2.9.0/types_aiobotocore_sqs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-13 20:00:34.000000 types-aiobotocore-sqs-2.9.0/types_aiobotocore_sqs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:52.729017 types-aiobotocore-sqs-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:18:12.000000 types-aiobotocore-sqs-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14963 2024-01-18 01:21:52.729017 types-aiobotocore-sqs-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13396 2024-01-18 01:18:12.000000 types-aiobotocore-sqs-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:52.729017 types-aiobotocore-sqs-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-01-18 01:18:12.000000 types-aiobotocore-sqs-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:52.725017 types-aiobotocore-sqs-2.9.1/types_aiobotocore_sqs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-01-18 01:18:12.000000 types-aiobotocore-sqs-2.9.1/types_aiobotocore_sqs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-01-18 01:18:12.000000 types-aiobotocore-sqs-2.9.1/types_aiobotocore_sqs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-01-18 01:18:12.000000 types-aiobotocore-sqs-2.9.1/types_aiobotocore_sqs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19689 2024-01-18 01:18:12.000000 types-aiobotocore-sqs-2.9.1/types_aiobotocore_sqs/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19686 2024-01-18 01:18:12.000000 types-aiobotocore-sqs-2.9.1/types_aiobotocore_sqs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10958 2024-01-18 01:18:12.000000 types-aiobotocore-sqs-2.9.1/types_aiobotocore_sqs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10958 2024-01-18 01:18:12.000000 types-aiobotocore-sqs-2.9.1/types_aiobotocore_sqs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-01-18 01:18:12.000000 types-aiobotocore-sqs-2.9.1/types_aiobotocore_sqs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-01-18 01:18:12.000000 types-aiobotocore-sqs-2.9.1/types_aiobotocore_sqs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:18:12.000000 types-aiobotocore-sqs-2.9.1/types_aiobotocore_sqs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    20997 2024-01-18 01:18:12.000000 types-aiobotocore-sqs-2.9.1/types_aiobotocore_sqs/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20989 2024-01-18 01:18:12.000000 types-aiobotocore-sqs-2.9.1/types_aiobotocore_sqs/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    20313 2024-01-18 01:18:13.000000 types-aiobotocore-sqs-2.9.1/types_aiobotocore_sqs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20313 2024-01-18 01:18:13.000000 types-aiobotocore-sqs-2.9.1/types_aiobotocore_sqs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:18:12.000000 types-aiobotocore-sqs-2.9.1/types_aiobotocore_sqs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:52.729017 types-aiobotocore-sqs-2.9.1/types_aiobotocore_sqs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14963 2024-01-18 01:21:52.000000 types-aiobotocore-sqs-2.9.1/types_aiobotocore_sqs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-01-18 01:21:52.000000 types-aiobotocore-sqs-2.9.1/types_aiobotocore_sqs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:52.000000 types-aiobotocore-sqs-2.9.1/types_aiobotocore_sqs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:52.000000 types-aiobotocore-sqs-2.9.1/types_aiobotocore_sqs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:52.000000 types-aiobotocore-sqs-2.9.1/types_aiobotocore_sqs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-18 01:21:52.000000 types-aiobotocore-sqs-2.9.1/types_aiobotocore_sqs.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-sqs-2.9.0/LICENSE` & `types-aiobotocore-sqs-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-sqs-2.9.0/PKG-INFO` & `types-aiobotocore-sqs-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sqs
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.SQS 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.SQS 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/
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
 
 <a id="types-aiobotocore-sqs"></a>
 
 # types-aiobotocore-sqs
 
 [![PyPI - types-aiobotocore-sqs](https://img.shields.io/pypi/v/types-aiobotocore-sqs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sqs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sqs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sqs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sqs)](https://pepy.tech/project/types-aiobotocore-sqs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SQS 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS)
+[aiobotocore.SQS 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS)
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
 [types-aiobotocore-sqs docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-sqs-2.9.0/README.md` & `types-aiobotocore-sqs-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sqs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sqs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sqs)](https://pepy.tech/project/types-aiobotocore-sqs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SQS 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS)
+[aiobotocore.SQS 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS)
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
 [types-aiobotocore-sqs docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-sqs-2.9.0/setup.py` & `types-aiobotocore-sqs-2.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-sqs",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_sqs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.SQS 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.SQS 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore sqs type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_sqs": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-sqs-2.9.0/types_aiobotocore_sqs/__init__.py` & `types-aiobotocore-sqs-2.9.1/types_aiobotocore_sqs/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,18 +27,16 @@
 
 from .client import SQSClient
 from .paginator import ListDeadLetterSourceQueuesPaginator, ListQueuesPaginator
 from .service_resource import SQSServiceResource
 
 Client = SQSClient
 
-
 ServiceResource = SQSServiceResource
 
-
 __all__ = (
     "Client",
     "ListDeadLetterSourceQueuesPaginator",
     "ListQueuesPaginator",
     "SQSClient",
     "SQSServiceResource",
     "ServiceResource",
```

### Comparing `types-aiobotocore-sqs-2.9.0/types_aiobotocore_sqs/__init__.pyi` & `types-aiobotocore-sqs-2.9.1/types_aiobotocore_sqs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sqs-2.9.0/types_aiobotocore_sqs/__main__.py` & `types-aiobotocore-sqs-2.9.1/types_aiobotocore_sqs/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SQS 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.SQS 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS\nOther"
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

### Comparing `types-aiobotocore-sqs-2.9.0/types_aiobotocore_sqs/client.py` & `types-aiobotocore-sqs-2.9.1/types_aiobotocore_sqs/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("SQSClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -159,15 +158,15 @@
         """
 
     async def create_queue(
         self,
         *,
         QueueName: str,
         Attributes: Mapping[QueueAttributeNameType, str] = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateQueueResultTypeDef:
         """
         Creates a new standard or FIFO queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.create_queue)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#create_queue)
         """
@@ -291,15 +290,15 @@
         *,
         QueueUrl: str,
         AttributeNames: Sequence[QueueAttributeFilterType] = ...,
         MessageAttributeNames: Sequence[str] = ...,
         MaxNumberOfMessages: int = ...,
         VisibilityTimeout: int = ...,
         WaitTimeSeconds: int = ...,
-        ReceiveRequestAttemptId: str = ...
+        ReceiveRequestAttemptId: str = ...,
     ) -> ReceiveMessageResultTypeDef:
         """
         Retrieves one or more messages (up to 10), from the specified queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.receive_message)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#receive_message)
         """
@@ -320,15 +319,15 @@
         MessageBody: str,
         DelaySeconds: int = ...,
         MessageAttributes: Mapping[str, MessageAttributeValueTypeDef] = ...,
         MessageSystemAttributes: Mapping[
             Literal["AWSTraceHeader"], MessageSystemAttributeValueTypeDef
         ] = ...,
         MessageDeduplicationId: str = ...,
-        MessageGroupId: str = ...
+        MessageGroupId: str = ...,
     ) -> SendMessageResultTypeDef:
         """
         Delivers a message to the specified queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.send_message)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#send_message)
         """
```

### Comparing `types-aiobotocore-sqs-2.9.0/types_aiobotocore_sqs/client.pyi` & `types-aiobotocore-sqs-2.9.1/types_aiobotocore_sqs/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,15 @@
         """
 
     async def create_queue(
         self,
         *,
         QueueName: str,
         Attributes: Mapping[QueueAttributeNameType, str] = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateQueueResultTypeDef:
         """
         Creates a new standard or FIFO queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.create_queue)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#create_queue)
         """
@@ -287,15 +287,15 @@
         *,
         QueueUrl: str,
         AttributeNames: Sequence[QueueAttributeFilterType] = ...,
         MessageAttributeNames: Sequence[str] = ...,
         MaxNumberOfMessages: int = ...,
         VisibilityTimeout: int = ...,
         WaitTimeSeconds: int = ...,
-        ReceiveRequestAttemptId: str = ...
+        ReceiveRequestAttemptId: str = ...,
     ) -> ReceiveMessageResultTypeDef:
         """
         Retrieves one or more messages (up to 10), from the specified queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.receive_message)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#receive_message)
         """
@@ -316,15 +316,15 @@
         MessageBody: str,
         DelaySeconds: int = ...,
         MessageAttributes: Mapping[str, MessageAttributeValueTypeDef] = ...,
         MessageSystemAttributes: Mapping[
             Literal["AWSTraceHeader"], MessageSystemAttributeValueTypeDef
         ] = ...,
         MessageDeduplicationId: str = ...,
-        MessageGroupId: str = ...
+        MessageGroupId: str = ...,
     ) -> SendMessageResultTypeDef:
         """
         Delivers a message to the specified queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.send_message)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#send_message)
         """
```

### Comparing `types-aiobotocore-sqs-2.9.0/types_aiobotocore_sqs/literals.py` & `types-aiobotocore-sqs-2.9.1/types_aiobotocore_sqs/literals.py`

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
     "ListDeadLetterSourceQueuesPaginatorName",
     "ListQueuesPaginatorName",
     "MessageSystemAttributeNameForSendsType",
     "MessageSystemAttributeNameType",
     "QueueAttributeFilterType",
     "QueueAttributeNameType",
     "SQSServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ListDeadLetterSourceQueuesPaginatorName = Literal["list_dead_letter_source_queues"]
 ListQueuesPaginatorName = Literal["list_queues"]
 MessageSystemAttributeNameForSendsType = Literal["AWSTraceHeader"]
 MessageSystemAttributeNameType = Literal[
     "AWSTraceHeader",
     "ApproximateFirstReceiveTimestamp",
     "ApproximateReceiveCount",
```

### Comparing `types-aiobotocore-sqs-2.9.0/types_aiobotocore_sqs/literals.pyi` & `types-aiobotocore-sqs-2.9.1/types_aiobotocore_sqs/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sqs-2.9.0/types_aiobotocore_sqs/paginator.py` & `types-aiobotocore-sqs-2.9.1/types_aiobotocore_sqs/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,14 @@
     ListDeadLetterSourceQueuesResultTypeDef,
     ListQueuesResultTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("ListDeadLetterSourceQueuesPaginator", "ListQueuesPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
```

### Comparing `types-aiobotocore-sqs-2.9.0/types_aiobotocore_sqs/paginator.pyi` & `types-aiobotocore-sqs-2.9.1/types_aiobotocore_sqs/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sqs-2.9.0/types_aiobotocore_sqs/service_resource.py` & `types-aiobotocore-sqs-2.9.1/types_aiobotocore_sqs/service_resource.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -55,24 +55,22 @@
 else:
     from typing_extensions import Literal
 try:
     from boto3.resources.base import ResourceMeta
 except ImportError:
     from builtins import object as ResourceMeta
 
-
 __all__ = (
     "SQSServiceResource",
     "Message",
     "Queue",
     "ServiceResourceQueuesCollection",
     "QueueDeadLetterSourceQueuesCollection",
 )
 
-
 class ServiceResourceQueuesCollection(AIOResourceCollection):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.ServiceResource.queues)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/service_resource/#serviceresourcequeuescollection)
     """
 
     def all(self) -> "ServiceResourceQueuesCollection":
@@ -129,15 +127,14 @@
         """
         A generator which yields Queues.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.ServiceResource.queues)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/service_resource/#serviceresourcequeuescollection)
         """
 
-
 class QueueDeadLetterSourceQueuesCollection(AIOResourceCollection):
     def all(self) -> "QueueDeadLetterSourceQueuesCollection":
         """
         Get all items from the collection, optionally with a custom page size and item count limit.
         """
 
     def filter(  # type: ignore
@@ -168,29 +165,29 @@
         """
 
     def __aiter__(self) -> AsyncIterator["Queue"]:
         """
         A generator which yields Queues.
         """
 
-
 class Message(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.ServiceResource.Message)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/service_resource/#message)
     """
 
     message_id: Awaitable[str]
     md5_of_body: Awaitable[str]
     body: Awaitable[str]
     attributes: Awaitable[Dict[MessageSystemAttributeNameType, str]]
     md5_of_message_attributes: Awaitable[str]
     message_attributes: Awaitable[Dict[str, MessageAttributeValueTypeDef]]
     queue_url: str
     receipt_handle: str
+    meta: Awaitable["SQSResourceMeta"]
 
     async def Queue(self) -> "_Queue":
         """
         Creates a Queue resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Message.Queue)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/service_resource/#messagequeue-method)
@@ -216,29 +213,28 @@
         """
         Returns a list of all the available sub-resources for this Resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Message.get_available_subresources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/service_resource/#messageget_available_subresources-method)
         """
 
-
 _Message = Message
 
-
 class Queue(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.ServiceResource.Queue)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/service_resource/#queue)
     """
 
     attributes: Awaitable[Dict[QueueAttributeNameType, str]]
     url: str
     dead_letter_source_queues: QueueDeadLetterSourceQueuesCollection
+    meta: Awaitable["SQSResourceMeta"]
 
-    async def Message(self, receipt_handle: str) -> _Message:
+    async def Message(self, receipt_handle: str) -> "_Message":
         """
         Creates a Message resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.Message)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/service_resource/#queuemessage-method)
         """
 
@@ -314,16 +310,16 @@
         self,
         *,
         AttributeNames: Sequence[QueueAttributeFilterType] = ...,
         MessageAttributeNames: Sequence[str] = ...,
         MaxNumberOfMessages: int = ...,
         VisibilityTimeout: int = ...,
         WaitTimeSeconds: int = ...,
-        ReceiveRequestAttemptId: str = ...
-    ) -> List[_Message]:
+        ReceiveRequestAttemptId: str = ...,
+    ) -> List["_Message"]:
         """
         Retrieves one or more messages (up to 10), from the specified queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.receive_messages)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/service_resource/#queuereceive_messages-method)
         """
 
@@ -352,15 +348,15 @@
         MessageBody: str,
         DelaySeconds: int = ...,
         MessageAttributes: Mapping[str, MessageAttributeValueQueueTypeDef] = ...,
         MessageSystemAttributes: Mapping[
             Literal["AWSTraceHeader"], MessageSystemAttributeValueTypeDef
         ] = ...,
         MessageDeduplicationId: str = ...,
-        MessageGroupId: str = ...
+        MessageGroupId: str = ...,
     ) -> SendMessageResultTypeDef:
         """
         Delivers a message to the specified queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.send_message)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/service_resource/#queuesend_message-method)
         """
@@ -382,54 +378,51 @@
         """
         Sets the value of one or more queue attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.set_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/service_resource/#queueset_attributes-method)
         """
 
-
 _Queue = Queue
 
-
 class SQSResourceMeta(ResourceMeta):
     client: SQSClient
 
-
 class SQSServiceResource(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.ServiceResource)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/service_resource/)
     """
 
     meta: "SQSResourceMeta"
     queues: ServiceResourceQueuesCollection
 
-    async def Message(self, queue_url: str, receipt_handle: str) -> _Message:
+    async def Message(self, queue_url: str, receipt_handle: str) -> "_Message":
         """
         Creates a Message resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.ServiceResource.Message)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/service_resource/#sqsserviceresourcemessage-method)
         """
 
-    async def Queue(self, url: str) -> _Queue:
+    async def Queue(self, url: str) -> "_Queue":
         """
         Creates a Queue resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.ServiceResource.Queue)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/service_resource/#sqsserviceresourcequeue-method)
         """
 
     async def create_queue(
         self,
         *,
         QueueName: str,
         Attributes: Mapping[QueueAttributeNameType, str] = ...,
-        tags: Mapping[str, str] = ...
-    ) -> _Queue:
+        tags: Mapping[str, str] = ...,
+    ) -> "_Queue":
         """
         Creates a new standard or FIFO queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.ServiceResource.create_queue)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/service_resource/#sqsserviceresourcecreate_queue-method)
         """
 
@@ -439,14 +432,14 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.ServiceResource.get_available_subresources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/service_resource/#sqsserviceresourceget_available_subresources-method)
         """
 
     async def get_queue_by_name(
         self, *, QueueName: str, QueueOwnerAWSAccountId: str = ...
-    ) -> _Queue:
+    ) -> "_Queue":
         """
         Returns the URL of an existing Amazon SQS queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.ServiceResource.get_queue_by_name)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/service_resource/#sqsserviceresourceget_queue_by_name-method)
         """
```

### Comparing `types-aiobotocore-sqs-2.9.0/types_aiobotocore_sqs/service_resource.pyi` & `types-aiobotocore-sqs-2.9.1/types_aiobotocore_sqs/service_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,15 @@
     "SQSServiceResource",
     "Message",
     "Queue",
     "ServiceResourceQueuesCollection",
     "QueueDeadLetterSourceQueuesCollection",
 )
 
+
 class ServiceResourceQueuesCollection(AIOResourceCollection):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.ServiceResource.queues)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/service_resource/#serviceresourcequeuescollection)
     """
 
     def all(self) -> "ServiceResourceQueuesCollection":
@@ -127,14 +128,15 @@
         """
         A generator which yields Queues.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.ServiceResource.queues)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/service_resource/#serviceresourcequeuescollection)
         """
 
+
 class QueueDeadLetterSourceQueuesCollection(AIOResourceCollection):
     def all(self) -> "QueueDeadLetterSourceQueuesCollection":
         """
         Get all items from the collection, optionally with a custom page size and item count limit.
         """
 
     def filter(  # type: ignore
@@ -165,28 +167,30 @@
         """
 
     def __aiter__(self) -> AsyncIterator["Queue"]:
         """
         A generator which yields Queues.
         """
 
+
 class Message(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.ServiceResource.Message)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/service_resource/#message)
     """
 
     message_id: Awaitable[str]
     md5_of_body: Awaitable[str]
     body: Awaitable[str]
     attributes: Awaitable[Dict[MessageSystemAttributeNameType, str]]
     md5_of_message_attributes: Awaitable[str]
     message_attributes: Awaitable[Dict[str, MessageAttributeValueTypeDef]]
     queue_url: str
     receipt_handle: str
+    meta: Awaitable["SQSResourceMeta"]
 
     async def Queue(self) -> "_Queue":
         """
         Creates a Queue resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Message.Queue)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/service_resource/#messagequeue-method)
@@ -212,27 +216,30 @@
         """
         Returns a list of all the available sub-resources for this Resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Message.get_available_subresources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/service_resource/#messageget_available_subresources-method)
         """
 
+
 _Message = Message
 
+
 class Queue(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.ServiceResource.Queue)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/service_resource/#queue)
     """
 
     attributes: Awaitable[Dict[QueueAttributeNameType, str]]
     url: str
     dead_letter_source_queues: QueueDeadLetterSourceQueuesCollection
+    meta: Awaitable["SQSResourceMeta"]
 
-    async def Message(self, receipt_handle: str) -> _Message:
+    async def Message(self, receipt_handle: str) -> "_Message":
         """
         Creates a Message resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.Message)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/service_resource/#queuemessage-method)
         """
 
@@ -308,16 +315,16 @@
         self,
         *,
         AttributeNames: Sequence[QueueAttributeFilterType] = ...,
         MessageAttributeNames: Sequence[str] = ...,
         MaxNumberOfMessages: int = ...,
         VisibilityTimeout: int = ...,
         WaitTimeSeconds: int = ...,
-        ReceiveRequestAttemptId: str = ...
-    ) -> List[_Message]:
+        ReceiveRequestAttemptId: str = ...,
+    ) -> List["_Message"]:
         """
         Retrieves one or more messages (up to 10), from the specified queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.receive_messages)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/service_resource/#queuereceive_messages-method)
         """
 
@@ -346,15 +353,15 @@
         MessageBody: str,
         DelaySeconds: int = ...,
         MessageAttributes: Mapping[str, MessageAttributeValueQueueTypeDef] = ...,
         MessageSystemAttributes: Mapping[
             Literal["AWSTraceHeader"], MessageSystemAttributeValueTypeDef
         ] = ...,
         MessageDeduplicationId: str = ...,
-        MessageGroupId: str = ...
+        MessageGroupId: str = ...,
     ) -> SendMessageResultTypeDef:
         """
         Delivers a message to the specified queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.send_message)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/service_resource/#queuesend_message-method)
         """
@@ -376,51 +383,54 @@
         """
         Sets the value of one or more queue attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.set_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/service_resource/#queueset_attributes-method)
         """
 
+
 _Queue = Queue
 
+
 class SQSResourceMeta(ResourceMeta):
     client: SQSClient
 
+
 class SQSServiceResource(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.ServiceResource)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/service_resource/)
     """
 
     meta: "SQSResourceMeta"
     queues: ServiceResourceQueuesCollection
 
-    async def Message(self, queue_url: str, receipt_handle: str) -> _Message:
+    async def Message(self, queue_url: str, receipt_handle: str) -> "_Message":
         """
         Creates a Message resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.ServiceResource.Message)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/service_resource/#sqsserviceresourcemessage-method)
         """
 
-    async def Queue(self, url: str) -> _Queue:
+    async def Queue(self, url: str) -> "_Queue":
         """
         Creates a Queue resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.ServiceResource.Queue)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/service_resource/#sqsserviceresourcequeue-method)
         """
 
     async def create_queue(
         self,
         *,
         QueueName: str,
         Attributes: Mapping[QueueAttributeNameType, str] = ...,
-        tags: Mapping[str, str] = ...
-    ) -> _Queue:
+        tags: Mapping[str, str] = ...,
+    ) -> "_Queue":
         """
         Creates a new standard or FIFO queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.ServiceResource.create_queue)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/service_resource/#sqsserviceresourcecreate_queue-method)
         """
 
@@ -430,14 +440,14 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.ServiceResource.get_available_subresources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/service_resource/#sqsserviceresourceget_available_subresources-method)
         """
 
     async def get_queue_by_name(
         self, *, QueueName: str, QueueOwnerAWSAccountId: str = ...
-    ) -> _Queue:
+    ) -> "_Queue":
         """
         Returns the URL of an existing Amazon SQS queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.ServiceResource.get_queue_by_name)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/service_resource/#sqsserviceresourceget_queue_by_name-method)
         """
```

### Comparing `types-aiobotocore-sqs-2.9.0/types_aiobotocore_sqs/type_defs.py` & `types-aiobotocore-sqs-2.9.1/types_aiobotocore_sqs/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AddPermissionRequestQueueAddPermissionTypeDef",
     "AddPermissionRequestRequestTypeDef",
     "BatchResultErrorEntryTypeDef",
     "BlobTypeDef",
     "CancelMessageMoveTaskRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
```

### Comparing `types-aiobotocore-sqs-2.9.0/types_aiobotocore_sqs/type_defs.pyi` & `types-aiobotocore-sqs-2.9.1/types_aiobotocore_sqs/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sqs-2.9.0/types_aiobotocore_sqs.egg-info/PKG-INFO` & `types-aiobotocore-sqs-2.9.1/types_aiobotocore_sqs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sqs
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.SQS 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.SQS 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/
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
 
 <a id="types-aiobotocore-sqs"></a>
 
 # types-aiobotocore-sqs
 
 [![PyPI - types-aiobotocore-sqs](https://img.shields.io/pypi/v/types-aiobotocore-sqs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sqs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sqs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sqs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sqs)](https://pepy.tech/project/types-aiobotocore-sqs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SQS 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS)
+[aiobotocore.SQS 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS)
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
 [types-aiobotocore-sqs docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-sqs-2.9.0/types_aiobotocore_sqs.egg-info/SOURCES.txt` & `types-aiobotocore-sqs-2.9.1/types_aiobotocore_sqs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

