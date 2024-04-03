# Comparing `tmp/types-aiobotocore-iam-2.9.0.tar.gz` & `tmp/types-aiobotocore-iam-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iam-2.9.0.tar", last modified: Wed Dec 13 19:59:26 2023, max compression
+gzip compressed data, was "types-aiobotocore-iam-2.9.1.tar", last modified: Thu Jan 18 01:20:50 2024, max compression
```

## Comparing `types-aiobotocore-iam-2.9.0.tar` & `types-aiobotocore-iam-2.9.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:26.921699 types-aiobotocore-iam-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:47:16.000000 types-aiobotocore-iam-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    23551 2023-12-13 19:59:26.921699 types-aiobotocore-iam-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22004 2023-12-13 19:47:16.000000 types-aiobotocore-iam-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:26.921699 types-aiobotocore-iam-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2023-12-13 19:47:16.000000 types-aiobotocore-iam-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:26.921699 types-aiobotocore-iam-2.9.0/types_aiobotocore_iam/
--rw-r--r--   0 runner    (1001) docker     (127)     8795 2023-12-13 19:47:16.000000 types-aiobotocore-iam-2.9.0/types_aiobotocore_iam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8793 2023-12-13 19:47:16.000000 types-aiobotocore-iam-2.9.0/types_aiobotocore_iam/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      905 2023-12-13 19:47:16.000000 types-aiobotocore-iam-2.9.0/types_aiobotocore_iam/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)   119388 2023-12-13 19:47:16.000000 types-aiobotocore-iam-2.9.0/types_aiobotocore_iam/client.py
--rw-r--r--   0 runner    (1001) docker     (127)   119384 2023-12-13 19:47:16.000000 types-aiobotocore-iam-2.9.0/types_aiobotocore_iam/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    16113 2023-12-13 19:47:19.000000 types-aiobotocore-iam-2.9.0/types_aiobotocore_iam/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    16111 2023-12-13 19:47:19.000000 types-aiobotocore-iam-2.9.0/types_aiobotocore_iam/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    40085 2023-12-13 19:47:19.000000 types-aiobotocore-iam-2.9.0/types_aiobotocore_iam/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    40049 2023-12-13 19:47:19.000000 types-aiobotocore-iam-2.9.0/types_aiobotocore_iam/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:47:16.000000 types-aiobotocore-iam-2.9.0/types_aiobotocore_iam/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   155187 2023-12-13 19:47:19.000000 types-aiobotocore-iam-2.9.0/types_aiobotocore_iam/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)   155111 2023-12-13 19:47:17.000000 types-aiobotocore-iam-2.9.0/types_aiobotocore_iam/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (127)   112224 2023-12-13 19:47:21.000000 types-aiobotocore-iam-2.9.0/types_aiobotocore_iam/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   112223 2023-12-13 19:47:20.000000 types-aiobotocore-iam-2.9.0/types_aiobotocore_iam/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:47:16.000000 types-aiobotocore-iam-2.9.0/types_aiobotocore_iam/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4213 2023-12-13 19:47:19.000000 types-aiobotocore-iam-2.9.0/types_aiobotocore_iam/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4209 2023-12-13 19:47:19.000000 types-aiobotocore-iam-2.9.0/types_aiobotocore_iam/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:26.921699 types-aiobotocore-iam-2.9.0/types_aiobotocore_iam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    23551 2023-12-13 19:59:26.000000 types-aiobotocore-iam-2.9.0/types_aiobotocore_iam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      887 2023-12-13 19:59:26.000000 types-aiobotocore-iam-2.9.0/types_aiobotocore_iam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:26.000000 types-aiobotocore-iam-2.9.0/types_aiobotocore_iam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:26.000000 types-aiobotocore-iam-2.9.0/types_aiobotocore_iam.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:26.000000 types-aiobotocore-iam-2.9.0/types_aiobotocore_iam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-13 19:59:26.000000 types-aiobotocore-iam-2.9.0/types_aiobotocore_iam.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:50.801296 types-aiobotocore-iam-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:09:06.000000 types-aiobotocore-iam-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    23571 2024-01-18 01:20:50.801296 types-aiobotocore-iam-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22004 2024-01-18 01:09:06.000000 types-aiobotocore-iam-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:50.801296 types-aiobotocore-iam-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-01-18 01:09:06.000000 types-aiobotocore-iam-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:50.801296 types-aiobotocore-iam-2.9.1/types_aiobotocore_iam/
+-rw-r--r--   0 runner    (1001) docker     (127)     8793 2024-01-18 01:09:06.000000 types-aiobotocore-iam-2.9.1/types_aiobotocore_iam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8793 2024-01-18 01:09:06.000000 types-aiobotocore-iam-2.9.1/types_aiobotocore_iam/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-01-18 01:09:06.000000 types-aiobotocore-iam-2.9.1/types_aiobotocore_iam/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   119400 2024-01-18 01:09:08.000000 types-aiobotocore-iam-2.9.1/types_aiobotocore_iam/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   119397 2024-01-18 01:09:08.000000 types-aiobotocore-iam-2.9.1/types_aiobotocore_iam/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    16111 2024-01-18 01:09:10.000000 types-aiobotocore-iam-2.9.1/types_aiobotocore_iam/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16111 2024-01-18 01:09:10.000000 types-aiobotocore-iam-2.9.1/types_aiobotocore_iam/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    40093 2024-01-18 01:09:10.000000 types-aiobotocore-iam-2.9.1/types_aiobotocore_iam/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40058 2024-01-18 01:09:10.000000 types-aiobotocore-iam-2.9.1/types_aiobotocore_iam/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:09:06.000000 types-aiobotocore-iam-2.9.1/types_aiobotocore_iam/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   156106 2024-01-18 01:09:09.000000 types-aiobotocore-iam-2.9.1/types_aiobotocore_iam/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)   156035 2024-01-18 01:09:09.000000 types-aiobotocore-iam-2.9.1/types_aiobotocore_iam/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)   112223 2024-01-18 01:09:13.000000 types-aiobotocore-iam-2.9.1/types_aiobotocore_iam/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   112223 2024-01-18 01:09:13.000000 types-aiobotocore-iam-2.9.1/types_aiobotocore_iam/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:09:06.000000 types-aiobotocore-iam-2.9.1/types_aiobotocore_iam/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4213 2024-01-18 01:09:10.000000 types-aiobotocore-iam-2.9.1/types_aiobotocore_iam/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-01-18 01:09:10.000000 types-aiobotocore-iam-2.9.1/types_aiobotocore_iam/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:50.801296 types-aiobotocore-iam-2.9.1/types_aiobotocore_iam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    23571 2024-01-18 01:20:50.000000 types-aiobotocore-iam-2.9.1/types_aiobotocore_iam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-01-18 01:20:50.000000 types-aiobotocore-iam-2.9.1/types_aiobotocore_iam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:50.000000 types-aiobotocore-iam-2.9.1/types_aiobotocore_iam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:50.000000 types-aiobotocore-iam-2.9.1/types_aiobotocore_iam.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:50.000000 types-aiobotocore-iam-2.9.1/types_aiobotocore_iam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-18 01:20:50.000000 types-aiobotocore-iam-2.9.1/types_aiobotocore_iam.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iam-2.9.0/LICENSE` & `types-aiobotocore-iam-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-iam-2.9.0/PKG-INFO` & `types-aiobotocore-iam-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iam
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.IAM 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.IAM 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/
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
 
 <a id="types-aiobotocore-iam"></a>
 
 # types-aiobotocore-iam
 
 [![PyPI - types-aiobotocore-iam](https://img.shields.io/pypi/v/types-aiobotocore-iam.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iam)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iam.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iam)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iam)](https://pepy.tech/project/types-aiobotocore-iam)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IAM 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM)
+[aiobotocore.IAM 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM)
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
 [types-aiobotocore-iam docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-iam-2.9.0/README.md` & `types-aiobotocore-iam-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iam.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iam)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iam)](https://pepy.tech/project/types-aiobotocore-iam)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IAM 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM)
+[aiobotocore.IAM 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM)
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
 [types-aiobotocore-iam docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-iam-2.9.0/setup.py` & `types-aiobotocore-iam-2.9.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iam",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_iam"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.IAM 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.IAM 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore iam type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_iam": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-iam-2.9.0/types_aiobotocore_iam/__init__.py` & `types-aiobotocore-iam-2.9.1/types_aiobotocore_iam/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,18 +141,16 @@
     PolicyExistsWaiter,
     RoleExistsWaiter,
     UserExistsWaiter,
 )
 
 Client = IAMClient
 
-
 ServiceResource = IAMServiceResource
 
-
 __all__ = (
     "Client",
     "GetAccountAuthorizationDetailsPaginator",
     "GetGroupPaginator",
     "IAMClient",
     "IAMServiceResource",
     "InstanceProfileExistsWaiter",
```

### Comparing `types-aiobotocore-iam-2.9.0/types_aiobotocore_iam/__init__.pyi` & `types-aiobotocore-iam-2.9.1/types_aiobotocore_iam/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iam-2.9.0/types_aiobotocore_iam/__main__.py` & `types-aiobotocore-iam-2.9.1/types_aiobotocore_iam/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IAM 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.IAM 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM\nOther"
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

### Comparing `types-aiobotocore-iam-2.9.0/types_aiobotocore_iam/client.py` & `types-aiobotocore-iam-2.9.1/types_aiobotocore_iam/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,15 +164,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("IAMClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -364,15 +363,15 @@
 
     async def create_open_id_connect_provider(
         self,
         *,
         Url: str,
         ThumbprintList: Sequence[str],
         ClientIDList: Sequence[str] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateOpenIDConnectProviderResponseTypeDef:
         """
         Creates an IAM entity to describe an identity provider (IdP) that supports
         `OpenID Connect (OIDC)
         <http://openid.net/connect/>`__.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_open_id_connect_provider)
@@ -382,15 +381,15 @@
     async def create_policy(
         self,
         *,
         PolicyName: str,
         PolicyDocument: str,
         Path: str = ...,
         Description: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreatePolicyResponseTypeDef:
         """
         Creates a new managed policy for your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/client/#create_policy)
         """
@@ -410,15 +409,15 @@
         *,
         RoleName: str,
         AssumeRolePolicyDocument: str,
         Path: str = ...,
         Description: str = ...,
         MaxSessionDuration: int = ...,
         PermissionsBoundary: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateRoleResponseTypeDef:
         """
         Creates a new role for your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_role)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/client/#create_role)
         """
@@ -459,15 +458,15 @@
 
     async def create_user(
         self,
         *,
         UserName: str,
         Path: str = ...,
         PermissionsBoundary: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateUserResponseTypeDef:
         """
         Creates a new IAM user for your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/client/#create_user)
         """
@@ -742,15 +741,15 @@
 
     async def enable_mfa_device(
         self,
         *,
         UserName: str,
         SerialNumber: str,
         AuthenticationCode1: str,
-        AuthenticationCode2: str
+        AuthenticationCode2: str,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Enables the specified MFA device and associates it with the specified IAM user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.enable_mfa_device)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/client/#enable_mfa_device)
         """
@@ -1135,15 +1134,15 @@
         self,
         *,
         PolicyArn: str,
         EntityFilter: EntityTypeType = ...,
         PathPrefix: str = ...,
         PolicyUsageFilter: PolicyUsageTypeType = ...,
         Marker: str = ...,
-        MaxItems: int = ...
+        MaxItems: int = ...,
     ) -> ListEntitiesForPolicyResponseTypeDef:
         """
         Lists all IAM users, groups, and roles that the specified managed policy is
         attached
         to.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_entities_for_policy)
@@ -1259,15 +1258,15 @@
         self,
         *,
         Scope: policyScopeTypeType = ...,
         OnlyAttached: bool = ...,
         PathPrefix: str = ...,
         PolicyUsageFilter: PolicyUsageTypeType = ...,
         Marker: str = ...,
-        MaxItems: int = ...
+        MaxItems: int = ...,
     ) -> ListPoliciesResponseTypeDef:
         """
         Lists all the managed policies that are available in your Amazon Web Services
         account, including your own customer-defined managed policies and all Amazon
         Web Services managed
         policies.
 
@@ -1446,15 +1445,15 @@
         """
 
     async def list_virtual_mfa_devices(
         self,
         *,
         AssignmentStatus: assignmentStatusTypeType = ...,
         Marker: str = ...,
-        MaxItems: int = ...
+        MaxItems: int = ...,
     ) -> ListVirtualMFADevicesResponseTypeDef:
         """
         Lists the virtual MFA devices defined in the Amazon Web Services account by
         assignment
         status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_virtual_mfa_devices)
