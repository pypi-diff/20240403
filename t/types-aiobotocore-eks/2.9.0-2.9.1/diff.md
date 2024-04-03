# Comparing `tmp/types-aiobotocore-eks-2.9.0.tar.gz` & `tmp/types-aiobotocore-eks-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-eks-2.9.0.tar", last modified: Wed Dec 13 19:59:13 2023, max compression
+gzip compressed data, was "types-aiobotocore-eks-2.9.1.tar", last modified: Thu Jan 18 01:20:38 2024, max compression
```

## Comparing `types-aiobotocore-eks-2.9.0.tar` & `types-aiobotocore-eks-2.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:13.413778 types-aiobotocore-eks-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:45:34.000000 types-aiobotocore-eks-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15503 2023-12-13 19:59:13.413778 types-aiobotocore-eks-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13956 2023-12-13 19:45:34.000000 types-aiobotocore-eks-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:13.413778 types-aiobotocore-eks-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2023-12-13 19:45:34.000000 types-aiobotocore-eks-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:13.413778 types-aiobotocore-eks-2.9.0/types_aiobotocore_eks/
--rw-r--r--   0 runner    (1001) docker     (127)     3899 2023-12-13 19:45:34.000000 types-aiobotocore-eks-2.9.0/types_aiobotocore_eks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3898 2023-12-13 19:45:34.000000 types-aiobotocore-eks-2.9.0/types_aiobotocore_eks/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      905 2023-12-13 19:45:34.000000 types-aiobotocore-eks-2.9.0/types_aiobotocore_eks/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43180 2023-12-13 19:45:34.000000 types-aiobotocore-eks-2.9.0/types_aiobotocore_eks/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    43176 2023-12-13 19:45:34.000000 types-aiobotocore-eks-2.9.0/types_aiobotocore_eks/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    16384 2023-12-13 19:45:34.000000 types-aiobotocore-eks-2.9.0/types_aiobotocore_eks/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    16382 2023-12-13 19:45:34.000000 types-aiobotocore-eks-2.9.0/types_aiobotocore_eks/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11413 2023-12-13 19:45:34.000000 types-aiobotocore-eks-2.9.0/types_aiobotocore_eks/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11402 2023-12-13 19:45:34.000000 types-aiobotocore-eks-2.9.0/types_aiobotocore_eks/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:45:34.000000 types-aiobotocore-eks-2.9.0/types_aiobotocore_eks/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    49604 2023-12-13 19:45:35.000000 types-aiobotocore-eks-2.9.0/types_aiobotocore_eks/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    49603 2023-12-13 19:45:35.000000 types-aiobotocore-eks-2.9.0/types_aiobotocore_eks/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:45:34.000000 types-aiobotocore-eks-2.9.0/types_aiobotocore_eks/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     8177 2023-12-13 19:45:34.000000 types-aiobotocore-eks-2.9.0/types_aiobotocore_eks/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8169 2023-12-13 19:45:34.000000 types-aiobotocore-eks-2.9.0/types_aiobotocore_eks/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:13.413778 types-aiobotocore-eks-2.9.0/types_aiobotocore_eks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15503 2023-12-13 19:59:13.000000 types-aiobotocore-eks-2.9.0/types_aiobotocore_eks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      802 2023-12-13 19:59:13.000000 types-aiobotocore-eks-2.9.0/types_aiobotocore_eks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:13.000000 types-aiobotocore-eks-2.9.0/types_aiobotocore_eks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:13.000000 types-aiobotocore-eks-2.9.0/types_aiobotocore_eks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:13.000000 types-aiobotocore-eks-2.9.0/types_aiobotocore_eks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-13 19:59:13.000000 types-aiobotocore-eks-2.9.0/types_aiobotocore_eks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:38.341354 types-aiobotocore-eks-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:07:29.000000 types-aiobotocore-eks-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15523 2024-01-18 01:20:38.341354 types-aiobotocore-eks-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13956 2024-01-18 01:07:29.000000 types-aiobotocore-eks-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:38.341354 types-aiobotocore-eks-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-01-18 01:07:29.000000 types-aiobotocore-eks-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:38.341354 types-aiobotocore-eks-2.9.1/types_aiobotocore_eks/
+-rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-01-18 01:07:29.000000 types-aiobotocore-eks-2.9.1/types_aiobotocore_eks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-01-18 01:07:29.000000 types-aiobotocore-eks-2.9.1/types_aiobotocore_eks/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-01-18 01:07:29.000000 types-aiobotocore-eks-2.9.1/types_aiobotocore_eks/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43198 2024-01-18 01:07:29.000000 types-aiobotocore-eks-2.9.1/types_aiobotocore_eks/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43195 2024-01-18 01:07:29.000000 types-aiobotocore-eks-2.9.1/types_aiobotocore_eks/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    16382 2024-01-18 01:07:30.000000 types-aiobotocore-eks-2.9.1/types_aiobotocore_eks/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16382 2024-01-18 01:07:30.000000 types-aiobotocore-eks-2.9.1/types_aiobotocore_eks/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11416 2024-01-18 01:07:30.000000 types-aiobotocore-eks-2.9.1/types_aiobotocore_eks/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11406 2024-01-18 01:07:29.000000 types-aiobotocore-eks-2.9.1/types_aiobotocore_eks/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:07:29.000000 types-aiobotocore-eks-2.9.1/types_aiobotocore_eks/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    49603 2024-01-18 01:07:32.000000 types-aiobotocore-eks-2.9.1/types_aiobotocore_eks/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49603 2024-01-18 01:07:32.000000 types-aiobotocore-eks-2.9.1/types_aiobotocore_eks/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:07:29.000000 types-aiobotocore-eks-2.9.1/types_aiobotocore_eks/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8177 2024-01-18 01:07:30.000000 types-aiobotocore-eks-2.9.1/types_aiobotocore_eks/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8169 2024-01-18 01:07:30.000000 types-aiobotocore-eks-2.9.1/types_aiobotocore_eks/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:38.341354 types-aiobotocore-eks-2.9.1/types_aiobotocore_eks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15523 2024-01-18 01:20:38.000000 types-aiobotocore-eks-2.9.1/types_aiobotocore_eks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-01-18 01:20:38.000000 types-aiobotocore-eks-2.9.1/types_aiobotocore_eks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:38.000000 types-aiobotocore-eks-2.9.1/types_aiobotocore_eks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:38.000000 types-aiobotocore-eks-2.9.1/types_aiobotocore_eks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:38.000000 types-aiobotocore-eks-2.9.1/types_aiobotocore_eks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-18 01:20:38.000000 types-aiobotocore-eks-2.9.1/types_aiobotocore_eks.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-eks-2.9.0/LICENSE` & `types-aiobotocore-eks-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-eks-2.9.0/PKG-INFO` & `types-aiobotocore-eks-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-eks
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.EKS 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.EKS 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/
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
 
 <a id="types-aiobotocore-eks"></a>
 
 # types-aiobotocore-eks
 
 [![PyPI - types-aiobotocore-eks](https://img.shields.io/pypi/v/types-aiobotocore-eks.svg?color=blue)](https://pypi.org/project/types-aiobotocore-eks)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-eks.svg?color=blue)](https://pypi.org/project/types-aiobotocore-eks)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-eks)](https://pepy.tech/project/types-aiobotocore-eks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EKS 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS)
+[aiobotocore.EKS 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS)
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
 [types-aiobotocore-eks docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-eks-2.9.0/README.md` & `types-aiobotocore-eks-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-eks.svg?color=blue)](https://pypi.org/project/types-aiobotocore-eks)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-eks)](https://pepy.tech/project/types-aiobotocore-eks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EKS 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS)
+[aiobotocore.EKS 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS)
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
 [types-aiobotocore-eks docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-eks-2.9.0/setup.py` & `types-aiobotocore-eks-2.9.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-eks",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_eks"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.EKS 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.EKS 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore eks type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_eks": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-eks-2.9.0/types_aiobotocore_eks/__init__.py` & `types-aiobotocore-eks-2.9.1/types_aiobotocore_eks/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,14 @@
     FargateProfileDeletedWaiter,
     NodegroupActiveWaiter,
     NodegroupDeletedWaiter,
 )
 
 Client = EKSClient
 
-
 __all__ = (
     "AddonActiveWaiter",
     "AddonDeletedWaiter",
     "Client",
     "ClusterActiveWaiter",
     "ClusterDeletedWaiter",
     "DescribeAddonVersionsPaginator",
```

### Comparing `types-aiobotocore-eks-2.9.0/types_aiobotocore_eks/__init__.pyi` & `types-aiobotocore-eks-2.9.1/types_aiobotocore_eks/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-eks-2.9.0/types_aiobotocore_eks/__main__.py` & `types-aiobotocore-eks-2.9.1/types_aiobotocore_eks/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.EKS 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.EKS 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS\nOther"
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

### Comparing `types-aiobotocore-eks-2.9.0/types_aiobotocore_eks/client.py` & `types-aiobotocore-eks-2.9.1/types_aiobotocore_eks/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("EKSClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -163,30 +162,30 @@
         """
 
     async def associate_encryption_config(
         self,
         *,
         clusterName: str,
         encryptionConfig: Sequence[EncryptionConfigTypeDef],
-        clientRequestToken: str = ...
+        clientRequestToken: str = ...,
     ) -> AssociateEncryptionConfigResponseTypeDef:
         """
         Associate encryption configuration to an existing cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.associate_encryption_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/client/#associate_encryption_config)
         """
 
     async def associate_identity_provider_config(
         self,
         *,
         clusterName: str,
         oidc: OidcIdentityProviderConfigRequestTypeDef,
         tags: Mapping[str, str] = ...,
-        clientRequestToken: str = ...
+        clientRequestToken: str = ...,
     ) -> AssociateIdentityProviderConfigResponseTypeDef:
         """
         Associate an identity provider configuration to a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.associate_identity_provider_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/client/#associate_identity_provider_config)
         """
@@ -213,15 +212,15 @@
         clusterName: str,
         addonName: str,
         addonVersion: str = ...,
         serviceAccountRoleArn: str = ...,
         resolveConflicts: ResolveConflictsType = ...,
         clientRequestToken: str = ...,
         tags: Mapping[str, str] = ...,
-        configurationValues: str = ...
+        configurationValues: str = ...,
     ) -> CreateAddonResponseTypeDef:
         """
         Creates an Amazon EKS add-on.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.create_addon)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/client/#create_addon)
         """
@@ -234,15 +233,15 @@
         resourcesVpcConfig: VpcConfigRequestTypeDef,
         version: str = ...,
         kubernetesNetworkConfig: KubernetesNetworkConfigRequestTypeDef = ...,
         logging: LoggingTypeDef = ...,
         clientRequestToken: str = ...,
         tags: Mapping[str, str] = ...,
         encryptionConfig: Sequence[EncryptionConfigTypeDef] = ...,
-        outpostConfig: OutpostConfigRequestTypeDef = ...
+        outpostConfig: OutpostConfigRequestTypeDef = ...,
     ) -> CreateClusterResponseTypeDef:
         """
         Creates an Amazon EKS control plane.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.create_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/client/#create_cluster)
         """
@@ -252,15 +251,15 @@
         *,
         name: str,
         term: EksAnywhereSubscriptionTermTypeDef,
         licenseQuantity: int = ...,
         licenseType: Literal["Cluster"] = ...,
         autoRenew: bool = ...,
         clientRequestToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateEksAnywhereSubscriptionResponseTypeDef:
         """
         Creates an EKS Anywhere subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.create_eks_anywhere_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/client/#create_eks_anywhere_subscription)
         """
@@ -270,15 +269,15 @@
         *,
         fargateProfileName: str,
         clusterName: str,
         podExecutionRoleArn: str,
         subnets: Sequence[str] = ...,
         selectors: Sequence[FargateProfileSelectorTypeDef] = ...,
         clientRequestToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateFargateProfileResponseTypeDef:
         """
         Creates an Fargate profile for your Amazon EKS cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.create_fargate_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/client/#create_fargate_profile)
         """
@@ -299,15 +298,15 @@
         taints: Sequence[TaintTypeDef] = ...,
         tags: Mapping[str, str] = ...,
         clientRequestToken: str = ...,
         launchTemplate: LaunchTemplateSpecificationTypeDef = ...,
         updateConfig: NodegroupUpdateConfigTypeDef = ...,
         capacityType: CapacityTypesType = ...,
         version: str = ...,
-        releaseVersion: str = ...
+        releaseVersion: str = ...,
     ) -> CreateNodegroupResponseTypeDef:
         """
         Creates a managed node group for an Amazon EKS cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.create_nodegroup)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/client/#create_nodegroup)
         """
@@ -316,15 +315,15 @@
         self,
         *,
         clusterName: str,
         namespace: str,
         serviceAccount: str,
         roleArn: str,
         clientRequestToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreatePodIdentityAssociationResponseTypeDef:
         """
         Creates an EKS Pod Identity association between a service account in an Amazon
         EKS cluster and an IAM role with *EKS Pod
         Identity*.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.create_pod_identity_association)
