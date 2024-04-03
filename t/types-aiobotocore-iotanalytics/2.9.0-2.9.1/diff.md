# Comparing `tmp/types-aiobotocore-iotanalytics-2.9.0.tar.gz` & `tmp/types-aiobotocore-iotanalytics-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iotanalytics-2.9.0.tar", last modified: Wed Dec 13 19:59:32 2023, max compression
+gzip compressed data, was "types-aiobotocore-iotanalytics-2.9.1.tar", last modified: Thu Jan 18 01:20:55 2024, max compression
```

## Comparing `types-aiobotocore-iotanalytics-2.9.0.tar` & `types-aiobotocore-iotanalytics-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:32.173654 types-aiobotocore-iotanalytics-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:47:50.000000 types-aiobotocore-iotanalytics-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13776 2023-12-13 19:59:32.173654 types-aiobotocore-iotanalytics-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12193 2023-12-13 19:47:50.000000 types-aiobotocore-iotanalytics-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:32.173654 types-aiobotocore-iotanalytics-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2023-12-13 19:47:50.000000 types-aiobotocore-iotanalytics-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:32.173654 types-aiobotocore-iotanalytics-2.9.0/types_aiobotocore_iotanalytics/
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2023-12-13 19:47:50.000000 types-aiobotocore-iotanalytics-2.9.0/types_aiobotocore_iotanalytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2023-12-13 19:47:50.000000 types-aiobotocore-iotanalytics-2.9.0/types_aiobotocore_iotanalytics/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      952 2023-12-13 19:47:50.000000 types-aiobotocore-iotanalytics-2.9.0/types_aiobotocore_iotanalytics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28141 2023-12-13 19:47:50.000000 types-aiobotocore-iotanalytics-2.9.0/types_aiobotocore_iotanalytics/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    28137 2023-12-13 19:47:50.000000 types-aiobotocore-iotanalytics-2.9.0/types_aiobotocore_iotanalytics/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9674 2023-12-13 19:47:52.000000 types-aiobotocore-iotanalytics-2.9.0/types_aiobotocore_iotanalytics/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9672 2023-12-13 19:47:50.000000 types-aiobotocore-iotanalytics-2.9.0/types_aiobotocore_iotanalytics/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6601 2023-12-13 19:47:50.000000 types-aiobotocore-iotanalytics-2.9.0/types_aiobotocore_iotanalytics/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6594 2023-12-13 19:47:50.000000 types-aiobotocore-iotanalytics-2.9.0/types_aiobotocore_iotanalytics/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:47:50.000000 types-aiobotocore-iotanalytics-2.9.0/types_aiobotocore_iotanalytics/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    38646 2023-12-13 19:47:53.000000 types-aiobotocore-iotanalytics-2.9.0/types_aiobotocore_iotanalytics/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    38645 2023-12-13 19:47:52.000000 types-aiobotocore-iotanalytics-2.9.0/types_aiobotocore_iotanalytics/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:47:50.000000 types-aiobotocore-iotanalytics-2.9.0/types_aiobotocore_iotanalytics/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:32.173654 types-aiobotocore-iotanalytics-2.9.0/types_aiobotocore_iotanalytics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13776 2023-12-13 19:59:32.000000 types-aiobotocore-iotanalytics-2.9.0/types_aiobotocore_iotanalytics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      908 2023-12-13 19:59:32.000000 types-aiobotocore-iotanalytics-2.9.0/types_aiobotocore_iotanalytics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:32.000000 types-aiobotocore-iotanalytics-2.9.0/types_aiobotocore_iotanalytics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:32.000000 types-aiobotocore-iotanalytics-2.9.0/types_aiobotocore_iotanalytics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:32.000000 types-aiobotocore-iotanalytics-2.9.0/types_aiobotocore_iotanalytics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-13 19:59:32.000000 types-aiobotocore-iotanalytics-2.9.0/types_aiobotocore_iotanalytics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:55.693273 types-aiobotocore-iotanalytics-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:09:41.000000 types-aiobotocore-iotanalytics-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13796 2024-01-18 01:20:55.693273 types-aiobotocore-iotanalytics-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12193 2024-01-18 01:09:41.000000 types-aiobotocore-iotanalytics-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:55.693273 types-aiobotocore-iotanalytics-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-01-18 01:09:41.000000 types-aiobotocore-iotanalytics-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:55.689273 types-aiobotocore-iotanalytics-2.9.1/types_aiobotocore_iotanalytics/
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-01-18 01:09:41.000000 types-aiobotocore-iotanalytics-2.9.1/types_aiobotocore_iotanalytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-01-18 01:09:41.000000 types-aiobotocore-iotanalytics-2.9.1/types_aiobotocore_iotanalytics/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-01-18 01:09:41.000000 types-aiobotocore-iotanalytics-2.9.1/types_aiobotocore_iotanalytics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28150 2024-01-18 01:09:41.000000 types-aiobotocore-iotanalytics-2.9.1/types_aiobotocore_iotanalytics/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28147 2024-01-18 01:09:41.000000 types-aiobotocore-iotanalytics-2.9.1/types_aiobotocore_iotanalytics/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9672 2024-01-18 01:09:41.000000 types-aiobotocore-iotanalytics-2.9.1/types_aiobotocore_iotanalytics/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9672 2024-01-18 01:09:41.000000 types-aiobotocore-iotanalytics-2.9.1/types_aiobotocore_iotanalytics/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6601 2024-01-18 01:09:41.000000 types-aiobotocore-iotanalytics-2.9.1/types_aiobotocore_iotanalytics/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6595 2024-01-18 01:09:41.000000 types-aiobotocore-iotanalytics-2.9.1/types_aiobotocore_iotanalytics/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:09:41.000000 types-aiobotocore-iotanalytics-2.9.1/types_aiobotocore_iotanalytics/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    38645 2024-01-18 01:09:44.000000 types-aiobotocore-iotanalytics-2.9.1/types_aiobotocore_iotanalytics/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38645 2024-01-18 01:09:43.000000 types-aiobotocore-iotanalytics-2.9.1/types_aiobotocore_iotanalytics/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:09:41.000000 types-aiobotocore-iotanalytics-2.9.1/types_aiobotocore_iotanalytics/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:55.689273 types-aiobotocore-iotanalytics-2.9.1/types_aiobotocore_iotanalytics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13796 2024-01-18 01:20:55.000000 types-aiobotocore-iotanalytics-2.9.1/types_aiobotocore_iotanalytics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-01-18 01:20:55.000000 types-aiobotocore-iotanalytics-2.9.1/types_aiobotocore_iotanalytics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:55.000000 types-aiobotocore-iotanalytics-2.9.1/types_aiobotocore_iotanalytics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:55.000000 types-aiobotocore-iotanalytics-2.9.1/types_aiobotocore_iotanalytics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:55.000000 types-aiobotocore-iotanalytics-2.9.1/types_aiobotocore_iotanalytics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-01-18 01:20:55.000000 types-aiobotocore-iotanalytics-2.9.1/types_aiobotocore_iotanalytics.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iotanalytics-2.9.0/LICENSE` & `types-aiobotocore-iotanalytics-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-iotanalytics-2.9.0/PKG-INFO` & `types-aiobotocore-iotanalytics-2.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotanalytics
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.IoTAnalytics 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.IoTAnalytics 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/
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
 
 <a id="types-aiobotocore-iotanalytics"></a>
 
 # types-aiobotocore-iotanalytics
 
 [![PyPI - types-aiobotocore-iotanalytics](https://img.shields.io/pypi/v/types-aiobotocore-iotanalytics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotanalytics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotanalytics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotanalytics)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotanalytics)](https://pepy.tech/project/types-aiobotocore-iotanalytics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTAnalytics 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics)
+[aiobotocore.IoTAnalytics 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics)
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
 [types-aiobotocore-iotanalytics docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-iotanalytics-2.9.0/README.md` & `types-aiobotocore-iotanalytics-2.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotanalytics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotanalytics)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotanalytics)](https://pepy.tech/project/types-aiobotocore-iotanalytics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTAnalytics 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics)
+[aiobotocore.IoTAnalytics 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics)
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
 [types-aiobotocore-iotanalytics docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-iotanalytics-2.9.0/setup.py` & `types-aiobotocore-iotanalytics-2.9.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iotanalytics",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_iotanalytics"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.IoTAnalytics 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.IoTAnalytics 2.9.1 service generated with"
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
     keywords="aiobotocore iotanalytics type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_iotanalytics": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-iotanalytics-2.9.0/types_aiobotocore_iotanalytics/__init__.py` & `types-aiobotocore-iotanalytics-2.9.1/types_aiobotocore_iotanalytics/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     ListDatasetsPaginator,
     ListDatastoresPaginator,
     ListPipelinesPaginator,
 )
 
 Client = IoTAnalyticsClient
 
-
 __all__ = (
     "Client",
     "IoTAnalyticsClient",
     "ListChannelsPaginator",
     "ListDatasetContentsPaginator",
     "ListDatasetsPaginator",
     "ListDatastoresPaginator",
```

### Comparing `types-aiobotocore-iotanalytics-2.9.0/types_aiobotocore_iotanalytics/__init__.pyi` & `types-aiobotocore-iotanalytics-2.9.1/types_aiobotocore_iotanalytics/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotanalytics-2.9.0/types_aiobotocore_iotanalytics/__main__.py` & `types-aiobotocore-iotanalytics-2.9.1/types_aiobotocore_iotanalytics/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IoTAnalytics 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.IoTAnalytics 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics\nOther"
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

### Comparing `types-aiobotocore-iotanalytics-2.9.0/types_aiobotocore_iotanalytics/client.py` & `types-aiobotocore-iotanalytics-2.9.1/types_aiobotocore_iotanalytics/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("IoTAnalyticsClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -153,15 +152,15 @@
 
     async def create_channel(
         self,
         *,
         channelName: str,
         channelStorage: ChannelStorageTypeDef = ...,
         retentionPeriod: RetentionPeriodTypeDef = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateChannelResponseTypeDef:
         """
         Used to create a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.create_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#create_channel)
         """
@@ -172,15 +171,15 @@
         datasetName: str,
         actions: Sequence[DatasetActionTypeDef],
         triggers: Sequence[DatasetTriggerTypeDef] = ...,
         contentDeliveryRules: Sequence[DatasetContentDeliveryRuleTypeDef] = ...,
         retentionPeriod: RetentionPeriodTypeDef = ...,
         versioningConfiguration: VersioningConfigurationTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
-        lateDataRules: Sequence[LateDataRuleTypeDef] = ...
+        lateDataRules: Sequence[LateDataRuleTypeDef] = ...,
     ) -> CreateDatasetResponseTypeDef:
         """
         Used to create a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.create_dataset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#create_dataset)
         """
@@ -201,29 +200,29 @@
         self,
         *,
         datastoreName: str,
         datastoreStorage: DatastoreStorageTypeDef = ...,
         retentionPeriod: RetentionPeriodTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         fileFormatConfiguration: FileFormatConfigurationTypeDef = ...,
-        datastorePartitions: DatastorePartitionsTypeDef = ...
+        datastorePartitions: DatastorePartitionsTypeDef = ...,
     ) -> CreateDatastoreResponseTypeDef:
         """
         Creates a data store, which is a repository for messages.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.create_datastore)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#create_datastore)
         """
 
     async def create_pipeline(
         self,
         *,
         pipelineName: str,
         pipelineActivities: Sequence[PipelineActivityTypeDef],
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreatePipelineResponseTypeDef:
         """
         Creates a pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.create_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#create_pipeline)
         """
@@ -351,15 +350,15 @@
     async def list_dataset_contents(
         self,
         *,
         datasetName: str,
         nextToken: str = ...,
         maxResults: int = ...,
         scheduledOnOrAfter: TimestampTypeDef = ...,
-        scheduledBefore: TimestampTypeDef = ...
+        scheduledBefore: TimestampTypeDef = ...,
     ) -> ListDatasetContentsResponseTypeDef:
         """
         Lists information about dataset contents that have been created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.list_dataset_contents)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#list_dataset_contents)
         """
@@ -426,15 +425,15 @@
 
     async def sample_channel_data(
         self,
         *,
         channelName: str,
         maxMessages: int = ...,
         startTime: TimestampTypeDef = ...,
-        endTime: TimestampTypeDef = ...
+        endTime: TimestampTypeDef = ...,
     ) -> SampleChannelDataResponseTypeDef:
         """
         Retrieves a sample of messages from the specified channel ingested during the
         specified
         timeframe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.sample_channel_data)
@@ -443,15 +442,15 @@
 
     async def start_pipeline_reprocessing(
         self,
         *,
         pipelineName: str,
         startTime: TimestampTypeDef = ...,
         endTime: TimestampTypeDef = ...,
-        channelMessages: ChannelMessagesTypeDef = ...
+        channelMessages: ChannelMessagesTypeDef = ...,
     ) -> StartPipelineReprocessingResponseTypeDef:
         """
         Starts the reprocessing of raw message data through the pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.start_pipeline_reprocessing)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#start_pipeline_reprocessing)
         """
@@ -473,15 +472,15 @@
         """
 
     async def update_channel(
         self,
         *,
         channelName: str,
         channelStorage: ChannelStorageTypeDef = ...,
-        retentionPeriod: RetentionPeriodTypeDef = ...
+        retentionPeriod: RetentionPeriodTypeDef = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Used to update the settings of a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.update_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#update_channel)
         """
@@ -491,30 +490,30 @@
         *,
         datasetName: str,
         actions: Sequence[DatasetActionTypeDef],
         triggers: Sequence[DatasetTriggerTypeDef] = ...,
         contentDeliveryRules: Sequence[DatasetContentDeliveryRuleTypeDef] = ...,
         retentionPeriod: RetentionPeriodTypeDef = ...,
         versioningConfiguration: VersioningConfigurationTypeDef = ...,
-        lateDataRules: Sequence[LateDataRuleTypeDef] = ...
+        lateDataRules: Sequence[LateDataRuleTypeDef] = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates the settings of a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.update_dataset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#update_dataset)
         """
 
     async def update_datastore(
         self,
         *,
         datastoreName: str,
         retentionPeriod: RetentionPeriodTypeDef = ...,
         datastoreStorage: DatastoreStorageTypeDef = ...,
-        fileFormatConfiguration: FileFormatConfigurationTypeDef = ...
+        fileFormatConfiguration: FileFormatConfigurationTypeDef = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Used to update the settings of a data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.update_datastore)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#update_datastore)
         """
```

### Comparing `types-aiobotocore-iotanalytics-2.9.0/types_aiobotocore_iotanalytics/client.pyi` & `types-aiobotocore-iotanalytics-2.9.1/types_aiobotocore_iotanalytics/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -149,15 +149,15 @@
 
     async def create_channel(
         self,
         *,
         channelName: str,
         channelStorage: ChannelStorageTypeDef = ...,
         retentionPeriod: RetentionPeriodTypeDef = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateChannelResponseTypeDef:
         """
         Used to create a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.create_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#create_channel)
         """
@@ -168,15 +168,15 @@
         datasetName: str,
         actions: Sequence[DatasetActionTypeDef],
         triggers: Sequence[DatasetTriggerTypeDef] = ...,
         contentDeliveryRules: Sequence[DatasetContentDeliveryRuleTypeDef] = ...,
         retentionPeriod: RetentionPeriodTypeDef = ...,
         versioningConfiguration: VersioningConfigurationTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
-        lateDataRules: Sequence[LateDataRuleTypeDef] = ...
+        lateDataRules: Sequence[LateDataRuleTypeDef] = ...,
     ) -> CreateDatasetResponseTypeDef:
         """
         Used to create a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.create_dataset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#create_dataset)
         """
@@ -197,29 +197,29 @@
         self,
         *,
         datastoreName: str,
         datastoreStorage: DatastoreStorageTypeDef = ...,
         retentionPeriod: RetentionPeriodTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         fileFormatConfiguration: FileFormatConfigurationTypeDef = ...,
-        datastorePartitions: DatastorePartitionsTypeDef = ...
+        datastorePartitions: DatastorePartitionsTypeDef = ...,
     ) -> CreateDatastoreResponseTypeDef:
         """
         Creates a data store, which is a repository for messages.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.create_datastore)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#create_datastore)
         """
 
     async def create_pipeline(
         self,
         *,
         pipelineName: str,
         pipelineActivities: Sequence[PipelineActivityTypeDef],
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreatePipelineResponseTypeDef:
         """
         Creates a pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.create_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#create_pipeline)
         """
@@ -347,15 +347,15 @@
     async def list_dataset_contents(
         self,
         *,
         datasetName: str,
         nextToken: str = ...,
         maxResults: int = ...,
         scheduledOnOrAfter: TimestampTypeDef = ...,
-        scheduledBefore: TimestampTypeDef = ...
+        scheduledBefore: TimestampTypeDef = ...,
     ) -> ListDatasetContentsResponseTypeDef:
         """
         Lists information about dataset contents that have been created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.list_dataset_contents)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#list_dataset_contents)
         """
@@ -422,15 +422,15 @@
 
     async def sample_channel_data(
         self,
         *,
         channelName: str,
         maxMessages: int = ...,
         startTime: TimestampTypeDef = ...,
-        endTime: TimestampTypeDef = ...
+        endTime: TimestampTypeDef = ...,
     ) -> SampleChannelDataResponseTypeDef:
         """
         Retrieves a sample of messages from the specified channel ingested during the
         specified
         timeframe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.sample_channel_data)