@@ -1561,15 +1560,15 @@
 
     async def resync_mfa_device(
         self,
         *,
         UserName: str,
         SerialNumber: str,
         AuthenticationCode1: str,
-        AuthenticationCode2: str
+        AuthenticationCode2: str,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Synchronizes the specified MFA device with its IAM resource object on the
         Amazon Web Services
         servers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.resync_mfa_device)
@@ -1609,15 +1608,15 @@
         ResourceArns: Sequence[str] = ...,
         ResourcePolicy: str = ...,
         ResourceOwner: str = ...,
         CallerArn: str = ...,
         ContextEntries: Sequence[ContextEntryTypeDef] = ...,
         ResourceHandlingOption: str = ...,
         MaxItems: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> SimulatePolicyResponseTypeDef:
         """
         Simulate how a set of IAM policies and optionally a resource-based policy works
         with a list of API operations and Amazon Web Services resources to determine
         the policies' effective
         permissions.
 
@@ -1635,15 +1634,15 @@
         ResourceArns: Sequence[str] = ...,
         ResourcePolicy: str = ...,
         ResourceOwner: str = ...,
         CallerArn: str = ...,
         ContextEntries: Sequence[ContextEntryTypeDef] = ...,
         ResourceHandlingOption: str = ...,
         MaxItems: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> SimulatePolicyResponseTypeDef:
         """
         Simulate how a set of IAM policies attached to an IAM entity works with a list
         of API operations and Amazon Web Services resources to determine the policies'
         effective
         permissions.
 
@@ -1837,15 +1836,15 @@
         RequireSymbols: bool = ...,
         RequireNumbers: bool = ...,
         RequireUppercaseCharacters: bool = ...,
         RequireLowercaseCharacters: bool = ...,
         AllowUsersToChangePassword: bool = ...,
         MaxPasswordAge: int = ...,
         PasswordReusePrevention: int = ...,
-        HardExpiry: bool = ...
+        HardExpiry: bool = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates the password policy settings for the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.update_account_password_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/client/#update_account_password_policy)
         """
@@ -1979,15 +1978,15 @@
         self,
         *,
         ServerCertificateName: str,
         CertificateBody: str,
         PrivateKey: str,
         Path: str = ...,
         CertificateChain: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> UploadServerCertificateResponseTypeDef:
         """
         Uploads a server certificate entity for the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.upload_server_certificate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/client/#upload_server_certificate)
         """
```

### Comparing `types-aiobotocore-iam-2.9.0/types_aiobotocore_iam/client.pyi` & `types-aiobotocore-iam-2.9.1/types_aiobotocore_iam/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -360,15 +360,15 @@
 
     async def create_open_id_connect_provider(
         self,
         *,
         Url: str,
         ThumbprintList: Sequence[str],
         ClientIDList: Sequence[str] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateOpenIDConnectProviderResponseTypeDef:
         """
         Creates an IAM entity to describe an identity provider (IdP) that supports
         `OpenID Connect (OIDC)
         <http://openid.net/connect/>`__.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_open_id_connect_provider)
@@ -378,15 +378,15 @@
     async def create_policy(
         self,
         *,
         PolicyName: str,
         PolicyDocument: str,
         Path: str = ...,
         Description: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreatePolicyResponseTypeDef:
         """
         Creates a new managed policy for your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/client/#create_policy)
         """
@@ -406,15 +406,15 @@
         *,
         RoleName: str,
         AssumeRolePolicyDocument: str,
         Path: str = ...,
         Description: str = ...,
         MaxSessionDuration: int = ...,
         PermissionsBoundary: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateRoleResponseTypeDef:
         """
         Creates a new role for your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_role)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/client/#create_role)
         """
@@ -455,15 +455,15 @@
 
     async def create_user(
         self,
         *,
         UserName: str,
         Path: str = ...,
         PermissionsBoundary: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateUserResponseTypeDef:
         """
         Creates a new IAM user for your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/client/#create_user)
         """
@@ -738,15 +738,15 @@
 
     async def enable_mfa_device(
         self,
         *,
         UserName: str,
         SerialNumber: str,
         AuthenticationCode1: str,
-        AuthenticationCode2: str
+        AuthenticationCode2: str,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Enables the specified MFA device and associates it with the specified IAM user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.enable_mfa_device)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/client/#enable_mfa_device)
         """
@@ -1131,15 +1131,15 @@
         self,
         *,
         PolicyArn: str,
         EntityFilter: EntityTypeType = ...,
         PathPrefix: str = ...,
         PolicyUsageFilter: PolicyUsageTypeType = ...,
         Marker: str = ...,
-        MaxItems: int = ...
+        MaxItems: int = ...,
     ) -> ListEntitiesForPolicyResponseTypeDef:
         """
         Lists all IAM users, groups, and roles that the specified managed policy is
         attached
         to.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_entities_for_policy)
@@ -1255,15 +1255,15 @@
         self,
         *,
         Scope: policyScopeTypeType = ...,
         OnlyAttached: bool = ...,
         PathPrefix: str = ...,
         PolicyUsageFilter: PolicyUsageTypeType = ...,
         Marker: str = ...,
-        MaxItems: int = ...
+        MaxItems: int = ...,
     ) -> ListPoliciesResponseTypeDef:
         """
         Lists all the managed policies that are available in your Amazon Web Services
         account, including your own customer-defined managed policies and all Amazon
         Web Services managed
         policies.
 
@@ -1442,15 +1442,15 @@
         """
 
     async def list_virtual_mfa_devices(
         self,
         *,
         AssignmentStatus: assignmentStatusTypeType = ...,
         Marker: str = ...,
-        MaxItems: int = ...
+        MaxItems: int = ...,
     ) -> ListVirtualMFADevicesResponseTypeDef:
         """
         Lists the virtual MFA devices defined in the Amazon Web Services account by
         assignment
         status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_virtual_mfa_devices)
@@ -1557,15 +1557,15 @@
 
     async def resync_mfa_device(
         self,
         *,
         UserName: str,
         SerialNumber: str,
         AuthenticationCode1: str,
-        AuthenticationCode2: str
+        AuthenticationCode2: str,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Synchronizes the specified MFA device with its IAM resource object on the
         Amazon Web Services
         servers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.resync_mfa_device)
@@ -1605,15 +1605,15 @@
         ResourceArns: Sequence[str] = ...,
         ResourcePolicy: str = ...,
         ResourceOwner: str = ...,
         CallerArn: str = ...,
         ContextEntries: Sequence[ContextEntryTypeDef] = ...,
         ResourceHandlingOption: str = ...,
         MaxItems: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> SimulatePolicyResponseTypeDef:
         """
         Simulate how a set of IAM policies and optionally a resource-based policy works
         with a list of API operations and Amazon Web Services resources to determine
         the policies' effective
         permissions.
 
@@ -1631,15 +1631,15 @@
         ResourceArns: Sequence[str] = ...,
         ResourcePolicy: str = ...,
         ResourceOwner: str = ...,
         CallerArn: str = ...,
         ContextEntries: Sequence[ContextEntryTypeDef] = ...,
         ResourceHandlingOption: str = ...,
         MaxItems: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> SimulatePolicyResponseTypeDef:
         """
         Simulate how a set of IAM policies attached to an IAM entity works with a list
         of API operations and Amazon Web Services resources to determine the policies'
         effective
         permissions.
 
@@ -1833,15 +1833,15 @@
         RequireSymbols: bool = ...,
         RequireNumbers: bool = ...,
         RequireUppercaseCharacters: bool = ...,
         RequireLowercaseCharacters: bool = ...,
         AllowUsersToChangePassword: bool = ...,
         MaxPasswordAge: int = ...,
         PasswordReusePrevention: int = ...,
-        HardExpiry: bool = ...
+        HardExpiry: bool = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates the password policy settings for the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.update_account_password_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/client/#update_account_password_policy)
         """
@@ -1975,15 +1975,15 @@
         self,
         *,
         ServerCertificateName: str,
         CertificateBody: str,
         PrivateKey: str,
         Path: str = ...,
         CertificateChain: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> UploadServerCertificateResponseTypeDef:
         """
         Uploads a server certificate entity for the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.upload_server_certificate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/client/#upload_server_certificate)
         """
```

### Comparing `types-aiobotocore-iam-2.9.0/types_aiobotocore_iam/literals.py` & `types-aiobotocore-iam-2.9.1/types_aiobotocore_iam/literals.py`

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
     "AccessAdvisorUsageGranularityTypeType",
     "ContextKeyTypeEnumType",
     "DeletionTaskStatusTypeType",
     "EntityTypeType",
     "GetAccountAuthorizationDetailsPaginatorName",
     "GetGroupPaginatorName",
@@ -82,15 +81,14 @@
     "IAMServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
 )
 
-
 AccessAdvisorUsageGranularityTypeType = Literal["ACTION_LEVEL", "SERVICE_LEVEL"]
 ContextKeyTypeEnumType = Literal[
     "binary",
     "binaryList",
     "boolean",
     "booleanList",
     "date",
```

### Comparing `types-aiobotocore-iam-2.9.0/types_aiobotocore_iam/literals.pyi` & `types-aiobotocore-iam-2.9.1/types_aiobotocore_iam/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iam-2.9.0/types_aiobotocore_iam/paginator.py` & `types-aiobotocore-iam-2.9.1/types_aiobotocore_iam/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,14 @@
     "ListUserTagsPaginator",
     "ListUsersPaginator",
     "ListVirtualMFADevicesPaginator",
     "SimulateCustomPolicyPaginator",
     "SimulatePrincipalPolicyPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -190,15 +189,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#getaccountauthorizationdetailspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: Sequence[EntityTypeType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetAccountAuthorizationDetailsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.GetAccountAuthorizationDetails.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#getaccountauthorizationdetailspaginator)
         """
 
 
@@ -254,15 +253,15 @@
     """
 
     def paginate(
         self,
         *,
         GroupName: str,
         PathPrefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAttachedGroupPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAttachedGroupPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listattachedgrouppoliciespaginator)
         """
 
 
@@ -273,15 +272,15 @@
     """
 
     def paginate(
         self,
         *,
         RoleName: str,
         PathPrefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAttachedRolePoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAttachedRolePolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listattachedrolepoliciespaginator)
         """
 
 
@@ -292,15 +291,15 @@
     """
 
     def paginate(
         self,
         *,
         UserName: str,
         PathPrefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAttachedUserPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAttachedUserPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listattacheduserpoliciespaginator)
         """
 
 
@@ -313,15 +312,15 @@
     def paginate(
         self,
         *,
         PolicyArn: str,
         EntityFilter: EntityTypeType = ...,
         PathPrefix: str = ...,
         PolicyUsageFilter: PolicyUsageTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEntitiesForPolicyResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListEntitiesForPolicy.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listentitiesforpolicypaginator)
         """
 
 
