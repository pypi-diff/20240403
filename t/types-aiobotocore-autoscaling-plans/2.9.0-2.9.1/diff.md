# Comparing `tmp/types-aiobotocore-autoscaling-plans-2.9.0.tar.gz` & `tmp/types-aiobotocore-autoscaling-plans-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-autoscaling-plans-2.9.0.tar", last modified: Wed Dec 13 19:58:39 2023, max compression
+gzip compressed data, was "types-aiobotocore-autoscaling-plans-2.9.1.tar", last modified: Thu Jan 18 01:20:06 2024, max compression
```

## Comparing `types-aiobotocore-autoscaling-plans-2.9.0.tar` & `types-aiobotocore-autoscaling-plans-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:39.110057 types-aiobotocore-autoscaling-plans-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:41:29.000000 types-aiobotocore-autoscaling-plans-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13806 2023-12-13 19:58:39.110057 types-aiobotocore-autoscaling-plans-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12204 2023-12-13 19:41:29.000000 types-aiobotocore-autoscaling-plans-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:39.110057 types-aiobotocore-autoscaling-plans-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2023-12-13 19:41:29.000000 types-aiobotocore-autoscaling-plans-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:39.110057 types-aiobotocore-autoscaling-plans-2.9.0/types_aiobotocore_autoscaling_plans/
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2023-12-13 19:41:29.000000 types-aiobotocore-autoscaling-plans-2.9.0/types_aiobotocore_autoscaling_plans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2023-12-13 19:41:29.000000 types-aiobotocore-autoscaling-plans-2.9.0/types_aiobotocore_autoscaling_plans/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      970 2023-12-13 19:41:29.000000 types-aiobotocore-autoscaling-plans-2.9.0/types_aiobotocore_autoscaling_plans/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10247 2023-12-13 19:41:29.000000 types-aiobotocore-autoscaling-plans-2.9.0/types_aiobotocore_autoscaling_plans/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    10243 2023-12-13 19:41:29.000000 types-aiobotocore-autoscaling-plans-2.9.0/types_aiobotocore_autoscaling_plans/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11417 2023-12-13 19:41:30.000000 types-aiobotocore-autoscaling-plans-2.9.0/types_aiobotocore_autoscaling_plans/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11415 2023-12-13 19:41:30.000000 types-aiobotocore-autoscaling-plans-2.9.0/types_aiobotocore_autoscaling_plans/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2023-12-13 19:41:30.000000 types-aiobotocore-autoscaling-plans-2.9.0/types_aiobotocore_autoscaling_plans/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3799 2023-12-13 19:41:29.000000 types-aiobotocore-autoscaling-plans-2.9.0/types_aiobotocore_autoscaling_plans/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:41:29.000000 types-aiobotocore-autoscaling-plans-2.9.0/types_aiobotocore_autoscaling_plans/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    15403 2023-12-13 19:41:30.000000 types-aiobotocore-autoscaling-plans-2.9.0/types_aiobotocore_autoscaling_plans/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15402 2023-12-13 19:41:30.000000 types-aiobotocore-autoscaling-plans-2.9.0/types_aiobotocore_autoscaling_plans/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:41:29.000000 types-aiobotocore-autoscaling-plans-2.9.0/types_aiobotocore_autoscaling_plans/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:39.110057 types-aiobotocore-autoscaling-plans-2.9.0/types_aiobotocore_autoscaling_plans.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13806 2023-12-13 19:58:39.000000 types-aiobotocore-autoscaling-plans-2.9.0/types_aiobotocore_autoscaling_plans.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2023-12-13 19:58:39.000000 types-aiobotocore-autoscaling-plans-2.9.0/types_aiobotocore_autoscaling_plans.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:39.000000 types-aiobotocore-autoscaling-plans-2.9.0/types_aiobotocore_autoscaling_plans.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:39.000000 types-aiobotocore-autoscaling-plans-2.9.0/types_aiobotocore_autoscaling_plans.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:39.000000 types-aiobotocore-autoscaling-plans-2.9.0/types_aiobotocore_autoscaling_plans.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-13 19:58:39.000000 types-aiobotocore-autoscaling-plans-2.9.0/types_aiobotocore_autoscaling_plans.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:06.841500 types-aiobotocore-autoscaling-plans-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:03:28.000000 types-aiobotocore-autoscaling-plans-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13826 2024-01-18 01:20:06.841500 types-aiobotocore-autoscaling-plans-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12204 2024-01-18 01:03:28.000000 types-aiobotocore-autoscaling-plans-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:06.841500 types-aiobotocore-autoscaling-plans-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-01-18 01:03:28.000000 types-aiobotocore-autoscaling-plans-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:06.841500 types-aiobotocore-autoscaling-plans-2.9.1/types_aiobotocore_autoscaling_plans/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-01-18 01:03:28.000000 types-aiobotocore-autoscaling-plans-2.9.1/types_aiobotocore_autoscaling_plans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-01-18 01:03:28.000000 types-aiobotocore-autoscaling-plans-2.9.1/types_aiobotocore_autoscaling_plans/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-01-18 01:03:28.000000 types-aiobotocore-autoscaling-plans-2.9.1/types_aiobotocore_autoscaling_plans/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10251 2024-01-18 01:03:28.000000 types-aiobotocore-autoscaling-plans-2.9.1/types_aiobotocore_autoscaling_plans/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10248 2024-01-18 01:03:28.000000 types-aiobotocore-autoscaling-plans-2.9.1/types_aiobotocore_autoscaling_plans/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11415 2024-01-18 01:03:28.000000 types-aiobotocore-autoscaling-plans-2.9.1/types_aiobotocore_autoscaling_plans/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11415 2024-01-18 01:03:28.000000 types-aiobotocore-autoscaling-plans-2.9.1/types_aiobotocore_autoscaling_plans/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-01-18 01:03:28.000000 types-aiobotocore-autoscaling-plans-2.9.1/types_aiobotocore_autoscaling_plans/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-01-18 01:03:28.000000 types-aiobotocore-autoscaling-plans-2.9.1/types_aiobotocore_autoscaling_plans/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:03:28.000000 types-aiobotocore-autoscaling-plans-2.9.1/types_aiobotocore_autoscaling_plans/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    15402 2024-01-18 01:03:29.000000 types-aiobotocore-autoscaling-plans-2.9.1/types_aiobotocore_autoscaling_plans/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15402 2024-01-18 01:03:28.000000 types-aiobotocore-autoscaling-plans-2.9.1/types_aiobotocore_autoscaling_plans/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:03:28.000000 types-aiobotocore-autoscaling-plans-2.9.1/types_aiobotocore_autoscaling_plans/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:06.841500 types-aiobotocore-autoscaling-plans-2.9.1/types_aiobotocore_autoscaling_plans.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13826 2024-01-18 01:20:06.000000 types-aiobotocore-autoscaling-plans-2.9.1/types_aiobotocore_autoscaling_plans.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-01-18 01:20:06.000000 types-aiobotocore-autoscaling-plans-2.9.1/types_aiobotocore_autoscaling_plans.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:06.000000 types-aiobotocore-autoscaling-plans-2.9.1/types_aiobotocore_autoscaling_plans.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:06.000000 types-aiobotocore-autoscaling-plans-2.9.1/types_aiobotocore_autoscaling_plans.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:06.000000 types-aiobotocore-autoscaling-plans-2.9.1/types_aiobotocore_autoscaling_plans.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-01-18 01:20:06.000000 types-aiobotocore-autoscaling-plans-2.9.1/types_aiobotocore_autoscaling_plans.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-autoscaling-plans-2.9.0/LICENSE` & `types-aiobotocore-autoscaling-plans-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-autoscaling-plans-2.9.0/PKG-INFO` & `types-aiobotocore-autoscaling-plans-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-autoscaling-plans
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.AutoScalingPlans 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.AutoScalingPlans 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/
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
 
 <a id="types-aiobotocore-autoscaling-plans"></a>
 
 # types-aiobotocore-autoscaling-plans
 
 [![PyPI - types-aiobotocore-autoscaling-plans](https://img.shields.io/pypi/v/types-aiobotocore-autoscaling-plans.svg?color=blue)](https://pypi.org/project/types-aiobotocore-autoscaling-plans)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-autoscaling-plans.svg?color=blue)](https://pypi.org/project/types-aiobotocore-autoscaling-plans)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-autoscaling-plans)](https://pepy.tech/project/types-aiobotocore-autoscaling-plans)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AutoScalingPlans 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans)
+[aiobotocore.AutoScalingPlans 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans)
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
 [types-aiobotocore-autoscaling-plans docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-autoscaling-plans-2.9.0/README.md` & `types-aiobotocore-autoscaling-plans-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-autoscaling-plans.svg?color=blue)](https://pypi.org/project/types-aiobotocore-autoscaling-plans)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-autoscaling-plans)](https://pepy.tech/project/types-aiobotocore-autoscaling-plans)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AutoScalingPlans 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans)
+[aiobotocore.AutoScalingPlans 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans)
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
 [types-aiobotocore-autoscaling-plans docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-autoscaling-plans-2.9.0/setup.py` & `types-aiobotocore-autoscaling-plans-2.9.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-autoscaling-plans",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_autoscaling_plans"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.AutoScalingPlans 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.AutoScalingPlans 2.9.1 service generated with"
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
     keywords="aiobotocore autoscaling-plans type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_autoscaling_plans": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-autoscaling-plans-2.9.0/types_aiobotocore_autoscaling_plans/__init__.py` & `types-aiobotocore-autoscaling-plans-2.9.1/types_aiobotocore_autoscaling_plans/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,14 +24,13 @@
 """
 
 from .client import AutoScalingPlansClient
 from .paginator import DescribeScalingPlanResourcesPaginator, DescribeScalingPlansPaginator
 
 Client = AutoScalingPlansClient
 
-
 __all__ = (
     "AutoScalingPlansClient",
     "Client",
     "DescribeScalingPlanResourcesPaginator",
     "DescribeScalingPlansPaginator",
 )
```

### Comparing `types-aiobotocore-autoscaling-plans-2.9.0/types_aiobotocore_autoscaling_plans/__init__.pyi` & `types-aiobotocore-autoscaling-plans-2.9.1/types_aiobotocore_autoscaling_plans/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-autoscaling-plans-2.9.0/types_aiobotocore_autoscaling_plans/__main__.py` & `types-aiobotocore-autoscaling-plans-2.9.1/types_aiobotocore_autoscaling_plans/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.AutoScalingPlans 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.AutoScalingPlans 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans\nOther"
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

### Comparing `types-aiobotocore-autoscaling-plans-2.9.0/types_aiobotocore_autoscaling_plans/client.py` & `types-aiobotocore-autoscaling-plans-2.9.1/types_aiobotocore_autoscaling_plans/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -34,36 +34,32 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("AutoScalingPlansClient",)
 
-
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     ConcurrentUpdateException: Type[BotocoreClientError]
     InternalServiceException: Type[BotocoreClientError]
     InvalidNextTokenException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     ObjectNotFoundException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class AutoScalingPlansClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/client/)
     """
 
     meta: ClientMeta
@@ -94,15 +90,15 @@
         """
 
     async def create_scaling_plan(
         self,
         *,
         ScalingPlanName: str,
         ApplicationSource: ApplicationSourceTypeDef,
-        ScalingInstructions: Sequence[ScalingInstructionTypeDef]
+        ScalingInstructions: Sequence[ScalingInstructionTypeDef],
     ) -> CreateScalingPlanResponseTypeDef:
         """
         Creates a scaling plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client.create_scaling_plan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/client/#create_scaling_plan)
         """
@@ -119,15 +115,15 @@
 
     async def describe_scaling_plan_resources(
         self,
         *,
         ScalingPlanName: str,
         ScalingPlanVersion: int,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeScalingPlanResourcesResponseTypeDef:
         """
         Describes the scalable resources in the specified scaling plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client.describe_scaling_plan_resources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/client/#describe_scaling_plan_resources)
         """
@@ -135,15 +131,15 @@
     async def describe_scaling_plans(
         self,
         *,
         ScalingPlanNames: Sequence[str] = ...,
         ScalingPlanVersion: int = ...,
         ApplicationSources: Sequence[ApplicationSourceTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeScalingPlansResponseTypeDef:
         """
         Describes one or more of your scaling plans.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client.describe_scaling_plans)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/client/#describe_scaling_plans)
         """
@@ -168,30 +164,30 @@
         ScalingPlanName: str,
         ScalingPlanVersion: int,
         ServiceNamespace: ServiceNamespaceType,
         ResourceId: str,
         ScalableDimension: ScalableDimensionType,
         ForecastDataType: ForecastDataTypeType,
         StartTime: TimestampTypeDef,
-        EndTime: TimestampTypeDef
+        EndTime: TimestampTypeDef,
     ) -> GetScalingPlanResourceForecastDataResponseTypeDef:
         """
         Retrieves the forecast data for a scalable resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client.get_scaling_plan_resource_forecast_data)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/client/#get_scaling_plan_resource_forecast_data)
         """
 
     async def update_scaling_plan(
         self,
         *,
         ScalingPlanName: str,
         ScalingPlanVersion: int,
         ApplicationSource: ApplicationSourceTypeDef = ...,
-        ScalingInstructions: Sequence[ScalingInstructionTypeDef] = ...
+        ScalingInstructions: Sequence[ScalingInstructionTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Updates the specified scaling plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client.update_scaling_plan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/client/#update_scaling_plan)
         """
```

### Comparing `types-aiobotocore-autoscaling-plans-2.9.0/types_aiobotocore_autoscaling_plans/client.pyi` & `types-aiobotocore-autoscaling-plans-2.9.1/types_aiobotocore_autoscaling_plans/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,30 +36,33 @@
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = ("AutoScalingPlansClient",)
 
+
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     ConcurrentUpdateException: Type[BotocoreClientError]
     InternalServiceException: Type[BotocoreClientError]
     InvalidNextTokenException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     ObjectNotFoundException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class AutoScalingPlansClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/client/)
     """
 
     meta: ClientMeta
@@ -90,15 +93,15 @@
         """
 
     async def create_scaling_plan(
         self,
         *,
         ScalingPlanName: str,
         ApplicationSource: ApplicationSourceTypeDef,
-        ScalingInstructions: Sequence[ScalingInstructionTypeDef]
+        ScalingInstructions: Sequence[ScalingInstructionTypeDef],
     ) -> CreateScalingPlanResponseTypeDef:
         """
         Creates a scaling plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client.create_scaling_plan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/client/#create_scaling_plan)
         """
