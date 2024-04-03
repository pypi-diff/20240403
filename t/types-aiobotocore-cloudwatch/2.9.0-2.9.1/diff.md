# Comparing `tmp/types-aiobotocore-cloudwatch-2.9.0.tar.gz` & `tmp/types-aiobotocore-cloudwatch-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cloudwatch-2.9.0.tar", last modified: Wed Dec 13 19:58:52 2023, max compression
+gzip compressed data, was "types-aiobotocore-cloudwatch-2.9.1.tar", last modified: Thu Jan 18 01:20:18 2024, max compression
```

## Comparing `types-aiobotocore-cloudwatch-2.9.0.tar` & `types-aiobotocore-cloudwatch-2.9.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:52.197952 types-aiobotocore-cloudwatch-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:42:37.000000 types-aiobotocore-cloudwatch-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16937 2023-12-13 19:58:52.197952 types-aiobotocore-cloudwatch-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15362 2023-12-13 19:42:37.000000 types-aiobotocore-cloudwatch-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:52.197952 types-aiobotocore-cloudwatch-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2023-12-13 19:42:37.000000 types-aiobotocore-cloudwatch-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:52.197952 types-aiobotocore-cloudwatch-2.9.0/types_aiobotocore_cloudwatch/
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2023-12-13 19:42:37.000000 types-aiobotocore-cloudwatch-2.9.0/types_aiobotocore_cloudwatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2023-12-13 19:42:37.000000 types-aiobotocore-cloudwatch-2.9.0/types_aiobotocore_cloudwatch/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      944 2023-12-13 19:42:37.000000 types-aiobotocore-cloudwatch-2.9.0/types_aiobotocore_cloudwatch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34927 2023-12-13 19:42:37.000000 types-aiobotocore-cloudwatch-2.9.0/types_aiobotocore_cloudwatch/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    34923 2023-12-13 19:42:37.000000 types-aiobotocore-cloudwatch-2.9.0/types_aiobotocore_cloudwatch/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11752 2023-12-13 19:42:38.000000 types-aiobotocore-cloudwatch-2.9.0/types_aiobotocore_cloudwatch/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11750 2023-12-13 19:42:38.000000 types-aiobotocore-cloudwatch-2.9.0/types_aiobotocore_cloudwatch/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9302 2023-12-13 19:42:37.000000 types-aiobotocore-cloudwatch-2.9.0/types_aiobotocore_cloudwatch/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9293 2023-12-13 19:42:37.000000 types-aiobotocore-cloudwatch-2.9.0/types_aiobotocore_cloudwatch/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:42:37.000000 types-aiobotocore-cloudwatch-2.9.0/types_aiobotocore_cloudwatch/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    25840 2023-12-13 19:42:37.000000 types-aiobotocore-cloudwatch-2.9.0/types_aiobotocore_cloudwatch/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    25830 2023-12-13 19:42:37.000000 types-aiobotocore-cloudwatch-2.9.0/types_aiobotocore_cloudwatch/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    47831 2023-12-13 19:42:38.000000 types-aiobotocore-cloudwatch-2.9.0/types_aiobotocore_cloudwatch/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    47830 2023-12-13 19:42:38.000000 types-aiobotocore-cloudwatch-2.9.0/types_aiobotocore_cloudwatch/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:42:37.000000 types-aiobotocore-cloudwatch-2.9.0/types_aiobotocore_cloudwatch/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2023-12-13 19:42:37.000000 types-aiobotocore-cloudwatch-2.9.0/types_aiobotocore_cloudwatch/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3334 2023-12-13 19:42:37.000000 types-aiobotocore-cloudwatch-2.9.0/types_aiobotocore_cloudwatch/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:52.197952 types-aiobotocore-cloudwatch-2.9.0/types_aiobotocore_cloudwatch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16937 2023-12-13 19:58:52.000000 types-aiobotocore-cloudwatch-2.9.0/types_aiobotocore_cloudwatch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2023-12-13 19:58:52.000000 types-aiobotocore-cloudwatch-2.9.0/types_aiobotocore_cloudwatch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:52.000000 types-aiobotocore-cloudwatch-2.9.0/types_aiobotocore_cloudwatch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:52.000000 types-aiobotocore-cloudwatch-2.9.0/types_aiobotocore_cloudwatch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:52.000000 types-aiobotocore-cloudwatch-2.9.0/types_aiobotocore_cloudwatch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-13 19:58:52.000000 types-aiobotocore-cloudwatch-2.9.0/types_aiobotocore_cloudwatch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:18.749450 types-aiobotocore-cloudwatch-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:04:33.000000 types-aiobotocore-cloudwatch-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16957 2024-01-18 01:20:18.749450 types-aiobotocore-cloudwatch-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15362 2024-01-18 01:04:33.000000 types-aiobotocore-cloudwatch-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:18.749450 types-aiobotocore-cloudwatch-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-01-18 01:04:33.000000 types-aiobotocore-cloudwatch-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:18.745450 types-aiobotocore-cloudwatch-2.9.1/types_aiobotocore_cloudwatch/
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-01-18 01:04:33.000000 types-aiobotocore-cloudwatch-2.9.1/types_aiobotocore_cloudwatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-01-18 01:04:33.000000 types-aiobotocore-cloudwatch-2.9.1/types_aiobotocore_cloudwatch/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-01-18 01:04:33.000000 types-aiobotocore-cloudwatch-2.9.1/types_aiobotocore_cloudwatch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34941 2024-01-18 01:04:34.000000 types-aiobotocore-cloudwatch-2.9.1/types_aiobotocore_cloudwatch/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34938 2024-01-18 01:04:33.000000 types-aiobotocore-cloudwatch-2.9.1/types_aiobotocore_cloudwatch/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11750 2024-01-18 01:04:34.000000 types-aiobotocore-cloudwatch-2.9.1/types_aiobotocore_cloudwatch/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11750 2024-01-18 01:04:34.000000 types-aiobotocore-cloudwatch-2.9.1/types_aiobotocore_cloudwatch/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9305 2024-01-18 01:04:34.000000 types-aiobotocore-cloudwatch-2.9.1/types_aiobotocore_cloudwatch/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9298 2024-01-18 01:04:34.000000 types-aiobotocore-cloudwatch-2.9.1/types_aiobotocore_cloudwatch/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:04:33.000000 types-aiobotocore-cloudwatch-2.9.1/types_aiobotocore_cloudwatch/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    25943 2024-01-18 01:04:34.000000 types-aiobotocore-cloudwatch-2.9.1/types_aiobotocore_cloudwatch/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25934 2024-01-18 01:04:34.000000 types-aiobotocore-cloudwatch-2.9.1/types_aiobotocore_cloudwatch/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    47830 2024-01-18 01:04:35.000000 types-aiobotocore-cloudwatch-2.9.1/types_aiobotocore_cloudwatch/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47830 2024-01-18 01:04:35.000000 types-aiobotocore-cloudwatch-2.9.1/types_aiobotocore_cloudwatch/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:04:33.000000 types-aiobotocore-cloudwatch-2.9.1/types_aiobotocore_cloudwatch/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-01-18 01:04:34.000000 types-aiobotocore-cloudwatch-2.9.1/types_aiobotocore_cloudwatch/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-01-18 01:04:34.000000 types-aiobotocore-cloudwatch-2.9.1/types_aiobotocore_cloudwatch/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:18.745450 types-aiobotocore-cloudwatch-2.9.1/types_aiobotocore_cloudwatch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16957 2024-01-18 01:20:18.000000 types-aiobotocore-cloudwatch-2.9.1/types_aiobotocore_cloudwatch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-01-18 01:20:18.000000 types-aiobotocore-cloudwatch-2.9.1/types_aiobotocore_cloudwatch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:18.000000 types-aiobotocore-cloudwatch-2.9.1/types_aiobotocore_cloudwatch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:18.000000 types-aiobotocore-cloudwatch-2.9.1/types_aiobotocore_cloudwatch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:18.000000 types-aiobotocore-cloudwatch-2.9.1/types_aiobotocore_cloudwatch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-01-18 01:20:18.000000 types-aiobotocore-cloudwatch-2.9.1/types_aiobotocore_cloudwatch.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cloudwatch-2.9.0/LICENSE` & `types-aiobotocore-cloudwatch-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-cloudwatch-2.9.0/PKG-INFO` & `types-aiobotocore-cloudwatch-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudwatch
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CloudWatch 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CloudWatch 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/
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
 
 <a id="types-aiobotocore-cloudwatch"></a>
 
 # types-aiobotocore-cloudwatch
 
 [![PyPI - types-aiobotocore-cloudwatch](https://img.shields.io/pypi/v/types-aiobotocore-cloudwatch.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudwatch)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudwatch.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudwatch)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudwatch)](https://pepy.tech/project/types-aiobotocore-cloudwatch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudWatch 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
+[aiobotocore.CloudWatch 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
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
 [types-aiobotocore-cloudwatch docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-cloudwatch-2.9.0/README.md` & `types-aiobotocore-cloudwatch-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudwatch.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudwatch)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudwatch)](https://pepy.tech/project/types-aiobotocore-cloudwatch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudWatch 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
+[aiobotocore.CloudWatch 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
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
 [types-aiobotocore-cloudwatch docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-cloudwatch-2.9.0/setup.py` & `types-aiobotocore-cloudwatch-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cloudwatch",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_cloudwatch"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CloudWatch 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.CloudWatch 2.9.1 service generated with"
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
     keywords="aiobotocore cloudwatch type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_cloudwatch": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-cloudwatch-2.9.0/types_aiobotocore_cloudwatch/__init__.py` & `types-aiobotocore-cloudwatch-2.9.1/types_aiobotocore_cloudwatch/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,18 +48,16 @@
     ListMetricsPaginator,
 )
 from .service_resource import CloudWatchServiceResource
 from .waiter import AlarmExistsWaiter, CompositeAlarmExistsWaiter
 
 Client = CloudWatchClient
 
-
 ServiceResource = CloudWatchServiceResource
 
-
 __all__ = (
     "AlarmExistsWaiter",
     "Client",
     "CloudWatchClient",
     "CloudWatchServiceResource",
     "CompositeAlarmExistsWaiter",
     "DescribeAlarmHistoryPaginator",
```

### Comparing `types-aiobotocore-cloudwatch-2.9.0/types_aiobotocore_cloudwatch/__init__.pyi` & `types-aiobotocore-cloudwatch-2.9.1/types_aiobotocore_cloudwatch/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudwatch-2.9.0/types_aiobotocore_cloudwatch/__main__.py` & `types-aiobotocore-cloudwatch-2.9.1/types_aiobotocore_cloudwatch/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CloudWatch 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.CloudWatch 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch\nOther"
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

### Comparing `types-aiobotocore-cloudwatch-2.9.0/types_aiobotocore_cloudwatch/client.py` & `types-aiobotocore-cloudwatch-2.9.1/types_aiobotocore_cloudwatch/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -81,26 +81,23 @@
 from .waiter import AlarmExistsWaiter, CompositeAlarmExistsWaiter
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("CloudWatchClient",)
 
-
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     ConcurrentModificationException: Type[BotocoreClientError]
     DashboardInvalidInputError: Type[BotocoreClientError]
     DashboardNotFoundError: Type[BotocoreClientError]
     InternalServiceFault: Type[BotocoreClientError]
     InvalidFormatFault: Type[BotocoreClientError]
@@ -109,15 +106,14 @@
     InvalidParameterValueException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     LimitExceededFault: Type[BotocoreClientError]
     MissingRequiredParameterException: Type[BotocoreClientError]
     ResourceNotFound: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
 
-
 class CloudWatchClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/client/)
     """
 
     meta: ClientMeta
@@ -159,15 +155,15 @@
         self,
         *,
         Namespace: str = ...,
         MetricName: str = ...,
         Dimensions: Sequence[DimensionTypeDef] = ...,
         Stat: str = ...,
         SingleMetricAnomalyDetector: SingleMetricAnomalyDetectorTypeDef = ...,
-        MetricMathAnomalyDetector: MetricMathAnomalyDetectorTypeDef = ...
+        MetricMathAnomalyDetector: MetricMathAnomalyDetectorTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Deletes the specified anomaly detection model from your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.delete_anomaly_detector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/client/#delete_anomaly_detector)
         """
@@ -204,15 +200,15 @@
         AlarmName: str = ...,
         AlarmTypes: Sequence[AlarmTypeType] = ...,
         HistoryItemType: HistoryItemTypeType = ...,
         StartDate: TimestampTypeDef = ...,
         EndDate: TimestampTypeDef = ...,
         MaxRecords: int = ...,
         NextToken: str = ...,
-        ScanBy: ScanByType = ...
+        ScanBy: ScanByType = ...,
     ) -> DescribeAlarmHistoryOutputTypeDef:
         """
         Retrieves the history for the specified alarm.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.describe_alarm_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/client/#describe_alarm_history)
         """
@@ -224,15 +220,15 @@
         AlarmNamePrefix: str = ...,
         AlarmTypes: Sequence[AlarmTypeType] = ...,
         ChildrenOfAlarmName: str = ...,
         ParentsOfAlarmName: str = ...,
         StateValue: StateValueType = ...,
         ActionPrefix: str = ...,
         MaxRecords: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeAlarmsOutputTypeDef:
         """
         Retrieves the specified alarms.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.describe_alarms)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/client/#describe_alarms)
         """
@@ -242,15 +238,15 @@
         *,
         MetricName: str,
         Namespace: str,
         Statistic: StatisticType = ...,
         ExtendedStatistic: str = ...,
         Dimensions: Sequence[DimensionTypeDef] = ...,
         Period: int = ...,
-        Unit: StandardUnitType = ...
+        Unit: StandardUnitType = ...,
     ) -> DescribeAlarmsForMetricOutputTypeDef:
         """
         Retrieves the alarms for the specified metric.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.describe_alarms_for_metric)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/client/#describe_alarms_for_metric)
         """
@@ -259,15 +255,15 @@
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         Namespace: str = ...,
         MetricName: str = ...,
         Dimensions: Sequence[DimensionTypeDef] = ...,
-        AnomalyDetectorTypes: Sequence[AnomalyDetectorTypeType] = ...
+        AnomalyDetectorTypes: Sequence[AnomalyDetectorTypeType] = ...,
     ) -> DescribeAnomalyDetectorsOutputTypeDef:
         """
         Lists the anomaly detection models that you have created in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.describe_anomaly_detectors)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/client/#describe_anomaly_detectors)
         """
