# Comparing `tmp/types-aiobotocore-elb-2.9.0.tar.gz` & `tmp/types-aiobotocore-elb-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-elb-2.9.0.tar", last modified: Wed Dec 13 19:59:15 2023, max compression
+gzip compressed data, was "types-aiobotocore-elb-2.9.1.tar", last modified: Thu Jan 18 01:20:40 2024, max compression
```

## Comparing `types-aiobotocore-elb-2.9.0.tar` & `types-aiobotocore-elb-2.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:15.317762 types-aiobotocore-elb-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:45:48.000000 types-aiobotocore-elb-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14152 2023-12-13 19:59:15.317762 types-aiobotocore-elb-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12588 2023-12-13 19:45:48.000000 types-aiobotocore-elb-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:15.317762 types-aiobotocore-elb-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2023-12-13 19:45:47.000000 types-aiobotocore-elb-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:15.313762 types-aiobotocore-elb-2.9.0/types_aiobotocore_elb/
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2023-12-13 19:45:48.000000 types-aiobotocore-elb-2.9.0/types_aiobotocore_elb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2023-12-13 19:45:48.000000 types-aiobotocore-elb-2.9.0/types_aiobotocore_elb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      939 2023-12-13 19:45:48.000000 types-aiobotocore-elb-2.9.0/types_aiobotocore_elb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26798 2023-12-13 19:45:48.000000 types-aiobotocore-elb-2.9.0/types_aiobotocore_elb/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    26794 2023-12-13 19:45:48.000000 types-aiobotocore-elb-2.9.0/types_aiobotocore_elb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9460 2023-12-13 19:45:49.000000 types-aiobotocore-elb-2.9.0/types_aiobotocore_elb/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9458 2023-12-13 19:45:48.000000 types-aiobotocore-elb-2.9.0/types_aiobotocore_elb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2023-12-13 19:45:48.000000 types-aiobotocore-elb-2.9.0/types_aiobotocore_elb/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2023-12-13 19:45:48.000000 types-aiobotocore-elb-2.9.0/types_aiobotocore_elb/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:45:48.000000 types-aiobotocore-elb-2.9.0/types_aiobotocore_elb/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    21890 2023-12-13 19:45:50.000000 types-aiobotocore-elb-2.9.0/types_aiobotocore_elb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    21889 2023-12-13 19:45:49.000000 types-aiobotocore-elb-2.9.0/types_aiobotocore_elb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:45:48.000000 types-aiobotocore-elb-2.9.0/types_aiobotocore_elb/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2023-12-13 19:45:48.000000 types-aiobotocore-elb-2.9.0/types_aiobotocore_elb/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2023-12-13 19:45:48.000000 types-aiobotocore-elb-2.9.0/types_aiobotocore_elb/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:15.317762 types-aiobotocore-elb-2.9.0/types_aiobotocore_elb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14152 2023-12-13 19:59:15.000000 types-aiobotocore-elb-2.9.0/types_aiobotocore_elb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      802 2023-12-13 19:59:15.000000 types-aiobotocore-elb-2.9.0/types_aiobotocore_elb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:15.000000 types-aiobotocore-elb-2.9.0/types_aiobotocore_elb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:15.000000 types-aiobotocore-elb-2.9.0/types_aiobotocore_elb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:15.000000 types-aiobotocore-elb-2.9.0/types_aiobotocore_elb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-13 19:59:15.000000 types-aiobotocore-elb-2.9.0/types_aiobotocore_elb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:40.105345 types-aiobotocore-elb-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:07:43.000000 types-aiobotocore-elb-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14172 2024-01-18 01:20:40.105345 types-aiobotocore-elb-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12588 2024-01-18 01:07:43.000000 types-aiobotocore-elb-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:40.105345 types-aiobotocore-elb-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-01-18 01:07:43.000000 types-aiobotocore-elb-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:40.105345 types-aiobotocore-elb-2.9.1/types_aiobotocore_elb/
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-01-18 01:07:43.000000 types-aiobotocore-elb-2.9.1/types_aiobotocore_elb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-01-18 01:07:43.000000 types-aiobotocore-elb-2.9.1/types_aiobotocore_elb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-01-18 01:07:43.000000 types-aiobotocore-elb-2.9.1/types_aiobotocore_elb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26799 2024-01-18 01:07:43.000000 types-aiobotocore-elb-2.9.1/types_aiobotocore_elb/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26796 2024-01-18 01:07:43.000000 types-aiobotocore-elb-2.9.1/types_aiobotocore_elb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9458 2024-01-18 01:07:45.000000 types-aiobotocore-elb-2.9.1/types_aiobotocore_elb/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9458 2024-01-18 01:07:43.000000 types-aiobotocore-elb-2.9.1/types_aiobotocore_elb/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-01-18 01:07:43.000000 types-aiobotocore-elb-2.9.1/types_aiobotocore_elb/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-01-18 01:07:43.000000 types-aiobotocore-elb-2.9.1/types_aiobotocore_elb/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:07:43.000000 types-aiobotocore-elb-2.9.1/types_aiobotocore_elb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    21889 2024-01-18 01:07:45.000000 types-aiobotocore-elb-2.9.1/types_aiobotocore_elb/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21889 2024-01-18 01:07:45.000000 types-aiobotocore-elb-2.9.1/types_aiobotocore_elb/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:07:43.000000 types-aiobotocore-elb-2.9.1/types_aiobotocore_elb/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-01-18 01:07:43.000000 types-aiobotocore-elb-2.9.1/types_aiobotocore_elb/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-01-18 01:07:43.000000 types-aiobotocore-elb-2.9.1/types_aiobotocore_elb/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:40.105345 types-aiobotocore-elb-2.9.1/types_aiobotocore_elb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14172 2024-01-18 01:20:40.000000 types-aiobotocore-elb-2.9.1/types_aiobotocore_elb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-01-18 01:20:40.000000 types-aiobotocore-elb-2.9.1/types_aiobotocore_elb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:40.000000 types-aiobotocore-elb-2.9.1/types_aiobotocore_elb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:40.000000 types-aiobotocore-elb-2.9.1/types_aiobotocore_elb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:40.000000 types-aiobotocore-elb-2.9.1/types_aiobotocore_elb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-18 01:20:40.000000 types-aiobotocore-elb-2.9.1/types_aiobotocore_elb.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-elb-2.9.0/LICENSE` & `types-aiobotocore-elb-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-elb-2.9.0/PKG-INFO` & `types-aiobotocore-elb-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-elb
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ElasticLoadBalancing 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ElasticLoadBalancing 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/
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
 
 <a id="types-aiobotocore-elb"></a>
 
 # types-aiobotocore-elb
 
 [![PyPI - types-aiobotocore-elb](https://img.shields.io/pypi/v/types-aiobotocore-elb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-elb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elb)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-elb)](https://pepy.tech/project/types-aiobotocore-elb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ElasticLoadBalancing 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing)
+[aiobotocore.ElasticLoadBalancing 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing)
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
 [types-aiobotocore-elb docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-elb-2.9.0/README.md` & `types-aiobotocore-elb-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-elb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elb)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-elb)](https://pepy.tech/project/types-aiobotocore-elb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ElasticLoadBalancing 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing)
+[aiobotocore.ElasticLoadBalancing 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing)
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
 [types-aiobotocore-elb docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-elb-2.9.0/setup.py` & `types-aiobotocore-elb-2.9.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-elb",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_elb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ElasticLoadBalancing 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.ElasticLoadBalancing 2.9.1 service generated with"
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
     keywords="aiobotocore elb type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_elb": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-elb-2.9.0/types_aiobotocore_elb/__init__.py` & `types-aiobotocore-elb-2.9.1/types_aiobotocore_elb/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 
 from .client import ElasticLoadBalancingClient
 from .paginator import DescribeAccountLimitsPaginator, DescribeLoadBalancersPaginator
 from .waiter import AnyInstanceInServiceWaiter, InstanceDeregisteredWaiter, InstanceInServiceWaiter
 
 Client = ElasticLoadBalancingClient
 
-
 __all__ = (
     "AnyInstanceInServiceWaiter",
     "Client",
     "DescribeAccountLimitsPaginator",
     "DescribeLoadBalancersPaginator",
     "ElasticLoadBalancingClient",
     "InstanceDeregisteredWaiter",
```

### Comparing `types-aiobotocore-elb-2.9.0/types_aiobotocore_elb/__init__.pyi` & `types-aiobotocore-elb-2.9.1/types_aiobotocore_elb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elb-2.9.0/types_aiobotocore_elb/__main__.py` & `types-aiobotocore-elb-2.9.1/types_aiobotocore_elb/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ElasticLoadBalancing 2.9.0\nVersion:        "
-        " 2.9.0\nBuilder version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.ElasticLoadBalancing 2.9.1\nVersion:        "
+        " 2.9.1\nBuilder version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing\nOther"
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

### Comparing `types-aiobotocore-elb-2.9.0/types_aiobotocore_elb/client.py` & `types-aiobotocore-elb-2.9.1/types_aiobotocore_elb/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,14 @@
 from .waiter import AnyInstanceInServiceWaiter, InstanceDeregisteredWaiter, InstanceInServiceWaiter
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ElasticLoadBalancingClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -201,15 +200,15 @@
         *,
         LoadBalancerName: str,
         Listeners: Sequence[ListenerTypeDef],
         AvailabilityZones: Sequence[str] = ...,
         Subnets: Sequence[str] = ...,
         SecurityGroups: Sequence[str] = ...,
         Scheme: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateAccessPointOutputTypeDef:
         """
         Creates a Classic Load Balancer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing.Client.create_load_balancer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/client/#create_load_balancer)
         """
@@ -226,15 +225,15 @@
 
     async def create_load_balancer_policy(
         self,
         *,
         LoadBalancerName: str,
         PolicyName: str,
         PolicyTypeName: str,
-        PolicyAttributes: Sequence[PolicyAttributeTypeDef] = ...
+        PolicyAttributes: Sequence[PolicyAttributeTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Creates a policy with the specified attributes for the specified load balancer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing.Client.create_load_balancer_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/client/#create_load_balancer_policy)
         """
```

### Comparing `types-aiobotocore-elb-2.9.0/types_aiobotocore_elb/client.pyi` & `types-aiobotocore-elb-2.9.1/types_aiobotocore_elb/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -197,15 +197,15 @@
         *,
         LoadBalancerName: str,
         Listeners: Sequence[ListenerTypeDef],
         AvailabilityZones: Sequence[str] = ...,
         Subnets: Sequence[str] = ...,
         SecurityGroups: Sequence[str] = ...,
         Scheme: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateAccessPointOutputTypeDef:
         """
         Creates a Classic Load Balancer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing.Client.create_load_balancer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/client/#create_load_balancer)
         """
@@ -222,15 +222,15 @@
 
     async def create_load_balancer_policy(
         self,
         *,
         LoadBalancerName: str,
         PolicyName: str,
         PolicyTypeName: str,
-        PolicyAttributes: Sequence[PolicyAttributeTypeDef] = ...
+        PolicyAttributes: Sequence[PolicyAttributeTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Creates a policy with the specified attributes for the specified load balancer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing.Client.create_load_balancer_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/client/#create_load_balancer_policy)
         """
```

### Comparing `types-aiobotocore-elb-2.9.0/types_aiobotocore_elb/literals.py` & `types-aiobotocore-elb-2.9.1/types_aiobotocore_elb/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,30 +15,28 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AnyInstanceInServiceWaiterName",
     "DescribeAccountLimitsPaginatorName",
     "DescribeLoadBalancersPaginatorName",
     "InstanceDeregisteredWaiterName",
     "InstanceInServiceWaiterName",
     "ElasticLoadBalancingServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 AnyInstanceInServiceWaiterName = Literal["any_instance_in_service"]
 DescribeAccountLimitsPaginatorName = Literal["describe_account_limits"]
 DescribeLoadBalancersPaginatorName = Literal["describe_load_balancers"]
 InstanceDeregisteredWaiterName = Literal["instance_deregistered"]
 InstanceInServiceWaiterName = Literal["instance_in_service"]
 ElasticLoadBalancingServiceName = Literal["elb"]
 ServiceName = Literal[
```

### Comparing `types-aiobotocore-elb-2.9.0/types_aiobotocore_elb/literals.pyi` & `types-aiobotocore-elb-2.9.1/types_aiobotocore_elb/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elb-2.9.0/types_aiobotocore_elb/paginator.py` & `types-aiobotocore-elb-2.9.1/types_aiobotocore_elb/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,14 @@
     DescribeAccessPointsOutputTypeDef,
     DescribeAccountLimitsOutputTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("DescribeAccountLimitsPaginator", "DescribeLoadBalancersPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -68,13 +67,13 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/paginators/#describeloadbalancerspaginator)
     """
 
     def paginate(
         self,
         *,
         LoadBalancerNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeAccessPointsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing.Paginator.DescribeLoadBalancers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/paginators/#describeloadbalancerspaginator)
         """
```

### Comparing `types-aiobotocore-elb-2.9.0/types_aiobotocore_elb/paginator.pyi` & `types-aiobotocore-elb-2.9.1/types_aiobotocore_elb/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -64,13 +64,13 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/paginators/#describeloadbalancerspaginator)
     """
 
     def paginate(
         self,
         *,
         LoadBalancerNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeAccessPointsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing.Paginator.DescribeLoadBalancers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/paginators/#describeloadbalancerspaginator)
         """
```

### Comparing `types-aiobotocore-elb-2.9.0/types_aiobotocore_elb/type_defs.py` & `types-aiobotocore-elb-2.9.1/types_aiobotocore_elb/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccessLogTypeDef",
     "AddAvailabilityZonesInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "TagTypeDef",
     "AdditionalAttributeTypeDef",
     "AppCookieStickinessPolicyTypeDef",
```

### Comparing `types-aiobotocore-elb-2.9.0/types_aiobotocore_elb/type_defs.pyi` & `types-aiobotocore-elb-2.9.1/types_aiobotocore_elb/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elb-2.9.0/types_aiobotocore_elb/waiter.py` & `types-aiobotocore-elb-2.9.1/types_aiobotocore_elb/waiter.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     """
 
     async def wait(
         self,
         *,
         LoadBalancerName: str,
         Instances: Sequence[InstanceTypeDef] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing.Waiter.AnyInstanceInService.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/waiters/#anyinstanceinservicewaiter)
         """
 
 
@@ -60,15 +60,15 @@
     """
 
     async def wait(
         self,
         *,
         LoadBalancerName: str,
         Instances: Sequence[InstanceTypeDef] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing.Waiter.InstanceDeregistered.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/waiters/#instancederegisteredwaiter)
         """
 
 
@@ -79,13 +79,13 @@
     """
 
     async def wait(
         self,
         *,
         LoadBalancerName: str,
         Instances: Sequence[InstanceTypeDef] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing.Waiter.InstanceInService.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/waiters/#instanceinservicewaiter)
         """
```

### Comparing `types-aiobotocore-elb-2.9.0/types_aiobotocore_elb/waiter.pyi` & `types-aiobotocore-elb-2.9.1/types_aiobotocore_elb/waiter.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     """
 
     async def wait(
         self,
         *,
         LoadBalancerName: str,
         Instances: Sequence[InstanceTypeDef] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing.Waiter.AnyInstanceInService.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/waiters/#anyinstanceinservicewaiter)
         """
 
 class InstanceDeregisteredWaiter(AIOWaiter):
@@ -58,15 +58,15 @@
     """
 
     async def wait(
         self,
         *,
         LoadBalancerName: str,
         Instances: Sequence[InstanceTypeDef] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing.Waiter.InstanceDeregistered.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/waiters/#instancederegisteredwaiter)
         """
 
 class InstanceInServiceWaiter(AIOWaiter):
@@ -76,13 +76,13 @@
     """
 
     async def wait(
         self,
         *,
         LoadBalancerName: str,
         Instances: Sequence[InstanceTypeDef] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing.Waiter.InstanceInService.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/waiters/#instanceinservicewaiter)
         """
```

### Comparing `types-aiobotocore-elb-2.9.0/types_aiobotocore_elb.egg-info/PKG-INFO` & `types-aiobotocore-elb-2.9.1/types_aiobotocore_elb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-elb
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ElasticLoadBalancing 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ElasticLoadBalancing 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/
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
 
 <a id="types-aiobotocore-elb"></a>
 
 # types-aiobotocore-elb
 
 [![PyPI - types-aiobotocore-elb](https://img.shields.io/pypi/v/types-aiobotocore-elb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-elb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elb)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-elb)](https://pepy.tech/project/types-aiobotocore-elb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ElasticLoadBalancing 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing)
+[aiobotocore.ElasticLoadBalancing 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing)
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
 [types-aiobotocore-elb docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-elb-2.9.0/types_aiobotocore_elb.egg-info/SOURCES.txt` & `types-aiobotocore-elb-2.9.1/types_aiobotocore_elb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