@@ -115,15 +118,15 @@
 
     async def describe_scaling_plan_resources(
         self,
         *,
         ScalingPlanName: str,
         ScalingPlanVersion: int,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeScalingPlanResourcesResponseTypeDef:
         """
         Describes the scalable resources in the specified scaling plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client.describe_scaling_plan_resources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/client/#describe_scaling_plan_resources)
         """
@@ -131,15 +134,15 @@
     async def describe_scaling_plans(
         self,
         *,
         ScalingPlanNames: Sequence[str] = ...,
         ScalingPlanVersion: int = ...,
         ApplicationSources: Sequence[ApplicationSourceTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeScalingPlansResponseTypeDef:
         """
         Describes one or more of your scaling plans.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client.describe_scaling_plans)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/client/#describe_scaling_plans)
         """
@@ -164,30 +167,30 @@
         ScalingPlanName: str,
         ScalingPlanVersion: int,
         ServiceNamespace: ServiceNamespaceType,
         ResourceId: str,
         ScalableDimension: ScalableDimensionType,
         ForecastDataType: ForecastDataTypeType,
         StartTime: TimestampTypeDef,
-        EndTime: TimestampTypeDef
+        EndTime: TimestampTypeDef,
     ) -> GetScalingPlanResourceForecastDataResponseTypeDef:
         """
         Retrieves the forecast data for a scalable resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client.get_scaling_plan_resource_forecast_data)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/client/#get_scaling_plan_resource_forecast_data)
         """
 
     async def update_scaling_plan(
         self,
         *,
         ScalingPlanName: str,
         ScalingPlanVersion: int,
         ApplicationSource: ApplicationSourceTypeDef = ...,
-        ScalingInstructions: Sequence[ScalingInstructionTypeDef] = ...
+        ScalingInstructions: Sequence[ScalingInstructionTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Updates the specified scaling plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client.update_scaling_plan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/client/#update_scaling_plan)
         """
```

### Comparing `types-aiobotocore-autoscaling-plans-2.9.0/types_aiobotocore_autoscaling_plans/literals.py` & `types-aiobotocore-autoscaling-plans-2.9.1/types_aiobotocore_autoscaling_plans/literals.py`

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
     "DescribeScalingPlanResourcesPaginatorName",
     "DescribeScalingPlansPaginatorName",
     "ForecastDataTypeType",
     "LoadMetricTypeType",
     "MetricStatisticType",
     "PolicyTypeType",
@@ -38,15 +37,14 @@
     "AutoScalingPlansServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 DescribeScalingPlanResourcesPaginatorName = Literal["describe_scaling_plan_resources"]
 DescribeScalingPlansPaginatorName = Literal["describe_scaling_plans"]
 ForecastDataTypeType = Literal[
     "CapacityForecast", "LoadForecast", "ScheduledActionMaxCapacity", "ScheduledActionMinCapacity"
 ]
 LoadMetricTypeType = Literal[
     "ALBTargetGroupRequestCount",
```

### Comparing `types-aiobotocore-autoscaling-plans-2.9.0/types_aiobotocore_autoscaling_plans/literals.pyi` & `types-aiobotocore-autoscaling-plans-2.9.1/types_aiobotocore_autoscaling_plans/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-autoscaling-plans-2.9.0/types_aiobotocore_autoscaling_plans/paginator.py` & `types-aiobotocore-autoscaling-plans-2.9.1/types_aiobotocore_autoscaling_plans/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     DescribeScalingPlanResourcesResponsePaginatorTypeDef,
     DescribeScalingPlansResponsePaginatorTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("DescribeScalingPlanResourcesPaginator", "DescribeScalingPlansPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -55,15 +54,15 @@
     """
 
     def paginate(
         self,
         *,
         ScalingPlanName: str,
         ScalingPlanVersion: int,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeScalingPlanResourcesResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Paginator.DescribeScalingPlanResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/paginators/#describescalingplanresourcespaginator)
         """
 
 
@@ -75,13 +74,13 @@
 
     def paginate(
         self,
         *,
         ScalingPlanNames: Sequence[str] = ...,
         ScalingPlanVersion: int = ...,
         ApplicationSources: Sequence[ApplicationSourceTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeScalingPlansResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Paginator.DescribeScalingPlans.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/paginators/#describescalingplanspaginator)
         """
```

### Comparing `types-aiobotocore-autoscaling-plans-2.9.0/types_aiobotocore_autoscaling_plans/paginator.pyi` & `types-aiobotocore-autoscaling-plans-2.9.1/types_aiobotocore_autoscaling_plans/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     """
 
     def paginate(
         self,
         *,
         ScalingPlanName: str,
         ScalingPlanVersion: int,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeScalingPlanResourcesResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Paginator.DescribeScalingPlanResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/paginators/#describescalingplanresourcespaginator)
         """
 
 class DescribeScalingPlansPaginator(AioPaginator):
@@ -71,13 +71,13 @@
 
     def paginate(
         self,
         *,
         ScalingPlanNames: Sequence[str] = ...,
         ScalingPlanVersion: int = ...,
         ApplicationSources: Sequence[ApplicationSourceTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeScalingPlansResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Paginator.DescribeScalingPlans.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/paginators/#describescalingplanspaginator)
         """
```

### Comparing `types-aiobotocore-autoscaling-plans-2.9.0/types_aiobotocore_autoscaling_plans/type_defs.py` & `types-aiobotocore-autoscaling-plans-2.9.1/types_aiobotocore_autoscaling_plans/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "TagFilterTypeDef",
     "ResponseMetadataTypeDef",
     "MetricDimensionTypeDef",
     "DatapointTypeDef",
     "DeleteScalingPlanRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
```

### Comparing `types-aiobotocore-autoscaling-plans-2.9.0/types_aiobotocore_autoscaling_plans/type_defs.pyi` & `types-aiobotocore-autoscaling-plans-2.9.1/types_aiobotocore_autoscaling_plans/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-autoscaling-plans-2.9.0/types_aiobotocore_autoscaling_plans.egg-info/PKG-INFO` & `types-aiobotocore-autoscaling-plans-2.9.1/types_aiobotocore_autoscaling_plans.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-autoscaling-plans
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.AutoScalingPlans 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.AutoScalingPlans 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/
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
 
 <a id="types-aiobotocore-autoscaling-plans"></a>
 
 # types-aiobotocore-autoscaling-plans
 
 [![PyPI - types-aiobotocore-autoscaling-plans](https://img.shields.io/pypi/v/types-aiobotocore-autoscaling-plans.svg?color=blue)](https://pypi.org/project/types-aiobotocore-autoscaling-plans)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-autoscaling-plans.svg?color=blue)](https://pypi.org/project/types-aiobotocore-autoscaling-plans)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-autoscaling-plans)](https://pepy.tech/project/types-aiobotocore-autoscaling-plans)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AutoScalingPlans 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans)
+[aiobotocore.AutoScalingPlans 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans)
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
 [types-aiobotocore-autoscaling-plans docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-autoscaling-plans-2.9.0/types_aiobotocore_autoscaling_plans.egg-info/SOURCES.txt` & `types-aiobotocore-autoscaling-plans-2.9.1/types_aiobotocore_autoscaling_plans.egg-info/SOURCES.txt`

 * *Files identical despite different names*