@@ -349,15 +345,15 @@
         *,
         RuleName: str,
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
         Period: int,
         MaxContributorCount: int = ...,
         Metrics: Sequence[str] = ...,
-        OrderBy: str = ...
+        OrderBy: str = ...,
     ) -> GetInsightRuleReportOutputTypeDef:
         """
         This operation returns the time series data collected by a Contributor Insights
         rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.get_insight_rule_report)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/client/#get_insight_rule_report)
@@ -368,15 +364,15 @@
         *,
         MetricDataQueries: Sequence[MetricDataQueryTypeDef],
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
         NextToken: str = ...,
         ScanBy: ScanByType = ...,
         MaxDatapoints: int = ...,
-        LabelOptions: LabelOptionsTypeDef = ...
+        LabelOptions: LabelOptionsTypeDef = ...,
     ) -> GetMetricDataOutputTypeDef:
         """
         You can use the `GetMetricData` API to retrieve CloudWatch metric values.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.get_metric_data)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/client/#get_metric_data)
         """
@@ -388,15 +384,15 @@
         MetricName: str,
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
         Period: int,
         Dimensions: Sequence[DimensionTypeDef] = ...,
         Statistics: Sequence[StatisticType] = ...,
         ExtendedStatistics: Sequence[str] = ...,
-        Unit: StandardUnitType = ...
+        Unit: StandardUnitType = ...,
     ) -> GetMetricStatisticsOutputTypeDef:
         """
         Gets statistics for the specified metric.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.get_metric_statistics)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/client/#get_metric_statistics)
         """
@@ -458,15 +454,15 @@
         *,
         Namespace: str = ...,
         MetricName: str = ...,
         Dimensions: Sequence[DimensionFilterTypeDef] = ...,
         NextToken: str = ...,
         RecentlyActive: Literal["PT3H"] = ...,
         IncludeLinkedAccounts: bool = ...,
-        OwningAccount: str = ...
+        OwningAccount: str = ...,
     ) -> ListMetricsOutputTypeDef:
         """
         List the specified metrics.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.list_metrics)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/client/#list_metrics)
         """
@@ -484,15 +480,15 @@
         *,
         Namespace: str = ...,
         MetricName: str = ...,
         Dimensions: Sequence[DimensionTypeDef] = ...,
         Stat: str = ...,
         Configuration: AnomalyDetectorConfigurationTypeDef = ...,
         SingleMetricAnomalyDetector: SingleMetricAnomalyDetectorTypeDef = ...,
-        MetricMathAnomalyDetector: MetricMathAnomalyDetectorTypeDef = ...
+        MetricMathAnomalyDetector: MetricMathAnomalyDetectorTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Creates an anomaly detection model for a CloudWatch metric.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.put_anomaly_detector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/client/#put_anomaly_detector)
         """