@@ -422,15 +421,15 @@
         *,
         kubernetesVersion: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         addonName: str = ...,
         types: Sequence[str] = ...,
         publishers: Sequence[str] = ...,
-        owners: Sequence[str] = ...
+        owners: Sequence[str] = ...,
     ) -> DescribeAddonVersionsResponseTypeDef:
         """
         Describes the versions for an add-on.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.describe_addon_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/client/#describe_addon_versions)
         """
@@ -506,15 +505,15 @@
         """
 
     async def disassociate_identity_provider_config(
         self,
         *,
         clusterName: str,
         identityProviderConfig: IdentityProviderConfigTypeDef,
-        clientRequestToken: str = ...
+        clientRequestToken: str = ...,
     ) -> DisassociateIdentityProviderConfigResponseTypeDef:
         """
         Disassociates an identity provider configuration from a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.disassociate_identity_provider_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/client/#disassociate_identity_provider_config)
         """
@@ -556,15 +555,15 @@
         """
 
     async def list_eks_anywhere_subscriptions(
         self,
         *,
         maxResults: int = ...,
         nextToken: str = ...,
-        includeStatus: Sequence[EksAnywhereSubscriptionStatusType] = ...
+        includeStatus: Sequence[EksAnywhereSubscriptionStatusType] = ...,
     ) -> ListEksAnywhereSubscriptionsResponseTypeDef:
         """
         Displays the full description of the subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.list_eks_anywhere_subscriptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/client/#list_eks_anywhere_subscriptions)
         """