@@ -439,15 +439,15 @@
 
     async def start_pipeline_reprocessing(
         self,
         *,
         pipelineName: str,
         startTime: TimestampTypeDef = ...,
         endTime: TimestampTypeDef = ...,
-        channelMessages: ChannelMessagesTypeDef = ...
+        channelMessages: ChannelMessagesTypeDef = ...,
     ) -> StartPipelineReprocessingResponseTypeDef:
         """
         Starts the reprocessing of raw message data through the pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.start_pipeline_reprocessing)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#start_pipeline_reprocessing)
         """
@@ -469,15 +469,15 @@
         """
 
     async def update_channel(
         self,
         *,
         channelName: str,
         channelStorage: ChannelStorageTypeDef = ...,
-        retentionPeriod: RetentionPeriodTypeDef = ...
+        retentionPeriod: RetentionPeriodTypeDef = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Used to update the settings of a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.update_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#update_channel)
         """
@@ -487,30 +487,30 @@
         *,
         datasetName: str,
         actions: Sequence[DatasetActionTypeDef],
         triggers: Sequence[DatasetTriggerTypeDef] = ...,
         contentDeliveryRules: Sequence[DatasetContentDeliveryRuleTypeDef] = ...,
         retentionPeriod: RetentionPeriodTypeDef = ...,
         versioningConfiguration: VersioningConfigurationTypeDef = ...,