@@ -506,15 +502,15 @@
         AlarmActions: Sequence[str] = ...,
         AlarmDescription: str = ...,
         InsufficientDataActions: Sequence[str] = ...,
         OKActions: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ActionsSuppressor: str = ...,
         ActionsSuppressorWaitPeriod: int = ...,
-        ActionsSuppressorExtensionPeriod: int = ...
+        ActionsSuppressorExtensionPeriod: int = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates or updates a *composite alarm*.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.put_composite_alarm)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/client/#put_composite_alarm)
         """
@@ -532,15 +528,15 @@
 
     async def put_insight_rule(
         self,
         *,
         RuleName: str,
         RuleDefinition: str,
         RuleState: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Creates a Contributor Insights rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.put_insight_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/client/#put_insight_rule)
         """
@@ -576,15 +572,15 @@
         Unit: StandardUnitType = ...,
         DatapointsToAlarm: int = ...,
         Threshold: float = ...,
         TreatMissingData: str = ...,
         EvaluateLowSampleCountPercentile: str = ...,
         Metrics: Sequence[MetricDataQueryTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ThresholdMetricId: str = ...
+        ThresholdMetricId: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates or updates an alarm and associates it with the specified metric, metric
         math expression, anomaly detection model, or Metrics Insights
         query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.put_metric_alarm)