@@ -469,15 +468,15 @@
     def paginate(
         self,
         *,
         Scope: policyScopeTypeType = ...,
         OnlyAttached: bool = ...,
         PathPrefix: str = ...,
         PolicyUsageFilter: PolicyUsageTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listpoliciespaginator)
         """
 
 
@@ -682,15 +681,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listvirtualmfadevicespaginator)
     """
 
     def paginate(
         self,
         *,
         AssignmentStatus: assignmentStatusTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListVirtualMFADevicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListVirtualMFADevices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listvirtualmfadevicespaginator)
         """
 
 
@@ -708,15 +707,15 @@
         PermissionsBoundaryPolicyInputList: Sequence[str] = ...,
         ResourceArns: Sequence[str] = ...,
         ResourcePolicy: str = ...,
         ResourceOwner: str = ...,
         CallerArn: str = ...,
         ContextEntries: Sequence[ContextEntryTypeDef] = ...,
         ResourceHandlingOption: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SimulatePolicyResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.SimulateCustomPolicy.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#simulatecustompolicypaginator)
         """
 
 
@@ -735,13 +734,13 @@
         PermissionsBoundaryPolicyInputList: Sequence[str] = ...,
         ResourceArns: Sequence[str] = ...,
         ResourcePolicy: str = ...,
         ResourceOwner: str = ...,
         CallerArn: str = ...,
         ContextEntries: Sequence[ContextEntryTypeDef] = ...,
         ResourceHandlingOption: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SimulatePolicyResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.SimulatePrincipalPolicy.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#simulateprincipalpolicypaginator)
         """
```

### Comparing `types-aiobotocore-iam-2.9.0/types_aiobotocore_iam/paginator.pyi` & `types-aiobotocore-iam-2.9.1/types_aiobotocore_iam/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -187,15 +187,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#getaccountauthorizationdetailspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: Sequence[EntityTypeType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetAccountAuthorizationDetailsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.GetAccountAuthorizationDetails.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#getaccountauthorizationdetailspaginator)
         """
 
 class GetGroupPaginator(AioPaginator):
@@ -247,15 +247,15 @@
     """
 
     def paginate(
         self,
         *,
         GroupName: str,
         PathPrefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAttachedGroupPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAttachedGroupPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listattachedgrouppoliciespaginator)
         """
 
 class ListAttachedRolePoliciesPaginator(AioPaginator):
@@ -265,15 +265,15 @@
     """
 
     def paginate(
         self,
         *,
         RoleName: str,
         PathPrefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAttachedRolePoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAttachedRolePolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listattachedrolepoliciespaginator)
         """
 
 class ListAttachedUserPoliciesPaginator(AioPaginator):
@@ -283,15 +283,15 @@
     """
 
     def paginate(
         self,
         *,
         UserName: str,
         PathPrefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAttachedUserPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAttachedUserPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listattacheduserpoliciespaginator)
         """
 
 class ListEntitiesForPolicyPaginator(AioPaginator):
@@ -303,15 +303,15 @@
     def paginate(
         self,
         *,
         PolicyArn: str,
         EntityFilter: EntityTypeType = ...,
         PathPrefix: str = ...,
         PolicyUsageFilter: PolicyUsageTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEntitiesForPolicyResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListEntitiesForPolicy.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listentitiesforpolicypaginator)
         """
 
 class ListGroupPoliciesPaginator(AioPaginator):
@@ -449,15 +449,15 @@
     def paginate(
         self,
         *,
         Scope: policyScopeTypeType = ...,
         OnlyAttached: bool = ...,
         PathPrefix: str = ...,
         PolicyUsageFilter: PolicyUsageTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listpoliciespaginator)
         """
 
 class ListPolicyTagsPaginator(AioPaginator):
@@ -648,15 +648,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listvirtualmfadevicespaginator)
     """
 
     def paginate(
         self,
         *,
         AssignmentStatus: assignmentStatusTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListVirtualMFADevicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListVirtualMFADevices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listvirtualmfadevicespaginator)
         """
 
 class SimulateCustomPolicyPaginator(AioPaginator):
@@ -673,15 +673,15 @@
         PermissionsBoundaryPolicyInputList: Sequence[str] = ...,
         ResourceArns: Sequence[str] = ...,
         ResourcePolicy: str = ...,
         ResourceOwner: str = ...,
         CallerArn: str = ...,
         ContextEntries: Sequence[ContextEntryTypeDef] = ...,
         ResourceHandlingOption: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SimulatePolicyResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.SimulateCustomPolicy.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#simulatecustompolicypaginator)
         """
 
 class SimulatePrincipalPolicyPaginator(AioPaginator):
@@ -699,13 +699,13 @@
         PermissionsBoundaryPolicyInputList: Sequence[str] = ...,
         ResourceArns: Sequence[str] = ...,
         ResourcePolicy: str = ...,
         ResourceOwner: str = ...,
         CallerArn: str = ...,
         ContextEntries: Sequence[ContextEntryTypeDef] = ...,
         ResourceHandlingOption: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SimulatePolicyResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.SimulatePrincipalPolicy.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#simulateprincipalpolicypaginator)
         """
```

### Comparing `types-aiobotocore-iam-2.9.0/types_aiobotocore_iam/service_resource.py` & `types-aiobotocore-iam-2.9.1/types_aiobotocore_iam/service_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,14 @@
 except ImportError:
     from builtins import object as AIOResourceCollection
 try:
     from boto3.resources.base import ResourceMeta
 except ImportError:
     from builtins import object as ResourceMeta
 
-
 __all__ = (
     "IAMServiceResource",
     "AccessKey",
     "AccessKeyPair",
     "AccountPasswordPolicy",
     "AccountSummary",
     "AssumeRolePolicy",
@@ -278,15 +277,15 @@
         self,
         *,
         Scope: policyScopeTypeType = ...,
         OnlyAttached: bool = ...,
         PathPrefix: str = ...,
         PolicyUsageFilter: PolicyUsageTypeType = ...,
         Marker: str = ...,
-        MaxItems: int = ...
+        MaxItems: int = ...,
     ) -> "ServiceResourcePoliciesCollection":
         """
         Get items from the collection, passing keyword arguments along as parameters to the underlying service operation, which are typically used to filter the results.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.policies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#serviceresourcepoliciescollection)
         """
@@ -605,15 +604,15 @@
         """
 
     def filter(  # type: ignore
         self,
         *,
         AssignmentStatus: assignmentStatusTypeType = ...,
         Marker: str = ...,
-        MaxItems: int = ...
+        MaxItems: int = ...,
     ) -> "ServiceResourceVirtualMfaDevicesCollection":
         """
         Get items from the collection, passing keyword arguments along as parameters to the underlying service operation, which are typically used to filter the results.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.virtual_mfa_devices)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#serviceresourcevirtualmfadevicescollection)
         """
@@ -902,15 +901,15 @@
     def filter(  # type: ignore
         self,
         *,
         EntityFilter: EntityTypeType = ...,
         PathPrefix: str = ...,
         PolicyUsageFilter: PolicyUsageTypeType = ...,
         Marker: str = ...,
-        MaxItems: int = ...
+        MaxItems: int = ...,
     ) -> "PolicyAttachedGroupsCollection":
         """
         Get items from the collection, passing keyword arguments along as parameters to the underlying service operation, which are typically used to filter the results.
         """
 
     def limit(self, count: int) -> "PolicyAttachedGroupsCollection":
         """
@@ -947,15 +946,15 @@
     def filter(  # type: ignore
         self,
         *,
         EntityFilter: EntityTypeType = ...,
         PathPrefix: str = ...,
         PolicyUsageFilter: PolicyUsageTypeType = ...,
         Marker: str = ...,
-        MaxItems: int = ...
+        MaxItems: int = ...,
     ) -> "PolicyAttachedRolesCollection":
         """
         Get items from the collection, passing keyword arguments along as parameters to the underlying service operation, which are typically used to filter the results.
         """
 
     def limit(self, count: int) -> "PolicyAttachedRolesCollection":
         """
@@ -992,15 +991,15 @@
     def filter(  # type: ignore
         self,
         *,
         EntityFilter: EntityTypeType = ...,
         PathPrefix: str = ...,
         PolicyUsageFilter: PolicyUsageTypeType = ...,
         Marker: str = ...,
-        MaxItems: int = ...
+        MaxItems: int = ...,
     ) -> "PolicyAttachedUsersCollection":
         """
         Get items from the collection, passing keyword arguments along as parameters to the underlying service operation, which are typically used to filter the results.
         """
 
     def limit(self, count: int) -> "PolicyAttachedUsersCollection":
         """
@@ -1427,14 +1426,15 @@
     access_key_id: Awaitable[str]
     status: Awaitable[statusTypeType]
     secret_access_key: Awaitable[str]
     create_date: Awaitable[datetime]
     user_name: str
     id: str
     secret: str
+    meta: Awaitable["IAMResourceMeta"]
 
     async def activate(self, *, Status: statusTypeType = "Active") -> None:
         """
         Changes the status of the specified access key from Active to Inactive, or vice
         versa.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.AccessKeyPair.activate)
@@ -1482,14 +1482,15 @@
     require_uppercase_characters: Awaitable[bool]
     require_lowercase_characters: Awaitable[bool]
     allow_users_to_change_password: Awaitable[bool]
     expire_passwords: Awaitable[bool]
     max_password_age: Awaitable[int]
     password_reuse_prevention: Awaitable[int]
     hard_expiry: Awaitable[bool]
+    meta: Awaitable["IAMResourceMeta"]
 
     async def delete(self) -> None:
         """
         Deletes the password policy for the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.AccountPasswordPolicy.delete)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#accountpasswordpolicydelete-method)
@@ -1530,15 +1531,15 @@
         RequireSymbols: bool = ...,
         RequireNumbers: bool = ...,
         RequireUppercaseCharacters: bool = ...,
         RequireLowercaseCharacters: bool = ...,
         AllowUsersToChangePassword: bool = ...,
         MaxPasswordAge: int = ...,
         PasswordReusePrevention: int = ...,
-        HardExpiry: bool = ...
+        HardExpiry: bool = ...,
     ) -> None:
         """
         Updates the password policy settings for the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.AccountPasswordPolicy.update)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#accountpasswordpolicyupdate-method)
         """
@@ -1550,14 +1551,15 @@
 class AccountSummary(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.AccountSummary)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#accountsummary)
     """
 
     summary_map: Awaitable[Dict[summaryKeyTypeType, int]]
+    meta: Awaitable["IAMResourceMeta"]
 
     async def get_available_subresources(self) -> Sequence[str]:
         """
         Returns a list of all the available sub-resources for this Resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.AccountSummary.get_available_subresources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#accountsummaryget_available_subresources-method)
