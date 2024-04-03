# Comparing `tmp/types-aiobotocore-emr-serverless-2.9.0.tar.gz` & `tmp/types-aiobotocore-emr-serverless-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-emr-serverless-2.9.0.tar", last modified: Wed Dec 13 19:59:16 2023, max compression
+gzip compressed data, was "types-aiobotocore-emr-serverless-2.9.1.tar", last modified: Thu Jan 18 01:20:41 2024, max compression
```

## Comparing `types-aiobotocore-emr-serverless-2.9.0.tar` & `types-aiobotocore-emr-serverless-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:16.809750 types-aiobotocore-emr-serverless-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:45:59.000000 types-aiobotocore-emr-serverless-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13501 2023-12-13 19:59:16.809750 types-aiobotocore-emr-serverless-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11911 2023-12-13 19:45:59.000000 types-aiobotocore-emr-serverless-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:16.809750 types-aiobotocore-emr-serverless-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2023-12-13 19:45:58.000000 types-aiobotocore-emr-serverless-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:16.809750 types-aiobotocore-emr-serverless-2.9.0/types_aiobotocore_emr_serverless/
--rw-r--r--   0 runner    (1001) docker     (127)      877 2023-12-13 19:45:59.000000 types-aiobotocore-emr-serverless-2.9.0/types_aiobotocore_emr_serverless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2023-12-13 19:45:59.000000 types-aiobotocore-emr-serverless-2.9.0/types_aiobotocore_emr_serverless/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      958 2023-12-13 19:45:59.000000 types-aiobotocore-emr-serverless-2.9.0/types_aiobotocore_emr_serverless/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15973 2023-12-13 19:45:59.000000 types-aiobotocore-emr-serverless-2.9.0/types_aiobotocore_emr_serverless/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    15969 2023-12-13 19:45:59.000000 types-aiobotocore-emr-serverless-2.9.0/types_aiobotocore_emr_serverless/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9223 2023-12-13 19:45:59.000000 types-aiobotocore-emr-serverless-2.9.0/types_aiobotocore_emr_serverless/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9221 2023-12-13 19:45:59.000000 types-aiobotocore-emr-serverless-2.9.0/types_aiobotocore_emr_serverless/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3515 2023-12-13 19:45:59.000000 types-aiobotocore-emr-serverless-2.9.0/types_aiobotocore_emr_serverless/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3511 2023-12-13 19:45:59.000000 types-aiobotocore-emr-serverless-2.9.0/types_aiobotocore_emr_serverless/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:45:59.000000 types-aiobotocore-emr-serverless-2.9.0/types_aiobotocore_emr_serverless/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    17767 2023-12-13 19:45:59.000000 types-aiobotocore-emr-serverless-2.9.0/types_aiobotocore_emr_serverless/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    17766 2023-12-13 19:45:59.000000 types-aiobotocore-emr-serverless-2.9.0/types_aiobotocore_emr_serverless/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:45:59.000000 types-aiobotocore-emr-serverless-2.9.0/types_aiobotocore_emr_serverless/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:16.809750 types-aiobotocore-emr-serverless-2.9.0/types_aiobotocore_emr_serverless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13501 2023-12-13 19:59:16.000000 types-aiobotocore-emr-serverless-2.9.0/types_aiobotocore_emr_serverless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      946 2023-12-13 19:59:16.000000 types-aiobotocore-emr-serverless-2.9.0/types_aiobotocore_emr_serverless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:16.000000 types-aiobotocore-emr-serverless-2.9.0/types_aiobotocore_emr_serverless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:16.000000 types-aiobotocore-emr-serverless-2.9.0/types_aiobotocore_emr_serverless.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:16.000000 types-aiobotocore-emr-serverless-2.9.0/types_aiobotocore_emr_serverless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-13 19:59:16.000000 types-aiobotocore-emr-serverless-2.9.0/types_aiobotocore_emr_serverless.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:41.485339 types-aiobotocore-emr-serverless-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:07:54.000000 types-aiobotocore-emr-serverless-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13521 2024-01-18 01:20:41.485339 types-aiobotocore-emr-serverless-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11911 2024-01-18 01:07:54.000000 types-aiobotocore-emr-serverless-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:41.485339 types-aiobotocore-emr-serverless-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-01-18 01:07:54.000000 types-aiobotocore-emr-serverless-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:41.481339 types-aiobotocore-emr-serverless-2.9.1/types_aiobotocore_emr_serverless/
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-01-18 01:07:54.000000 types-aiobotocore-emr-serverless-2.9.1/types_aiobotocore_emr_serverless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-01-18 01:07:54.000000 types-aiobotocore-emr-serverless-2.9.1/types_aiobotocore_emr_serverless/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-01-18 01:07:54.000000 types-aiobotocore-emr-serverless-2.9.1/types_aiobotocore_emr_serverless/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15977 2024-01-18 01:07:54.000000 types-aiobotocore-emr-serverless-2.9.1/types_aiobotocore_emr_serverless/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15974 2024-01-18 01:07:54.000000 types-aiobotocore-emr-serverless-2.9.1/types_aiobotocore_emr_serverless/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9221 2024-01-18 01:07:54.000000 types-aiobotocore-emr-serverless-2.9.1/types_aiobotocore_emr_serverless/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9221 2024-01-18 01:07:54.000000 types-aiobotocore-emr-serverless-2.9.1/types_aiobotocore_emr_serverless/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-01-18 01:07:54.000000 types-aiobotocore-emr-serverless-2.9.1/types_aiobotocore_emr_serverless/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-01-18 01:07:54.000000 types-aiobotocore-emr-serverless-2.9.1/types_aiobotocore_emr_serverless/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:07:54.000000 types-aiobotocore-emr-serverless-2.9.1/types_aiobotocore_emr_serverless/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    17766 2024-01-18 01:07:55.000000 types-aiobotocore-emr-serverless-2.9.1/types_aiobotocore_emr_serverless/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17766 2024-01-18 01:07:54.000000 types-aiobotocore-emr-serverless-2.9.1/types_aiobotocore_emr_serverless/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:07:54.000000 types-aiobotocore-emr-serverless-2.9.1/types_aiobotocore_emr_serverless/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:41.481339 types-aiobotocore-emr-serverless-2.9.1/types_aiobotocore_emr_serverless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13521 2024-01-18 01:20:41.000000 types-aiobotocore-emr-serverless-2.9.1/types_aiobotocore_emr_serverless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-01-18 01:20:41.000000 types-aiobotocore-emr-serverless-2.9.1/types_aiobotocore_emr_serverless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:41.000000 types-aiobotocore-emr-serverless-2.9.1/types_aiobotocore_emr_serverless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:41.000000 types-aiobotocore-emr-serverless-2.9.1/types_aiobotocore_emr_serverless.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:41.000000 types-aiobotocore-emr-serverless-2.9.1/types_aiobotocore_emr_serverless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-18 01:20:41.000000 types-aiobotocore-emr-serverless-2.9.1/types_aiobotocore_emr_serverless.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-emr-serverless-2.9.0/LICENSE` & `types-aiobotocore-emr-serverless-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-emr-serverless-2.9.0/PKG-INFO` & `types-aiobotocore-emr-serverless-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-emr-serverless
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.EMRServerless 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.EMRServerless 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/
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
 
 <a id="types-aiobotocore-emr-serverless"></a>
 
 # types-aiobotocore-emr-serverless
 
 [![PyPI - types-aiobotocore-emr-serverless](https://img.shields.io/pypi/v/types-aiobotocore-emr-serverless.svg?color=blue)](https://pypi.org/project/types-aiobotocore-emr-serverless)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-emr-serverless.svg?color=blue)](https://pypi.org/project/types-aiobotocore-emr-serverless)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-emr-serverless)](https://pepy.tech/project/types-aiobotocore-emr-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EMRServerless 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
+[aiobotocore.EMRServerless 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
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
 [types-aiobotocore-emr-serverless docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-emr-serverless-2.9.0/README.md` & `types-aiobotocore-emr-serverless-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-emr-serverless.svg?color=blue)](https://pypi.org/project/types-aiobotocore-emr-serverless)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-emr-serverless)](https://pepy.tech/project/types-aiobotocore-emr-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EMRServerless 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
+[aiobotocore.EMRServerless 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
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
 [types-aiobotocore-emr-serverless docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-emr-serverless-2.9.0/setup.py` & `types-aiobotocore-emr-serverless-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-emr-serverless",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_emr_serverless"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.EMRServerless 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.EMRServerless 2.9.1 service generated with"
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
     keywords="aiobotocore emr-serverless type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_emr_serverless": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-emr-serverless-2.9.0/types_aiobotocore_emr_serverless/__init__.py` & `types-aiobotocore-emr-serverless-2.9.1/types_aiobotocore_emr_serverless/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,9 +24,8 @@
 """
 
 from .client import EMRServerlessClient
 from .paginator import ListApplicationsPaginator, ListJobRunsPaginator
 
 Client = EMRServerlessClient
 
-
 __all__ = ("Client", "EMRServerlessClient", "ListApplicationsPaginator", "ListJobRunsPaginator")
```

### Comparing `types-aiobotocore-emr-serverless-2.9.0/types_aiobotocore_emr_serverless/__init__.pyi` & `types-aiobotocore-emr-serverless-2.9.1/types_aiobotocore_emr_serverless/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-serverless-2.9.0/types_aiobotocore_emr_serverless/__main__.py` & `types-aiobotocore-emr-serverless-2.9.1/types_aiobotocore_emr_serverless/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.EMRServerless 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.EMRServerless 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless\nOther"
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

### Comparing `types-aiobotocore-emr-serverless-2.9.0/types_aiobotocore_emr_serverless/client.py` & `types-aiobotocore-emr-serverless-2.9.1/types_aiobotocore_emr_serverless/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("EMRServerlessClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -130,15 +129,15 @@
         autoStartConfiguration: AutoStartConfigTypeDef = ...,
         autoStopConfiguration: AutoStopConfigTypeDef = ...,
         networkConfiguration: NetworkConfigurationTypeDef = ...,
         architecture: ArchitectureType = ...,
         imageConfiguration: ImageConfigurationInputTypeDef = ...,
         workerTypeSpecifications: Mapping[str, WorkerTypeSpecificationInputTypeDef] = ...,
         runtimeConfiguration: Sequence["ConfigurationTypeDef"] = ...,
-        monitoringConfiguration: MonitoringConfigurationTypeDef = ...
+        monitoringConfiguration: MonitoringConfigurationTypeDef = ...,
     ) -> CreateApplicationResponseTypeDef:
         """
         Creates an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.create_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/client/#create_application)
         """
@@ -194,15 +193,15 @@
         """
 
     async def list_applications(
         self,
         *,
         nextToken: str = ...,
         maxResults: int = ...,
-        states: Sequence[ApplicationStateType] = ...
+        states: Sequence[ApplicationStateType] = ...,
     ) -> ListApplicationsResponseTypeDef:
         """
         Lists applications based on a set of parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.list_applications)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/client/#list_applications)
         """
@@ -211,15 +210,15 @@
         self,
         *,
         applicationId: str,
         nextToken: str = ...,
         maxResults: int = ...,
         createdAtAfter: TimestampTypeDef = ...,
         createdAtBefore: TimestampTypeDef = ...,
-        states: Sequence[JobRunStateType] = ...
+        states: Sequence[JobRunStateType] = ...,
     ) -> ListJobRunsResponseTypeDef:
         """
         Lists job runs based on a set of parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.list_job_runs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/client/#list_job_runs)
         """
@@ -248,15 +247,15 @@
         applicationId: str,
         clientToken: str,
         executionRoleArn: str,
         jobDriver: JobDriverTypeDef = ...,
         configurationOverrides: ConfigurationOverridesTypeDef = ...,
         tags: Mapping[str, str] = ...,
         executionTimeoutMinutes: int = ...,
-        name: str = ...
+        name: str = ...,
     ) -> StartJobRunResponseTypeDef:
         """
         Starts a job run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.start_job_run)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/client/#start_job_run)
         """
@@ -296,15 +295,15 @@
         autoStopConfiguration: AutoStopConfigTypeDef = ...,
         networkConfiguration: NetworkConfigurationTypeDef = ...,
         architecture: ArchitectureType = ...,
         imageConfiguration: ImageConfigurationInputTypeDef = ...,
         workerTypeSpecifications: Mapping[str, WorkerTypeSpecificationInputTypeDef] = ...,
         releaseLabel: str = ...,
         runtimeConfiguration: Sequence["ConfigurationTypeDef"] = ...,
-        monitoringConfiguration: MonitoringConfigurationTypeDef = ...
+        monitoringConfiguration: MonitoringConfigurationTypeDef = ...,
     ) -> UpdateApplicationResponseTypeDef:
         """
         Updates a specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.update_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/client/#update_application)
         """
```

### Comparing `types-aiobotocore-emr-serverless-2.9.0/types_aiobotocore_emr_serverless/client.pyi` & `types-aiobotocore-emr-serverless-2.9.1/types_aiobotocore_emr_serverless/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -126,15 +126,15 @@
         autoStartConfiguration: AutoStartConfigTypeDef = ...,
         autoStopConfiguration: AutoStopConfigTypeDef = ...,
         networkConfiguration: NetworkConfigurationTypeDef = ...,
         architecture: ArchitectureType = ...,
         imageConfiguration: ImageConfigurationInputTypeDef = ...,
         workerTypeSpecifications: Mapping[str, WorkerTypeSpecificationInputTypeDef] = ...,
         runtimeConfiguration: Sequence["ConfigurationTypeDef"] = ...,
-        monitoringConfiguration: MonitoringConfigurationTypeDef = ...
+        monitoringConfiguration: MonitoringConfigurationTypeDef = ...,
     ) -> CreateApplicationResponseTypeDef:
         """
         Creates an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.create_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/client/#create_application)
         """
@@ -190,15 +190,15 @@
         """
 
     async def list_applications(
         self,
         *,
         nextToken: str = ...,
         maxResults: int = ...,
-        states: Sequence[ApplicationStateType] = ...
+        states: Sequence[ApplicationStateType] = ...,
     ) -> ListApplicationsResponseTypeDef:
         """
         Lists applications based on a set of parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.list_applications)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/client/#list_applications)
         """
@@ -207,15 +207,15 @@
         self,
         *,
         applicationId: str,
         nextToken: str = ...,
         maxResults: int = ...,
         createdAtAfter: TimestampTypeDef = ...,
         createdAtBefore: TimestampTypeDef = ...,
-        states: Sequence[JobRunStateType] = ...
+        states: Sequence[JobRunStateType] = ...,
     ) -> ListJobRunsResponseTypeDef:
         """
         Lists job runs based on a set of parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.list_job_runs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/client/#list_job_runs)
         """
@@ -244,15 +244,15 @@
         applicationId: str,
         clientToken: str,
         executionRoleArn: str,
         jobDriver: JobDriverTypeDef = ...,
         configurationOverrides: ConfigurationOverridesTypeDef = ...,
         tags: Mapping[str, str] = ...,
         executionTimeoutMinutes: int = ...,
-        name: str = ...
+        name: str = ...,
     ) -> StartJobRunResponseTypeDef:
         """
         Starts a job run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.start_job_run)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/client/#start_job_run)
         """
@@ -292,15 +292,15 @@
         autoStopConfiguration: AutoStopConfigTypeDef = ...,
         networkConfiguration: NetworkConfigurationTypeDef = ...,
         architecture: ArchitectureType = ...,
         imageConfiguration: ImageConfigurationInputTypeDef = ...,
         workerTypeSpecifications: Mapping[str, WorkerTypeSpecificationInputTypeDef] = ...,
         releaseLabel: str = ...,
         runtimeConfiguration: Sequence["ConfigurationTypeDef"] = ...,
-        monitoringConfiguration: MonitoringConfigurationTypeDef = ...
+        monitoringConfiguration: MonitoringConfigurationTypeDef = ...,
     ) -> UpdateApplicationResponseTypeDef:
         """
         Updates a specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.update_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/client/#update_application)
         """
```

### Comparing `types-aiobotocore-emr-serverless-2.9.0/types_aiobotocore_emr_serverless/literals.py` & `types-aiobotocore-emr-serverless-2.9.1/types_aiobotocore_emr_serverless/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,29 +15,27 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ApplicationStateType",
     "ArchitectureType",
     "JobRunStateType",
     "ListApplicationsPaginatorName",
     "ListJobRunsPaginatorName",
     "EMRServerlessServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ApplicationStateType = Literal[
     "CREATED", "CREATING", "STARTED", "STARTING", "STOPPED", "STOPPING", "TERMINATED"
 ]
 ArchitectureType = Literal["ARM64", "X86_64"]
 JobRunStateType = Literal[
     "CANCELLED", "CANCELLING", "FAILED", "PENDING", "RUNNING", "SCHEDULED", "SUBMITTED", "SUCCESS"
 ]
```

### Comparing `types-aiobotocore-emr-serverless-2.9.0/types_aiobotocore_emr_serverless/literals.pyi` & `types-aiobotocore-emr-serverless-2.9.1/types_aiobotocore_emr_serverless/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-serverless-2.9.0/types_aiobotocore_emr_serverless/paginator.py` & `types-aiobotocore-emr-serverless-2.9.1/types_aiobotocore_emr_serverless/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,14 @@
     ListJobRunsResponseTypeDef,
     PaginatorConfigTypeDef,
     TimestampTypeDef,
 )
 
 __all__ = ("ListApplicationsPaginator", "ListJobRunsPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -55,15 +54,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/paginators/#listapplicationspaginator)
     """
 
     def paginate(
         self,
         *,
         states: Sequence[ApplicationStateType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Paginator.ListApplications.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/paginators/#listapplicationspaginator)
         """
 
 
@@ -76,13 +75,13 @@
     def paginate(
         self,
         *,
         applicationId: str,
         createdAtAfter: TimestampTypeDef = ...,
         createdAtBefore: TimestampTypeDef = ...,
         states: Sequence[JobRunStateType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListJobRunsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Paginator.ListJobRuns.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/paginators/#listjobrunspaginator)
         """
```

### Comparing `types-aiobotocore-emr-serverless-2.9.0/types_aiobotocore_emr_serverless/paginator.pyi` & `types-aiobotocore-emr-serverless-2.9.1/types_aiobotocore_emr_serverless/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/paginators/#listapplicationspaginator)
     """
 
     def paginate(
         self,
         *,
         states: Sequence[ApplicationStateType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Paginator.ListApplications.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/paginators/#listapplicationspaginator)
         """
 
 class ListJobRunsPaginator(AioPaginator):
@@ -72,13 +72,13 @@
     def paginate(
         self,
         *,
         applicationId: str,
         createdAtAfter: TimestampTypeDef = ...,
         createdAtBefore: TimestampTypeDef = ...,
         states: Sequence[JobRunStateType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListJobRunsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Paginator.ListJobRuns.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/paginators/#listjobrunspaginator)
         """
```

### Comparing `types-aiobotocore-emr-serverless-2.9.0/types_aiobotocore_emr_serverless/type_defs.py` & `types-aiobotocore-emr-serverless-2.9.1/types_aiobotocore_emr_serverless/type_defs.py`

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
     "ApplicationSummaryTypeDef",
     "AutoStartConfigTypeDef",
     "AutoStopConfigTypeDef",
     "ImageConfigurationTypeDef",
     "MaximumAllowedResourcesTypeDef",
     "NetworkConfigurationTypeDef",
```

### Comparing `types-aiobotocore-emr-serverless-2.9.0/types_aiobotocore_emr_serverless/type_defs.pyi` & `types-aiobotocore-emr-serverless-2.9.1/types_aiobotocore_emr_serverless/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-serverless-2.9.0/types_aiobotocore_emr_serverless.egg-info/PKG-INFO` & `types-aiobotocore-emr-serverless-2.9.1/types_aiobotocore_emr_serverless.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-emr-serverless
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.EMRServerless 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.EMRServerless 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/
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
 
 <a id="types-aiobotocore-emr-serverless"></a>
 
 # types-aiobotocore-emr-serverless
 
 [![PyPI - types-aiobotocore-emr-serverless](https://img.shields.io/pypi/v/types-aiobotocore-emr-serverless.svg?color=blue)](https://pypi.org/project/types-aiobotocore-emr-serverless)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-emr-serverless.svg?color=blue)](https://pypi.org/project/types-aiobotocore-emr-serverless)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-emr-serverless)](https://pepy.tech/project/types-aiobotocore-emr-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EMRServerless 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
+[aiobotocore.EMRServerless 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
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
 [types-aiobotocore-emr-serverless docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-emr-serverless-2.9.0/types_aiobotocore_emr_serverless.egg-info/SOURCES.txt` & `types-aiobotocore-emr-serverless-2.9.1/types_aiobotocore_emr_serverless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