@@ -608,30 +604,30 @@
         FirehoseArn: str,
         RoleArn: str,
         OutputFormat: MetricStreamOutputFormatType,
         IncludeFilters: Sequence[MetricStreamFilterTypeDef] = ...,
         ExcludeFilters: Sequence[MetricStreamFilterTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         StatisticsConfigurations: Sequence[MetricStreamStatisticsConfigurationTypeDef] = ...,
-        IncludeLinkedAccountsMetrics: bool = ...
+        IncludeLinkedAccountsMetrics: bool = ...,
     ) -> PutMetricStreamOutputTypeDef:
         """
         Creates or updates a metric stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.put_metric_stream)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/client/#put_metric_stream)
         """
 
     async def set_alarm_state(
         self,
         *,
         AlarmName: str,
         StateValue: StateValueType,
         StateReason: str,
-        StateReasonData: str = ...
+        StateReasonData: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Temporarily sets the state of an alarm for testing purposes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.set_alarm_state)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/client/#set_alarm_state)
         """
```

### Comparing `types-aiobotocore-cloudwatch-2.9.0/types_aiobotocore_cloudwatch/client.pyi` & `types-aiobotocore-cloudwatch-2.9.1/types_aiobotocore_cloudwatch/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,21 +83,23 @@
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = ("CloudWatchClient",)
 
+
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     ConcurrentModificationException: Type[BotocoreClientError]
     DashboardInvalidInputError: Type[BotocoreClientError]
     DashboardNotFoundError: Type[BotocoreClientError]
     InternalServiceFault: Type[BotocoreClientError]
     InvalidFormatFault: Type[BotocoreClientError]
@@ -106,14 +108,15 @@
     InvalidParameterValueException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     LimitExceededFault: Type[BotocoreClientError]
     MissingRequiredParameterException: Type[BotocoreClientError]
     ResourceNotFound: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
 
+
 class CloudWatchClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/client/)
     """
 
     meta: ClientMeta
@@ -155,15 +158,15 @@
         self,
         *,
         Namespace: str = ...,
         MetricName: str = ...,
         Dimensions: Sequence[DimensionTypeDef] = ...,
         Stat: str = ...,
         SingleMetricAnomalyDetector: SingleMetricAnomalyDetectorTypeDef = ...,
-        MetricMathAnomalyDetector: MetricMathAnomalyDetectorTypeDef = ...
+        MetricMathAnomalyDetector: MetricMathAnomalyDetectorTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Deletes the specified anomaly detection model from your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.delete_anomaly_detector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/client/#delete_anomaly_detector)
         """
@@ -200,15 +203,15 @@
         AlarmName: str = ...,
         AlarmTypes: Sequence[AlarmTypeType] = ...,
         HistoryItemType: HistoryItemTypeType = ...,
         StartDate: TimestampTypeDef = ...,
         EndDate: TimestampTypeDef = ...,
         MaxRecords: int = ...,
         NextToken: str = ...,
-        ScanBy: ScanByType = ...
+        ScanBy: ScanByType = ...,
     ) -> DescribeAlarmHistoryOutputTypeDef:
         """
         Retrieves the history for the specified alarm.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.describe_alarm_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/client/#describe_alarm_history)
         """
@@ -220,15 +223,15 @@
         AlarmNamePrefix: str = ...,
         AlarmTypes: Sequence[AlarmTypeType] = ...,
         ChildrenOfAlarmName: str = ...,
         ParentsOfAlarmName: str = ...,
         StateValue: StateValueType = ...,
         ActionPrefix: str = ...,
         MaxRecords: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeAlarmsOutputTypeDef:
         """
         Retrieves the specified alarms.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.describe_alarms)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/client/#describe_alarms)
         """
@@ -238,15 +241,15 @@
         *,
         MetricName: str,
         Namespace: str,
         Statistic: StatisticType = ...,
         ExtendedStatistic: str = ...,
         Dimensions: Sequence[DimensionTypeDef] = ...,
         Period: int = ...,
-        Unit: StandardUnitType = ...
+        Unit: StandardUnitType = ...,
     ) -> DescribeAlarmsForMetricOutputTypeDef:
         """
         Retrieves the alarms for the specified metric.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.describe_alarms_for_metric)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/client/#describe_alarms_for_metric)
         """
@@ -255,15 +258,15 @@
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         Namespace: str = ...,
         MetricName: str = ...,
         Dimensions: Sequence[DimensionTypeDef] = ...,
-        AnomalyDetectorTypes: Sequence[AnomalyDetectorTypeType] = ...
+        AnomalyDetectorTypes: Sequence[AnomalyDetectorTypeType] = ...,
     ) -> DescribeAnomalyDetectorsOutputTypeDef:
         """
         Lists the anomaly detection models that you have created in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.describe_anomaly_detectors)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/client/#describe_anomaly_detectors)
         """
@@ -345,15 +348,15 @@
         *,
         RuleName: str,
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
         Period: int,
         MaxContributorCount: int = ...,
         Metrics: Sequence[str] = ...,
-        OrderBy: str = ...
+        OrderBy: str = ...,
     ) -> GetInsightRuleReportOutputTypeDef:
         """
         This operation returns the time series data collected by a Contributor Insights
         rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.get_insight_rule_report)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/client/#get_insight_rule_report)
@@ -364,15 +367,15 @@
         *,
         MetricDataQueries: Sequence[MetricDataQueryTypeDef],
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
         NextToken: str = ...,
         ScanBy: ScanByType = ...,
         MaxDatapoints: int = ...,
-        LabelOptions: LabelOptionsTypeDef = ...
+        LabelOptions: LabelOptionsTypeDef = ...,
     ) -> GetMetricDataOutputTypeDef:
         """
         You can use the `GetMetricData` API to retrieve CloudWatch metric values.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.get_metric_data)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/client/#get_metric_data)
         """
@@ -384,15 +387,15 @@
         MetricName: str,
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
         Period: int,
         Dimensions: Sequence[DimensionTypeDef] = ...,
         Statistics: Sequence[StatisticType] = ...,
         ExtendedStatistics: Sequence[str] = ...,
-        Unit: StandardUnitType = ...
+        Unit: StandardUnitType = ...,
     ) -> GetMetricStatisticsOutputTypeDef:
         """
         Gets statistics for the specified metric.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.get_metric_statistics)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/client/#get_metric_statistics)
         """
@@ -454,15 +457,15 @@
         *,
         Namespace: str = ...,
         MetricName: str = ...,
         Dimensions: Sequence[DimensionFilterTypeDef] = ...,
         NextToken: str = ...,
         RecentlyActive: Literal["PT3H"] = ...,
         IncludeLinkedAccounts: bool = ...,