@@ -1601,14 +1603,15 @@
     password_last_used: Awaitable[datetime]
     permissions_boundary: Awaitable[AttachedPermissionsBoundaryTypeDef]
     tags: Awaitable[List[TagTypeDef]]
     user: "User"
     access_keys: CurrentUserAccessKeysCollection
     mfa_devices: CurrentUserMfaDevicesCollection
     signing_certificates: CurrentUserSigningCertificatesCollection
+    meta: Awaitable["IAMResourceMeta"]
 
     async def get_available_subresources(self) -> Sequence[str]:
         """
         Returns a list of all the available sub-resources for this Resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.CurrentUser.get_available_subresources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#currentuserget_available_subresources-method)
@@ -1649,14 +1652,15 @@
     instance_profile_id: Awaitable[str]
     arn: Awaitable[str]
     create_date: Awaitable[datetime]
     roles_attribute: Awaitable[List[RoleTypeDef]]
     tags: Awaitable[List[TagTypeDef]]
     name: str
     roles: List["Role"]
+    meta: Awaitable["IAMResourceMeta"]
 
     async def add_role(self, *, RoleName: str) -> None:
         """
         Adds the specified IAM role to the specified instance profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.InstanceProfile.add_role)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#instanceprofileadd_role-method)
@@ -1717,14 +1721,15 @@
     """
 
     document: Awaitable[PolicyDocumentTypeDef]
     is_default_version: Awaitable[bool]
     create_date: Awaitable[datetime]
     arn: str
     version_id: str
+    meta: Awaitable["IAMResourceMeta"]
 
     async def delete(self) -> None:
         """
         Deletes the specified version from the specified managed policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.PolicyVersion.delete)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#policyversiondelete-method)
@@ -1779,14 +1784,15 @@
     """
 
     saml_metadata_document: Awaitable[str]
     create_date: Awaitable[datetime]
     valid_until: Awaitable[datetime]
     tags: Awaitable[List[TagTypeDef]]
     arn: str
+    meta: Awaitable["IAMResourceMeta"]
 
     async def delete(self) -> None:
         """
         Deletes a SAML provider resource in IAM.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.SamlProvider.delete)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#samlproviderdelete-method)
@@ -1841,14 +1847,15 @@
     base32_string_seed: Awaitable[bytes]
     qr_code_png: Awaitable[bytes]
     user_attribute: Awaitable[UserResponseTypeDef]
     enable_date: Awaitable[datetime]
     tags: Awaitable[List[TagTypeDef]]
     serial_number: str
     user: "User"
+    meta: Awaitable["IAMResourceMeta"]
 
     async def delete(self) -> None:
         """
         Deletes a virtual MFA device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.VirtualMfaDevice.delete)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#virtualmfadevicedelete-method)
@@ -1873,14 +1880,15 @@
     """
 
     access_key_id: Awaitable[str]
     status: Awaitable[statusTypeType]
     create_date: Awaitable[datetime]
     user_name: str
     id: str
+    meta: Awaitable["IAMResourceMeta"]
 
     async def User(self) -> "_User":
         """
         Creates a User resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.AccessKey.User)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#accesskeyuser-method)
@@ -1927,14 +1935,15 @@
 class AssumeRolePolicy(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.AssumeRolePolicy)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#assumerolepolicy)
     """
 
     role_name: str
+    meta: Awaitable["IAMResourceMeta"]
 
     async def Role(self) -> "_Role":
         """
         Creates a Role resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.AssumeRolePolicy.Role)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#assumerolepolicyrole-method)
@@ -1966,14 +1975,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#grouppolicy)
     """
 
     policy_name: Awaitable[str]
     policy_document: Awaitable[PolicyDocumentTypeDef]
     group_name: str
     name: str
+    meta: Awaitable["IAMResourceMeta"]
 
     async def Group(self) -> "_Group":
         """
         Creates a Group resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.GroupPolicy.Group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#grouppolicygroup-method)
@@ -2033,14 +2043,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.MfaDevice)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#mfadevice)
     """
 
     enable_date: Awaitable[datetime]
     user_name: str
     serial_number: str
+    meta: Awaitable["IAMResourceMeta"]
 
     async def User(self) -> "_User":
         """
         Creates a User resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.MfaDevice.User)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#mfadeviceuser-method)
@@ -2105,14 +2116,15 @@
     tags: Awaitable[List[TagTypeDef]]
     arn: str
     default_version: "PolicyVersion"
     attached_groups: PolicyAttachedGroupsCollection
     attached_roles: PolicyAttachedRolesCollection
     attached_users: PolicyAttachedUsersCollection
     versions: PolicyVersionsCollection
+    meta: Awaitable["IAMResourceMeta"]
 
     async def attach_group(self, *, GroupName: str) -> None:
         """
         Attaches the specified managed policy to the specified IAM group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Policy.attach_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#policyattach_group-method)
@@ -2132,15 +2144,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Policy.attach_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#policyattach_user-method)
         """
 
     async def create_version(
         self, *, PolicyDocument: str, SetAsDefault: bool = ...
-    ) -> _PolicyVersion:
+    ) -> "_PolicyVersion":
         """
         Creates a new version of the specified managed policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Policy.create_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#policycreate_version-method)
         """
 
@@ -2212,14 +2224,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#rolepolicy)
     """
 
     policy_name: Awaitable[str]
     policy_document: Awaitable[PolicyDocumentTypeDef]
     role_name: str
     name: str
+    meta: Awaitable["IAMResourceMeta"]
 
     async def Role(self) -> "_Role":
         """
         Creates a Role resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.RolePolicy.Role)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#rolepolicyrole-method)
@@ -2281,14 +2294,15 @@
     """
 
     server_certificate_metadata: Awaitable[ServerCertificateMetadataResponseTypeDef]
     certificate_body: Awaitable[str]
     certificate_chain: Awaitable[str]
     tags: Awaitable[List[TagTypeDef]]
     name: str
+    meta: Awaitable["IAMResourceMeta"]
 
     async def delete(self) -> None:
         """
         Deletes the specified server certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServerCertificate.delete)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#servercertificatedelete-method)
@@ -2345,14 +2359,15 @@
 
     certificate_id: Awaitable[str]
     certificate_body: Awaitable[str]
     status: Awaitable[statusTypeType]
     upload_date: Awaitable[datetime]
     user_name: str
     id: str
+    meta: Awaitable["IAMResourceMeta"]
 
     async def User(self) -> "_User":
         """
         Creates a User resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.SigningCertificate.User)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#signingcertificateuser-method)
@@ -2404,14 +2419,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#userpolicy)
     """
 
     policy_name: Awaitable[str]
     policy_document: Awaitable[PolicyDocumentTypeDef]
     user_name: str
     name: str
+    meta: Awaitable["IAMResourceMeta"]
 
     async def User(self) -> "_User":
         """
         Creates a User resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.UserPolicy.User)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#userpolicyuser-method)
@@ -2462,23 +2478,144 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#userpolicyreload-method)
         """
 
 
 _UserPolicy = UserPolicy
 
 
+class Group(AIOBoto3ServiceResource):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.Group)
+    [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#group)
+    """
+
+    path: Awaitable[str]
+    group_name: Awaitable[str]
+    group_id: Awaitable[str]
+    arn: Awaitable[str]
+    create_date: Awaitable[datetime]
+    name: str
+    attached_policies: GroupAttachedPoliciesCollection
+    policies: GroupPoliciesCollection
+    users: GroupUsersCollection
+    meta: Awaitable["IAMResourceMeta"]
+
+    async def Policy(self, name: str) -> "_GroupPolicy":
+        """
+        Creates a GroupPolicy resource.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Group.Policy)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#grouppolicy-method)
+        """
+
+    async def add_user(self, *, UserName: str) -> None:
+        """
+        Adds the specified user to the specified group.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Group.add_user)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#groupadd_user-method)
+        """
+
+    async def attach_policy(self, *, PolicyArn: str) -> None:
+        """
+        Attaches the specified managed policy to the specified IAM group.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Group.attach_policy)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#groupattach_policy-method)
+        """
+
+    async def create(self, *, Path: str = ...) -> "_Group":
+        """
+        Creates a new group.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Group.create)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#groupcreate-method)
+        """
+
+    async def create_policy(self, *, PolicyName: str, PolicyDocument: str) -> "_GroupPolicy":
+        """
+        Adds or updates an inline policy document that is embedded in the specified IAM
+        group.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Group.create_policy)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#groupcreate_policy-method)
+        """
+
+    async def delete(self) -> None:
+        """
+        Deletes the specified IAM group.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Group.delete)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#groupdelete-method)
+        """
+
+    async def detach_policy(self, *, PolicyArn: str) -> None:
+        """
+        Removes the specified managed policy from the specified IAM group.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Group.detach_policy)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#groupdetach_policy-method)
+        """
+
+    async def get_available_subresources(self) -> Sequence[str]:
+        """
+        Returns a list of all the available sub-resources for this Resource.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Group.get_available_subresources)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#groupget_available_subresources-method)
+        """
+
+    async def load(self) -> None:
+        """
+        Calls :py:meth:`IAM.Client.get_group` to update the attributes of the Group
+        resource.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Group.load)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#groupload-method)
+        """
+
+    async def reload(self) -> None:
+        """
+        Calls :py:meth:`IAM.Client.get_group` to update the attributes of the Group
+        resource.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Group.reload)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#groupreload-method)
+        """
+
+    async def remove_user(self, *, UserName: str) -> None:
+        """
+        Removes the specified user from the specified group.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Group.remove_user)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#groupremove_user-method)
+        """
+
+    async def update(self, *, NewPath: str = ..., NewGroupName: str = ...) -> "_Group":
+        """
+        Updates the name and/or the path of the specified IAM group.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Group.update)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#groupupdate-method)
+        """
+
+
+_Group = Group
+
+
 class LoginProfile(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.LoginProfile)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#loginprofile)
     """
 
     create_date: Awaitable[datetime]
     password_reset_required: Awaitable[bool]
     user_name: str
+    meta: Awaitable["IAMResourceMeta"]
 
     async def User(self) -> "_User":
         """
         Creates a User resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.LoginProfile.User)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#loginprofileuser-method)
@@ -2559,24 +2696,25 @@
     permissions_boundary: Awaitable[AttachedPermissionsBoundaryTypeDef]
     tags: Awaitable[List[TagTypeDef]]
     role_last_used: Awaitable[RoleLastUsedResponseTypeDef]
     name: str
     attached_policies: RoleAttachedPoliciesCollection
     instance_profiles: RoleInstanceProfilesCollection
     policies: RolePoliciesCollection
+    meta: Awaitable["IAMResourceMeta"]
 
-    async def AssumeRolePolicy(self) -> _AssumeRolePolicy:
+    async def AssumeRolePolicy(self) -> "_AssumeRolePolicy":
         """
         Creates a AssumeRolePolicy resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Role.AssumeRolePolicy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#roleassumerolepolicy-method)
         """
 
-    async def Policy(self, name: str) -> _RolePolicy:
+    async def Policy(self, name: str) -> "_RolePolicy":
         """
         Creates a RolePolicy resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Role.Policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#rolepolicy-method)
         """
 