-        lateDataRules: Sequence[LateDataRuleTypeDef] = ...
+        lateDataRules: Sequence[LateDataRuleTypeDef] = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates the settings of a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.update_dataset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#update_dataset)
         """
 
     async def update_datastore(
         self,
         *,
         datastoreName: str,
         retentionPeriod: RetentionPeriodTypeDef = ...,
         datastoreStorage: DatastoreStorageTypeDef = ...,
-        fileFormatConfiguration: FileFormatConfigurationTypeDef = ...
+        fileFormatConfiguration: FileFormatConfigurationTypeDef = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Used to update the settings of a data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.update_datastore)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#update_datastore)
         """
```

### Comparing `types-aiobotocore-iotanalytics-2.9.0/types_aiobotocore_iotanalytics/literals.py` & `types-aiobotocore-iotanalytics-2.9.1/types_aiobotocore_iotanalytics/literals.py`

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
     "ChannelStatusType",
     "ComputeTypeType",
     "DatasetActionTypeType",
     "DatasetContentStateType",
     "DatasetStatusType",
     "DatastoreStatusType",
@@ -38,15 +37,14 @@
     "IoTAnalyticsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ChannelStatusType = Literal["ACTIVE", "CREATING", "DELETING"]
 ComputeTypeType = Literal["ACU_1", "ACU_2"]
 DatasetActionTypeType = Literal["CONTAINER", "QUERY"]
 DatasetContentStateType = Literal["CREATING", "FAILED", "SUCCEEDED"]
 DatasetStatusType = Literal["ACTIVE", "CREATING", "DELETING"]
 DatastoreStatusType = Literal["ACTIVE", "CREATING", "DELETING"]
 FileFormatTypeType = Literal["JSON", "PARQUET"]
```