-        OwningAccount: str = ...
+        OwningAccount: str = ...,
     ) -> ListMetricsOutputTypeDef:
         """
         List the specified metrics.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.list_metrics)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/client/#list_metrics)
         """
@@ -480,15 +483,15 @@
         *,
         Namespace: str = ...,
         MetricName: str = ...,
         Dimensions: Sequence[DimensionTypeDef] = ...,
         Stat: str = ...,
         Configuration: AnomalyDetectorConfigurationTypeDef = ...,
         SingleMetricAnomalyDetector: SingleMetricAnomalyDetectorTypeDef = ...,
-        MetricMathAnomalyDetector: MetricMathAnomalyDetectorTypeDef = ...
+        MetricMathAnomalyDetector: MetricMathAnomalyDetectorTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Creates an anomaly detection model for a CloudWatch metric.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.put_anomaly_detector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/client/#put_anomaly_detector)
         """
@@ -502,15 +505,15 @@
         AlarmActions: Sequence[str] = ...,
         AlarmDescription: str = ...,
         InsufficientDataActions: Sequence[str] = ...,
         OKActions: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ActionsSuppressor: str = ...,
         ActionsSuppressorWaitPeriod: int = ...,
-        ActionsSuppressorExtensionPeriod: int = ...
+        ActionsSuppressorExtensionPeriod: int = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates or updates a *composite alarm*.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.put_composite_alarm)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/client/#put_composite_alarm)
         """
@@ -528,15 +531,15 @@
 
     async def put_insight_rule(
         self,
         *,
         RuleName: str,
         RuleDefinition: str,
         RuleState: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Creates a Contributor Insights rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.put_insight_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/client/#put_insight_rule)
         """
@@ -572,15 +575,15 @@
         Unit: StandardUnitType = ...,
         DatapointsToAlarm: int = ...,
         Threshold: float = ...,
         TreatMissingData: str = ...,
         EvaluateLowSampleCountPercentile: str = ...,
         Metrics: Sequence[MetricDataQueryTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ThresholdMetricId: str = ...
+        ThresholdMetricId: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates or updates an alarm and associates it with the specified metric, metric
         math expression, anomaly detection model, or Metrics Insights
         query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.put_metric_alarm)
@@ -604,30 +607,30 @@
         FirehoseArn: str,
         RoleArn: str,
         OutputFormat: MetricStreamOutputFormatType,
         IncludeFilters: Sequence[MetricStreamFilterTypeDef] = ...,
         ExcludeFilters: Sequence[MetricStreamFilterTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         StatisticsConfigurations: Sequence[MetricStreamStatisticsConfigurationTypeDef] = ...,
-        IncludeLinkedAccountsMetrics: bool = ...
+        IncludeLinkedAccountsMetrics: bool = ...,
     ) -> PutMetricStreamOutputTypeDef:
         """
         Creates or updates a metric stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.put_metric_stream)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/client/#put_metric_stream)
         """
 
     async def set_alarm_state(
         self,
         *,
         AlarmName: str,
         StateValue: StateValueType,
         StateReason: str,
-        StateReasonData: str = ...
+        StateReasonData: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Temporarily sets the state of an alarm for testing purposes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.set_alarm_state)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/client/#set_alarm_state)
         """
```

### Comparing `types-aiobotocore-cloudwatch-2.9.0/types_aiobotocore_cloudwatch/literals.py` & `types-aiobotocore-cloudwatch-2.9.1/types_aiobotocore_cloudwatch/literals.py`

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
     "ActionsSuppressedByType",
     "AlarmExistsWaiterName",
     "AlarmTypeType",
     "AnomalyDetectorStateValueType",
     "AnomalyDetectorTypeType",
     "ComparisonOperatorType",
@@ -47,15 +46,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 ActionsSuppressedByType = Literal["Alarm", "ExtensionPeriod", "WaitPeriod"]
 AlarmExistsWaiterName = Literal["alarm_exists"]
 AlarmTypeType = Literal["CompositeAlarm", "MetricAlarm"]
 AnomalyDetectorStateValueType = Literal["PENDING_TRAINING", "TRAINED", "TRAINED_INSUFFICIENT_DATA"]
 AnomalyDetectorTypeType = Literal["METRIC_MATH", "SINGLE_METRIC"]
 ComparisonOperatorType = Literal[
     "GreaterThanOrEqualToThreshold",
```

### Comparing `types-aiobotocore-cloudwatch-2.9.0/types_aiobotocore_cloudwatch/literals.pyi` & `types-aiobotocore-cloudwatch-2.9.1/types_aiobotocore_cloudwatch/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudwatch-2.9.0/types_aiobotocore_cloudwatch/paginator.py` & `types-aiobotocore-cloudwatch-2.9.1/types_aiobotocore_cloudwatch/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,25 +60,23 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "DescribeAlarmHistoryPaginator",
     "DescribeAlarmsPaginator",
     "DescribeAnomalyDetectorsPaginator",
     "GetMetricDataPaginator",
     "ListDashboardsPaginator",
     "ListMetricsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -96,15 +94,15 @@
         *,
         AlarmName: str = ...,
         AlarmTypes: Sequence[AlarmTypeType] = ...,
         HistoryItemType: HistoryItemTypeType = ...,
         StartDate: TimestampTypeDef = ...,
         EndDate: TimestampTypeDef = ...,
         ScanBy: ScanByType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeAlarmHistoryOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.DescribeAlarmHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/paginators/#describealarmhistorypaginator)
         """
 
 
@@ -120,15 +118,15 @@
         AlarmNames: Sequence[str] = ...,
         AlarmNamePrefix: str = ...,
         AlarmTypes: Sequence[AlarmTypeType] = ...,
         ChildrenOfAlarmName: str = ...,
         ParentsOfAlarmName: str = ...,
         StateValue: StateValueType = ...,
         ActionPrefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeAlarmsOutputPaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.DescribeAlarms.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/paginators/#describealarmspaginator)
         """
 
 