@@ -2630,133 +2768,14 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#rolereload-method)
         """
 
 
 _Role = Role
 
 
-class Group(AIOBoto3ServiceResource):
-    """
-    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.Group)
-    [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#group)
-    """
-
-    path: Awaitable[str]
-    group_name: Awaitable[str]
-    group_id: Awaitable[str]
-    arn: Awaitable[str]
-    create_date: Awaitable[datetime]
-    name: str
-    attached_policies: GroupAttachedPoliciesCollection
-    policies: GroupPoliciesCollection
-    users: GroupUsersCollection
-
-    async def Policy(self, name: str) -> _GroupPolicy:
-        """
-        Creates a GroupPolicy resource.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Group.Policy)
-        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#grouppolicy-method)
-        """
-
-    async def add_user(self, *, UserName: str) -> None:
-        """
-        Adds the specified user to the specified group.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Group.add_user)
-        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#groupadd_user-method)
-        """
-
-    async def attach_policy(self, *, PolicyArn: str) -> None:
-        """
-        Attaches the specified managed policy to the specified IAM group.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Group.attach_policy)
-        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#groupattach_policy-method)
-        """
-
-    async def create(self, *, Path: str = ...) -> "_Group":
-        """
-        Creates a new group.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Group.create)
-        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#groupcreate-method)
-        """
-
-    async def create_policy(self, *, PolicyName: str, PolicyDocument: str) -> _GroupPolicy:
-        """
-        Adds or updates an inline policy document that is embedded in the specified IAM
-        group.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Group.create_policy)
-        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#groupcreate_policy-method)
-        """
-
-    async def delete(self) -> None:
-        """
-        Deletes the specified IAM group.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Group.delete)
-        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#groupdelete-method)
-        """
-
-    async def detach_policy(self, *, PolicyArn: str) -> None:
-        """
-        Removes the specified managed policy from the specified IAM group.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Group.detach_policy)
-        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#groupdetach_policy-method)
-        """
-
-    async def get_available_subresources(self) -> Sequence[str]:
-        """
-        Returns a list of all the available sub-resources for this Resource.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Group.get_available_subresources)
-        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#groupget_available_subresources-method)
-        """
-
-    async def load(self) -> None:
-        """
-        Calls :py:meth:`IAM.Client.get_group` to update the attributes of the Group
-        resource.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Group.load)
-        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#groupload-method)
-        """
-
-    async def reload(self) -> None:
-        """
-        Calls :py:meth:`IAM.Client.get_group` to update the attributes of the Group
-        resource.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Group.reload)
-        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#groupreload-method)
-        """
-
-    async def remove_user(self, *, UserName: str) -> None:
-        """
-        Removes the specified user from the specified group.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Group.remove_user)
-        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#groupremove_user-method)
-        """
-
-    async def update(self, *, NewPath: str = ..., NewGroupName: str = ...) -> "_Group":
-        """
-        Updates the name and/or the path of the specified IAM group.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Group.update)
-        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#groupupdate-method)
-        """
-
-
-_Group = Group
-
-
 class User(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.User)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#user)
     """
 
     path: Awaitable[str]
@@ -2770,48 +2789,49 @@
     name: str
     access_keys: UserAccessKeysCollection
     attached_policies: UserAttachedPoliciesCollection
     groups: UserGroupsCollection
     mfa_devices: UserMfaDevicesCollection
     policies: UserPoliciesCollection
     signing_certificates: UserSigningCertificatesCollection
+    meta: Awaitable["IAMResourceMeta"]
 
-    async def AccessKey(self, id: str) -> _AccessKey:
+    async def AccessKey(self, id: str) -> "_AccessKey":
         """
         Creates a AccessKey resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.User.AccessKey)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#useraccesskey-method)
         """
 
-    async def LoginProfile(self) -> _LoginProfile:
+    async def LoginProfile(self) -> "_LoginProfile":
         """
         Creates a LoginProfile resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.User.LoginProfile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#userloginprofile-method)
         """
 
-    async def MfaDevice(self, serial_number: str) -> _MfaDevice:
+    async def MfaDevice(self, serial_number: str) -> "_MfaDevice":
         """
         Creates a MfaDevice resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.User.MfaDevice)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#usermfadevice-method)
         """
 
-    async def Policy(self, name: str) -> _UserPolicy:
+    async def Policy(self, name: str) -> "_UserPolicy":
         """
         Creates a UserPolicy resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.User.Policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#userpolicy-method)
         """
 
-    async def SigningCertificate(self, id: str) -> _SigningCertificate:
+    async def SigningCertificate(self, id: str) -> "_SigningCertificate":
         """
         Creates a SigningCertificate resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.User.SigningCertificate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#usersigningcertificate-method)
         """
 
@@ -2837,35 +2857,35 @@
         """
         Creates a new IAM user for your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.User.create)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#usercreate-method)
         """
 
-    async def create_access_key_pair(self) -> _AccessKeyPair:
+    async def create_access_key_pair(self) -> "_AccessKeyPair":
         """
         Creates a new Amazon Web Services secret access key and corresponding Amazon
         Web Services access key ID for the specified
         user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.User.create_access_key_pair)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#usercreate_access_key_pair-method)
         """
 
     async def create_login_profile(
         self, *, Password: str, PasswordResetRequired: bool = ...
-    ) -> _LoginProfile:
+    ) -> "_LoginProfile":
         """
         Creates a password for the specified IAM user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.User.create_login_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#usercreate_login_profile-method)
         """
 
-    async def create_policy(self, *, PolicyName: str, PolicyDocument: str) -> _UserPolicy:
+    async def create_policy(self, *, PolicyName: str, PolicyDocument: str) -> "_UserPolicy":
         """
         Adds or updates an inline policy document that is embedded in the specified IAM
         user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.User.create_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#usercreate_policy-method)
         """
@@ -2884,15 +2904,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.User.detach_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#userdetach_policy-method)
         """
 
     async def enable_mfa(
         self, *, SerialNumber: str, AuthenticationCode1: str, AuthenticationCode2: str
-    ) -> _MfaDevice:
+    ) -> "_MfaDevice":
         """
         Enables the specified MFA device and associates it with the specified IAM user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.User.enable_mfa)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#userenable_mfa-method)
         """
 
@@ -2958,175 +2978,175 @@
     policies: ServiceResourcePoliciesCollection
     roles: ServiceResourceRolesCollection
     saml_providers: ServiceResourceSamlProvidersCollection
     server_certificates: ServiceResourceServerCertificatesCollection
     users: ServiceResourceUsersCollection
     virtual_mfa_devices: ServiceResourceVirtualMfaDevicesCollection
 
-    async def AccessKey(self, user_name: str, id: str) -> _AccessKey:
+    async def AccessKey(self, user_name: str, id: str) -> "_AccessKey":
         """
         Creates a AccessKey resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.AccessKey)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourceaccesskey-method)
         """
 
-    async def AccessKeyPair(self, user_name: str, id: str, secret: str) -> _AccessKeyPair:
+    async def AccessKeyPair(self, user_name: str, id: str, secret: str) -> "_AccessKeyPair":
         """
         Creates a AccessKeyPair resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.AccessKeyPair)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourceaccesskeypair-method)
         """
 
-    async def AccountPasswordPolicy(self) -> _AccountPasswordPolicy:
+    async def AccountPasswordPolicy(self) -> "_AccountPasswordPolicy":
         """
         Creates a AccountPasswordPolicy resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.AccountPasswordPolicy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourceaccountpasswordpolicy-method)
         """
 
-    async def AccountSummary(self) -> _AccountSummary:
+    async def AccountSummary(self) -> "_AccountSummary":
         """
         Creates a AccountSummary resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.AccountSummary)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourceaccountsummary-method)
         """
 
-    async def AssumeRolePolicy(self, role_name: str) -> _AssumeRolePolicy:
+    async def AssumeRolePolicy(self, role_name: str) -> "_AssumeRolePolicy":
         """
         Creates a AssumeRolePolicy resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.AssumeRolePolicy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourceassumerolepolicy-method)
         """
 
-    async def CurrentUser(self) -> _CurrentUser:
+    async def CurrentUser(self) -> "_CurrentUser":
         """
         Creates a CurrentUser resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.CurrentUser)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourcecurrentuser-method)
         """
 
-    async def Group(self, name: str) -> _Group:
+    async def Group(self, name: str) -> "_Group":
         """
         Creates a Group resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.Group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourcegroup-method)
         """
 
-    async def GroupPolicy(self, group_name: str, name: str) -> _GroupPolicy:
+    async def GroupPolicy(self, group_name: str, name: str) -> "_GroupPolicy":
         """
         Creates a GroupPolicy resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.GroupPolicy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourcegrouppolicy-method)
         """
 
-    async def InstanceProfile(self, name: str) -> _InstanceProfile:
+    async def InstanceProfile(self, name: str) -> "_InstanceProfile":
         """
         Creates a InstanceProfile resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.InstanceProfile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourceinstanceprofile-method)
         """
 
-    async def LoginProfile(self, user_name: str) -> _LoginProfile:
+    async def LoginProfile(self, user_name: str) -> "_LoginProfile":
         """
         Creates a LoginProfile resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.LoginProfile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourceloginprofile-method)
         """
 
-    async def MfaDevice(self, user_name: str, serial_number: str) -> _MfaDevice:
+    async def MfaDevice(self, user_name: str, serial_number: str) -> "_MfaDevice":
         """
         Creates a MfaDevice resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.MfaDevice)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourcemfadevice-method)
         """
 
-    async def Policy(self, arn: str) -> _Policy:
+    async def Policy(self, arn: str) -> "_Policy":
         """
         Creates a Policy resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.Policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourcepolicy-method)
         """
 
-    async def PolicyVersion(self, arn: str, version_id: str) -> _PolicyVersion:
+    async def PolicyVersion(self, arn: str, version_id: str) -> "_PolicyVersion":
         """
         Creates a PolicyVersion resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.PolicyVersion)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourcepolicyversion-method)
         """
 
-    async def Role(self, name: str) -> _Role:
+    async def Role(self, name: str) -> "_Role":
         """
         Creates a Role resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.Role)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourcerole-method)
         """
 
-    async def RolePolicy(self, role_name: str, name: str) -> _RolePolicy:
+    async def RolePolicy(self, role_name: str, name: str) -> "_RolePolicy":
         """
         Creates a RolePolicy resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.RolePolicy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourcerolepolicy-method)
         """
 
-    async def SamlProvider(self, arn: str) -> _SamlProvider:
+    async def SamlProvider(self, arn: str) -> "_SamlProvider":
         """
         Creates a SamlProvider resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.SamlProvider)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourcesamlprovider-method)
         """
 
-    async def ServerCertificate(self, name: str) -> _ServerCertificate:
+    async def ServerCertificate(self, name: str) -> "_ServerCertificate":
         """
         Creates a ServerCertificate resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.ServerCertificate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourceservercertificate-method)
         """
 
-    async def SigningCertificate(self, user_name: str, id: str) -> _SigningCertificate:
+    async def SigningCertificate(self, user_name: str, id: str) -> "_SigningCertificate":
         """
         Creates a SigningCertificate resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.SigningCertificate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourcesigningcertificate-method)
         """
 
-    async def User(self, name: str) -> _User:
+    async def User(self, name: str) -> "_User":
         """
         Creates a User resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.User)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourceuser-method)
         """
 
-    async def UserPolicy(self, user_name: str, name: str) -> _UserPolicy:
+    async def UserPolicy(self, user_name: str, name: str) -> "_UserPolicy":
         """
         Creates a UserPolicy resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.UserPolicy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourceuserpolicy-method)
         """
 
-    async def VirtualMfaDevice(self, serial_number: str) -> _VirtualMfaDevice:
+    async def VirtualMfaDevice(self, serial_number: str) -> "_VirtualMfaDevice":
         """
         Creates a VirtualMfaDevice resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.VirtualMfaDevice)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourcevirtualmfadevice-method)
         """
 
@@ -3153,50 +3173,50 @@
         RequireSymbols: bool = ...,
         RequireNumbers: bool = ...,
         RequireUppercaseCharacters: bool = ...,
         RequireLowercaseCharacters: bool = ...,
         AllowUsersToChangePassword: bool = ...,
         MaxPasswordAge: int = ...,
         PasswordReusePrevention: int = ...,
-        HardExpiry: bool = ...
-    ) -> _AccountPasswordPolicy:
+        HardExpiry: bool = ...,
+    ) -> "_AccountPasswordPolicy":
         """
         Updates the password policy settings for the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.create_account_password_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourcecreate_account_password_policy-method)
         """
 
-    async def create_group(self, *, GroupName: str, Path: str = ...) -> _Group:
+    async def create_group(self, *, GroupName: str, Path: str = ...) -> "_Group":
         """
         Creates a new group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.create_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourcecreate_group-method)
         """
 
     async def create_instance_profile(
         self, *, InstanceProfileName: str, Path: str = ..., Tags: Sequence[TagTypeDef] = ...
-    ) -> _InstanceProfile:
+    ) -> "_InstanceProfile":
         """
         Creates a new instance profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.create_instance_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourcecreate_instance_profile-method)
         """
 
     async def create_policy(
         self,
         *,
         PolicyName: str,
         PolicyDocument: str,
         Path: str = ...,
         Description: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
-    ) -> _Policy:
+        Tags: Sequence[TagTypeDef] = ...,
+    ) -> "_Policy":
         """
         Creates a new managed policy for your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.create_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourcecreate_policy-method)
         """
 
@@ -3205,26 +3225,26 @@
         *,
         RoleName: str,
         AssumeRolePolicyDocument: str,
         Path: str = ...,
         Description: str = ...,
         MaxSessionDuration: int = ...,
         PermissionsBoundary: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
-    ) -> _Role:
+        Tags: Sequence[TagTypeDef] = ...,
+    ) -> "_Role":
         """
         Creates a new role for your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.create_role)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourcecreate_role-method)
         """
 
     async def create_saml_provider(
         self, *, SAMLMetadataDocument: str, Name: str, Tags: Sequence[TagTypeDef] = ...
-    ) -> _SamlProvider:
+    ) -> "_SamlProvider":
         """
         Creates an IAM resource that describes an identity provider (IdP) that supports
         SAML
         2.0.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.create_saml_provider)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourcecreate_saml_provider-method)