@@ -606,15 +605,15 @@
     async def list_pod_identity_associations(
         self,
         *,
         clusterName: str,
         namespace: str = ...,
         serviceAccount: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListPodIdentityAssociationsResponseTypeDef:
         """
         List the EKS Pod Identity associations in a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.list_pod_identity_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/client/#list_pod_identity_associations)
         """
@@ -632,15 +631,15 @@
     async def list_updates(
         self,
         *,
         name: str,
         nodegroupName: str = ...,
         addonName: str = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListUpdatesResponseTypeDef:
         """
         Lists the updates associated with an Amazon EKS cluster or managed node group
         in your Amazon Web Services account, in the specified
         Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.list_updates)
@@ -649,15 +648,15 @@
 
     async def register_cluster(
         self,
         *,
         name: str,
         connectorConfig: ConnectorConfigRequestTypeDef,
         clientRequestToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> RegisterClusterResponseTypeDef:
         """
         Connects a Kubernetes cluster to the Amazon EKS control plane.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.register_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/client/#register_cluster)
         """
@@ -683,30 +682,30 @@
         *,
         clusterName: str,
         addonName: str,
         addonVersion: str = ...,
         serviceAccountRoleArn: str = ...,
         resolveConflicts: ResolveConflictsType = ...,
         clientRequestToken: str = ...,
-        configurationValues: str = ...
+        configurationValues: str = ...,
     ) -> UpdateAddonResponseTypeDef:
         """
         Updates an Amazon EKS add-on.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.update_addon)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/client/#update_addon)
         """
 
     async def update_cluster_config(
         self,
         *,
         name: str,
         resourcesVpcConfig: VpcConfigRequestTypeDef = ...,
         logging: LoggingTypeDef = ...,
-        clientRequestToken: str = ...
+        clientRequestToken: str = ...,
     ) -> UpdateClusterConfigResponseTypeDef:
         """
         Updates an Amazon EKS cluster configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.update_cluster_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/client/#update_cluster_config)
         """
@@ -736,15 +735,15 @@
         *,
         clusterName: str,
         nodegroupName: str,
         labels: UpdateLabelsPayloadTypeDef = ...,
         taints: UpdateTaintsPayloadTypeDef = ...,
         scalingConfig: NodegroupScalingConfigTypeDef = ...,
         updateConfig: NodegroupUpdateConfigTypeDef = ...,
-        clientRequestToken: str = ...
+        clientRequestToken: str = ...,
     ) -> UpdateNodegroupConfigResponseTypeDef:
         """
         Updates an Amazon EKS managed node group configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.update_nodegroup_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/client/#update_nodegroup_config)
         """
@@ -754,15 +753,15 @@
         *,
         clusterName: str,
         nodegroupName: str,
         version: str = ...,
         releaseVersion: str = ...,
         launchTemplate: LaunchTemplateSpecificationTypeDef = ...,
         force: bool = ...,
-        clientRequestToken: str = ...
+        clientRequestToken: str = ...,
     ) -> UpdateNodegroupVersionResponseTypeDef:
         """
         Updates the Kubernetes version or AMI version of an Amazon EKS managed node
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.update_nodegroup_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/client/#update_nodegroup_version)
@@ -770,15 +769,15 @@
 
     async def update_pod_identity_association(
         self,
         *,
         clusterName: str,
         associationId: str,
         roleArn: str = ...,
-        clientRequestToken: str = ...
+        clientRequestToken: str = ...,
     ) -> UpdatePodIdentityAssociationResponseTypeDef:
         """
         Updates a EKS Pod Identity association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.update_pod_identity_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/client/#update_pod_identity_association)
         """
```

### Comparing `types-aiobotocore-eks-2.9.0/types_aiobotocore_eks/client.pyi` & `types-aiobotocore-eks-2.9.1/types_aiobotocore_eks/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -159,30 +159,30 @@
         """
 
     async def associate_encryption_config(
         self,
         *,
         clusterName: str,
         encryptionConfig: Sequence[EncryptionConfigTypeDef],
-        clientRequestToken: str = ...
+        clientRequestToken: str = ...,
     ) -> AssociateEncryptionConfigResponseTypeDef:
         """
         Associate encryption configuration to an existing cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.associate_encryption_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/client/#associate_encryption_config)
         """
 
     async def associate_identity_provider_config(
         self,
         *,
         clusterName: str,
         oidc: OidcIdentityProviderConfigRequestTypeDef,
         tags: Mapping[str, str] = ...,
-        clientRequestToken: str = ...
+        clientRequestToken: str = ...,
     ) -> AssociateIdentityProviderConfigResponseTypeDef:
         """
         Associate an identity provider configuration to a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.associate_identity_provider_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/client/#associate_identity_provider_config)
         """
@@ -209,15 +209,15 @@
         clusterName: str,
         addonName: str,
         addonVersion: str = ...,
         serviceAccountRoleArn: str = ...,
         resolveConflicts: ResolveConflictsType = ...,
         clientRequestToken: str = ...,
         tags: Mapping[str, str] = ...,
-        configurationValues: str = ...
+        configurationValues: str = ...,
     ) -> CreateAddonResponseTypeDef:
         """
         Creates an Amazon EKS add-on.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.create_addon)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/client/#create_addon)
         """
@@ -230,15 +230,15 @@
         resourcesVpcConfig: VpcConfigRequestTypeDef,
         version: str = ...,
         kubernetesNetworkConfig: KubernetesNetworkConfigRequestTypeDef = ...,
         logging: LoggingTypeDef = ...,
         clientRequestToken: str = ...,
         tags: Mapping[str, str] = ...,
         encryptionConfig: Sequence[EncryptionConfigTypeDef] = ...,
-        outpostConfig: OutpostConfigRequestTypeDef = ...
+        outpostConfig: OutpostConfigRequestTypeDef = ...,
     ) -> CreateClusterResponseTypeDef:
         """
         Creates an Amazon EKS control plane.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.create_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/client/#create_cluster)
         """
@@ -248,15 +248,15 @@
         *,
         name: str,
         term: EksAnywhereSubscriptionTermTypeDef,
         licenseQuantity: int = ...,
         licenseType: Literal["Cluster"] = ...,
         autoRenew: bool = ...,
         clientRequestToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateEksAnywhereSubscriptionResponseTypeDef:
         """
         Creates an EKS Anywhere subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.create_eks_anywhere_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/client/#create_eks_anywhere_subscription)
         """
@@ -266,15 +266,15 @@
         *,
         fargateProfileName: str,
         clusterName: str,
         podExecutionRoleArn: str,
         subnets: Sequence[str] = ...,
         selectors: Sequence[FargateProfileSelectorTypeDef] = ...,
         clientRequestToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateFargateProfileResponseTypeDef:
         """
         Creates an Fargate profile for your Amazon EKS cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.create_fargate_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/client/#create_fargate_profile)
         """
@@ -295,15 +295,15 @@
         taints: Sequence[TaintTypeDef] = ...,
         tags: Mapping[str, str] = ...,
         clientRequestToken: str = ...,
         launchTemplate: LaunchTemplateSpecificationTypeDef = ...,
         updateConfig: NodegroupUpdateConfigTypeDef = ...,
         capacityType: CapacityTypesType = ...,
         version: str = ...,
-        releaseVersion: str = ...
+        releaseVersion: str = ...,
     ) -> CreateNodegroupResponseTypeDef:
         """
         Creates a managed node group for an Amazon EKS cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.create_nodegroup)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/client/#create_nodegroup)
         """
@@ -312,15 +312,15 @@
         self,
         *,
         clusterName: str,
         namespace: str,
         serviceAccount: str,
         roleArn: str,
         clientRequestToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreatePodIdentityAssociationResponseTypeDef:
         """
         Creates an EKS Pod Identity association between a service account in an Amazon
         EKS cluster and an IAM role with *EKS Pod
         Identity*.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.create_pod_identity_association)