@@ -141,15 +139,15 @@
     def paginate(
         self,
         *,
         Namespace: str = ...,
         MetricName: str = ...,
         Dimensions: Sequence[DimensionTypeDef] = ...,
         AnomalyDetectorTypes: Sequence[AnomalyDetectorTypeType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeAnomalyDetectorsOutputPaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.DescribeAnomalyDetectors.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/paginators/#describeanomalydetectorspaginator)
         """
 
 
@@ -163,15 +161,15 @@
         self,
         *,
         MetricDataQueries: Sequence[MetricDataQueryPaginatorTypeDef],
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
         ScanBy: ScanByType = ...,
         LabelOptions: LabelOptionsTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetMetricDataOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.GetMetricData.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/paginators/#getmetricdatapaginator)
         """
 
 
@@ -201,13 +199,13 @@
         *,
         Namespace: str = ...,
         MetricName: str = ...,
         Dimensions: Sequence[DimensionFilterTypeDef] = ...,
         RecentlyActive: Literal["PT3H"] = ...,
         IncludeLinkedAccounts: bool = ...,
         OwningAccount: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListMetricsOutputPaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.ListMetrics.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/paginators/#listmetricspaginator)
         """
```

### Comparing `types-aiobotocore-cloudwatch-2.9.0/types_aiobotocore_cloudwatch/paginator.pyi` & `types-aiobotocore-cloudwatch-2.9.1/types_aiobotocore_cloudwatch/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         *,
         AlarmName: str = ...,
         AlarmTypes: Sequence[AlarmTypeType] = ...,
         HistoryItemType: HistoryItemTypeType = ...,
         StartDate: TimestampTypeDef = ...,
         EndDate: TimestampTypeDef = ...,
         ScanBy: ScanByType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeAlarmHistoryOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.DescribeAlarmHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/paginators/#describealarmhistorypaginator)
         """
 
 class DescribeAlarmsPaginator(AioPaginator):
@@ -115,15 +115,15 @@
         AlarmNames: Sequence[str] = ...,
         AlarmNamePrefix: str = ...,
         AlarmTypes: Sequence[AlarmTypeType] = ...,
         ChildrenOfAlarmName: str = ...,
         ParentsOfAlarmName: str = ...,
         StateValue: StateValueType = ...,
         ActionPrefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeAlarmsOutputPaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.DescribeAlarms.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/paginators/#describealarmspaginator)
         """
 
 class DescribeAnomalyDetectorsPaginator(AioPaginator):
@@ -135,15 +135,15 @@
     def paginate(
         self,
         *,
         Namespace: str = ...,
         MetricName: str = ...,
         Dimensions: Sequence[DimensionTypeDef] = ...,
         AnomalyDetectorTypes: Sequence[AnomalyDetectorTypeType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeAnomalyDetectorsOutputPaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.DescribeAnomalyDetectors.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/paginators/#describeanomalydetectorspaginator)
         """
 
 class GetMetricDataPaginator(AioPaginator):
@@ -156,15 +156,15 @@
         self,
         *,
         MetricDataQueries: Sequence[MetricDataQueryPaginatorTypeDef],
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
         ScanBy: ScanByType = ...,
         LabelOptions: LabelOptionsTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetMetricDataOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.GetMetricData.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/paginators/#getmetricdatapaginator)
         """
 
 class ListDashboardsPaginator(AioPaginator):
@@ -192,13 +192,13 @@
         *,
         Namespace: str = ...,
         MetricName: str = ...,
         Dimensions: Sequence[DimensionFilterTypeDef] = ...,
         RecentlyActive: Literal["PT3H"] = ...,
         IncludeLinkedAccounts: bool = ...,
         OwningAccount: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListMetricsOutputPaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.ListMetrics.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/paginators/#listmetricspaginator)
         """
```

### Comparing `types-aiobotocore-cloudwatch-2.9.0/types_aiobotocore_cloudwatch/service_resource.py` & `types-aiobotocore-cloudwatch-2.9.1/types_aiobotocore_cloudwatch/service_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,14 @@
 else:
     from typing_extensions import Literal
 try:
     from boto3.resources.base import ResourceMeta
 except ImportError:
     from builtins import object as ResourceMeta
 
-
 __all__ = (
     "CloudWatchServiceResource",
     "Alarm",
     "Metric",
     "ServiceResourceAlarmsCollection",
     "ServiceResourceMetricsCollection",
     "MetricAlarmsCollection",
@@ -94,15 +93,15 @@
         AlarmNamePrefix: str = ...,
         AlarmTypes: Sequence[AlarmTypeType] = ...,
         ChildrenOfAlarmName: str = ...,
         ParentsOfAlarmName: str = ...,
         StateValue: StateValueType = ...,
         ActionPrefix: str = ...,
         MaxRecords: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> "ServiceResourceAlarmsCollection":
         """
         Get items from the collection, passing keyword arguments along as parameters to the underlying service operation, which are typically used to filter the results.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.ServiceResource.alarms)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/service_resource/#serviceresourcealarmscollection)
         """
@@ -191,15 +190,15 @@
         *,
         Namespace: str = ...,
         MetricName: str = ...,
         Dimensions: Sequence[DimensionFilterTypeDef] = ...,
         NextToken: str = ...,
         RecentlyActive: Literal["PT3H"] = ...,
         IncludeLinkedAccounts: bool = ...,
-        OwningAccount: str = ...
+        OwningAccount: str = ...,
     ) -> "ServiceResourceMetricsCollection":
         """
         Get items from the collection, passing keyword arguments along as parameters to the underlying service operation, which are typically used to filter the results.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.ServiceResource.metrics)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/service_resource/#serviceresourcemetricscollection)
         """
@@ -254,15 +253,15 @@
     def filter(  # type: ignore
         self,
         *,
         Statistic: StatisticType = ...,
         ExtendedStatistic: str = ...,
         Dimensions: Sequence[DimensionTypeDef] = ...,
         Period: int = ...,
-        Unit: StandardUnitType = ...
+        Unit: StandardUnitType = ...,
     ) -> "MetricAlarmsCollection":
         """
         Get items from the collection, passing keyword arguments along as parameters to the underlying service operation, which are typically used to filter the results.
         """
 
     async def delete(self) -> None:
         """
@@ -338,14 +337,15 @@
     evaluate_low_sample_count_percentile: Awaitable[str]
     metrics: Awaitable[List[MetricDataQueryAlarmTypeDef]]
     threshold_metric_id: Awaitable[str]
     evaluation_state: Awaitable[Literal["PARTIAL_DATA"]]
     state_transitioned_timestamp: Awaitable[datetime]
     name: str
     metric: "Metric"
+    meta: Awaitable["CloudWatchResourceMeta"]
 
     async def delete(self) -> None:
         """
         Deletes the specified alarms.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Alarm.delete)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/service_resource/#alarmdelete-method)
@@ -356,15 +356,15 @@
         *,
         AlarmTypes: Sequence[AlarmTypeType] = ...,
         HistoryItemType: HistoryItemTypeType = ...,
         StartDate: TimestampTypeDef = ...,
         EndDate: TimestampTypeDef = ...,
         MaxRecords: int = ...,
         NextToken: str = ...,
-        ScanBy: ScanByType = ...
+        ScanBy: ScanByType = ...,
     ) -> DescribeAlarmHistoryOutputTypeDef:
         """
         Retrieves the history for the specified alarm.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Alarm.describe_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/service_resource/#alarmdescribe_history-method)
         """