@@ -3234,52 +3254,52 @@
         self,
         *,
         ServerCertificateName: str,
         CertificateBody: str,
         PrivateKey: str,
         Path: str = ...,
         CertificateChain: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
-    ) -> _ServerCertificate:
+        Tags: Sequence[TagTypeDef] = ...,
+    ) -> "_ServerCertificate":
         """
         Uploads a server certificate entity for the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.create_server_certificate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourcecreate_server_certificate-method)
         """
 
     async def create_signing_certificate(
         self, *, CertificateBody: str, UserName: str = ...
-    ) -> _SigningCertificate:
+    ) -> "_SigningCertificate":
         """
         Uploads an X.509 signing certificate and associates it with the specified IAM
         user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.create_signing_certificate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourcecreate_signing_certificate-method)
         """
 
     async def create_user(
         self,
         *,
         UserName: str,
         Path: str = ...,
         PermissionsBoundary: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
-    ) -> _User:
+        Tags: Sequence[TagTypeDef] = ...,
+    ) -> "_User":
         """
         Creates a new IAM user for your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.create_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourcecreate_user-method)
         """
 
     async def create_virtual_mfa_device(
         self, *, VirtualMFADeviceName: str, Path: str = ..., Tags: Sequence[TagTypeDef] = ...
-    ) -> _VirtualMfaDevice:
+    ) -> "_VirtualMfaDevice":
         """
         Creates a new virtual MFA device for the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.create_virtual_mfa_device)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourcecreate_virtual_mfa_device-method)
         """
```

### Comparing `types-aiobotocore-iam-2.9.0/types_aiobotocore_iam/service_resource.pyi` & `types-aiobotocore-iam-2.9.1/types_aiobotocore_iam/service_resource.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -274,15 +274,15 @@
         self,
         *,
         Scope: policyScopeTypeType = ...,
         OnlyAttached: bool = ...,
         PathPrefix: str = ...,
         PolicyUsageFilter: PolicyUsageTypeType = ...,
         Marker: str = ...,
-        MaxItems: int = ...
+        MaxItems: int = ...,
     ) -> "ServiceResourcePoliciesCollection":
         """
         Get items from the collection, passing keyword arguments along as parameters to the underlying service operation, which are typically used to filter the results.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.policies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#serviceresourcepoliciescollection)
         """
@@ -596,15 +596,15 @@
         """
 
     def filter(  # type: ignore
         self,
         *,
         AssignmentStatus: assignmentStatusTypeType = ...,
         Marker: str = ...,
-        MaxItems: int = ...
+        MaxItems: int = ...,
     ) -> "ServiceResourceVirtualMfaDevicesCollection":
         """
         Get items from the collection, passing keyword arguments along as parameters to the underlying service operation, which are typically used to filter the results.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.virtual_mfa_devices)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#serviceresourcevirtualmfadevicescollection)
         """
@@ -886,15 +886,15 @@
     def filter(  # type: ignore
         self,
         *,
         EntityFilter: EntityTypeType = ...,
         PathPrefix: str = ...,
         PolicyUsageFilter: PolicyUsageTypeType = ...,
         Marker: str = ...,
-        MaxItems: int = ...
+        MaxItems: int = ...,
     ) -> "PolicyAttachedGroupsCollection":
         """
         Get items from the collection, passing keyword arguments along as parameters to the underlying service operation, which are typically used to filter the results.
         """
 
     def limit(self, count: int) -> "PolicyAttachedGroupsCollection":
         """
@@ -930,15 +930,15 @@
     def filter(  # type: ignore
         self,
         *,
         EntityFilter: EntityTypeType = ...,
         PathPrefix: str = ...,
         PolicyUsageFilter: PolicyUsageTypeType = ...,
         Marker: str = ...,
-        MaxItems: int = ...
+        MaxItems: int = ...,
     ) -> "PolicyAttachedRolesCollection":
         """
         Get items from the collection, passing keyword arguments along as parameters to the underlying service operation, which are typically used to filter the results.
         """
 
     def limit(self, count: int) -> "PolicyAttachedRolesCollection":
         """
@@ -974,15 +974,15 @@
     def filter(  # type: ignore
         self,
         *,
         EntityFilter: EntityTypeType = ...,
         PathPrefix: str = ...,
         PolicyUsageFilter: PolicyUsageTypeType = ...,
         Marker: str = ...,
-        MaxItems: int = ...
+        MaxItems: int = ...,
     ) -> "PolicyAttachedUsersCollection":
         """
         Get items from the collection, passing keyword arguments along as parameters to the underlying service operation, which are typically used to filter the results.
         """
 
     def limit(self, count: int) -> "PolicyAttachedUsersCollection":
         """
@@ -1398,14 +1398,15 @@
     access_key_id: Awaitable[str]
     status: Awaitable[statusTypeType]
     secret_access_key: Awaitable[str]
     create_date: Awaitable[datetime]
     user_name: str
     id: str
     secret: str
+    meta: Awaitable["IAMResourceMeta"]
 
     async def activate(self, *, Status: statusTypeType = "Active") -> None:
         """
         Changes the status of the specified access key from Active to Inactive, or vice
         versa.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.AccessKeyPair.activate)
@@ -1451,14 +1452,15 @@
     require_uppercase_characters: Awaitable[bool]
     require_lowercase_characters: Awaitable[bool]
     allow_users_to_change_password: Awaitable[bool]
     expire_passwords: Awaitable[bool]
     max_password_age: Awaitable[int]
     password_reuse_prevention: Awaitable[int]
     hard_expiry: Awaitable[bool]
+    meta: Awaitable["IAMResourceMeta"]
 
     async def delete(self) -> None:
         """
         Deletes the password policy for the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.AccountPasswordPolicy.delete)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#accountpasswordpolicydelete-method)
@@ -1499,15 +1501,15 @@
         RequireSymbols: bool = ...,
         RequireNumbers: bool = ...,
         RequireUppercaseCharacters: bool = ...,
         RequireLowercaseCharacters: bool = ...,
         AllowUsersToChangePassword: bool = ...,
         MaxPasswordAge: int = ...,
         PasswordReusePrevention: int = ...,
-        HardExpiry: bool = ...
+        HardExpiry: bool = ...,
     ) -> None:
         """
         Updates the password policy settings for the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.AccountPasswordPolicy.update)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#accountpasswordpolicyupdate-method)
         """
@@ -1517,14 +1519,15 @@
 class AccountSummary(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.AccountSummary)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#accountsummary)
     """
 
     summary_map: Awaitable[Dict[summaryKeyTypeType, int]]
+    meta: Awaitable["IAMResourceMeta"]
 
     async def get_available_subresources(self) -> Sequence[str]:
         """
         Returns a list of all the available sub-resources for this Resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.AccountSummary.get_available_subresources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#accountsummaryget_available_subresources-method)
@@ -1566,14 +1569,15 @@
     password_last_used: Awaitable[datetime]
     permissions_boundary: Awaitable[AttachedPermissionsBoundaryTypeDef]
     tags: Awaitable[List[TagTypeDef]]
     user: "User"
     access_keys: CurrentUserAccessKeysCollection
     mfa_devices: CurrentUserMfaDevicesCollection
     signing_certificates: CurrentUserSigningCertificatesCollection
+    meta: Awaitable["IAMResourceMeta"]
 
     async def get_available_subresources(self) -> Sequence[str]:
         """
         Returns a list of all the available sub-resources for this Resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.CurrentUser.get_available_subresources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#currentuserget_available_subresources-method)
@@ -1612,14 +1616,15 @@
     instance_profile_id: Awaitable[str]
     arn: Awaitable[str]
     create_date: Awaitable[datetime]
     roles_attribute: Awaitable[List[RoleTypeDef]]
     tags: Awaitable[List[TagTypeDef]]
     name: str
     roles: List["Role"]
+    meta: Awaitable["IAMResourceMeta"]
 
     async def add_role(self, *, RoleName: str) -> None:
         """
         Adds the specified IAM role to the specified instance profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.InstanceProfile.add_role)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#instanceprofileadd_role-method)
@@ -1678,14 +1683,15 @@
     """
 
     document: Awaitable[PolicyDocumentTypeDef]
     is_default_version: Awaitable[bool]
     create_date: Awaitable[datetime]
     arn: str
     version_id: str
+    meta: Awaitable["IAMResourceMeta"]
 
     async def delete(self) -> None:
         """
         Deletes the specified version from the specified managed policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.PolicyVersion.delete)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#policyversiondelete-method)
@@ -1738,14 +1744,15 @@
     """
 
     saml_metadata_document: Awaitable[str]
     create_date: Awaitable[datetime]
     valid_until: Awaitable[datetime]
     tags: Awaitable[List[TagTypeDef]]
     arn: str
+    meta: Awaitable["IAMResourceMeta"]
 
     async def delete(self) -> None:
         """
         Deletes a SAML provider resource in IAM.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.SamlProvider.delete)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#samlproviderdelete-method)