@@ -418,15 +418,15 @@
         *,
         kubernetesVersion: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         addonName: str = ...,
         types: Sequence[str] = ...,
         publishers: Sequence[str] = ...,
-        owners: Sequence[str] = ...
+        owners: Sequence[str] = ...,
     ) -> DescribeAddonVersionsResponseTypeDef:
         """
         Describes the versions for an add-on.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.describe_addon_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/client/#describe_addon_versions)
         """
@@ -502,15 +502,15 @@
         """
 
     async def disassociate_identity_provider_config(
         self,
         *,
         clusterName: str,
         identityProviderConfig: IdentityProviderConfigTypeDef,
-        clientRequestToken: str = ...
+        clientRequestToken: str = ...,
     ) -> DisassociateIdentityProviderConfigResponseTypeDef:
         """
         Disassociates an identity provider configuration from a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.disassociate_identity_provider_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/client/#disassociate_identity_provider_config)
         """
@@ -552,15 +552,15 @@
         """
 
     async def list_eks_anywhere_subscriptions(
         self,
         *,
         maxResults: int = ...,
         nextToken: str = ...,
-        includeStatus: Sequence[EksAnywhereSubscriptionStatusType] = ...
+        includeStatus: Sequence[EksAnywhereSubscriptionStatusType] = ...,
     ) -> ListEksAnywhereSubscriptionsResponseTypeDef:
         """
         Displays the full description of the subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.list_eks_anywhere_subscriptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/client/#list_eks_anywhere_subscriptions)
         """