@@ -434,14 +434,15 @@
     """
 
     metric_name: Awaitable[str]
     dimensions: Awaitable[List[DimensionTypeDef]]
     namespace: str
     name: str
     alarms: MetricAlarmsCollection
+    meta: Awaitable["CloudWatchResourceMeta"]
 
     async def get_available_subresources(self) -> Sequence[str]:
         """
         Returns a list of all the available sub-resources for this Resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Metric.get_available_subresources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/service_resource/#metricget_available_subresources-method)
@@ -452,15 +453,15 @@
         *,
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
         Period: int,
         Dimensions: Sequence[DimensionTypeDef] = ...,
         Statistics: Sequence[StatisticType] = ...,
         ExtendedStatistics: Sequence[str] = ...,
-        Unit: StandardUnitType = ...
+        Unit: StandardUnitType = ...,
     ) -> GetMetricStatisticsOutputTypeDef:
         """
         Gets statistics for the specified metric.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Metric.get_statistics)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/service_resource/#metricget_statistics-method)
         """
@@ -493,16 +494,16 @@
         Unit: StandardUnitType = ...,
         DatapointsToAlarm: int = ...,
         Threshold: float = ...,
         TreatMissingData: str = ...,
         EvaluateLowSampleCountPercentile: str = ...,
         Metrics: Sequence[MetricDataQueryTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ThresholdMetricId: str = ...
-    ) -> _Alarm:
+        ThresholdMetricId: str = ...,
+    ) -> "_Alarm":
         """
         Creates or updates an alarm and associates it with the specified metric, metric
         math expression, anomaly detection model, or Metrics Insights
         query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Metric.put_alarm)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/service_resource/#metricput_alarm-method)
@@ -540,23 +541,23 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/service_resource/)
     """
 
     meta: "CloudWatchResourceMeta"
     alarms: ServiceResourceAlarmsCollection
     metrics: ServiceResourceMetricsCollection
 
-    async def Alarm(self, name: str) -> _Alarm:
+    async def Alarm(self, name: str) -> "_Alarm":
         """
         Creates a Alarm resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.ServiceResource.Alarm)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/service_resource/#cloudwatchserviceresourcealarm-method)
         """
 
-    async def Metric(self, namespace: str, name: str) -> _Metric:
+    async def Metric(self, namespace: str, name: str) -> "_Metric":
         """
         Creates a Metric resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.ServiceResource.Metric)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/service_resource/#cloudwatchserviceresourcemetric-method)
         """
```

### Comparing `types-aiobotocore-cloudwatch-2.9.0/types_aiobotocore_cloudwatch/service_resource.pyi` & `types-aiobotocore-cloudwatch-2.9.1/types_aiobotocore_cloudwatch/service_resource.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         AlarmNamePrefix: str = ...,
         AlarmTypes: Sequence[AlarmTypeType] = ...,
         ChildrenOfAlarmName: str = ...,
         ParentsOfAlarmName: str = ...,
         StateValue: StateValueType = ...,
         ActionPrefix: str = ...,
         MaxRecords: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> "ServiceResourceAlarmsCollection":
         """
         Get items from the collection, passing keyword arguments along as parameters to the underlying service operation, which are typically used to filter the results.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.ServiceResource.alarms)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/service_resource/#serviceresourcealarmscollection)
         """
@@ -188,15 +188,15 @@
         *,
         Namespace: str = ...,
         MetricName: str = ...,
         Dimensions: Sequence[DimensionFilterTypeDef] = ...,
         NextToken: str = ...,
         RecentlyActive: Literal["PT3H"] = ...,
         IncludeLinkedAccounts: bool = ...,
-        OwningAccount: str = ...
+        OwningAccount: str = ...,
     ) -> "ServiceResourceMetricsCollection":
         """
         Get items from the collection, passing keyword arguments along as parameters to the underlying service operation, which are typically used to filter the results.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.ServiceResource.metrics)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/service_resource/#serviceresourcemetricscollection)
         """
@@ -250,15 +250,15 @@
     def filter(  # type: ignore
         self,
         *,
         Statistic: StatisticType = ...,
         ExtendedStatistic: str = ...,
         Dimensions: Sequence[DimensionTypeDef] = ...,
         Period: int = ...,
-        Unit: StandardUnitType = ...
+        Unit: StandardUnitType = ...,
     ) -> "MetricAlarmsCollection":
         """
         Get items from the collection, passing keyword arguments along as parameters to the underlying service operation, which are typically used to filter the results.
         """
 
     async def delete(self) -> None:
         """
@@ -333,14 +333,15 @@
     evaluate_low_sample_count_percentile: Awaitable[str]
     metrics: Awaitable[List[MetricDataQueryAlarmTypeDef]]
     threshold_metric_id: Awaitable[str]
     evaluation_state: Awaitable[Literal["PARTIAL_DATA"]]
     state_transitioned_timestamp: Awaitable[datetime]
     name: str
     metric: "Metric"
+    meta: Awaitable["CloudWatchResourceMeta"]
 
     async def delete(self) -> None:
         """
         Deletes the specified alarms.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Alarm.delete)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/service_resource/#alarmdelete-method)
@@ -351,15 +352,15 @@
         *,
         AlarmTypes: Sequence[AlarmTypeType] = ...,
         HistoryItemType: HistoryItemTypeType = ...,
         StartDate: TimestampTypeDef = ...,
         EndDate: TimestampTypeDef = ...,
         MaxRecords: int = ...,
         NextToken: str = ...,
-        ScanBy: ScanByType = ...
+        ScanBy: ScanByType = ...,
     ) -> DescribeAlarmHistoryOutputTypeDef:
         """
         Retrieves the history for the specified alarm.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Alarm.describe_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/service_resource/#alarmdescribe_history-method)
         """