@@ -1798,14 +1805,15 @@
     base32_string_seed: Awaitable[bytes]
     qr_code_png: Awaitable[bytes]
     user_attribute: Awaitable[UserResponseTypeDef]
     enable_date: Awaitable[datetime]
     tags: Awaitable[List[TagTypeDef]]
     serial_number: str
     user: "User"
+    meta: Awaitable["IAMResourceMeta"]
 
     async def delete(self) -> None:
         """
         Deletes a virtual MFA device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.VirtualMfaDevice.delete)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#virtualmfadevicedelete-method)
@@ -1828,14 +1836,15 @@
     """
 
     access_key_id: Awaitable[str]
     status: Awaitable[statusTypeType]
     create_date: Awaitable[datetime]
     user_name: str
     id: str
+    meta: Awaitable["IAMResourceMeta"]
 
     async def User(self) -> "_User":
         """
         Creates a User resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.AccessKey.User)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#accesskeyuser-method)
@@ -1880,14 +1889,15 @@
 class AssumeRolePolicy(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.AssumeRolePolicy)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#assumerolepolicy)
     """
 
     role_name: str
+    meta: Awaitable["IAMResourceMeta"]
 
     async def Role(self) -> "_Role":
         """
         Creates a Role resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.AssumeRolePolicy.Role)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#assumerolepolicyrole-method)
@@ -1917,14 +1927,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#grouppolicy)
     """
 
     policy_name: Awaitable[str]
     policy_document: Awaitable[PolicyDocumentTypeDef]
     group_name: str
     name: str
+    meta: Awaitable["IAMResourceMeta"]
 
     async def Group(self) -> "_Group":
         """
         Creates a Group resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.GroupPolicy.Group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#grouppolicygroup-method)
@@ -1982,14 +1993,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.MfaDevice)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#mfadevice)
     """
 
     enable_date: Awaitable[datetime]
     user_name: str
     serial_number: str
+    meta: Awaitable["IAMResourceMeta"]
 
     async def User(self) -> "_User":
         """
         Creates a User resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.MfaDevice.User)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#mfadeviceuser-method)
@@ -2052,14 +2064,15 @@
     tags: Awaitable[List[TagTypeDef]]
     arn: str
     default_version: "PolicyVersion"
     attached_groups: PolicyAttachedGroupsCollection
     attached_roles: PolicyAttachedRolesCollection
     attached_users: PolicyAttachedUsersCollection
     versions: PolicyVersionsCollection
+    meta: Awaitable["IAMResourceMeta"]
 
     async def attach_group(self, *, GroupName: str) -> None:
         """
         Attaches the specified managed policy to the specified IAM group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Policy.attach_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#policyattach_group-method)
@@ -2079,15 +2092,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Policy.attach_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#policyattach_user-method)
         """
 
     async def create_version(
         self, *, PolicyDocument: str, SetAsDefault: bool = ...
-    ) -> _PolicyVersion:
+    ) -> "_PolicyVersion":
         """
         Creates a new version of the specified managed policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Policy.create_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#policycreate_version-method)
         """
 
@@ -2157,14 +2170,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#rolepolicy)
     """
 
     policy_name: Awaitable[str]
     policy_document: Awaitable[PolicyDocumentTypeDef]
     role_name: str
     name: str
+    meta: Awaitable["IAMResourceMeta"]
 
     async def Role(self) -> "_Role":
         """
         Creates a Role resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.RolePolicy.Role)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#rolepolicyrole-method)
@@ -2224,14 +2238,15 @@
     """
 
     server_certificate_metadata: Awaitable[ServerCertificateMetadataResponseTypeDef]
     certificate_body: Awaitable[str]
     certificate_chain: Awaitable[str]
     tags: Awaitable[List[TagTypeDef]]
     name: str
+    meta: Awaitable["IAMResourceMeta"]
 
     async def delete(self) -> None:
         """
         Deletes the specified server certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServerCertificate.delete)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#servercertificatedelete-method)
@@ -2286,14 +2301,15 @@
 
     certificate_id: Awaitable[str]
     certificate_body: Awaitable[str]
     status: Awaitable[statusTypeType]
     upload_date: Awaitable[datetime]
     user_name: str
     id: str
+    meta: Awaitable["IAMResourceMeta"]
 
     async def User(self) -> "_User":
         """
         Creates a User resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.SigningCertificate.User)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#signingcertificateuser-method)
@@ -2343,14 +2359,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#userpolicy)
     """
 
     policy_name: Awaitable[str]
     policy_document: Awaitable[PolicyDocumentTypeDef]
     user_name: str
     name: str
+    meta: Awaitable["IAMResourceMeta"]
 
     async def User(self) -> "_User":
         """
         Creates a User resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.UserPolicy.User)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#userpolicyuser-method)
@@ -2414,16 +2431,17 @@
     group_id: Awaitable[str]
     arn: Awaitable[str]
     create_date: Awaitable[datetime]
     name: str
     attached_policies: GroupAttachedPoliciesCollection
     policies: GroupPoliciesCollection
     users: GroupUsersCollection
+    meta: Awaitable["IAMResourceMeta"]
 
-    async def Policy(self, name: str) -> _GroupPolicy:
+    async def Policy(self, name: str) -> "_GroupPolicy":
         """
         Creates a GroupPolicy resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Group.Policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#grouppolicy-method)
         """
 
@@ -2447,15 +2465,15 @@
         """
         Creates a new group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Group.create)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#groupcreate-method)
         """
 
-    async def create_policy(self, *, PolicyName: str, PolicyDocument: str) -> _GroupPolicy:
+    async def create_policy(self, *, PolicyName: str, PolicyDocument: str) -> "_GroupPolicy":
         """
         Adds or updates an inline policy document that is embedded in the specified IAM
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Group.create_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#groupcreate_policy-method)
         """
@@ -2506,15 +2524,15 @@
         """
         Removes the specified user from the specified group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Group.remove_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#groupremove_user-method)
         """
 
-    async def update(self, *, NewPath: str = ..., NewGroupName: str = ...) -> _Group:
+    async def update(self, *, NewPath: str = ..., NewGroupName: str = ...) -> "_Group":
         """
         Updates the name and/or the path of the specified IAM group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Group.update)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#groupupdate-method)
         """
 
@@ -2525,14 +2543,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.LoginProfile)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#loginprofile)
     """
 
     create_date: Awaitable[datetime]
     password_reset_required: Awaitable[bool]
     user_name: str
+    meta: Awaitable["IAMResourceMeta"]
 
     async def User(self) -> "_User":
         """
         Creates a User resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.LoginProfile.User)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#loginprofileuser-method)
@@ -2611,24 +2630,25 @@
     permissions_boundary: Awaitable[AttachedPermissionsBoundaryTypeDef]
     tags: Awaitable[List[TagTypeDef]]
     role_last_used: Awaitable[RoleLastUsedResponseTypeDef]
     name: str
     attached_policies: RoleAttachedPoliciesCollection
     instance_profiles: RoleInstanceProfilesCollection
     policies: RolePoliciesCollection
+    meta: Awaitable["IAMResourceMeta"]
 
-    async def AssumeRolePolicy(self) -> _AssumeRolePolicy:
+    async def AssumeRolePolicy(self) -> "_AssumeRolePolicy":
         """
         Creates a AssumeRolePolicy resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Role.AssumeRolePolicy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#roleassumerolepolicy-method)
         """
 
-    async def Policy(self, name: str) -> _RolePolicy:
+    async def Policy(self, name: str) -> "_RolePolicy":
         """
         Creates a RolePolicy resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Role.Policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#rolepolicy-method)
         """
 
@@ -2701,48 +2721,49 @@
     name: str
     access_keys: UserAccessKeysCollection
     attached_policies: UserAttachedPoliciesCollection
     groups: UserGroupsCollection
     mfa_devices: UserMfaDevicesCollection
     policies: UserPoliciesCollection
     signing_certificates: UserSigningCertificatesCollection
+    meta: Awaitable["IAMResourceMeta"]
 
-    async def AccessKey(self, id: str) -> _AccessKey:
+    async def AccessKey(self, id: str) -> "_AccessKey":
         """
         Creates a AccessKey resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.User.AccessKey)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#useraccesskey-method)
         """
 
-    async def LoginProfile(self) -> _LoginProfile:
+    async def LoginProfile(self) -> "_LoginProfile":
         """
         Creates a LoginProfile resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.User.LoginProfile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#userloginprofile-method)
         """
 
-    async def MfaDevice(self, serial_number: str) -> _MfaDevice:
+    async def MfaDevice(self, serial_number: str) -> "_MfaDevice":
         """
         Creates a MfaDevice resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.User.MfaDevice)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#usermfadevice-method)
         """
 
-    async def Policy(self, name: str) -> _UserPolicy:
+    async def Policy(self, name: str) -> "_UserPolicy":
         """
         Creates a UserPolicy resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.User.Policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#userpolicy-method)
         """
 
-    async def SigningCertificate(self, id: str) -> _SigningCertificate:
+    async def SigningCertificate(self, id: str) -> "_SigningCertificate":
         """
         Creates a SigningCertificate resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.User.SigningCertificate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#usersigningcertificate-method)
         """
 
@@ -2768,35 +2789,35 @@
         """
         Creates a new IAM user for your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.User.create)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#usercreate-method)
         """
 
-    async def create_access_key_pair(self) -> _AccessKeyPair:
+    async def create_access_key_pair(self) -> "_AccessKeyPair":
         """
         Creates a new Amazon Web Services secret access key and corresponding Amazon
         Web Services access key ID for the specified
         user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.User.create_access_key_pair)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#usercreate_access_key_pair-method)
         """
 
     async def create_login_profile(
         self, *, Password: str, PasswordResetRequired: bool = ...
-    ) -> _LoginProfile:
+    ) -> "_LoginProfile":
         """
         Creates a password for the specified IAM user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.User.create_login_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#usercreate_login_profile-method)
         """
 
-    async def create_policy(self, *, PolicyName: str, PolicyDocument: str) -> _UserPolicy:
+    async def create_policy(self, *, PolicyName: str, PolicyDocument: str) -> "_UserPolicy":
         """
         Adds or updates an inline policy document that is embedded in the specified IAM
         user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.User.create_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#usercreate_policy-method)
         """