### Comparing `types-aiobotocore-iotanalytics-2.9.0/types_aiobotocore_iotanalytics/literals.pyi` & `types-aiobotocore-iotanalytics-2.9.1/types_aiobotocore_iotanalytics/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotanalytics-2.9.0/types_aiobotocore_iotanalytics/paginator.py` & `types-aiobotocore-iotanalytics-2.9.1/types_aiobotocore_iotanalytics/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,14 @@
     "ListChannelsPaginator",
     "ListDatasetContentsPaginator",
     "ListDatasetsPaginator",
     "ListDatastoresPaginator",
     "ListPipelinesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -86,15 +85,15 @@
 
     def paginate(
         self,
         *,
         datasetName: str,
         scheduledOnOrAfter: TimestampTypeDef = ...,
         scheduledBefore: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDatasetContentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListDatasetContents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/paginators/#listdatasetcontentspaginator)
         """
```

### Comparing `types-aiobotocore-iotanalytics-2.9.0/types_aiobotocore_iotanalytics/paginator.pyi` & `types-aiobotocore-iotanalytics-2.9.1/types_aiobotocore_iotanalytics/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
     def paginate(
         self,
         *,
         datasetName: str,
         scheduledOnOrAfter: TimestampTypeDef = ...,
         scheduledBefore: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDatasetContentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListDatasetContents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/paginators/#listdatasetcontentspaginator)
         """
 
 class ListDatasetsPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-iotanalytics-2.9.0/types_aiobotocore_iotanalytics/type_defs.py` & `types-aiobotocore-iotanalytics-2.9.1/types_aiobotocore_iotanalytics/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AddAttributesActivityTypeDef",
     "BatchPutMessageErrorEntryTypeDef",
     "ResponseMetadataTypeDef",
     "BlobTypeDef",
     "CancelPipelineReprocessingRequestRequestTypeDef",
     "ChannelActivityTypeDef",
```

### Comparing `types-aiobotocore-iotanalytics-2.9.0/types_aiobotocore_iotanalytics/type_defs.pyi` & `types-aiobotocore-iotanalytics-2.9.1/types_aiobotocore_iotanalytics/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotanalytics-2.9.0/types_aiobotocore_iotanalytics.egg-info/PKG-INFO` & `types-aiobotocore-iotanalytics-2.9.1/types_aiobotocore_iotanalytics.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotanalytics
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.IoTAnalytics 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.IoTAnalytics 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/
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
 
 <a id="types-aiobotocore-iotanalytics"></a>
 
 # types-aiobotocore-iotanalytics
 
 [![PyPI - types-aiobotocore-iotanalytics](https://img.shields.io/pypi/v/types-aiobotocore-iotanalytics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotanalytics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotanalytics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotanalytics)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotanalytics)](https://pepy.tech/project/types-aiobotocore-iotanalytics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTAnalytics 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics)
+[aiobotocore.IoTAnalytics 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics)
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
 [types-aiobotocore-iotanalytics docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-iotanalytics-2.9.0/types_aiobotocore_iotanalytics.egg-info/SOURCES.txt` & `types-aiobotocore-iotanalytics-2.9.1/types_aiobotocore_iotanalytics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