@@ -427,14 +428,15 @@
     """
 
     metric_name: Awaitable[str]
     dimensions: Awaitable[List[DimensionTypeDef]]
     namespace: str
     name: str
     alarms: MetricAlarmsCollection
+    meta: Awaitable["CloudWatchResourceMeta"]
 
     async def get_available_subresources(self) -> Sequence[str]:
         """
         Returns a list of all the available sub-resources for this Resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Metric.get_available_subresources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/service_resource/#metricget_available_subresources-method)
@@ -445,15 +447,15 @@
         *,
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
         Period: int,
         Dimensions: Sequence[DimensionTypeDef] = ...,
         Statistics: Sequence[StatisticType] = ...,
         ExtendedStatistics: Sequence[str] = ...,
-        Unit: StandardUnitType = ...
+        Unit: StandardUnitType = ...,
     ) -> GetMetricStatisticsOutputTypeDef:
         """
         Gets statistics for the specified metric.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Metric.get_statistics)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/service_resource/#metricget_statistics-method)
         """
@@ -486,16 +488,16 @@
         Unit: StandardUnitType = ...,
         DatapointsToAlarm: int = ...,
         Threshold: float = ...,
         TreatMissingData: str = ...,
         EvaluateLowSampleCountPercentile: str = ...,
         Metrics: Sequence[MetricDataQueryTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ThresholdMetricId: str = ...
-    ) -> _Alarm:
+        ThresholdMetricId: str = ...,
+    ) -> "_Alarm":
         """
         Creates or updates an alarm and associates it with the specified metric, metric
         math expression, anomaly detection model, or Metrics Insights
         query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Metric.put_alarm)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/service_resource/#metricput_alarm-method)
@@ -530,23 +532,23 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/service_resource/)
     """
 
     meta: "CloudWatchResourceMeta"
     alarms: ServiceResourceAlarmsCollection
     metrics: ServiceResourceMetricsCollection
 
-    async def Alarm(self, name: str) -> _Alarm:
+    async def Alarm(self, name: str) -> "_Alarm":
         """
         Creates a Alarm resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.ServiceResource.Alarm)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/service_resource/#cloudwatchserviceresourcealarm-method)
         """
 
-    async def Metric(self, namespace: str, name: str) -> _Metric:
+    async def Metric(self, namespace: str, name: str) -> "_Metric":
         """
         Creates a Metric resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.ServiceResource.Metric)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/service_resource/#cloudwatchserviceresourcemetric-method)
         """
```

### Comparing `types-aiobotocore-cloudwatch-2.9.0/types_aiobotocore_cloudwatch/type_defs.py` & `types-aiobotocore-cloudwatch-2.9.1/types_aiobotocore_cloudwatch/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AlarmHistoryItemTypeDef",
     "RangeTypeDef",
     "DimensionTypeDef",
     "CloudwatchEventStateTypeDef",
     "CloudwatchEventMetricStatsMetricTypeDef",
     "CompositeAlarmTypeDef",
```

### Comparing `types-aiobotocore-cloudwatch-2.9.0/types_aiobotocore_cloudwatch/type_defs.pyi` & `types-aiobotocore-cloudwatch-2.9.1/types_aiobotocore_cloudwatch/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudwatch-2.9.0/types_aiobotocore_cloudwatch/waiter.py` & `types-aiobotocore-cloudwatch-2.9.1/types_aiobotocore_cloudwatch/waiter.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         AlarmTypes: Sequence[AlarmTypeType] = ...,
         ChildrenOfAlarmName: str = ...,
         ParentsOfAlarmName: str = ...,
         StateValue: StateValueType = ...,
         ActionPrefix: str = ...,
         MaxRecords: int = ...,
         NextToken: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Waiter.AlarmExists.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/waiters/#alarmexistswaiter)
         """
 
 
@@ -73,13 +73,13 @@
         AlarmTypes: Sequence[AlarmTypeType] = ...,
         ChildrenOfAlarmName: str = ...,
         ParentsOfAlarmName: str = ...,
         StateValue: StateValueType = ...,
         ActionPrefix: str = ...,
         MaxRecords: int = ...,
         NextToken: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Waiter.CompositeAlarmExists.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/waiters/#compositealarmexistswaiter)
         """
```

### Comparing `types-aiobotocore-cloudwatch-2.9.0/types_aiobotocore_cloudwatch/waiter.pyi` & `types-aiobotocore-cloudwatch-2.9.1/types_aiobotocore_cloudwatch/waiter.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         AlarmTypes: Sequence[AlarmTypeType] = ...,
         ChildrenOfAlarmName: str = ...,
         ParentsOfAlarmName: str = ...,
         StateValue: StateValueType = ...,
         ActionPrefix: str = ...,
         MaxRecords: int = ...,
         NextToken: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Waiter.AlarmExists.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/waiters/#alarmexistswaiter)
         """
 
 class CompositeAlarmExistsWaiter(AIOWaiter):
@@ -71,13 +71,13 @@
         AlarmTypes: Sequence[AlarmTypeType] = ...,
         ChildrenOfAlarmName: str = ...,
         ParentsOfAlarmName: str = ...,
         StateValue: StateValueType = ...,
         ActionPrefix: str = ...,
         MaxRecords: int = ...,
         NextToken: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Waiter.CompositeAlarmExists.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/waiters/#compositealarmexistswaiter)
         """
```

### Comparing `types-aiobotocore-cloudwatch-2.9.0/types_aiobotocore_cloudwatch.egg-info/PKG-INFO` & `types-aiobotocore-cloudwatch-2.9.1/types_aiobotocore_cloudwatch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudwatch
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CloudWatch 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CloudWatch 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/
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
 
 <a id="types-aiobotocore-cloudwatch"></a>
 
 # types-aiobotocore-cloudwatch
 
 [![PyPI - types-aiobotocore-cloudwatch](https://img.shields.io/pypi/v/types-aiobotocore-cloudwatch.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudwatch)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudwatch.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudwatch)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudwatch)](https://pepy.tech/project/types-aiobotocore-cloudwatch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudWatch 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
+[aiobotocore.CloudWatch 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
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
 [types-aiobotocore-cloudwatch docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-cloudwatch-2.9.0/types_aiobotocore_cloudwatch.egg-info/SOURCES.txt` & `types-aiobotocore-cloudwatch-2.9.1/types_aiobotocore_cloudwatch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