@@ -2815,15 +2836,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.User.detach_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#userdetach_policy-method)
         """
 
     async def enable_mfa(
         self, *, SerialNumber: str, AuthenticationCode1: str, AuthenticationCode2: str
-    ) -> _MfaDevice:
+    ) -> "_MfaDevice":
         """
         Enables the specified MFA device and associates it with the specified IAM user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.User.enable_mfa)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#userenable_mfa-method)
         """
 
@@ -2857,15 +2878,15 @@
         """
         Removes the specified user from the specified group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.User.remove_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#userremove_group-method)
         """
 
-    async def update(self, *, NewPath: str = ..., NewUserName: str = ...) -> _User:
+    async def update(self, *, NewPath: str = ..., NewUserName: str = ...) -> "_User":
         """
         Updates the name and/or the path of the specified IAM user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.User.update)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#userupdate-method)
         """
 
@@ -2886,175 +2907,175 @@
     policies: ServiceResourcePoliciesCollection
     roles: ServiceResourceRolesCollection
     saml_providers: ServiceResourceSamlProvidersCollection
     server_certificates: ServiceResourceServerCertificatesCollection
     users: ServiceResourceUsersCollection
     virtual_mfa_devices: ServiceResourceVirtualMfaDevicesCollection
 
-    async def AccessKey(self, user_name: str, id: str) -> _AccessKey:
+    async def AccessKey(self, user_name: str, id: str) -> "_AccessKey":
         """
         Creates a AccessKey resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.AccessKey)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourceaccesskey-method)
         """
 
-    async def AccessKeyPair(self, user_name: str, id: str, secret: str) -> _AccessKeyPair:
+    async def AccessKeyPair(self, user_name: str, id: str, secret: str) -> "_AccessKeyPair":
         """
         Creates a AccessKeyPair resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.AccessKeyPair)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourceaccesskeypair-method)
         """
 
-    async def AccountPasswordPolicy(self) -> _AccountPasswordPolicy:
+    async def AccountPasswordPolicy(self) -> "_AccountPasswordPolicy":
         """
         Creates a AccountPasswordPolicy resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.AccountPasswordPolicy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourceaccountpasswordpolicy-method)
         """
 
-    async def AccountSummary(self) -> _AccountSummary:
+    async def AccountSummary(self) -> "_AccountSummary":
         """
         Creates a AccountSummary resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.AccountSummary)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourceaccountsummary-method)
         """
 
-    async def AssumeRolePolicy(self, role_name: str) -> _AssumeRolePolicy:
+    async def AssumeRolePolicy(self, role_name: str) -> "_AssumeRolePolicy":
         """
         Creates a AssumeRolePolicy resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.AssumeRolePolicy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourceassumerolepolicy-method)
         """
 
-    async def CurrentUser(self) -> _CurrentUser:
+    async def CurrentUser(self) -> "_CurrentUser":
         """
         Creates a CurrentUser resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.CurrentUser)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourcecurrentuser-method)
         """
 
-    async def Group(self, name: str) -> _Group:
+    async def Group(self, name: str) -> "_Group":
         """
         Creates a Group resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.Group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourcegroup-method)
         """
 
-    async def GroupPolicy(self, group_name: str, name: str) -> _GroupPolicy:
+    async def GroupPolicy(self, group_name: str, name: str) -> "_GroupPolicy":
         """
         Creates a GroupPolicy resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.GroupPolicy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourcegrouppolicy-method)
         """
 
-    async def InstanceProfile(self, name: str) -> _InstanceProfile:
+    async def InstanceProfile(self, name: str) -> "_InstanceProfile":
         """
         Creates a InstanceProfile resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.InstanceProfile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourceinstanceprofile-method)
         """
 
-    async def LoginProfile(self, user_name: str) -> _LoginProfile:
+    async def LoginProfile(self, user_name: str) -> "_LoginProfile":
         """
         Creates a LoginProfile resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.LoginProfile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourceloginprofile-method)
         """
 
-    async def MfaDevice(self, user_name: str, serial_number: str) -> _MfaDevice:
+    async def MfaDevice(self, user_name: str, serial_number: str) -> "_MfaDevice":
         """
         Creates a MfaDevice resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.MfaDevice)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourcemfadevice-method)
         """
 
-    async def Policy(self, arn: str) -> _Policy:
+    async def Policy(self, arn: str) -> "_Policy":
         """
         Creates a Policy resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.Policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourcepolicy-method)
         """
 
-    async def PolicyVersion(self, arn: str, version_id: str) -> _PolicyVersion:
+    async def PolicyVersion(self, arn: str, version_id: str) -> "_PolicyVersion":
         """
         Creates a PolicyVersion resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.PolicyVersion)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourcepolicyversion-method)
         """
 
-    async def Role(self, name: str) -> _Role:
+    async def Role(self, name: str) -> "_Role":
         """
         Creates a Role resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.Role)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourcerole-method)
         """
 
-    async def RolePolicy(self, role_name: str, name: str) -> _RolePolicy:
+    async def RolePolicy(self, role_name: str, name: str) -> "_RolePolicy":
         """
         Creates a RolePolicy resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.RolePolicy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourcerolepolicy-method)
         """
 
-    async def SamlProvider(self, arn: str) -> _SamlProvider:
+    async def SamlProvider(self, arn: str) -> "_SamlProvider":
         """
         Creates a SamlProvider resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.SamlProvider)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourcesamlprovider-method)
         """
 
-    async def ServerCertificate(self, name: str) -> _ServerCertificate:
+    async def ServerCertificate(self, name: str) -> "_ServerCertificate":
         """
         Creates a ServerCertificate resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.ServerCertificate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourceservercertificate-method)
         """
 
-    async def SigningCertificate(self, user_name: str, id: str) -> _SigningCertificate:
+    async def SigningCertificate(self, user_name: str, id: str) -> "_SigningCertificate":
         """
         Creates a SigningCertificate resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.SigningCertificate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourcesigningcertificate-method)
         """
 
-    async def User(self, name: str) -> _User:
+    async def User(self, name: str) -> "_User":
         """
         Creates a User resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.User)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourceuser-method)
         """
 
-    async def UserPolicy(self, user_name: str, name: str) -> _UserPolicy:
+    async def UserPolicy(self, user_name: str, name: str) -> "_UserPolicy":
         """
         Creates a UserPolicy resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.UserPolicy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourceuserpolicy-method)
         """
 
-    async def VirtualMfaDevice(self, serial_number: str) -> _VirtualMfaDevice:
+    async def VirtualMfaDevice(self, serial_number: str) -> "_VirtualMfaDevice":
         """
         Creates a VirtualMfaDevice resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.VirtualMfaDevice)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourcevirtualmfadevice-method)
         """
 
@@ -3081,50 +3102,50 @@
         RequireSymbols: bool = ...,
         RequireNumbers: bool = ...,
         RequireUppercaseCharacters: bool = ...,
         RequireLowercaseCharacters: bool = ...,
         AllowUsersToChangePassword: bool = ...,
         MaxPasswordAge: int = ...,
         PasswordReusePrevention: int = ...,
-        HardExpiry: bool = ...
-    ) -> _AccountPasswordPolicy:
+        HardExpiry: bool = ...,
+    ) -> "_AccountPasswordPolicy":
         """
         Updates the password policy settings for the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.create_account_password_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourcecreate_account_password_policy-method)
         """
 
-    async def create_group(self, *, GroupName: str, Path: str = ...) -> _Group:
+    async def create_group(self, *, GroupName: str, Path: str = ...) -> "_Group":
         """
         Creates a new group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.create_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourcecreate_group-method)
         """
 
     async def create_instance_profile(
         self, *, InstanceProfileName: str, Path: str = ..., Tags: Sequence[TagTypeDef] = ...
-    ) -> _InstanceProfile:
+    ) -> "_InstanceProfile":
         """
         Creates a new instance profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.create_instance_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourcecreate_instance_profile-method)
         """
 
     async def create_policy(
         self,
         *,
         PolicyName: str,
         PolicyDocument: str,
         Path: str = ...,
         Description: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
-    ) -> _Policy:
+        Tags: Sequence[TagTypeDef] = ...,
+    ) -> "_Policy":
         """
         Creates a new managed policy for your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.create_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourcecreate_policy-method)
         """
 
@@ -3133,26 +3154,26 @@
         *,
         RoleName: str,
         AssumeRolePolicyDocument: str,
         Path: str = ...,
         Description: str = ...,
         MaxSessionDuration: int = ...,
         PermissionsBoundary: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
-    ) -> _Role:
+        Tags: Sequence[TagTypeDef] = ...,
+    ) -> "_Role":
         """
         Creates a new role for your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.create_role)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourcecreate_role-method)
         """
 
     async def create_saml_provider(
         self, *, SAMLMetadataDocument: str, Name: str, Tags: Sequence[TagTypeDef] = ...
-    ) -> _SamlProvider:
+    ) -> "_SamlProvider":
         """
         Creates an IAM resource that describes an identity provider (IdP) that supports
         SAML
         2.0.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.create_saml_provider)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourcecreate_saml_provider-method)
@@ -3162,52 +3183,52 @@
         self,
         *,
         ServerCertificateName: str,
         CertificateBody: str,
         PrivateKey: str,
         Path: str = ...,
         CertificateChain: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
-    ) -> _ServerCertificate:
+        Tags: Sequence[TagTypeDef] = ...,
+    ) -> "_ServerCertificate":
         """
         Uploads a server certificate entity for the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.create_server_certificate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourcecreate_server_certificate-method)
         """
 
     async def create_signing_certificate(
         self, *, CertificateBody: str, UserName: str = ...
-    ) -> _SigningCertificate:
+    ) -> "_SigningCertificate":
         """
         Uploads an X.509 signing certificate and associates it with the specified IAM
         user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.create_signing_certificate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourcecreate_signing_certificate-method)
         """
 
     async def create_user(
         self,
         *,
         UserName: str,
         Path: str = ...,
         PermissionsBoundary: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
-    ) -> _User:
+        Tags: Sequence[TagTypeDef] = ...,
+    ) -> "_User":
         """
         Creates a new IAM user for your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.create_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourcecreate_user-method)
         """
 
     async def create_virtual_mfa_device(
         self, *, VirtualMFADeviceName: str, Path: str = ..., Tags: Sequence[TagTypeDef] = ...
-    ) -> _VirtualMfaDevice:
+    ) -> "_VirtualMfaDevice":
         """
         Creates a new virtual MFA device for the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.create_virtual_mfa_device)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#iamserviceresourcecreate_virtual_mfa_device-method)
         """
```

### Comparing `types-aiobotocore-iam-2.9.0/types_aiobotocore_iam/type_defs.py` & `types-aiobotocore-iam-2.9.1/types_aiobotocore_iam/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccessDetailTypeDef",
     "AccessKeyLastUsedTypeDef",
     "AccessKeyMetadataTypeDef",
     "AccessKeyTypeDef",
     "AddClientIDToOpenIDConnectProviderRequestRequestTypeDef",
     "AddRoleToInstanceProfileRequestInstanceProfileAddRoleTypeDef",
```

### Comparing `types-aiobotocore-iam-2.9.0/types_aiobotocore_iam/type_defs.pyi` & `types-aiobotocore-iam-2.9.1/types_aiobotocore_iam/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iam-2.9.0/types_aiobotocore_iam/waiter.py` & `types-aiobotocore-iam-2.9.1/types_aiobotocore_iam/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iam-2.9.0/types_aiobotocore_iam/waiter.pyi` & `types-aiobotocore-iam-2.9.1/types_aiobotocore_iam/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iam-2.9.0/types_aiobotocore_iam.egg-info/PKG-INFO` & `types-aiobotocore-iam-2.9.1/types_aiobotocore_iam.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iam
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.IAM 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.IAM 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/
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
 
 <a id="types-aiobotocore-iam"></a>
 
 # types-aiobotocore-iam
 
 [![PyPI - types-aiobotocore-iam](https://img.shields.io/pypi/v/types-aiobotocore-iam.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iam)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iam.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iam)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iam)](https://pepy.tech/project/types-aiobotocore-iam)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IAM 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM)
+[aiobotocore.IAM 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM)
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
 [types-aiobotocore-iam docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-iam-2.9.0/types_aiobotocore_iam.egg-info/SOURCES.txt` & `types-aiobotocore-iam-2.9.1/types_aiobotocore_iam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