@@ -602,15 +602,15 @@
     async def list_pod_identity_associations(
         self,
         *,
         clusterName: str,
         namespace: str = ...,
         serviceAccount: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListPodIdentityAssociationsResponseTypeDef:
         """
         List the EKS Pod Identity associations in a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.list_pod_identity_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/client/#list_pod_identity_associations)
         """
@@ -628,15 +628,15 @@
     async def list_updates(
         self,
         *,
         name: str,
         nodegroupName: str = ...,
         addonName: str = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListUpdatesResponseTypeDef:
         """
         Lists the updates associated with an Amazon EKS cluster or managed node group
         in your Amazon Web Services account, in the specified
         Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.list_updates)
@@ -645,15 +645,15 @@
 
     async def register_cluster(
         self,
         *,
         name: str,
         connectorConfig: ConnectorConfigRequestTypeDef,
         clientRequestToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> RegisterClusterResponseTypeDef:
         """
         Connects a Kubernetes cluster to the Amazon EKS control plane.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.register_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/client/#register_cluster)
         """
@@ -679,30 +679,30 @@
         *,
         clusterName: str,
         addonName: str,
         addonVersion: str = ...,
         serviceAccountRoleArn: str = ...,
         resolveConflicts: ResolveConflictsType = ...,
         clientRequestToken: str = ...,
-        configurationValues: str = ...
+        configurationValues: str = ...,
     ) -> UpdateAddonResponseTypeDef:
         """
         Updates an Amazon EKS add-on.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.update_addon)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/client/#update_addon)
         """
 
     async def update_cluster_config(
         self,
         *,
         name: str,
         resourcesVpcConfig: VpcConfigRequestTypeDef = ...,
         logging: LoggingTypeDef = ...,
-        clientRequestToken: str = ...
+        clientRequestToken: str = ...,
     ) -> UpdateClusterConfigResponseTypeDef:
         """
         Updates an Amazon EKS cluster configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.update_cluster_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/client/#update_cluster_config)
         """
@@ -732,15 +732,15 @@
         *,
         clusterName: str,
         nodegroupName: str,
         labels: UpdateLabelsPayloadTypeDef = ...,
         taints: UpdateTaintsPayloadTypeDef = ...,
         scalingConfig: NodegroupScalingConfigTypeDef = ...,
         updateConfig: NodegroupUpdateConfigTypeDef = ...,
-        clientRequestToken: str = ...
+        clientRequestToken: str = ...,
     ) -> UpdateNodegroupConfigResponseTypeDef:
         """
         Updates an Amazon EKS managed node group configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.update_nodegroup_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/client/#update_nodegroup_config)
         """
@@ -750,15 +750,15 @@
         *,
         clusterName: str,
         nodegroupName: str,
         version: str = ...,
         releaseVersion: str = ...,
         launchTemplate: LaunchTemplateSpecificationTypeDef = ...,
         force: bool = ...,
-        clientRequestToken: str = ...
+        clientRequestToken: str = ...,
     ) -> UpdateNodegroupVersionResponseTypeDef:
         """
         Updates the Kubernetes version or AMI version of an Amazon EKS managed node
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.update_nodegroup_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/client/#update_nodegroup_version)
@@ -766,15 +766,15 @@
 
     async def update_pod_identity_association(
         self,
         *,
         clusterName: str,
         associationId: str,
         roleArn: str = ...,
-        clientRequestToken: str = ...
+        clientRequestToken: str = ...,
     ) -> UpdatePodIdentityAssociationResponseTypeDef:
         """
         Updates a EKS Pod Identity association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.update_pod_identity_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/client/#update_pod_identity_association)
         """
```

### Comparing `types-aiobotocore-eks-2.9.0/types_aiobotocore_eks/literals.py` & `types-aiobotocore-eks-2.9.1/types_aiobotocore_eks/literals.py`

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
     "AMITypesType",
     "AddonActiveWaiterName",
     "AddonDeletedWaiterName",
     "AddonIssueCodeType",
     "AddonStatusType",
     "CapacityTypesType",
@@ -64,15 +63,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 AMITypesType = Literal[
     "AL2_ARM_64",
     "AL2_x86_64",
     "AL2_x86_64_GPU",
     "BOTTLEROCKET_ARM_64",
     "BOTTLEROCKET_ARM_64_NVIDIA",
     "BOTTLEROCKET_x86_64",
```

### Comparing `types-aiobotocore-eks-2.9.0/types_aiobotocore_eks/literals.pyi` & `types-aiobotocore-eks-2.9.1/types_aiobotocore_eks/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-eks-2.9.0/types_aiobotocore_eks/paginator.py` & `types-aiobotocore-eks-2.9.1/types_aiobotocore_eks/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,14 @@
     "ListFargateProfilesPaginator",
     "ListIdentityProviderConfigsPaginator",
     "ListNodegroupsPaginator",
     "ListPodIdentityAssociationsPaginator",
     "ListUpdatesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -89,15 +88,15 @@
         self,
         *,
         kubernetesVersion: str = ...,
         addonName: str = ...,
         types: Sequence[str] = ...,
         publishers: Sequence[str] = ...,
         owners: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeAddonVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.DescribeAddonVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/paginators/#describeaddonversionspaginator)
         """
 
 
@@ -137,15 +136,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/paginators/#listeksanywheresubscriptionspaginator)
     """
 
     def paginate(
         self,
         *,
         includeStatus: Sequence[EksAnywhereSubscriptionStatusType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEksAnywhereSubscriptionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListEksAnywhereSubscriptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/paginators/#listeksanywheresubscriptionspaginator)
         """
 
 
@@ -202,15 +201,15 @@
 
     def paginate(
         self,
         *,
         clusterName: str,
         namespace: str = ...,
         serviceAccount: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPodIdentityAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListPodIdentityAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/paginators/#listpodidentityassociationspaginator)
         """
 
 
@@ -222,13 +221,13 @@
 
     def paginate(
         self,
         *,
         name: str,
         nodegroupName: str = ...,
         addonName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListUpdatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListUpdates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/paginators/#listupdatespaginator)
         """
```

### Comparing `types-aiobotocore-eks-2.9.0/types_aiobotocore_eks/paginator.pyi` & `types-aiobotocore-eks-2.9.1/types_aiobotocore_eks/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         self,
         *,
         kubernetesVersion: str = ...,
         addonName: str = ...,
         types: Sequence[str] = ...,
         publishers: Sequence[str] = ...,
         owners: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeAddonVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.DescribeAddonVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/paginators/#describeaddonversionspaginator)
         """
 
 class ListAddonsPaginator(AioPaginator):
@@ -131,15 +131,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/paginators/#listeksanywheresubscriptionspaginator)
     """
 
     def paginate(
         self,
         *,
         includeStatus: Sequence[EksAnywhereSubscriptionStatusType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEksAnywhereSubscriptionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListEksAnywhereSubscriptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/paginators/#listeksanywheresubscriptionspaginator)
         """
 
 class ListFargateProfilesPaginator(AioPaginator):
@@ -192,15 +192,15 @@
 
     def paginate(
         self,
         *,
         clusterName: str,
         namespace: str = ...,
         serviceAccount: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPodIdentityAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListPodIdentityAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/paginators/#listpodidentityassociationspaginator)
         """
 
 class ListUpdatesPaginator(AioPaginator):
@@ -211,13 +211,13 @@
 
     def paginate(
         self,
         *,
         name: str,
         nodegroupName: str = ...,
         addonName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListUpdatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListUpdates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/paginators/#listupdatespaginator)
         """
```

### Comparing `types-aiobotocore-eks-2.9.0/types_aiobotocore_eks/type_defs.py` & `types-aiobotocore-eks-2.9.1/types_aiobotocore_eks/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AddonIssueTypeDef",
     "MarketplaceInformationTypeDef",
     "CompatibilityTypeDef",
     "ResponseMetadataTypeDef",
     "OidcIdentityProviderConfigRequestTypeDef",
     "AutoScalingGroupTypeDef",
```

### Comparing `types-aiobotocore-eks-2.9.0/types_aiobotocore_eks/type_defs.pyi` & `types-aiobotocore-eks-2.9.1/types_aiobotocore_eks/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-eks-2.9.0/types_aiobotocore_eks/waiter.py` & `types-aiobotocore-eks-2.9.1/types_aiobotocore_eks/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-eks-2.9.0/types_aiobotocore_eks/waiter.pyi` & `types-aiobotocore-eks-2.9.1/types_aiobotocore_eks/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-eks-2.9.0/types_aiobotocore_eks.egg-info/PKG-INFO` & `types-aiobotocore-eks-2.9.1/types_aiobotocore_eks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-eks
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.EKS 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.EKS 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/
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
 
 <a id="types-aiobotocore-eks"></a>
 
 # types-aiobotocore-eks
 
 [![PyPI - types-aiobotocore-eks](https://img.shields.io/pypi/v/types-aiobotocore-eks.svg?color=blue)](https://pypi.org/project/types-aiobotocore-eks)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-eks.svg?color=blue)](https://pypi.org/project/types-aiobotocore-eks)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-eks)](https://pepy.tech/project/types-aiobotocore-eks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EKS 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS)
+[aiobotocore.EKS 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS)
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
 [types-aiobotocore-eks docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-eks-2.9.0/types_aiobotocore_eks.egg-info/SOURCES.txt` & `types-aiobotocore-eks-2.9.1/types_aiobotocore_eks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

